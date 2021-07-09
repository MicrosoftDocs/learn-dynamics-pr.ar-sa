---
ms.openlocfilehash: b8ea19b46ed9002bde959f182ba79e15493cd725
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072324"
---
<span data-ttu-id="c501f-101">النطاق هو المنطقة التي يوجد بها أحد الأصناف أو يمكن الوصول إليه منها.</span><span class="sxs-lookup"><span data-stu-id="c501f-101">Scope is the area where an item is located or can be accessed.</span></span> <span data-ttu-id="c501f-102">توجد متغيرات X++‎ وأساليبها داخل نطاق محدد.</span><span class="sxs-lookup"><span data-stu-id="c501f-102">X++ variables and methods are within a defined scope.</span></span> <span data-ttu-id="c501f-103">يمكن تعيين النطاق بواسطة وضع الإقرار واستخدام معرفات الوصول.</span><span class="sxs-lookup"><span data-stu-id="c501f-103">The scope can be set by the placement of declaration and the use of access identifiers.</span></span>
 
<span data-ttu-id="c501f-104">معرفات الوصول هي `[public]` و`[protected]` و`[private]`.</span><span class="sxs-lookup"><span data-stu-id="c501f-104">Access identifiers are `[public]`, `[protected]`, and `[private]`.</span></span>
 
-   <span data-ttu-id="c501f-105">**عام** - يمكن استدعاء الأساليب التي تم إقرارها باعتبارها عامة من أي مكان يمكن للفئة الوصول إليه.</span><span class="sxs-lookup"><span data-stu-id="c501f-105">**Public** - Methods that are declared as public can be called from anywhere that the class is accessible.</span></span> <span data-ttu-id="c501f-106">بالإضافة إلى ذلك، يمكن تجاوز أسلوب عام بواسطة فئة فرعية ما لم يتم إقرار الأسلوب كنهائي.</span><span class="sxs-lookup"><span data-stu-id="c501f-106">In addition, a public method can be overridden by a subclass unless the method is declared as final.</span></span>
-   <span data-ttu-id="c501f-107">**محمي** - يمكن تجاوز الأساليب المحمية في الفئات الفرعية.</span><span class="sxs-lookup"><span data-stu-id="c501f-107">**Protected** - Methods that are protected can be overridden in subclasses.</span></span> <span data-ttu-id="c501f-108">يمكن استدعاء الأساليب التي تم إعلانها على أنها محمية فقط من:</span><span class="sxs-lookup"><span data-stu-id="c501f-108">Methods that are declared as protected can be called only from:</span></span>
    -   <span data-ttu-id="c501f-109">الأساليب الموجودة في الفئة.</span><span class="sxs-lookup"><span data-stu-id="c501f-109">Methods in the class.</span></span>
    -   <span data-ttu-id="c501f-110">الأساليب الموجودة في فئة فرعية خاصة بفئة تحتوي على الأسلوب المحمي.</span><span class="sxs-lookup"><span data-stu-id="c501f-110">Methods in a subclass of the class that contains the protected method.</span></span>
-   <span data-ttu-id="c501f-111">**خاص** - يمكن استدعاء الأساليب التي تم إقرارها كخاصة فقط من الأساليب الموجودة في الفئة التي تم إقرار الأسلوب الخاص منها.</span><span class="sxs-lookup"><span data-stu-id="c501f-111">**Private** - Methods that are declared as private can be called only from methods in the class where the private method is declared.</span></span>
    <span data-ttu-id="c501f-112">لا يمكن تجاوز أي أسلوب خاص في فئة فرعية.</span><span class="sxs-lookup"><span data-stu-id="c501f-112">No private method can be overridden in a subclass.</span></span> <span data-ttu-id="c501f-113">عندما تقوم بإنشاء أسلوب جديد، تكون الكلمة الأساسية للموصل الافتراضي التي تظهر في محرر الأكواد خاصة.</span><span class="sxs-lookup"><span data-stu-id="c501f-113">When you create a new method, the default accessor keyword that appears in the code editor is private.</span></span> <span data-ttu-id="c501f-114">وهذا هو الوضع الافتراضي الأكثر محافظة لأقصى حد من الأمان.</span><span class="sxs-lookup"><span data-stu-id="c501f-114">This is the most conservative default for maximum security.</span></span>

## <a name="internal"></a><span data-ttu-id="c501f-115">‏‏داخلي</span><span class="sxs-lookup"><span data-stu-id="c501f-115">Internal</span></span>

<span data-ttu-id="c501f-116">*داخلي* هي كلمة أساسية في X++‎.</span><span class="sxs-lookup"><span data-stu-id="c501f-116">*Internal* is a keyword in X++.</span></span> <span data-ttu-id="c501f-117">لها نفس الدلالات التي في C#‎ انظر [داخلي (مرجع C#‎)](https://docs.microsoft.com/dotnet/csharp/language-reference/keywords/internal/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="c501f-117">It has the same semantics as in C# see [internal (C# Reference)](https://docs.microsoft.com/dotnet/csharp/language-reference/keywords/internal/?azure-portal=true).</span></span>

