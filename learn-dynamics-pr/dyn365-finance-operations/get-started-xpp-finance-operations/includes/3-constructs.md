---
ms.openlocfilehash: 08bb770c989795df35ec6763e09484d6e979f7cd
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071857"
---
<span data-ttu-id="5f945-101">يستخدم X++ فئات لتعريف البيانات وإنشاء الكائنات.</span><span class="sxs-lookup"><span data-stu-id="5f945-101">X++ uses classes to define data and create objects.</span></span> <span data-ttu-id="5f945-102">البيانات التي يتم تحديدها في فئة تمثل حالة الكائن ويتم تخزينها في متغيرات.</span><span class="sxs-lookup"><span data-stu-id="5f945-102">The data that is defined in a class represents the state of the object and is stored in variables.</span></span> <span data-ttu-id="5f945-103">تحتوي الفئات أيضاً على الأساليب، التي ستخبر الكائن بما يجب فعله.</span><span class="sxs-lookup"><span data-stu-id="5f945-103">Classes also contain methods, which will tell the object what to do.</span></span> 

<span data-ttu-id="5f945-104">الجزء الأول من الفئة هو إعلان الفئة.</span><span class="sxs-lookup"><span data-stu-id="5f945-104">The first piece of a class is the class declaration.</span></span> <span data-ttu-id="5f945-105">يحتوي تعريف الفئة على اسم الفئة ومتغيرات المثيل والمعدلات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="5f945-105">The class declaration holds the name of the class, the instance variables, and other modifiers.</span></span> <span data-ttu-id="5f945-106">يمكنك تحديد رؤية المتغيرات باستخدام ثلاثة مُعدِّلات: `private`، و`protected`، و`public`.</span><span class="sxs-lookup"><span data-stu-id="5f945-106">You can determine the visibility of the variables by using three modifiers: `private`, `protected`, and `public`.</span></span> <span data-ttu-id="5f945-107">إذا لم تقم بإضافة معدل، فمن المفترض أن تكون فئة عامة.</span><span class="sxs-lookup"><span data-stu-id="5f945-107">If you do not add a modifier, it is presumed to be a public class.</span></span> <span data-ttu-id="5f945-108">ومع ذلك، فمن الأفضل توفير معدل.</span><span class="sxs-lookup"><span data-stu-id="5f945-108">However, it is best practice to provide a modifier.</span></span>

-   <span data-ttu-id="5f945-109">**خاص** - يجعل المتغيرات قابلة للاستخدام فقط داخل الفئة التي تم تحديدها فيها.</span><span class="sxs-lookup"><span data-stu-id="5f945-109">**Private** - Makes the variables only usable within the class that it is defined in.</span></span>
-   <span data-ttu-id="5f945-110">**محمٍ** - تجعل المتغير قابلاً للاستخدام فقط داخل الفئة المحددة فيه وأي فئة فرعية من تلك الفئة.</span><span class="sxs-lookup"><span data-stu-id="5f945-110">**Protected** - Makes the variable only usable within the class that it is defined in and any subclass of that class.</span></span>
-   <span data-ttu-id="5f945-111">**عام** - يجعل المتغير قابلاً للاستخدام في أي مكان وهو المعدل الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="5f945-111">**Public** - Makes the variable usable anywhere and is the default    modifier.</span></span>

<span data-ttu-id="5f945-112">فيما يلي مثال على إعلان فئة بالإضافة إلى إعلان عن متغير عضو:</span><span class="sxs-lookup"><span data-stu-id="5f945-112">The following is an example of a class declaration plus declaration of a member variable:</span></span>
```xpp
public class CustomerDetails
{
private str custName;
}
```
<span data-ttu-id="5f945-113">يجب إنشاء مثيل للفئات، ما لم تكن فئات ثابتة، قبل استخدامها.</span><span class="sxs-lookup"><span data-stu-id="5f945-113">Classes, unless they are static classes, need to be instantiated before they can be used.</span></span> <span data-ttu-id="5f945-114">فيما يلي مثال على كيفية إنشاء مثيل لفئة *TruckLoad* داخل فئة أخرى *الشاحنة*.</span><span class="sxs-lookup"><span data-stu-id="5f945-114">The following is an example of how to create an instance of a class *TruckLoad* inside another class *Truck*.</span></span> <span data-ttu-id="5f945-115">تم الإعلان عن متغير للفئة TruckLoad في أسلوب فئة *createNewTruckLoad*، ثم يتم إنشاء مثيل لكائن Truckload هذا وإعادته إلى المتصل باستخدام المُنشئ الافتراضي `new` متبوعاً ببيان إرجاع.</span><span class="sxs-lookup"><span data-stu-id="5f945-115">A variable for the class TruckLoad is declared in a class method *createNewTruckLoad*, and then an instance of that Truckload object is created and returned to the caller by using the default constructor `new` followed by a return statement.</span></span>

