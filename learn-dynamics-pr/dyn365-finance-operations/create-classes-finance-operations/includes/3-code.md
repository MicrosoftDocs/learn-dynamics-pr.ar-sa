---
ms.openlocfilehash: aead7e4144e65310f523305d313a7baaadf9d980
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071563"
---
<span data-ttu-id="c6763-101">تطبيقات Finance and Operations تستخدم لغة التطوير X++ في فئاتها.</span><span class="sxs-lookup"><span data-stu-id="c6763-101">Finance and Operations apps use X++ development language in its classes.</span></span>
<span data-ttu-id="c6763-102">تُعد X++ لغة موجهه للعناصر.</span><span class="sxs-lookup"><span data-stu-id="c6763-102">X++ is an object-oriented language.</span></span> <span data-ttu-id="c6763-103">إذا لم تكن قد استخدمتها من قبل، ولكنك معتاد على لغة أخرى موجهة للكائنات، فستجد أنه من السهل تعلمها.</span><span class="sxs-lookup"><span data-stu-id="c6763-103">If you haven't used it before, but are familiar with another object-oriented language, you will find it easy to learn.</span></span> 

<span data-ttu-id="c6763-104">بعد إنشاء فئة من **مستكشف الحلول**، يمكنك إضافة رمز إلى الفئة.</span><span class="sxs-lookup"><span data-stu-id="c6763-104">After you create a class from **Solution Explorer**, you can add code to the class.</span></span> <span data-ttu-id="c6763-105">توفر البيانات حالة الكائن، بينما يوفر الأسلوب سلوكاً لكائن.</span><span class="sxs-lookup"><span data-stu-id="c6763-105">Data provides the state of an object, while a method provides behavior to an object.</span></span> <span data-ttu-id="c6763-106">تتضمن الأساليب التي ستواجهها وستنشئها أثناء التطوير لتطبيقات Finance and Operations ما يلي:</span><span class="sxs-lookup"><span data-stu-id="c6763-106">Methods that you will encounter and create in development for Finance and Operations apps include:</span></span> 

- <span data-ttu-id="c6763-107">**الأسلوب الجديد** - إنشاء مثيل الفئة باستخدام الكلمة الأساسية `new`.</span><span class="sxs-lookup"><span data-stu-id="c6763-107">**New method** - Creates an instance of the class by using the `new` keyword.</span></span> <span data-ttu-id="c6763-108">المنشئ الجديد هو **new()**.</span><span class="sxs-lookup"><span data-stu-id="c6763-108">The default constructor is **new()**.</span></span> <span data-ttu-id="c6763-109">فيما يلي مثال على الإعلان عن متغير وإنشاء مثيل لكائن باستدعاء الأسلوب الجديد:</span><span class="sxs-lookup"><span data-stu-id="c6763-109">The following is an example of declaring a variable and creating an instance of an object by calling the new method:</span></span>

    ```xpp
    Sample mySample; //this declares a variable to refer to a sample object
            
    mySample = new Sample(); //this creates an instance of a sample object
    ```

- <span data-ttu-id="c6763-110">**أسلوب الإنهاء** - أسلوب متلف يُنهي مثيل فئة عن طريق استخدام الكلمة الأساسية `finalize`.</span><span class="sxs-lookup"><span data-stu-id="c6763-110">**Finalize method** - A destructor method that finalizes an instance of a class by using the `finalize` keyword.</span></span> <span data-ttu-id="c6763-111">فيما يلي مثال، باستخدام عبارة `if`، التي توضح كيفية استدعاء أسلوب الإنهاء.</span><span class="sxs-lookup"><span data-stu-id="c6763-111">The following is an example, using an `if` statement, which shows how to call a finalize method:</span></span>
    
    ```xpp
    if (condition) //state the condition that should be met
    {
    this.finalize();
    }
    ```

- <span data-ttu-id="c6763-112">**الأسلوب الرئيسي** - إنشاء مثيل لكائن واستدعاء أساليب الأعضاء المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="c6763-112">**Main method** - Creates an instance of an object and calls the required member methods.</span></span> <span data-ttu-id="c6763-113">إنه أسلوب فئة يتم تشغيل مباشرةً من خيار قائمة.</span><span class="sxs-lookup"><span data-stu-id="c6763-113">It is a class method that is run directly from a menu option.</span></span> <span data-ttu-id="c6763-114">لتحويل البيانات إلى الأسلوب، استخدم معلمة `_args`.</span><span class="sxs-lookup"><span data-stu-id="c6763-114">To transfer data to the method, use the `_args` parameter.</span></span> <span data-ttu-id="c6763-115">فيما يلي مثال للبنية المستخدمة لتحديد أسلوب رئيسي:</span><span class="sxs-lookup"><span data-stu-id="c6763-115">The following is an example of the syntax that is used to define a main method:</span></span>

    ```xpp
    Static void main (Args _args)
    {
        //This comment represents where you would insert your code.
    }
    ```

