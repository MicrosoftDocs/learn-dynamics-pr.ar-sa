---
ms.openlocfilehash: d01bafa39f14c86cc1256722e64958c5503e5217
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073692"
---
<span data-ttu-id="78d55-101">تتضمن تكاليف الإنتاج تحليل التكاليف الفعلية مقابل التكاليف المقدرة لأوامر الإنتاج، وتحليل تكاليف أنشطة الإنتاج الحالية.</span><span class="sxs-lookup"><span data-stu-id="78d55-101">Production costs involve the analysis of actual costs versus estimated costs for production orders, and the analysis of costs for current production activities.</span></span>

<span data-ttu-id="78d55-102">عند تحليل تكاليف الإنتاج، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="78d55-102">When analyzing production costs, you can do the following:</span></span>

-   <span data-ttu-id="78d55-103">حساب التكاليف المقدرة لأمر إنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-103">Calculate the estimated costs for a production order.</span></span>

-   <span data-ttu-id="78d55-104">حساب سعر مبيعات مقترح بناءً على تكاليف أمر الإنتاج المقدرة.</span><span class="sxs-lookup"><span data-stu-id="78d55-104">Calculate a suggested sales price based on estimated production order costs.</span></span>

-   <span data-ttu-id="78d55-105">تحليل التكاليف الفعلية مقابل التكاليف المقدرة لأمر إنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-105">Analyze actual costs versus estimated costs for a production order.</span></span>

-   <span data-ttu-id="78d55-106">تحليل التكاليف التي تم الإبلاغ عنها لأوامر الإنتاج الحالية.</span><span class="sxs-lookup"><span data-stu-id="78d55-106">Analyze reported costs for current production orders.</span></span>

-   <span data-ttu-id="78d55-107">تحليل فروق الإنتاج لأمر إنتاج مكتمل لبند تكلفة قياسية.</span><span class="sxs-lookup"><span data-stu-id="78d55-107">Analyze production variances for a completed production order for a standard cost item.</span></span>

-   <span data-ttu-id="78d55-108">تحديد مصادر فروق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-108">Identify sources of production variances.</span></span>

-   <span data-ttu-id="78d55-109">اقترح تكاليف معيارية جديدة على أساس الفروق التاريخية.</span><span class="sxs-lookup"><span data-stu-id="78d55-109">Suggest new standard costs based on historical variances.</span></span>

-   <span data-ttu-id="78d55-110">تحليل الفروق لفترات زمنية محددة.</span><span class="sxs-lookup"><span data-stu-id="78d55-110">Analyze variances for specified time periods.</span></span>

<span data-ttu-id="78d55-111">يتم ترحيل تكاليف الإنتاج في كل مرة يتم فيها ترحيل دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="78d55-111">Production costs are posted every time a journal is posted.</span></span> <span data-ttu-id="78d55-112">تتراكم تكاليف الإنتاج في حسابي **الأصناف في الإنتاج** و **العمل قيد المعالجة** حتى يكتمل أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-112">The production costs accumulate in the **Items in production** and **Work in process** accounts until the production order is complete.</span></span>

<span data-ttu-id="78d55-113">أوامر الإنتاج غير المنتهية لها تكاليف إنتاج مقدرة استناداً إلى الكميات المقدرة، ويتم ترحيل التكاليف الفردية للكميات التي تم الإبلاغ عنها كمنتهية.</span><span class="sxs-lookup"><span data-stu-id="78d55-113">Production orders that are not ended have estimated production costs based on estimated quantities, and individual costs of quantities reported as finished are posted.</span></span> <span data-ttu-id="78d55-114">ومع ذلك، لا يتم حساب تكلفة الإنتاج المحققة حتى يتم إنهاء أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-114">However, the realized production cost is not calculated until the production order is ended.</span></span> <span data-ttu-id="78d55-115">عند انتهاء أمر الإنتاج، يتم حساب تكلفة الإنتاج النهائية باستخدام مبالغ الإنتاج الفعلية.</span><span class="sxs-lookup"><span data-stu-id="78d55-115">When the production order is ended, the final production cost is calculated by using actual production amounts.</span></span>

## <a name="estimate-material-and-capacity-consumption"></a><span data-ttu-id="78d55-116">تقدير استهلاك المواد والقدرة</span><span class="sxs-lookup"><span data-stu-id="78d55-116">Estimate material and capacity consumption</span></span>

