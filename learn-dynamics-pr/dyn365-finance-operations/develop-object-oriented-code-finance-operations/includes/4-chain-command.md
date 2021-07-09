---
ms.openlocfilehash: ac0bca3737d14e99f895f27f7ab6416e4e0ab8c6
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071218"
---

<span data-ttu-id="cd6a9-101">سلسلة الأوامر (CoC) وظيفة لملحقات الفئة.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-101">Chain of Command (CoC) is a functionality for class extensions.</span></span> <span data-ttu-id="cd6a9-102">يمكنك استخدام سلسلة الأوامر لالتفاف الكود X++ حول الأساليب التي تم تعريفها في الفئة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-102">You can use CoC to wrap X++ code around methods that are defined in the base class.</span></span> <span data-ttu-id="cd6a9-103">تسمح لك سلسلة الأوامر بتخصيص فئات قياسية بدون استخدام معالجات الأحداث.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-103">CoC allows you to customize standard classes without using event handlers.</span></span> <span data-ttu-id="cd6a9-104">تتيح لك هذه الوظيفة إضافة منطق مخصص يتم تشغيله قبل و/أو بعد تشغيل الكود القياسي.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-104">This function allows you to add custom logic that will run before and/or after the standard code runs.</span></span> <span data-ttu-id="cd6a9-105">يمكنك فقط توسيع منطق الأساليب العامة والمحمية.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-105">You can only extend the logic of public and protected methods.</span></span> <span data-ttu-id="cd6a9-106">عند التفاف أسلوب، يمكنك أيضاً الوصول إلى الأساليب المحمية للفئة الأساسية، والأساليب العامة، والمتغيرات.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-106">When you wrap a method, you can also access the base class's protected methods, public methods, and variables.</span></span> <span data-ttu-id="cd6a9-107">من المهم فهم هذا المفهوم، لأنه لا يمكن تغيير الكود الأساسي في تطوير تطبيقات Dynamics 365 Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-107">It is important to understand this concept, as base code cannot be changed in Dynamics 365 Finance and Operations apps development.</span></span>
 
<span data-ttu-id="cd6a9-108">لاستخدام سلسلة الأوامر، تحتاج إلى إنشاء فئة جديدة تستخدم نفس الاسم كالفئة التي تقوم بتوسيعها مع إضافة `_Extension` إلى الاسم كلاحقة له.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-108">To use CoC, you need to create a new class that uses the same name as the class that you are extending with `_Extension` added to the name as a suffix.</span></span> <span data-ttu-id="cd6a9-109">يحتاج إقرار الفئة أيضاً إلى استخدام الكلمة الأساسية **النهائية** للإشارة إلى أنه لا يمكن الحصول عليها فيما بعد.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-109">The class declaration also needs to use the **final** keyword to indicate that it cannot be further inherited from.</span></span>
<span data-ttu-id="cd6a9-110">وأخيراً، يجب استخدام سمة `ExtensionOf` عندما تقوم بإقرار الفئة.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-110">Finally, the `ExtensionOf` attribute must be used when you are declaring the class.</span></span> <span data-ttu-id="cd6a9-111">ثم يمكنك إعادة استخدام نفس إقرار الأسلوب من الفئة الأساسية في الفئة الممتدة.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-111">You can then reuse the same method declaration from the base class in the extended class.</span></span> <span data-ttu-id="cd6a9-112">داخل الأسلوب الممتد، يمكنك إضافة الكود المخصص.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-112">Inside the extended method, you can add your custom code.</span></span> <span data-ttu-id="cd6a9-113">أنت مطالب باستخدام الكلمة الأساسية **التالية** لإنشاء سلسة أوامر.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-113">You are required to use the **next** keyword to create a CoC.</span></span> <span data-ttu-id="cd6a9-114">سيقوم الأمر التالي باستدعاء الأسلوب التالي في سلسلة الأوامر.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-114">The next command will call the next method in the Chain of Command.</span></span> <span data-ttu-id="cd6a9-115">عندما لا توجد أساليب أخرى في السلسلة، يتم استدعاء الأسلوب الأصلي (بمعنى آخر، الممتد).</span><span class="sxs-lookup"><span data-stu-id="cd6a9-115">When no more methods exist in the chain, the original (in other words, extended) method is called.</span></span>

### <a name="example"></a><span data-ttu-id="cd6a9-116">مثال</span><span class="sxs-lookup"><span data-stu-id="cd6a9-116">Example</span></span>

<span data-ttu-id="cd6a9-117">يوضح مثال الكود التالي كيف يجب إقرار الفئة لاستخدام سلسلة الأوامر.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-117">The following code example shows how the class must be declared to use CoC.</span></span> <span data-ttu-id="cd6a9-118">عند استدعاء أسلوب `ExampleClass.doSomething()`، سيقوم الكود أولاً بتشغيل كل الكود قبل الكلمة الأساسية التالية.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-118">When the `ExampleClass.doSomething()` method is called, the code will first run all the code before the next keyword.</span></span> <span data-ttu-id="cd6a9-119">ثم سيتم تشغيل الكود الأصلي في الأسلوب `ExampleClass.doSomething()`.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-119">Then, the original code in the `ExampleClass.doSomething()` method will run.</span></span> <span data-ttu-id="cd6a9-120">وأخيراً، سيتم تشغيل الكود بعد الكلمة الأساسية التالية.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-120">Finally, all code after the next keyword will run.</span></span>

```xpp
[ExtensionOf(classStr(ExampleClass))]
final class ExampleClass_Extension
{
   str doSomething(int arg)
   {
     // Custom logic before standard code.
     var s = next doSomething(arg);
     // Custom logic after standard code.
     return s;
   }
}

```

<span data-ttu-id="cd6a9-121">لا يمكن التفاف بعض الأساليب باستخدام سلسلة الأوامر.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-121">Certain methods cannot be wrapped by using CoC.</span></span> <span data-ttu-id="cd6a9-122">إذا كان الأسلوب يستخدم سمة قابلة للربط تم تعيينها على خطأ أو `[Hookable(false)]`، أو سمة قابلة للالتفاف تم تعيينها على خطأ، أو `[Wrappable(false)]` فإنه لا يمكن التفاف الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-122">If the method uses a hookable attribute that is set to false, `[Hookable(false)]`, or a wrappable attribute that is set to false, `[Wrappable(false)]`, the method cannot be wrapped.</span></span>
<span data-ttu-id="cd6a9-123">لا يمكن التفاف الأساليب التي تستخدم الكلمة الأساسية النهائية في فئة الملحق.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-123">Methods that use the final keyword cannot be wrapped in an extension class.</span></span> <span data-ttu-id="cd6a9-124">يتم أيضاً استبعاد الأساليب الخاصة من قابلية التوسعة.</span><span class="sxs-lookup"><span data-stu-id="cd6a9-124">Private methods are also excluded from extensibility.</span></span>
