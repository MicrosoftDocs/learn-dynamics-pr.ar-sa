---
ms.openlocfilehash: 4f71a51ae9da899f82d52a357cf2e4203a3182b7
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071946"
---
<span data-ttu-id="1c9f1-101">تُستخدَم العبارات المشروطة لتحديد ما إذا كان يجب تشغيل كتلة كود.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-101">Conditional statements are used to determine if a block of code should be run.</span></span> <span data-ttu-id="1c9f1-102">وتتمتع العبارات المشروطة المختلفة بمزايا واستخدامات تختلف تبعاً للموقف.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-102">Different conditional statements have different advantages and uses depending on the situation.</span></span> <span data-ttu-id="1c9f1-103">العبارات المشروطة الأربعة هي: if وif...else وswitch وعوامل التشغيل الثلاثية.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-103">The four conditional statements are: if, if...else, switch, and ternary operators.</span></span> 

## <a name="if-statement"></a><span data-ttu-id="1c9f1-104">عبارة If</span><span class="sxs-lookup"><span data-stu-id="1c9f1-104">If statement</span></span>  

<span data-ttu-id="1c9f1-105">تقيِّم العبارة `if` ما إذا كان التعبير صحيحاً أم لا.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-105">The `if` statement evaluates whether an expression is true.</span></span> <span data-ttu-id="1c9f1-106">إذا كان التعبير صحيحاً، فسيشغِّل مجموعة من العبارات المسردة في الأقواس.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-106">If the expression is true, it will run the set of statements that are listed in the braces.</span></span> <span data-ttu-id="1c9f1-107">في عبارة `if` التالية، تتحقق العبارة من التعبير الذي بين الأقواس.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-107">In the following `if` statement, the statement checks the expression in parentheses.</span></span> <span data-ttu-id="1c9f1-108">وفي هذه الحالة، تتحقق العبارة مما إذا كان المتغير x يساوي 5.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-108">In this case, the statement checks if the variable x is equal to 5.</span></span> <span data-ttu-id="1c9f1-109">وإذا كان التعبير صحيحاً، فسيتم تشغيل الكود الذي في الأقواس.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-109">If the expression is true, then the code in the braces will run.</span></span> <span data-ttu-id="1c9f1-110">أما إذا كان التعبير خطأ، فسيتم تخطي الكود الذي بين الأقواس.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-110">If the expression is false, the code in the braces is skipped.</span></span> <span data-ttu-id="1c9f1-111">تأخذ العبارة `if` عبارة واحدة بالضبط للتشغيل.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-111">The `if` statement takes exactly one statement to run.</span></span> <span data-ttu-id="1c9f1-112">يمكن أن تحتوي الأقواس على قائمة عبارات محاطة في عبارة واحدة، تسمى عبارة مركبة.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-112">The braces can contain a list of statements that are enclosed into one statement, called a compound statement.</span></span>
```xpp
if (x == 5)
{
    info('X equals five');
}
```
## <a name="ifelse-statement"></a><span data-ttu-id="1c9f1-113">عبارة If...else</span><span class="sxs-lookup"><span data-stu-id="1c9f1-113">If...else statement</span></span>  