<span data-ttu-id="5f945-116">ستقبل أسلوب المثيل *shipTruckLoad* مثيل فئة *TruckLoad* لإجراء عملية شحن على هذا المثال بالإضافة إلى أسلوب ثابتة لحساب الوزن الإجمالي.</span><span class="sxs-lookup"><span data-stu-id="5f945-116">The instance method *shipTruckLoad* will accept an instance of the *TruckLoad* class to perform a shipping operation on that instance as well as a static method to calculate a total weight.</span></span>
```xpp
public class Truck
{
    public TruckLoad createNewTruckLoad()
    {
        TruckLoad myTruckLoad = new TruckLoad();
        return myTruckLoad;
    }
    public void shipTruckLoad(TruckLoad _truckLoad)
    {
        _truckLoad.ship();
    }
    public static int calcTotalWeight(int  netWeight,int tareWeight)
    {
        return netWeight+tareWeight;
    }
}
```
<span data-ttu-id="5f945-117">يمكن أن تكون الأساليب على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="5f945-117">Methods can be as follows:</span></span>

-   <span data-ttu-id="5f945-118">**أساليب المثيل (أو أساليب الكائن)** - مضمنة في الكائن الذي تم إنشاؤه من فئة.</span><span class="sxs-lookup"><span data-stu-id="5f945-118">**Instance methods (or object methods)** - Are embedded in the object that was created from a class.</span></span> <span data-ttu-id="5f945-119">يجب إنشاء مثيل للكائن قبل أن تتمكن من استخدام هذه الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="5f945-119">The object must be instantiated before you can use this method.</span></span> <span data-ttu-id="5f945-120">يمكن لأسلوب المثيل الوصول إلى المثيل والحالة الثابتة، في حين أن الأسلوب الثابتة يمكنها فقط الوصول إلى الحالة الثابتة.</span><span class="sxs-lookup"><span data-stu-id="5f945-120">An instance method can access the instance and static state, whereas a static method can only access the static state.</span></span>

-   <span data-ttu-id="5f945-121">**الأساليب الثابتة (المعروفة أيضاً باسم أساليب الفئة)** - لا تحتاج إلى إنشاء مثيل لكائن لاستخدام هذه الأساليب.</span><span class="sxs-lookup"><span data-stu-id="5f945-121">**Static methods (also known as class methods)** - You do not need to instantiate an object to use these methods.</span></span> <span data-ttu-id="5f945-122">يمكنك إعلان أسلوب ثابتة باستخدام الكلمة الأساسية `static`.</span><span class="sxs-lookup"><span data-stu-id="5f945-122">You can declare a method as static with the keyword `static`.</span></span> <span data-ttu-id="5f945-123">نوع معين من الأسلوب الثابت هو الأسلوب الرئيسية، والتي يمكن استدعاؤها مباشرة من خيار القائمة.</span><span class="sxs-lookup"><span data-stu-id="5f945-123">A specific type of static method is the Main method, which can be called directly from a menu option.</span></span>

<span data-ttu-id="5f945-124">الأساليب تتكون من التوقيع والنص.</span><span class="sxs-lookup"><span data-stu-id="5f945-124">Methods are made up of a signature and a body.</span></span> <span data-ttu-id="5f945-125">يحتفظ رأس الأسلوب باسم الأسلوب ونوع الإرجاع ومعدلات الأسلوب والمعلمات.</span><span class="sxs-lookup"><span data-stu-id="5f945-125">The method header holds the method's name, return type, method modifiers, and parameters.</span></span> <span data-ttu-id="5f945-126">إذا لم يكن هناك نوع إرجاع، فسيتم استخدام الكلمة الأساسية `void`.</span><span class="sxs-lookup"><span data-stu-id="5f945-126">If there is no return type, then the keyword `void` is used.</span></span> <span data-ttu-id="5f945-127">يحتوي النص الأساسي على الإعلانات المتغيرة وإعلانات الأساليب والعبارات.</span><span class="sxs-lookup"><span data-stu-id="5f945-127">The body holds the variable declarations, method declarations, and statements.</span></span>

<span data-ttu-id="5f945-128">التالي مثال على أسلوب.</span><span class="sxs-lookup"><span data-stu-id="5f945-128">The following is an example of a method.</span></span> <span data-ttu-id="5f945-129">الأسلوب هو أسلوب عام يقوم بإرجاع نوع بيانات حقيقي.</span><span class="sxs-lookup"><span data-stu-id="5f945-129">The method is a public method that returns a real data type.</span></span> <span data-ttu-id="5f945-130">يُسمى هذا الأسلوب بـ ReturnCalculation.</span><span class="sxs-lookup"><span data-stu-id="5f945-130">The method is called ReturnCalculation.</span></span> <span data-ttu-id="5f945-131">كما أنه يحتوي على معلمة نوع بيانات حقيقية `_expression1`.</span><span class="sxs-lookup"><span data-stu-id="5f945-131">It also has a real data type parameter `_expression1`.</span></span> <span data-ttu-id="5f945-132">يجب أن تبدأ المعلمات بـ "_" لتحديد المعلمات بسهولة داخل الرمز.</span><span class="sxs-lookup"><span data-stu-id="5f945-132">Parameters should begin with "_" to easily identify parameters within the code.</span></span>
```xpp
public real ReturnCalculation(real _expression1)
{
    real expression2 = 2;
    return _expression1 * expression2;
}
```
<span data-ttu-id="5f945-133">الآن، يمكنك جمع كل القطع المختلفة للفئة لإنشاء الفئة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="5f945-133">Now, you can collect all the different pieces of a class to create your own class.</span></span>
