---
ms.openlocfilehash: 604a3fffae3f721fd1a0f0602541e5c7ccbc469b
ms.sourcegitcommit: 442020b85a494c94b76f90102daf2916649c8c2e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/28/2022
ms.locfileid: "8490149"
---
توفر لك تطبيقات التمويل والعمليات عدة طرق لتشغيل عمليات تستغرق وقتًا طويلاً. 

- يُمكنك استخدام العمليات المجمعة لأداء مهام طويلة يتم تنفيذها على خوادم الدُفعات. 
- في بعض الأحيان، ستحتاج إلى تشغيل العمليات في عميل الويب. سيتم تجميد متصفح الويب حتى تكتمل العملية، إذا قمت بتشغيل العملية في الوضع المتزامن. قد يفصل Application Object Server (AOS) العميل إذا استغرقت العملية وقتًا طويلاً، مما سيؤدي في النهاية إلى فشل العملية التي كانت قيد التشغيل في عميل الويب. لتجنب هذا الموقف، يُمكنك تشغيل عملية غير متزامنة، والتي ستترك عميل الويب مجانيًا للمستخدم. 
- يُمكنك استخدام إطار عمل SysOperationSandbox، والذي سينفذ العملية طويلة المدى في جلسة منفصلة في الوضع غير المتزامن. بالإضافة إلى ذلك، يُظهر صَفحة الانتظار لعملية عدم التزامن، دون تجميد واجهة المستخدم. كما أن لديه الزر **إلغاء** للتخلي عن العملية.

## <a name="sysoperationsandbox"></a>SysOperationSandbox
باستخدام SysOperationSandbox، يُمكنك تشغيل عملية متزامنة على الجلسة غير المتزامنة التي تحدث على عميل الويب. سيساعدك إطار العمل على تشغيل جلستين للعميل بالتوازي. الجلسة الأولى هي جلسة غير متزامنة تقوم بتشغيل منطق الأعمال في فئة ثابتة. تتواصل الجلسة الثانية مع واجهة المستخدم لإبقائها مباشرة دون السماح بانتهاء المهلة. نتيجة لذلك، يُمكنك تشغيل جلسة متزامنة في نموذج دون المخاطرة بفصل عميل الويب. 

يُنشئ إطار عمل الحماية مثيلًا جديدًا للفئة ويقوم بتشغيله في وضع غير متزامن. ستستمر العملية المتزامنة بعد انتهاء الفصل من التنفيذ. باستخدام الأسلوب pack()/unpack() قبل بدء الأسلوب run()، يُمكن لإطار العمل تنظيم حالة المثيل الحالي إلى المثيل الجديد. تتواصل نفس العملية عندما يعود المثيل الجديد إلى المثيل الحالي. ومن ثم، يجب إجراء تسلسل صحيح لحالة الفئة في الأسلوبين pack() وunpack()، والتي تتوفر بالفعل للفئات المشتقة من RunBaseBatch.

### <a name="example"></a>مثال
يحتوي الجدول المخصص المسمى BankCheck على حقلين: **الحساب البنكي** و **رقم الشيك**. باستخدام إطار عمل بيئة الاختبار المعزولة، تحتاج إلى تشغيل عملية تعتمد على واجهة المستخدم لإضافة 100 رقم تحقق جديد، بدءًا من 10000. 

1. قم بإنشاء فئة جديدة باستخدام منطق الأعمال لإنشاء 100 رقم شيك جديد. يتم أيضًا إنشاء طرق التجميع والتفريغ في الفصل.

```xpp
class SandBoxLabHelper
{
    public static container AsyncInfo(container _parameters)
    {

        str bankAccount = conPeek(_parameters, 1);
        int checkStart = conPeek(_parameters, 2);
        int checkCount = conPeek(_parameters, 3);
        
        BankCheck   bankCheck;

        for(int i = checkStart; i < (checkStart + checkCount); i++)
        {
            bankCheck.clear();
            bankCheck.BankAccount = bankAccount;
            bankCheck.CheckNo = int2Str(i);
            bankCheck.insert();
        }
        return [true];
    }

    public container pack()
    {
        return conNull();
    }

    public boolean unpack(container _packedClass)
    {
        return true;
    }

    }
```



2. إنشاء نموذج جديد وإضافة أحد الأزرار. اكتب التعليمات البرمجية بالأسلوب clicked() ليقوم الزر بتشغيل الأسلوب AsyncInfo الثابت السابق باستخدام إطار عمل بيئة الاختبار المعزولة.

```xpp
public void clicked()
{
   boolean result;
   container mCon;
   mCon = conIns(mCon, 1, "1111111111");
   mCon = conIns(mCon, 2, 100000);
   mCon = conIns(mCon, 3, 100);
            
   [result] = SysOperationSandbox::callStaticMethod(classNum(SandBoxLabHelper), staticMethodStr(SandBoxLabHelper, AsyncInfo), mCon, "Processing", "Completed", "Cancelled");
   super();
}
```