<span data-ttu-id="1c9f1-114">يمكنك تعيين العبارات كي يتم تشغيلها عندما يكون التعبير خاطئاً باستخدام العبارة `if...else`.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-114">You can set statements to run when the expression is false by using the `if...else` statement.</span></span> <span data-ttu-id="1c9f1-115">يمكنك إنشاء عبارة `if` عادية، ولكن في نهاية عبارة `if`، ستستخدم الكلمة الأساسية `else` متبوعة بأقواس، كما يوضح المثال التالي.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-115">You can create a normal `if` statement, but at the end of the `if` statement, you will use the keyword `else` followed by brackets, as shown in the following example.</span></span> <span data-ttu-id="1c9f1-116">يمكنك إضافة المزيد من الأكواد في الأقواس التي سيتم تشغيلها عندما يكون التعبير الموجود في العبارة `if` خطأ.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-116">You can add more code in the brackets that will run when the expression in the `if` statement is false.</span></span> <span data-ttu-id="1c9f1-117">في المثال التالي، تتحقق العبارة مما إذا كان x يساوي 5.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-117">In the following example, the statement checks if x is equal to 5.</span></span> <span data-ttu-id="1c9f1-118">وإذا كان الأمر كذلك، فسيتم تشغيل عبارة x المعلوماتية.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-118">If it is, it will run the info x statement.</span></span> <span data-ttu-id="1c9f1-119">وإذا لم يكن يساوي 5، فسيتم تشغيل عبارة "X لا تساوي 5" المعلوماتية.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-119">If it is not equal to 5, it will run the info "X does not equal 5" statement.</span></span>
```xpp
if (x == 5)
{
    info('x equals five');
}
else
{
    info('x does not equal five');
}
```
<span data-ttu-id="1c9f1-120">يمكنك استخدام عوامل التشغيل في عوامل التشغيل الارتباطية الخاصة بالشرط لتحديد ما إذا كان التعبير صحيحاً أم خاطئاً.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-120">You can use operators in the condition’s relational operators to determine if the expression is true or false.</span></span> <span data-ttu-id="1c9f1-121">يمكنك استخدام عوامل التشغيل && و|| في التعبيرات الخاصة بك لتحديد ما إذا كان يجب أن يكون تعبيران أو أكثر صحيحين، أو أن تعبيراً واحداً فقط من عدة تعبيرات يجب أن يكون صحيحاً.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-121">You can use the operators && and || in your expressions to determine if two or more expressions must be true, or only one expression out of many must be true.</span></span>
<span data-ttu-id="1c9f1-122">بالإضافة إلى ذلك، يمكنك تضمين عبارات `if` للتحقق من تعبيرات متعددة، ولكن إذا كنت تقوم بتضمين عبارات `if` متعددة، فقد تحتاج إلى التفكير في عبارة switch.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-122">Additionally, you can nest `if` statements to check for multiple expressions, but if you are nesting multiple `if` statements, you might want to consider a switch statement.</span></span>

## <a name="switch-statement"></a><span data-ttu-id="1c9f1-123">عبارة Switch</span><span class="sxs-lookup"><span data-stu-id="1c9f1-123">Switch statement</span></span>  

<span data-ttu-id="1c9f1-124">عبارة `switch` هي عبارة شرطية متعددة الأفرع يتم التحقق منها مقابل عدة حالات.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-124">A `switch` statement is a multibranch conditional statement that is checked against multiple cases.</span></span> <span data-ttu-id="1c9f1-125">فإذا كانت إحدى قيم الحالات مساوية لتعبير switch، فيتم تشغيل عبارة الحالة.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-125">If one of the case values are equal to the switch expression, then the case statement is run.</span></span> <span data-ttu-id="1c9f1-126">تستخدم عبارات الحالة عبارة فصل لإعلام الأكواد بتشغيل عبارة switch، والذي سيمنع تشغيل العبارة التالية.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-126">The case statements use a break statement to tell the code to start running the switch statement, which will prevent the next statement from being run.</span></span>
<span data-ttu-id="1c9f1-127">كما يمكنك أيضاً تعيين عبارة افتراضية إذا لم يكن أي تعبير حالة مطابقاً.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-127">You can also set a default statement if no case expressions match.</span></span> <span data-ttu-id="1c9f1-128">يوضح المثال التالي عبارة switch، يتم فيها التحقق من قيمة المتغير x مقابل حالات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-128">The following example shows a switch statement where the value for variable x is checked against different cases.</span></span> <span data-ttu-id="1c9f1-129">إذا كان x يساوي 5، فإنه يقوم بتشغيل الكود الموجود ضمن هذه الحالة حتى تصل إلى عبارة فصل.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-129">If x is 5, then it runs the code under that case until it comes to a break statement.</span></span> <span data-ttu-id="1c9f1-130">وإذا كان x يساوي 10، فإنه يقوم بتشغيل الكود الموجود ضمن هذه الحالة.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-130">If x is 10, it runs the code under that case.</span></span> <span data-ttu-id="1c9f1-131">إذا لم تكن x تساوي 5 ولا 10، فإنها تقوم بتشغيل الكود ضمن العبارة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-131">If x is neither 5 nor 10, it runs the code under the default statement.</span></span>
```xpp
Switch (x)
        {
    Case 5:
        //do something
        break;
    Case 10:
        //do something
        break;
    default:
        //do something
        break;
}
```
## <a name="using-iterative-statements"></a><span data-ttu-id="1c9f1-132">استخدام العبارات التكرارية</span><span class="sxs-lookup"><span data-stu-id="1c9f1-132">Using iterative statements</span></span>  

<span data-ttu-id="1c9f1-133">العبارات التكرارية أو الحلقات، تكرر كتلة عبارة حتى يتم استيفاء أحد الشروط.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-133">Iterative statements, or loops, repeat a statement block until a condition has been satisfied.</span></span> <span data-ttu-id="1c9f1-134">وتُستخدم هذه الأنواع من العبارات التكرارية بلغة X++‎.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-134">These types of iterative statements are used in X++.</span></span>