<span data-ttu-id="78d55-117">يوفر لك التقدير المواد المتوقعة وتكاليف استهلاك السعة لإنتاج صنف في كمية أمر الإنتاج المخطط لها.</span><span class="sxs-lookup"><span data-stu-id="78d55-117">Estimation provides you with the projected material and capacity consumption costs of producing an item in the planned production order quantity.</span></span> <span data-ttu-id="78d55-118">إنها خطوة إلزامية في عملية الإنتاج ويتم إجراؤها بعد إنشاء أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-118">It is a mandatory step in the production process and is conducted after the production order is created.</span></span> <span data-ttu-id="78d55-119">تتمثل وظيفة التقدير الأساسية في تقدير استهلاك الصنف والمسار أثناء عملية الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-119">Estimation's essential function is to estimate item and route consumption during the production process.</span></span> <span data-ttu-id="78d55-120">تشكل هذه التقديرات الأساس للجدولة اللاحقة وعمليات الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-120">These estimates form the basis for subsequent scheduling and production processes.</span></span>

<span data-ttu-id="78d55-121">انتقل إلى **التحكم بالإنتاج > أوامر الإنتاج > جميع أوامر الإنتاج**، حدد أمر الإنتاج الذي تم تقديره، وحدد جزء الإجراءات **إدارة التكاليف**، وحدد **عرض تفاصيل الحساب**.</span><span class="sxs-lookup"><span data-stu-id="78d55-121">Go to **Production control > Production orders > All production orders**, select the production order that has been estimated, select the **Manage costs** action pane, and select **View calculation details**.</span></span>

<span data-ttu-id="78d55-122">يستند التقدير إلى تكلفة الموارد، إذا لم تتم جدولة الإنتاج بعد.</span><span class="sxs-lookup"><span data-stu-id="78d55-122">Estimation is based on costing resource, if production is not yet scheduled.</span></span> <span data-ttu-id="78d55-123">إذا تمت جدولة الإنتاج بالفعل، فإن التقدير يستند إلى الموارد المجدولة الفعلية أو مجموعة الموارد.</span><span class="sxs-lookup"><span data-stu-id="78d55-123">If production is already scheduled, estimation is based on the actual scheduled resource or resource group.</span></span> 

<span data-ttu-id="78d55-124">عند تقدير تكاليف أمر الإنتاج، يقوم النظام بحسابات التكلفة المتوقعة بناءً على مجموعة مما يلي:</span><span class="sxs-lookup"><span data-stu-id="78d55-124">When you estimate production order costs, the system bases projected cost calculations on a combination of the following:</span></span>

-   <span data-ttu-id="78d55-125">كميه أمر الإنتاج</span><span class="sxs-lookup"><span data-stu-id="78d55-125">Production order quantity</span></span>

-   <span data-ttu-id="78d55-126">المكونات في قائمة مكونات الصنف</span><span class="sxs-lookup"><span data-stu-id="78d55-126">Components in the BOM</span></span>

-   <span data-ttu-id="78d55-127">عمليات التوجيه في مسار الإنتاج</span><span class="sxs-lookup"><span data-stu-id="78d55-127">Routing operations in the production route</span></span>

-   <span data-ttu-id="78d55-128">التكاليف غير المباشرة التي تنطبق على هذه المكونات والعمليات</span><span class="sxs-lookup"><span data-stu-id="78d55-128">Indirect costs that are applicable to these components and operations</span></span>

-   <span data-ttu-id="78d55-129">بيانات التكلفة النشطة اعتباراً من تاريخ الحساب</span><span class="sxs-lookup"><span data-stu-id="78d55-129">Active cost data as of the calculation date</span></span>

<span data-ttu-id="78d55-130">في حالة وجود صنف بند وهمي في قائمة مكونات الصنف للإنتاج، فإن الحسابات تعكس المكونات الوهمية وعمليات المسار.</span><span class="sxs-lookup"><span data-stu-id="78d55-130">If a phantom line item is present in the production BOM, the calculations reflect the phantom's components and route operations.</span></span> <span data-ttu-id="78d55-131">يمكنك حساب التكاليف المقدرة لتضمين معلومات جديدة.</span><span class="sxs-lookup"><span data-stu-id="78d55-131">You can recalculate estimated costs to include new information.</span></span> <span data-ttu-id="78d55-132">قد يكون ذلك ضرورياً، على سبيل المثال، إذا كانت هناك تغييرات في كمية الأمر، أو المكونات في قائمة مكونات الصنف للإنتاج، أو عمليات التوجيه في مسار الإنتاج، أو التكاليف غير المباشرة التي تنطبق على هذه المكونات والعمليات، أو بيانات التكلفة النشطة اعتباراً من تاريخ إعادة الحساب .</span><span class="sxs-lookup"><span data-stu-id="78d55-132">This can be necessary if, for example, there are changes in the order quantity, components in the production BOM, routing operations in the production route, indirect costs that are applicable to these components and operations, or active cost data as of the recalculation date.</span></span>