<span data-ttu-id="c501f-118">عندما تقوم بتحديد فئة أو أسلوب كداخلي، فإنه يمكن الوصول إليه فقط من داخل النموذج الذي يتم تعريفه فيه.</span><span class="sxs-lookup"><span data-stu-id="c501f-118">When you select a class or method as internal, it can only be accessed from within the model where it is defined.</span></span>
```xpp
internal class MyInternalClass
{
   internal void myInternalMethod()
   {
   }
}
```
<span data-ttu-id="c501f-119">لاحظ أنه يمكنك تعريف الأساليب الداخلية في الفئات العامة أيضاً.</span><span class="sxs-lookup"><span data-stu-id="c501f-119">Notice that you can define internal methods on public classes, too.</span></span>

## <a name="instance-variables"></a><span data-ttu-id="c501f-120">متغيرات المثيل</span><span class="sxs-lookup"><span data-stu-id="c501f-120">Instance variables</span></span>

<span data-ttu-id="c501f-121">تحتوي متغيرات المثيل على نطاق كبير ويشار إليها أيضاً باسم حقول الفئات في X++‎.</span><span class="sxs-lookup"><span data-stu-id="c501f-121">Instance variables have a large scope and are also referred to as class fields in X++.</span></span> <span data-ttu-id="c501f-122">يتم إقرار هذه المتغيرات في إقرار الفئة ويمكن الوصول إليها من أي أسلوب في الفئة والفئات الفرعية التي تقوم بتوسيع الفئة، إذا تم إقرارها كعامة أو محمية.</span><span class="sxs-lookup"><span data-stu-id="c501f-122">These variables are declared in the class declaration and can be accessed from any method in the class and subclasses that extend the class, if they are declared public or protected.</span></span>

## <a name="local-variables"></a><span data-ttu-id="c501f-123">المتغيرات المحلية</span><span class="sxs-lookup"><span data-stu-id="c501f-123">Local variables</span></span>

<span data-ttu-id="c501f-124">المتغيرات المحلية لها نطاق صغير.</span><span class="sxs-lookup"><span data-stu-id="c501f-124">Local variables have a small scope.</span></span> <span data-ttu-id="c501f-125">يتم تحديد هذه المتغيرات في أسلوب ويمكن الوصول إليها في هذا الأسلوب فقط.</span><span class="sxs-lookup"><span data-stu-id="c501f-125">These variables are defined in a method and can only be accessed in that method.</span></span>

<span data-ttu-id="c501f-126">المحددات هي نوع من المتغيرات المحلية التي يتم تحديدها في أسلوب.</span><span class="sxs-lookup"><span data-stu-id="c501f-126">Parameters are a kind of local variable that is defined on a method.</span></span>

<span data-ttu-id="c501f-127">لاستخدام متغير من أحد النطاقات إلى نطاق آخر، يجب تمرير المتغير باستخدام المُحددات.</span><span class="sxs-lookup"><span data-stu-id="c501f-127">To use a variable from one scope to another scope, the variable must be passed by using parameters.</span></span> <span data-ttu-id="c501f-128">يمكن للأساليب استخدام محددات متعددة.</span><span class="sxs-lookup"><span data-stu-id="c501f-128">Methods can use multiple parameters.</span></span> <span data-ttu-id="c501f-129">تُعامل المحددات مثل المتغيرات المحلية وتتم تهيئتها بالقيمة من المحدد في استدعاء الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="c501f-129">The parameters are treated like local variables and initialized with the value from the parameter in the method-call.</span></span> <span data-ttu-id="c501f-130">في المثال التالي، يكون لأسلوب الفئة مُحددان.</span><span class="sxs-lookup"><span data-stu-id="c501f-130">In the following example, the class method has two parameters.</span></span> <span data-ttu-id="c501f-131">وهذا يعطي *method1* إمكانية الوصول إلى أربعة متغيرات.</span><span class="sxs-lookup"><span data-stu-id="c501f-131">This gives *method1* access to four variables.</span></span> <span data-ttu-id="c501f-132">يمكن الوصول إلى متغيرَي المثيل *a* و *b*، ويعمل المحددان *x* و *y* كمتغيرات محلية.</span><span class="sxs-lookup"><span data-stu-id="c501f-132">The instance variables *a* and *b* can be accessed, and the parameters *x* and *y* act like local variables.</span></span> <span data-ttu-id="c501f-133">يسمح استخدام المحددات بتعيين القيم لهذه المحددات عند استدعاء الأسلوب.</span><span class="sxs-lookup"><span data-stu-id="c501f-133">Using parameters allows values to be assigned to those parameters when the method is called.</span></span> <span data-ttu-id="c501f-134">إذا تم استدعاء *الأسلوب* باستخدام الكود `Test.method1(a,b);`، فسيتم تعيين المتغير *x* على القيمة **السيارة** وسيتم تعيين المتغير *y* إلى القيمة **20**.</span><span class="sxs-lookup"><span data-stu-id="c501f-134">If *method1* is called by using the code `Test.method1(a,b);`, the *x* variable will be assigned the value **Car** and the *y* variable will be assigned the value **20**.</span></span> <span data-ttu-id="c501f-135">ثم يمكنك استخدام قيم متغيرات المحدد لتعيين القيم إلى متغيرات المثيل *c* و *d*.</span><span class="sxs-lookup"><span data-stu-id="c501f-135">You can then use the values of the parameter variables to assign values to the instance variables *c* and *d*.</span></span>