<span data-ttu-id="1c9f1-135">الحلقات هي بنيات تكرارية.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-135">Loops are repetitive constructs.</span></span> <span data-ttu-id="1c9f1-136">تحتوي X++‎ على ثلاثة أنواع من الحلقات هي:</span><span class="sxs-lookup"><span data-stu-id="1c9f1-136">X++ has three kinds of loops:</span></span>

-   <span data-ttu-id="1c9f1-137">while</span><span class="sxs-lookup"><span data-stu-id="1c9f1-137">while</span></span> 
-   <span data-ttu-id="1c9f1-138">do...while</span><span class="sxs-lookup"><span data-stu-id="1c9f1-138">do...while</span></span> 
-   <span data-ttu-id="1c9f1-139">for</span><span class="sxs-lookup"><span data-stu-id="1c9f1-139">for</span></span> 

<span data-ttu-id="1c9f1-140">ويمكن جمع الحلقات مع ما يلي:</span><span class="sxs-lookup"><span data-stu-id="1c9f1-140">Loops can be combined with the following:</span></span>

-   <span data-ttu-id="1c9f1-141">عبارات الفصل</span><span class="sxs-lookup"><span data-stu-id="1c9f1-141">break statements</span></span>
-   <span data-ttu-id="1c9f1-142">عبارات الاستمرار</span><span class="sxs-lookup"><span data-stu-id="1c9f1-142">continue statements</span></span>

## <a name="while-loops"></a><span data-ttu-id="1c9f1-143">حلقات While</span><span class="sxs-lookup"><span data-stu-id="1c9f1-143">While loops</span></span>  

<span data-ttu-id="1c9f1-144">تتيح لك حلقة `while` تشغيل عبارة واحدة بشكل متكرر أو عبارة مركبة إذا كان أحد الشروط صحيحاً.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-144">A `while` loop enables you to repeatedly run one statement or a compound statement if a condition is true.</span></span> <span data-ttu-id="1c9f1-145">ويتم تشغيل العبارة من صفر (وليس على الإطلاق) إلى عدة مرات، حسب عدد المرات التي يقيِّم فيها الشرط وصولاً إلى "صواب".</span><span class="sxs-lookup"><span data-stu-id="1c9f1-145">The statement is run from zero (not at all) to many times, depending on how many times the condition evaluates to true.</span></span> <span data-ttu-id="1c9f1-146">ويتناقض هذا مع حلقة `do...while` ، حيث يتم دائماً تشغيل العبارات مرة واحدة على الأقل قبل تقييم الشرط.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-146">This contrasts with a `do...while` loop, where the statements are always run at least once before the condition is evaluated.</span></span>
```xpp
int loopCount = 1;
container cont;

while (loopCount <= conlen(cont))
{
    print conpeek(cont,loopCount);
    loopCount = loopCount + 1;
}
```
## <a name="dowhile-loops"></a><span data-ttu-id="1c9f1-147">حلقات Do...while</span><span class="sxs-lookup"><span data-stu-id="1c9f1-147">Do...while loops</span></span> 

<span data-ttu-id="1c9f1-148">تشبه حلقة `do...while` حلقة `while`، ولكن تختلف في أن الشرط التالي يتبع العبارات.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-148">The `do...while` loop is like the `while` loop but differs in that the condition follows the statements.</span></span> <span data-ttu-id="1c9f1-149">يتم دائماً تنفيذ العبارات مرة واحدة على الأقل.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-149">The statements are always performed at least once.</span></span> <span data-ttu-id="1c9f1-150">تناسب حلقة `do...while` على أفضل نحو المهام التي يجب إجراؤها دائماً مرة واحدة على الأقل، مثلاً للحصول على محددات لتقرير.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-150">The `do...while` loop is well suited for tasks that always must be done at least once, for example, to get parameters for a report.</span></span>
```xpp
int FindPower(real _Value)
    {
        int ex=-1;
        real curVal;

        do
        {
            ex += 1;
            curVal = power(10, ex);
        }

        while (_Value > curVal);

        return ex;
    }
```
## <a name="for-loops"></a><span data-ttu-id="1c9f1-151">لحلقات For</span><span class="sxs-lookup"><span data-stu-id="1c9f1-151">For loops</span></span> 

<span data-ttu-id="1c9f1-152">تشبه حلقة `for` حلقة `while`، ولكنها تحتوي على الإضافات التالية:</span><span class="sxs-lookup"><span data-stu-id="1c9f1-152">The `for` loop is similar to the `while` loop, but has the following additions:</span></span>