- <span data-ttu-id="c6763-116">**أسلوب المثيل** - يُشار إليه أيضاً باسم أسلوب الكائن، وهو مضمن في كل كائن يتم إنشاؤه من الفئة التي تحتوي على أسلوب المثيل.</span><span class="sxs-lookup"><span data-stu-id="c6763-116">**Instance method** - Also referred to as an object method, it is embedded in each object that is created from the class that contains the instance method.</span></span> <span data-ttu-id="c6763-117">قبل أن تتمكن من استخدام الأسلوب، يجب إنشاء مثيل لهذا الكائن.</span><span class="sxs-lookup"><span data-stu-id="c6763-117">Before you can use the method, you must instantiate that object.</span></span> <span data-ttu-id="c6763-118">ما يلي هو مثال على البنية المستخدمة لاستدعاء أسلوب مثيل:</span><span class="sxs-lookup"><span data-stu-id="c6763-118">The following is an example of the syntax that is used to call an instance method:</span></span>

    ```xpp
    ClassName objectReference = new ClassName();
    objectHandleName.methodName();
    ```

- <span data-ttu-id="c6763-119">**الأسلوب الثابت** - يُشار إليه أيضاً كأسلوب فئة، ويستخدم الكلمة الأساسية `static` وينتمي إلى فئة.</span><span class="sxs-lookup"><span data-stu-id="c6763-119">**Static method** - Also referred to as a class method, it uses the `static` keyword and belongs to a class.</span></span> <span data-ttu-id="c6763-120">باستخدام أسلوب ثابت، على عكس أسلوب المثيل، لا تحتاج إلى إنشاء مثيل لكائن قبل استخدام الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="c6763-120">With a static method, unlike with an instance method, you don't need to instantiate an object before you use the method.</span></span> <span data-ttu-id="c6763-121">تُستخدم الأساليب الثابتة بشكل شائع للعمل مع البيانات المخزنة في الجداول.</span><span class="sxs-lookup"><span data-stu-id="c6763-121">Static methods are commonly used to work with data that is stored in tables.</span></span> <span data-ttu-id="c6763-122">فيما يلي مثال على البنية المستخدمة لاستدعاء أسلوب ثابت:</span><span class="sxs-lookup"><span data-stu-id="c6763-122">The following is an example of the syntax that is used to call a static method:</span></span>

    ```xpp
    ClassName::methodName();
    ```
<span data-ttu-id="c6763-123">يمكن استخدام الكلمات الأساسية الخاصة بالوصول للتحكم في ما إذا كانت الأساليب في الفئات الأخرى يمكنها استدعاء الأساليب الموجودة في فئتك.</span><span class="sxs-lookup"><span data-stu-id="c6763-123">Accessor keywords can be used to control whether the methods in other classes can call the methods in your class.</span></span> <span data-ttu-id="c6763-124">يتأثر توريث الفئات أيضاً بالكلمات الأساسية الموصلة التالية.</span><span class="sxs-lookup"><span data-stu-id="c6763-124">Class inheritance is also affected by the following accessor keywords.</span></span>

- <span data-ttu-id="c6763-125">**`public`** - يمكن استدعاء الأساليب التي تم الإعلان عنها على أنها `public` من أي مكان يمكن للفئة الوصول إليه.</span><span class="sxs-lookup"><span data-stu-id="c6763-125">**`public`** - Methods declared as `public` can be called from anywhere that the class is accessible.</span></span> <span data-ttu-id="c6763-126">يمكن تجاوز أسلوب `public` بفئة فرعية، ما لم يتم الإعلان عن هذا الأسلوب كـ `final`.</span><span class="sxs-lookup"><span data-stu-id="c6763-126">A `public` method can be overridden by a subclass, unless that method is declared as `final`.</span></span>

- <span data-ttu-id="c6763-127">**`protected`** - يمكن استدعاء الأساليب التي تم تعريفها على أنها `protected` فقط من الأساليب في الفئة أو الأساليب الموجودة في فئة فرعيه لهذه الفئة.</span><span class="sxs-lookup"><span data-stu-id="c6763-127">**`protected`** - Methods declared as `protected` can only be called from methods in the same class or methods in a subclass of that class.</span></span> <span data-ttu-id="c6763-128">لا يزال من الممكن تجاوز أسلوب `protected` في فئة فرعية.</span><span class="sxs-lookup"><span data-stu-id="c6763-128">A `protected` method can still be overridden in a subclass.</span></span>

- <span data-ttu-id="c6763-129">**`private`** - يمكن استدعاء الأساليب التي تم تعريفها على أنها `private` من الأساليب فقط ضمن نفس الفئة.</span><span class="sxs-lookup"><span data-stu-id="c6763-129">**`private`** - Methods declared as `private` can only be called from methods within the same class.</span></span> <span data-ttu-id="c6763-130">بخلاف الأساليب `public` و`protected`، لا يمكن تجاوز أساليب `private` في فئة فرعية.</span><span class="sxs-lookup"><span data-stu-id="c6763-130">Unlike `public` and `protected` methods, `private` methods can't be overridden in a subclass.</span></span>
