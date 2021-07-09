---
ms.openlocfilehash: d99279ec0468998ee4692ba90fa593c138ecbe24
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071221"
---

<span data-ttu-id="3868c-101">تمثل السمات أو تخزن بيانات التعريف حول سلوك الفئات والطرق.</span><span class="sxs-lookup"><span data-stu-id="3868c-101">Attributes represent or store metadata about the behaviors of classes and methods.</span></span> <span data-ttu-id="3868c-102">يمكن إرفاق السمة ببساطة عن طريق كتابة اسم السمة المحاط بأقواس مربعة قبل إعلان الفئة/الوظيفة حيث يلزم تطبيقها.</span><span class="sxs-lookup"><span data-stu-id="3868c-102">An attribute can be attached by simply typing the name of the attribute that is enclosed in square brackets before the declaration of class/function where it needs to be applied.</span></span> 

### <a name="example"></a><span data-ttu-id="3868c-103">مثال</span><span class="sxs-lookup"><span data-stu-id="3868c-103">Example</span></span>
<span data-ttu-id="3868c-104">على سبيل المثال، يمكن استخدام سمة `SysObsoleteAttribute(message,setError)` في الطرق أو الفئات التي لا ينبغي استخدامها بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="3868c-104">For example, the `SysObsoleteAttribute(message,setError)` attribute can be used on methods or classes that should no longer be used.</span></span> <span data-ttu-id="3868c-105">أثناء عملية الإنشاء، سيتم إخطار المستخدم برسالة مفصلة تظهر في نوافذ الإخراج.</span><span class="sxs-lookup"><span data-stu-id="3868c-105">During the build process, the user will be notified with a detailed message that appears in the output windows.</span></span> <span data-ttu-id="3868c-106">المعلمة الأولى هي الرسالة، وتشير المعلمة الثانية إلى ما إذا كان سيتم تعيين خطأ (صواب) أو تحذير (خطأ).</span><span class="sxs-lookup"><span data-stu-id="3868c-106">The first parameter is the message, and the second parameter indicates if an error (true) or a warning (false) is to be set.</span></span> <span data-ttu-id="3868c-107">يمكنك جعل المؤلف يرفض أو يعرض تحذيراً.</span><span class="sxs-lookup"><span data-stu-id="3868c-107">You can have the compiler reject or display a warning.</span></span>

<span data-ttu-id="3868c-108">إذا لم تعد واجهة برمجة التطبيقات (API) تعمل، فقم بتعيين `isError = true` في سمة `SysObsoleteAttribute` حتى يقوم المؤلف بالإبلاغ عن أي استخدام لواجهة برمجة التطبيقات (API) هذه كخطأ في المؤلف</span><span class="sxs-lookup"><span data-stu-id="3868c-108">If the API is no longer functioning, set `isError = true` in the `SysObsoleteAttribute` attribute so the compiler will report any use of that API as a compiler error</span></span>

```xpp
 [SysObsoleteAttribute("The Automobile class might have faster  performance.", false)]
 class Bicycle
 {
    // Members of the Bicycle class go here.
 }

```

## <a name="attribute-classes"></a><span data-ttu-id="3868c-109">فئات السمات</span><span class="sxs-lookup"><span data-stu-id="3868c-109">Attribute classes</span></span> 
<span data-ttu-id="3868c-110">يمكن أيضاً إنشاء السمات باستخدام فئات السمات.</span><span class="sxs-lookup"><span data-stu-id="3868c-110">Attributes can also be created by using attribute classes.</span></span> <span data-ttu-id="3868c-111">لإنشاء فئة سمة، قم بتوسيع فئة `SysAttribute` عن طريق إضافة `extend SysAttribute` في نهاية إعلان الفئة.</span><span class="sxs-lookup"><span data-stu-id="3868c-111">To create an attribute class, extend the `SysAttribute` class by adding `extend SysAttribute` at the end of your class declaration.</span></span>
<span data-ttu-id="3868c-112">يمكنك بعد ذلك تزيين فئة بالسمة التي تم إنشاؤها من فئة السمة.</span><span class="sxs-lookup"><span data-stu-id="3868c-112">You can then decorate a class with the attribute that was created from the attribute class.</span></span> <span data-ttu-id="3868c-113">يمكنك تحديد معلمات السمة من المنشئ.</span><span class="sxs-lookup"><span data-stu-id="3868c-113">You can specify the attribute parameters from the constructor.</span></span> <span data-ttu-id="3868c-114">في التعليمة البرمجية التالية، يتم إنشاء فئة سمة `PracticeAttribute` ثم تقوم فئة `RegularClass` باستخدام `PracticeAttribute` كسمة.</span><span class="sxs-lookup"><span data-stu-id="3868c-114">In the following code, the `PracticeAttribute` attribute class is created, and then the `RegularClass` class uses `PracticeAttribute` as an attribute.</span></span>

### <a name="example"></a><span data-ttu-id="3868c-115">مثال</span><span class="sxs-lookup"><span data-stu-id="3868c-115">Example</span></span>

<span data-ttu-id="3868c-116">يوضح المثال التالي إعلان وتصميم فئة السمات العادية التي يمكنك إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="3868c-116">The following example shows the declaration and design of an ordinary attribute class that you could create.</span></span>

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
<span data-ttu-id="3868c-117">للسمات استخدامات عديدة، منها ما يلي:</span><span class="sxs-lookup"><span data-stu-id="3868c-117">Attributes have many uses, including the following:</span></span>

-   <span data-ttu-id="3868c-118">استخدام السمة `WebMethod` في خدمات الويب للإشارة إلى ما إذا كان يجب أن تكون الطريقة قابلة للاستدعاء عبر بروتوكول الوصول إلى الكائنات البسيط (SOAP) لتبادل المعلومات.</span><span class="sxs-lookup"><span data-stu-id="3868c-118">Using the `WebMethod` attribute in Web services to indicate if the method should be callable over the Simple Object Access Protocol (SOAP) to exchange information.</span></span>
-   <span data-ttu-id="3868c-119">استخدام `DLLImportAttribute` لاستدعاء التعليمة البرمجية غير المُدارة.</span><span class="sxs-lookup"><span data-stu-id="3868c-119">Using `DLLImportAttribute` to call unmanaged code.</span></span>
-   <span data-ttu-id="3868c-120">وصف العنوان أو الإصدار أو الوصف أو العلامة التجارية لتجميع.</span><span class="sxs-lookup"><span data-stu-id="3868c-120">Describing the title, version, description, or trademark of an assembly.</span></span>
-   <span data-ttu-id="3868c-121">وصف كيفية التعيين بين الفئات والأعضاء وعقد لغة التوصيف الموسعة (XML) للتسلسل.</span><span class="sxs-lookup"><span data-stu-id="3868c-121">Describing how to map between classes, members, and eXtensible Markup Language (XML) nodes for serialization.</span></span>
-   <span data-ttu-id="3868c-122">وصف متطلبات الأمان للطرق.</span><span class="sxs-lookup"><span data-stu-id="3868c-122">Describing the security requirements for methods.</span></span>
-   <span data-ttu-id="3868c-123">تحديد الخصائص لفرض الأمان.</span><span class="sxs-lookup"><span data-stu-id="3868c-123">Specifying characteristics to enforce security.</span></span>
-   <span data-ttu-id="3868c-124">الحصول على معلومات حول المتصل إلى طريقة.</span><span class="sxs-lookup"><span data-stu-id="3868c-124">Getting information about the caller to a method.</span></span>