<span data-ttu-id="78d55-133">عند تشغيل التقدير، يحسب النظام الأنواع التالية من قيم التكلفة:</span><span class="sxs-lookup"><span data-stu-id="78d55-133">When you run estimation, the system calculates the following types of cost values:</span></span>

-   <span data-ttu-id="78d55-134">**تكلفة الإنتاج** - هذا هو البند العلوي للتقدير.</span><span class="sxs-lookup"><span data-stu-id="78d55-134">**Production cost** - This is the top line of the estimate.</span></span> <span data-ttu-id="78d55-135">يوضح التكلفة الكاملة لتشغيل أمر الإنتاج وإجمالي سعر البيع للإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-135">It shows the complete cost of running the production order and the total sales price for the production.</span></span> <span data-ttu-id="78d55-136">إنه مجموع كل بنود التكلفة في التقدير.</span><span class="sxs-lookup"><span data-stu-id="78d55-136">It is the sum of all the cost lines on the estimate.</span></span>

-   <span data-ttu-id="78d55-137">**تكاليف المسار أو المورد** - هذه هي تكاليف العمليات المتضمنة في الإنتاج، بما في ذلك عناصر مثل وقت الإعداد ووقت التشغيل والنفقات العامة.</span><span class="sxs-lookup"><span data-stu-id="78d55-137">**Route or resource costs** - These are the costs for the operations that are involved in a production, including elements such as setup time, run time, and overhead.</span></span>

-   <span data-ttu-id="78d55-138">**تكاليف المواد** - هذه هي تكاليف وأسعار مكونات قائمة المواد اللازمة لإنتاج الصنف.</span><span class="sxs-lookup"><span data-stu-id="78d55-138">**Material costs** - These are the costs and prices of the BOM components that are needed to produce the item.</span></span> <span data-ttu-id="78d55-139">تم إنشاء هذه مسبقاً وإدخالها في النظام.</span><span class="sxs-lookup"><span data-stu-id="78d55-139">These have been previously established and entered into the system.</span></span>


<span data-ttu-id="78d55-140">يمكن أن يوفر تقدير التكلفة أيضاً ما يلي:</span><span class="sxs-lookup"><span data-stu-id="78d55-140">A cost estimate can also provide the following:</span></span>

-   <span data-ttu-id="78d55-141">عروض أسعار ذات مغزى</span><span class="sxs-lookup"><span data-stu-id="78d55-141">Meaningful price quotations</span></span>

-   <span data-ttu-id="78d55-142">تقديرات ربحية الأمر</span><span class="sxs-lookup"><span data-stu-id="78d55-142">Estimates of the profitability of the order</span></span>

-   <span data-ttu-id="78d55-143">تقديرات استخدام المواد الخام</span><span class="sxs-lookup"><span data-stu-id="78d55-143">Estimates of raw material usage</span></span>

-   <span data-ttu-id="78d55-144">مقارنات معلومات التكلفة من المنتجات السابقة</span><span class="sxs-lookup"><span data-stu-id="78d55-144">Comparisons of cost information from previous productions</span></span>

-   <span data-ttu-id="78d55-145">معلومات الموازنة والتنبؤ</span><span class="sxs-lookup"><span data-stu-id="78d55-145">Budget and forecasting information</span></span>

-   <span data-ttu-id="78d55-146">تقديرات حجم الإنتاج المطلوب للحفاظ على تكلفة معينة</span><span class="sxs-lookup"><span data-stu-id="78d55-146">Estimates of the production size that is required to maintain a particular cost</span></span>

-   <span data-ttu-id="78d55-147">اقتراح سعر مبيعات لعنصر الإنتاج بناءً على نهج التكلفة بالإضافة إلى العلامات</span><span class="sxs-lookup"><span data-stu-id="78d55-147">A sales price suggestion for the production item based on a cost plus-markup approach</span></span>

## <a name="analyzing-production-order-costs"></a><span data-ttu-id="78d55-148">تحليل تكاليف أمر الإنتاج</span><span class="sxs-lookup"><span data-stu-id="78d55-148">Analyzing production order costs</span></span>

