---
ms.openlocfilehash: 9262498c017a246e12671668388dde3a093efe25
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072325"
---
<span data-ttu-id="f7c88-101">فئتا التوريث والخلاصة هما نوعان من بنيات البرمجة المهمة التي توجد في لغات البرمجة الموجهة للكائنات.</span><span class="sxs-lookup"><span data-stu-id="f7c88-101">Inheritance and abstract classes are two important programming constructs that are found in object-oriented programming languages.</span></span> <span data-ttu-id="f7c88-102">تُستخدم هذه المفاهيم لإنشاء علاقات الأصل والتابع بين الفئات.</span><span class="sxs-lookup"><span data-stu-id="f7c88-102">These concepts are used to create parent-child relationships between classes.</span></span>
<span data-ttu-id="f7c88-103">يسمح التوريث للفئة الفرعية بتوسيع فئة أعلى.</span><span class="sxs-lookup"><span data-stu-id="f7c88-103">Inheritance allows a subclass to extend a super class.</span></span> <span data-ttu-id="f7c88-104">ترث الفئة الفرعية جميع سمات الفئة الأعلى وأساليبها.</span><span class="sxs-lookup"><span data-stu-id="f7c88-104">The subclass inherits all the attributes and methods of the super class.</span></span> <span data-ttu-id="f7c88-105">يمكن للفئات الفرعية أيضاً تجاوز سلوك أو إضافة المزيد من الوظائف إلى الأساليب الموروثة من الفئة الأعلى.</span><span class="sxs-lookup"><span data-stu-id="f7c88-105">Subclasses can also override the behavior of or add more functionality to methods that are inherited from the super class.</span></span> 

## <a name="inheritance"></a><span data-ttu-id="f7c88-106">التوريث</span><span class="sxs-lookup"><span data-stu-id="f7c88-106">Inheritance</span></span>

<span data-ttu-id="f7c88-107">لفهم مفهوم التوريث بشكل أفضل في البرمجة الموجهة للكائنات، دعنا نراجع مثالاً من العالم الحقيقي.</span><span class="sxs-lookup"><span data-stu-id="f7c88-107">To better understand the concept of inheritance in object-oriented programming, lets review a real-world example.</span></span> <span data-ttu-id="f7c88-108">في هذا المثال، **المركبة** هي الفئة الأصل.</span><span class="sxs-lookup"><span data-stu-id="f7c88-108">In this example, **Vehicle** is the parent class.</span></span> <span data-ttu-id="f7c88-109">هناك العديد من أنواع المركبات المختلفة، على سبيل المثال: السيارات والحافلات والشاحنات.</span><span class="sxs-lookup"><span data-stu-id="f7c88-109">There are many different types of vehicles, for instance: cars, buses, and trucks.</span></span> <span data-ttu-id="f7c88-110">في هذا السيناريو، **المركبة** هي الفئة الأصل.</span><span class="sxs-lookup"><span data-stu-id="f7c88-110">In this scenario, **Vehicle** is the parent class.</span></span> <span data-ttu-id="f7c88-111">السيارات والحافلات والشاحنات هي فئات ترث من **المركبة**.</span><span class="sxs-lookup"><span data-stu-id="f7c88-111">Cars, buses, and trucks are derived classes that inherit from **Vehicle**.</span></span> <span data-ttu-id="f7c88-112">تحتوي فئة **المركبة** على الخصائص التي تتم مشاركتها عبر جميع أنواع المركبات (السرعة واللون والتروس مثلاً).</span><span class="sxs-lookup"><span data-stu-id="f7c88-112">The **Vehicle** class has characteristics that  are shared across all the vehicle types (speed, color, and gears for example).</span></span> <span data-ttu-id="f7c88-113">قد تختلف خصائص كل نوع من أنواع المركبات.</span><span class="sxs-lookup"><span data-stu-id="f7c88-113">The characteristics for each of the vehicles types may be different.</span></span> <span data-ttu-id="f7c88-114">على سبيل المثال، قد تحتوي الشاحنة على نظام دفع رباعي، لكن السيارة ليست كذلك.</span><span class="sxs-lookup"><span data-stu-id="f7c88-114">For instance, a truck might have all-wheel drive, but a car does not.</span></span>

![رسم تخطيطي للتوريث من الفئة الأصل "المركبة" إلى الفئات المشتقة السيارة والحافلة والشاحنة.](../media/inheritance.png)

### <a name="example"></a><span data-ttu-id="f7c88-116">مثال</span><span class="sxs-lookup"><span data-stu-id="f7c88-116">Example</span></span>

