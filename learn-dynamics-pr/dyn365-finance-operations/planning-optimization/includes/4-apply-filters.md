---
ms.openlocfilehash: 5ce17c9a89d2277cf40c81e9b4b38258d7196a7f
ms.sourcegitcommit: 01f8d224bf1e548ba0cbe53b3e2150c43302c125
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "6072093"
---
<span data-ttu-id="26d78-101">عند استخدام "تحسين التخطيط"، يمكنك تطبيق عامل تصفية على خطة.</span><span class="sxs-lookup"><span data-stu-id="26d78-101">When using Planning Optimization, you can apply a filter to a plan.</span></span> <span data-ttu-id="26d78-102">سيجعل عامل التصفية الخطة تقتصر على مجموعة محددة من العناصر ويضمن عدم تضمين أي عناصر أخرى كجزء من الحسابات.</span><span class="sxs-lookup"><span data-stu-id="26d78-102">A plan filter will limit a plan to a specific group of items and make sure that no other items are included as part of the calculations.</span></span> 

<span data-ttu-id="26d78-103">يمكن تطبيق عوامل تصفية الخطة وعوامل تصفية وقت التشغيل، التي تقوم بتعيينها عند تشغيل خطة ما، عند تشغيل التخطيط الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="26d78-103">Plan filters and runtime filters, that you set when running a plan, can be applied when you run master planning.</span></span> <span data-ttu-id="26d78-104">يتم تضمين تقاطع عاملين من عوامل التصفية فقط في تشغيل التخطيط.</span><span class="sxs-lookup"><span data-stu-id="26d78-104">Only the intersection of the two filters is included in the planning run.</span></span> 

<span data-ttu-id="26d78-105">لا ينتج عن تشغيل "تحسين التخطيط" الذي تمت تصفيته لوقت التشغيل حذف النتائج الحالية في الخطة الناتجة عن تشغيل سابق.</span><span class="sxs-lookup"><span data-stu-id="26d78-105">A runtime filtered Planning Optimization run does not delete current results in the plan from a previous run.</span></span> <span data-ttu-id="26d78-106">على سبيل المثال، إذا قمت بتشغيل خطة للعنصر أ، فستمنحك نتائج للعنصر أ، ويتم الاحتفاظ بهذه الأوامر عند تشغيل خطة تمت تصفيتها للعنصر ب. سيتضمن التشغيل الثاني الآن أ وب.</span><span class="sxs-lookup"><span data-stu-id="26d78-106">For example, if you run a plan for item A, it will give you results for item A, and these orders are kept when you run a plan that is filtered for item B. The second run will now include A and B.</span></span> 

<span data-ttu-id="26d78-107">لا يحتفظ التشغيل الذي لم يتم تصفيته سوى بالأوامر المخططة المعتمدة بين عمليات التشغيل.</span><span class="sxs-lookup"><span data-stu-id="26d78-107">An unfiltered run only keeps approved planned orders between runs.</span></span> 

<span data-ttu-id="26d78-108">يمكن الوصول إلى **عامل تصفيه الخطة** من **التخطيط الرئيسي > الإعداد > الخطط > الخطط الرئيسية** عندما تكون خاصية تحسين التخطيط مفعلة.</span><span class="sxs-lookup"><span data-stu-id="26d78-108">The **Plan filter** can be accessed from **Master planning > Setup > Plans > Master plans** when Planning Optimization is active.</span></span> <span data-ttu-id="26d78-109">تُظهر لقطات الشاشة التالية علامة تبويب **عامل تصفية الخطة** وصفحة **الاستعلام**.</span><span class="sxs-lookup"><span data-stu-id="26d78-109">The following screenshots show the **Plan filter** tab and the **Inquiry** page.</span></span>

![لقطة شاشة لصفحة الخطط الرئيسية تبرز علامة تبويب عامل تصفية الخطة.](../media/filters-1-ssm.png)


<span data-ttu-id="26d78-111">[ ![ لقطة شاشة لصفحة الاستعلام الخاصة بعامل تصفية الخطة.](../media/filters-2-ss.png) ](../media/filters-2-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="26d78-111">[ ![ Screenshot of the Plan filter Inquiry page.](../media/filters-2-ss.png) ](../media/filters-2-ss.png#lightbox)</span></span>


## <a name="example"></a><span data-ttu-id="26d78-112">مثال</span><span class="sxs-lookup"><span data-stu-id="26d78-112">Example</span></span>

<span data-ttu-id="26d78-113">يوضح الرسم البياني التالي ما يحدث عند تخصيص عامل تصفية الخطة للعناصر أ وب وج، ويضم أيضاً عامل تصفية وقت التشغيل الذي يتم تعيينه عند تشغيل خاصية تحسين التخطيط.</span><span class="sxs-lookup"><span data-stu-id="26d78-113">The following diagram shows what happens when the Plan filter is for Items A, B, and C, and it also has a runtime filter that is set when the Planning Optimization is run.</span></span> <span data-ttu-id="26d78-114">في الرسم البياني، تمثل المربعات المسماة 1 و2 و3 و4 عمليات تشغيل التخطيط الرئيسي، ولكل منها عامل تصفية لوقت التشغيل إلى جانب عامل تصفية الخطة.</span><span class="sxs-lookup"><span data-stu-id="26d78-114">In the diagram, the boxes that are labeled 1, 2, 3, and 4 represent master planning runs, each with a runtime filter along with the plan filter.</span></span> 

<span data-ttu-id="26d78-115">تكتمل عمليات التشغيل بالتسلسل وتُترك النتيجة من التشغيل السابق دون تغيير.</span><span class="sxs-lookup"><span data-stu-id="26d78-115">The runs are completed in sequence and the result from the previous run is left untouched.</span></span> 

<span data-ttu-id="26d78-116">علي سبيل المثال، في عملية التشغيل الثانية، يقوم عامل تصفية وقت التشغيل في العنصر أ ود وعامل تصفية الخطة الخاص بالعنصر أ وب وج بتوفير النتائج للعنصر أ.</span><span class="sxs-lookup"><span data-stu-id="26d78-116">For example, in the second run, a runtime filter on A and D and a plan filter of A, B, and C will provide results for item A.</span></span> 

<span data-ttu-id="26d78-117">في عملية التشغيل الثالثة، يتم الاحتفاظ بالنتيجة الخاصة بالعنصر أ من عملية التشغيل الثانية كعملية تشغيل تمت تصفيتها ولا تتضمن إعادة احتساب للعنصر أ بل ب فحسب.</span><span class="sxs-lookup"><span data-stu-id="26d78-117">In the third run, the result for A from the second run is kept as a filtered run that does not include a recalculation for A but only B.</span></span>


<span data-ttu-id="26d78-118">[ ![رسم بياني يمثل ما يحدث عندما يكون عامل تصفيه الخطة خاص بالعناصر أ وب وج ويضم أيضاً عامل تصفية وقت التشغيل.](../media/filters-3-c.png) ](../media/filters-3-c.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="26d78-118">[ ![Diagram representing what happens when the Plan filter is for Items A, B, and C and it also has a runtime filter.](../media/filters-3-c.png) ](../media/filters-3-c.png#lightbox)</span></span>

 
<span data-ttu-id="26d78-119">شاهد الفيديو التالي لمعرفة كيفية استخدام عوامل تصفية الخطة.</span><span class="sxs-lookup"><span data-stu-id="26d78-119">Watch the following video to see how to use plan filters.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4Ihni]