<span data-ttu-id="78d55-149">بعد تقدير أمر الإنتاج، يمكنك تحليل تكاليفه المقدرة والفعلية باستخدام صفحة **حساب الأسعار** أو صفحة **تقديرات التكاليف وتقارير التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="78d55-149">After a production order has been estimated, you can analyze its estimated and actual costs by using the **Price calculation** page or the **Cost estimates and costings reports** page.</span></span> <span data-ttu-id="78d55-150">في هذه الصفحات، يتم عرض معلومات حول التكاليف المقدرة والفعلية (والكمية) لكل صنف مكون، وعملية التوجيه، والتكلفة غير المباشرة.</span><span class="sxs-lookup"><span data-stu-id="78d55-150">On these pages, information about the estimated and actual costs (and quantity) is shown for each component item, routing operation, and indirect cost.</span></span> <span data-ttu-id="78d55-151">تستند التكاليف الفعلية لأمر الإنتاج إلى الاستهلاك المبلغ عنه لعمليات المواد والتوجيه.</span><span class="sxs-lookup"><span data-stu-id="78d55-151">The actual costs for a production order are based on the reported consumption of material and routing operations.</span></span>

<span data-ttu-id="78d55-152">يمكنك الوصول إلى الحركات التفصيلية حول الاستهلاك المبلغ عنه للمواد وعمليات التوجيه والتكاليف غير المباشرة في صفحة **ترحيل الإنتاج** لأمر إنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-152">You can access the detailed transactions about reported consumption of material, routing operations, and indirect costs on the **Production posting** page for a production order.</span></span>

<span data-ttu-id="78d55-153">تعرض صفحة **حساب الأسعار** استهلاك المواد والوقت المقدّر في أمر إنتاج لإنشاء خط أساس يمكن من خلاله قياس التكاليف الفعلية.</span><span class="sxs-lookup"><span data-stu-id="78d55-153">The **Price calculation** page shows the estimated material and time consumption in a production order to establish a baseline from which to measure actual costs.</span></span> <span data-ttu-id="78d55-154">عند إنهاء أمر الإنتاج، تعتمد التكلفة النهائية على استهلاك المواد والوقت الفعلي، وتسمح بمقارنة التكاليف المتوقعة والتكاليف المحققة.</span><span class="sxs-lookup"><span data-stu-id="78d55-154">When a production order is ended, final costing is based on the actual material and time consumption, and allows for the comparison of expected and realized costs.</span></span> <span data-ttu-id="78d55-155">يمكنك استخدام هذه الصفحة لتحليل التكاليف المقدرة والفعلية المرتبطة بالمكونات وعمليات التوجيه لأمر إنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-155">You can use this page to analyze estimated and actual costs that are related to components and routing operations for a production order.</span></span> <span data-ttu-id="78d55-156">يمكنك أيضاً عرض معلومات تكلفة البضائع المباعة في تنسيق صحيفة التكاليف، وتحليل مصدر تباينات الإنتاج لأمر إنتاج منتهي لبند تكلفة قياسي.</span><span class="sxs-lookup"><span data-stu-id="78d55-156">You can also view the cost of goods sold information in the costing sheet format, and analyze the source of production variances for an ended production order for a standard cost item.</span></span>

<span data-ttu-id="78d55-157">**التحكم بالإنتاج > أوامر الإنتاج > جميع أوامر الإنتاج > إدارة التكاليف > عرض تفاصيل الحساب**</span><span class="sxs-lookup"><span data-stu-id="78d55-157">**Production control > Production orders > All production orders > Manage costs > View calculation details**</span></span>

![لقطة شاشة لعلامة تبويب ورقة التكاليف في صفحة حساب الأسعار.](../media/costing-sheet.png) 



<span data-ttu-id="78d55-159">ضع في اعتبارك المثال التالي: تريد شركة مقارنة تكاليف الإنتاج المقدرة بتكاليف الإنتاج الفعلية.</span><span class="sxs-lookup"><span data-stu-id="78d55-159">Consider the following example: A company wants to compare its estimated production costs with actual production costs.</span></span> <span data-ttu-id="78d55-160">باستخدام صفحة **حساب الأسعار**، يمكن للشركة عرض تكلفة الإنتاج المقدرة قبل وأثناء عملية الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="78d55-160">By using the **Price calculation** page, the company can view the estimated production cost before and during the production process.</span></span> <span data-ttu-id="78d55-161">نظراً لترحيل دفاتر اليومية أثناء الإنتاج، يستمر ترحيل التكاليف الفعلية للأصناف والعمالة/النفقات العامة في صفحة **حساب الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="78d55-161">As journals are posted during production, actual costs of items and labor/overhead continue to be posted on the **Price calculation** page.</span></span> <span data-ttu-id="78d55-162">عند إنهاء أمر الإنتاج، يتم تجميع التكاليف المرّحلة في التكاليف المحققة بحيث يمكن مقارنة التكاليف الفعلية بالتقدير الأصلي.</span><span class="sxs-lookup"><span data-stu-id="78d55-162">When the production order is ended, the posted costs are accumulated into the realized costs so that actual costs can be compared to the original estimation.</span></span>