<span data-ttu-id="f7c88-117">يوضح المثال التالي كيفية استخدام فئة للتوريث.</span><span class="sxs-lookup"><span data-stu-id="f7c88-117">The following example demonstrates how a class uses inheritance.</span></span> <span data-ttu-id="f7c88-118">تقوم فئة "السيارة" بتوسيع فئة "المركبة" للحصول على الطول والعرض ولكنها تضيف أيضاً متغير عدد الركاب.</span><span class="sxs-lookup"><span data-stu-id="f7c88-118">The Car class extends the Vehicle class to get the height and width but also adds the number of passengers variable.</span></span> 

```xpp
class Vehicle
   {
    // Instance fields.
        real height;
        real width;
    // Constructor to initialize fields height and width.
    new(real _height, real _width)
    {
            height = _ height;
        width = _ width;
     }
   }

class Car extends Vehicle
    {
      // Additional instance field numberOfPassengers. Fields height and width are inherited.
      int numberOfPassengers;

     // Constructor is overridden to initialize z.
     new(real _height, real _width, int _numberOfPassengers)
     {
       // Initialize the fields.
       super(_height, _ width);
       numberOfPassengers = _numberOfPassengers;
     }
    }
 ```

## <a name="abstract"></a><span data-ttu-id="f7c88-119">الخلاصة</span><span class="sxs-lookup"><span data-stu-id="f7c88-119">Abstract</span></span> 

<span data-ttu-id="f7c88-120">يتم تحيد فئات الخلاصة بواسطة الكلمة الأساسية *الخلاصة*.</span><span class="sxs-lookup"><span data-stu-id="f7c88-120">Abstract classes are identified by the keyword *abstract*.</span></span> <span data-ttu-id="f7c88-121">لا يمكن إنشاء مثيل لها ولكنها تتطلب فئة فرعية موروثة من فئة الخلاصة.</span><span class="sxs-lookup"><span data-stu-id="f7c88-121">They cannot be instantiated but require a subclass that is inherited from the abstract class.</span></span> <span data-ttu-id="f7c88-122">تُستخدم فئات الخلاصة لتنفيذ مفهوم ستكمله الفئة الفرعية بعد ذلك.</span><span class="sxs-lookup"><span data-stu-id="f7c88-122">Abstract classes are used to implement a concept that the subclass will then complete.</span></span> <span data-ttu-id="f7c88-123">يمكن أيضاً الإعلان عن أساليب الخلاصة في فئات الخلاصة.</span><span class="sxs-lookup"><span data-stu-id="f7c88-123">Abstract methods can also be declared in abstract classes.</span></span> <span data-ttu-id="f7c88-124">لا تسمح أساليب الخلاصة بالرمز أو الإعلانات في الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="f7c88-124">Abstract methods do not allow code or declarations in the method.</span></span> <span data-ttu-id="f7c88-125">يجب أن تقوم الفئة الفرعية بتوسيع فئة الخلاصة لاستخدام أسلوب الخلاصة.</span><span class="sxs-lookup"><span data-stu-id="f7c88-125">A subclass must extend the abstract class to use the abstract method.</span></span>

### <a name="example"></a><span data-ttu-id="f7c88-126">مثال</span><span class="sxs-lookup"><span data-stu-id="f7c88-126">Example</span></span>

<span data-ttu-id="f7c88-127">فيما يلي مثال لفئة خلاصة.</span><span class="sxs-lookup"><span data-stu-id="f7c88-127">The following is an example of an abstract class.</span></span> <span data-ttu-id="f7c88-128">تقوم فئة "السيارة" بتوسيع فئة الخلاصة "المركبة"</span><span class="sxs-lookup"><span data-stu-id="f7c88-128">The Car class extends the abstract class Vehicle.</span></span> <span data-ttu-id="f7c88-129">يسمح هذا لفئة "السيارة" بتجاوز أسلوب `printInfo()` ويسمح لك بإضافة وظيفة إلى أسلوب `operate()` الذي لم يتم تضمينه في فئة الخلاصة.</span><span class="sxs-lookup"><span data-stu-id="f7c88-129">This allows the Car class to override the `printInfo()` method and it allows you to add functionality to the `operate()` method that was not included in the abstract class.</span></span>

```xpp
abstract class Vehicle
{
      str owner;
      int age;

    void printInfo()
      {
        Info(strfmt("%1, %2",owner, age));
      }
    abstract void operate()
    {
    }
 }

class Car extends Vehicle
{
     str model;
     void printInfo()
     {
            // overriding default functionality
            Info(strfmt("%1, %2, %3",owner, age, model));
     }
   void operate()
   {
        Info('running');
   }
}
 ```
