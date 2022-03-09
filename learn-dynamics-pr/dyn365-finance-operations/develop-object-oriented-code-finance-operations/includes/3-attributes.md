---
ms.openlocfilehash: a4ddd472a8420cec62993508fa754b8144cf7adedcfc15cf6cd361ceed6a93a4
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7079245"
---

تمثل السمات أو تخزن بيانات التعريف حول سلوك الفئات والطرق. يمكن إرفاق السمة ببساطة عن طريق كتابة اسم السمة المحاط بأقواس مربعة قبل إعلان الفئة/الوظيفة حيث يلزم تطبيقها. 

### <a name="example"></a>مثال
على سبيل المثال، يمكن استخدام سمة `SysObsoleteAttribute(message,setError)` في الطرق أو الفئات التي لا ينبغي استخدامها بعد الآن. أثناء عملية الإنشاء، سيتم إخطار المستخدم برسالة مفصلة تظهر في نوافذ الإخراج. المعلمة الأولى هي الرسالة، وتشير المعلمة الثانية إلى ما إذا كان سيتم تعيين خطأ (صواب) أو تحذير (خطأ). يمكنك جعل المؤلف يرفض أو يعرض تحذيراً.

إذا لم تعد واجهة برمجة التطبيقات (API) تعمل، فقم بتعيين `isError = true` في سمة `SysObsoleteAttribute` حتى يقوم المؤلف بالإبلاغ عن أي استخدام لواجهة برمجة التطبيقات (API) هذه كخطأ في المؤلف

```xpp
 [SysObsoleteAttribute("The Automobile class might have faster  performance.", false)]
 class Bicycle
 {
    // Members of the Bicycle class go here.
 }

```

## <a name="attribute-classes"></a>فئات السمات 
يمكن أيضاً إنشاء السمات باستخدام فئات السمات. لإنشاء فئة سمة، قم بتوسيع فئة `SysAttribute` عن طريق إضافة `extend SysAttribute` في نهاية إعلان الفئة.
يمكنك بعد ذلك تزيين فئة بالسمة التي تم إنشاؤها من فئة السمة. يمكنك تحديد معلمات السمة من المنشئ. في التعليمة البرمجية التالية، يتم إنشاء فئة سمة `PracticeAttribute` ثم تقوم فئة `RegularClass` باستخدام `PracticeAttribute` كسمة.

### <a name="example"></a>مثال

يوضح المثال التالي إعلان وتصميم فئة السمات العادية التي يمكنك إنشاؤها.

```xpp
 public class PracticeAttribute extends SysAttribute
 {
   // Fields in the classDeclaration.
   StartEnd startEndEnum;
   str reason;

   // Constructor.
   public void new(StartEnd _startEndEnum, str _reason)
  {
    startEndEnum = _startEndEnum;
    reason = _reason;
  }
 }
[PracticeAttribute(StartEnd::End, "Use the RegularClass class at the end.")]
 public class RegularClass
 {
    [PracticeAttribute(Startend::Start, "Use the rehearse method at the start.")]
    public int rehearse()
    {
      // Logic goes here.
    }
      // More fields and methods belong here.
}

```
للسمات استخدامات عديدة، منها ما يلي:

-   استخدام السمة `WebMethod` في خدمات الويب للإشارة إلى ما إذا كان يجب أن تكون الطريقة قابلة للاستدعاء عبر بروتوكول الوصول إلى الكائنات البسيط (SOAP) لتبادل المعلومات.
-   استخدام `DLLImportAttribute` لاستدعاء التعليمة البرمجية غير المُدارة.
-   وصف العنوان أو الإصدار أو الوصف أو العلامة التجارية لتجميع.
-   وصف كيفية التعيين بين الفئات والأعضاء وعقد لغة التوصيف الموسعة (XML) للتسلسل.
-   وصف متطلبات الأمان للطرق.
-   تحديد الخصائص لفرض الأمان.
-   الحصول على معلومات حول المتصل إلى طريقة.