```xpp
class Test
{
     str a = "Car";
     int b = 20;
     str c;
     int d:

    void method1(str x, int y)
        {
          c = x;
          d = y;
        }
}
```

<span data-ttu-id="c501f-136">خذ في اعتبارك أنه عند تمرير قيمة من خلال المحددات، فإنك لا تغيِّر قيمة المتغير الأصلي افتراضياً.</span><span class="sxs-lookup"><span data-stu-id="c501f-136">Keep in mind that when you pass a value through parameters, you do not by default change the value of the original variable.</span></span> <span data-ttu-id="c501f-137">ويكون المصطلح الخاص بهذا هو "الاستدعاء بالقيمة" بالمقارنة بالمرجع "استدعاء حسب المرجع".</span><span class="sxs-lookup"><span data-stu-id="c501f-137">The term for this is "call by value" as opposed to "call by reference."</span></span> <span data-ttu-id="c501f-138">يتم تغيير المتغير المحلي فقط.</span><span class="sxs-lookup"><span data-stu-id="c501f-138">Only the local variable is changed.</span></span> 

### <a name="example"></a><span data-ttu-id="c501f-139">مثال</span><span class="sxs-lookup"><span data-stu-id="c501f-139">Example</span></span>

<span data-ttu-id="c501f-140">في المثال التالي، يكون لدى *method2* متغير محلي *a* بالقيمة 5.</span><span class="sxs-lookup"><span data-stu-id="c501f-140">In the following example, *method2* has a local variable *a* with a value of 5.</span></span> <span data-ttu-id="c501f-141">تعرض عبارة `info()` الأولى قيمة *a*، وهي 5.</span><span class="sxs-lookup"><span data-stu-id="c501f-141">The first `info()` statement displays the value of *a*, which is 5.</span></span> <span data-ttu-id="c501f-142">وتقوم باستدعاء *method1* وتمرير قيمة المتغير المحلي الخاص به *a*.</span><span class="sxs-lookup"><span data-stu-id="c501f-142">It calls *method1* and passes the value of its local variable *a*.</span></span> <span data-ttu-id="c501f-143">*Method1* لديه الآن متغير محلي مختلف *a*، بالقيمة 5.</span><span class="sxs-lookup"><span data-stu-id="c501f-143">*Method1* now has a different local variable *a*, with the value of 5.</span></span> <span data-ttu-id="c501f-144">ثم يزيد *Method1* القيمة بمقدار واحد، مما يؤدي إلى جعل *a* بقيمة 6.</span><span class="sxs-lookup"><span data-stu-id="c501f-144">*Method1* then increments the value by one, making *a* the value of 6.</span></span> <span data-ttu-id="c501f-145">ثم يعرض `info()` العبارة قيمة 6.</span><span class="sxs-lookup"><span data-stu-id="c501f-145">The `info()` statement then displays the value of 6.</span></span> <span data-ttu-id="c501f-146">ستعود الأكواد إلى *method2* وتقوم بتشغيل عبارة `info()` الثانية.</span><span class="sxs-lookup"><span data-stu-id="c501f-146">The code will go back to *method2* and run the second `info()` statement.</span></span> <span data-ttu-id="c501f-147">سيؤدي ذلك إلى عرض قيمة 5.</span><span class="sxs-lookup"><span data-stu-id="c501f-147">This will display a value of 5.</span></span> <span data-ttu-id="c501f-148">وذلك لأنه رغم أن اسم المتغير هو نفسه، إلا أن النطاق فريد للأساليب الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="c501f-148">This is because even though the variable name is the same, the scope is unique to their respective methods.</span></span>

```xpp
class infoValue
{
     void method1(int a)
     {
       a = a ++;
       info(int2str(a));
     }

      void method2()
      {
        int a = 5;
        info(int2str(a));
        this.method1(a);
        info(int2str(a));
      }
}

```

<span data-ttu-id="c501f-149">توضح الصورة التالية كيفية عرض *المعلومات* في واجهة المستخدم.</span><span class="sxs-lookup"><span data-stu-id="c501f-149">The following image shows how the *info* displays in the user interface.</span></span>

![تعرض لقطة الشاشة هذه طريقة عرض أسلوب المعلومات في واجهة المستخدم.](../media/info.png)