-   <span data-ttu-id="1c9f1-153">يمكن تعيين القيمة الأولية إلى متغير عنصر تحكم.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-153">The initial value to a control variable can be assigned.</span></span>
-   <span data-ttu-id="1c9f1-154">وتحتوي على عبارة لتحديث المتغير.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-154">It contains a statement for updating the variable.</span></span>

<span data-ttu-id="1c9f1-155">تجعل هذه الإضافات العبارة ذات فائدة خاصة لعبور القوائم والحاويات والمصفوفات نظراً لاحتوائها على عدد ثابت من العناصر.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-155">These additions make it especially useful for traversing lists, containers, and arrays because they have a fixed number of elements.</span></span> <span data-ttu-id="1c9f1-156">يمكنك أيضاً تطبيق عبارة على كل عنصر والتزايد وصولاً إلى العناصر، وتعيين الشرط للاختبار للعنصر الأخير.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-156">You can also apply a statement to each element and increment your way through the elements, setting the condition to test for the last element.</span></span>
```xpp
for (int i=1; i<=100; i+=1)
{
    print ra[i];
}
```
## <a name="break-statements"></a><span data-ttu-id="1c9f1-157">عبارات الفصل</span><span class="sxs-lookup"><span data-stu-id="1c9f1-157">Break statements</span></span> 

<span data-ttu-id="1c9f1-158">توفر X++‎ عبارة `break` لما يلي:</span><span class="sxs-lookup"><span data-stu-id="1c9f1-158">X++ provides a `break` statement for the following:</span></span>

-   <span data-ttu-id="1c9f1-159">إنهاء الحلقات</span><span class="sxs-lookup"><span data-stu-id="1c9f1-159">Terminating loops</span></span>
-   <span data-ttu-id="1c9f1-160">فصل عبارات الحالة في عبارة switch</span><span class="sxs-lookup"><span data-stu-id="1c9f1-160">Separation of case statements in a switch statement</span></span>

<span data-ttu-id="1c9f1-161">عند استخدام الحلقة داخل حلقة `while` أو  `do...while` أو  `for` يتم إنهاؤها ويستمر التنفيذ من العبارة التي تلي التكرار الحلقي، كما يوضح المثال التالي.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-161">When used within a `while`, `do...while`, or `for` loop, the loop is terminated and implementation continues from the statement that follows the loop, as shown in the following example.</span></span>
```xpp
mainMenu = SysDictMenu::newMainMenu();
enum = mainMenu.getEnumerator();
found = false;

while (enum.moveNext())
{
    menuItem = enum.current();
    if (menuItem.label() == parentDictsecuritykey.label())
    {
        found = true;
        break;
    }
}
if (found) //Belongs in Navigation Pane.
{
    ...
}
```
<span data-ttu-id="1c9f1-162">عند استخدام break داخل [عبارة Switch](https://docs.microsoft.com/dynamicsax-2012/developer/switch-statements/?azure-portal=true) ، ينتهي تشغيل فرع الحالة ويتم تشغيل العبارة التي تلي switch، كما يوضح المثال التالي.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-162">When break is used within a [Switch Statement](https://docs.microsoft.com/dynamicsax-2012/developer/switch-statements/?azure-portal=true) statement, the running of the case branch terminates and the statement that follows the switch is run as shown in the following example.</span></span>
```xpp
switch (Debtor.AccountNo)
{
    case "1000":  do_something;
            break;
    case "2000": do_something_else;
            break;
    default: default_statement; 
            break;
}
```
<span data-ttu-id="1c9f1-163">وإذا كان رقم حساب المدين 1000، فإن البرنامج يشغِّل `do_something` ثم يستمر في تشغيله بعد عبارة switch.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-163">If the Debtor account number is 1000, the program runs `do_something` and then continues running after the switch statement.</span></span> <span data-ttu-id="1c9f1-164">إذا كان لديك break داخل حلقة، فإنك تحتاج إلى فصله عن الحلقة.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-164">If you have a break within a loop, you need to break out of the loop.</span></span> <span data-ttu-id="1c9f1-165">وإذا كان لديك استمرار داخل حلقة، فإنه يُنهي التكرار الحالي ويُعيد تقييم شرط الحلقة.</span><span class="sxs-lookup"><span data-stu-id="1c9f1-165">If you have a continue within a loop, it ends the current iteration and reevaluates the loop condition.</span></span>

<span data-ttu-id="1c9f1-166">شاهد الفيديو التالي للتعرف على العبارات المشروطة:</span><span class="sxs-lookup"><span data-stu-id="1c9f1-166">Watch the following video to learn about conditional statements:</span></span>  

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4byCj]
