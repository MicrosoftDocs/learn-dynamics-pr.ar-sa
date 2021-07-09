---
ms.openlocfilehash: c593ec67a533328581230c497b0eaed39bc381a9
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073242"
---
<span data-ttu-id="1cf36-101">تتيح لك أكواد السبب تحليل نتائج عملية الجرد وأية اختلافات تحدث أثناء هذه العملية.</span><span class="sxs-lookup"><span data-stu-id="1cf36-101">Reason codes let you analyze the results of a counting process and any discrepancies that occur during that process.</span></span> <span data-ttu-id="1cf36-102">يمكنك تحديد سبب إجراء الجرد، مثل البالتة المكسورة أو تعديل المخزون المستند إلى عينات المخزون.</span><span class="sxs-lookup"><span data-stu-id="1cf36-102">You can specify the reason for doing the count, such as a broken pallet or a stock adjustment that is based on inventory samples.</span></span>

<span data-ttu-id="1cf36-103">قبل إعداد النظام، نوصي بتحديد استراتيجية للعمل مع أكواد السبب‬.</span><span class="sxs-lookup"><span data-stu-id="1cf36-103">Before you set up the system, we recommend that you define a strategy for working with reason codes.</span></span> <span data-ttu-id="1cf36-104">على سبيل المثال، حاول الإجابة عن الأسئلة التالية أثناء تعريف استراتيجيتك:</span><span class="sxs-lookup"><span data-stu-id="1cf36-104">For example, try to answer the following questions while defining your strategy:</span></span>

- <span data-ttu-id="1cf36-105">هل يجب أن تكون أكواد السبب إلزامية في المستودعات؟</span><span class="sxs-lookup"><span data-stu-id="1cf36-105">Should reason codes be mandatory on warehouses?</span></span>
- <span data-ttu-id="1cf36-106">هل يجب أن تكون أكواد السبب إلزامية أم اختيارية في بعض العناصر؟</span><span class="sxs-lookup"><span data-stu-id="1cf36-106">Should reason codes be mandatory or optional on some items?</span></span>
- <span data-ttu-id="1cf36-107">كم عدد أكواد السبب التي تحتاجها؟</span><span class="sxs-lookup"><span data-stu-id="1cf36-107">How many reason codes do you require?</span></span>
- <span data-ttu-id="1cf36-108">كيف يمكن لمستخدمي الماسحات الشريطية استخدام أكواد السبب؟</span><span class="sxs-lookup"><span data-stu-id="1cf36-108">How should users of barcode scanners use reason codes?</span></span> <span data-ttu-id="1cf36-109">هل يجب أن تكون أكواد السبب محددة مسبقاً أم إلزامية أم غير قابلة للتحرير؟</span><span class="sxs-lookup"><span data-stu-id="1cf36-109">Should the reason codes be preselected, mandatory, or not editable?</span></span>
- <span data-ttu-id="1cf36-110">هل يحتاج عمال المستودع إلى سلوك مختلف لكود السبب في الماسحات المتحركة؟</span><span class="sxs-lookup"><span data-stu-id="1cf36-110">Do warehouse workers require different reason code behavior on mobile scanners?</span></span>
<span data-ttu-id="1cf36-111">إذا كانت الإجابة نعم، يمكنك إنشاء المزيد من عناصر القائمة وتعيينها إلى أشخاص مختلفين.</span><span class="sxs-lookup"><span data-stu-id="1cf36-111">If the answer is yes, you can create more menu items and assign them to different people.</span></span>

<span data-ttu-id="1cf36-112">يمكنك إنشاء نهج متعددة لكود السبب، ويمكن أن يكون لكل كود سبب نهجين لكود سبب الجرد.</span><span class="sxs-lookup"><span data-stu-id="1cf36-112">You can create multiple reason code policies, and each reason code policy can have two counting reason code policies.</span></span> <span data-ttu-id="1cf36-113">يمكن استخدام نهج كود سبب الجرد على مستوى المستودع أو مستوى الصنف.</span><span class="sxs-lookup"><span data-stu-id="1cf36-113">The counting reason code policies can be used at the warehouse level or the item level.</span></span>

<span data-ttu-id="1cf36-114">لإعداد سياسات كود السبب، استخدم الإجراء التالي:</span><span class="sxs-lookup"><span data-stu-id="1cf36-114">To set up reason code policies, use the following procedure:</span></span>

1. <span data-ttu-id="1cf36-115">انتقل إلى **إدارة المخزون > إعداد > المخزون > نهج كود سبب الجرد**، وقم بإنشاء نهج جديد لكود السبب.</span><span class="sxs-lookup"><span data-stu-id="1cf36-115">Go to  **Inventory management > Setup > Inventory > Counting reason code policies**, and create a new reason code policy.</span></span>
1. <span data-ttu-id="1cf36-116">في الحقل **نوع كود سبب الجرد**، حدد إما **إلزامياً** أو **اختيارياً** لتحديد ما إذا كان يجب أن يكون تحديد كود السبب إجراءً اختيارياً أم إلزامياً في أحد دفاتر يومية الجرد التالية:</span><span class="sxs-lookup"><span data-stu-id="1cf36-116">In the **Counting reason code type** field, select either **Mandatory** or **Optional** to specify whether selection of a reason code should be an optional or a mandatory action in one of the following counting journals:</span></span>
    - <span data-ttu-id="1cf36-117">الجرد الدوري‬ (جهاز محمول)</span><span class="sxs-lookup"><span data-stu-id="1cf36-117">Cycle Count (mobile device)</span></span>
    - <span data-ttu-id="1cf36-118">الجرد الفوري‬ (جهاز محمول)</span><span class="sxs-lookup"><span data-stu-id="1cf36-118">Spot Count (mobile device)</span></span>
    - <span data-ttu-id="1cf36-119">جرد الحدود‬ (جهاز محمول)</span><span class="sxs-lookup"><span data-stu-id="1cf36-119">Threshold Count (mobile device)</span></span>
    - <span data-ttu-id="1cf36-120">تسوية واردة (جهاز محمول)</span><span class="sxs-lookup"><span data-stu-id="1cf36-120">Adjustment In (mobile device)</span></span>
    - <span data-ttu-id="1cf36-121">تسوية صادرة (جهاز محمول)</span><span class="sxs-lookup"><span data-stu-id="1cf36-121">Adjustment Out (mobile device)</span></span>
    - <span data-ttu-id="1cf36-122">دفتر يومية الجرد (عميل غني)</span><span class="sxs-lookup"><span data-stu-id="1cf36-122">Counting Journal (rich client)</span></span>

<span data-ttu-id="1cf36-123">يمكنك أيضاً إعداد أكواد السبب للمستودعات الفردية والمنتجات.</span><span class="sxs-lookup"><span data-stu-id="1cf36-123">You can also set up reason codes for individual warehouses and for products.</span></span> <span data-ttu-id="1cf36-124">يمكن لإعداد كود السبب للمنتجات تجاهل الإعداد للمستودعات.</span><span class="sxs-lookup"><span data-stu-id="1cf36-124">The reason code setup for products can disregard the setup for warehouses.</span></span>

## <a name="mandatory-reason-codes"></a><span data-ttu-id="1cf36-125">أكواد السبب إلزامية</span><span class="sxs-lookup"><span data-stu-id="1cf36-125">Mandatory reason codes</span></span> 

<span data-ttu-id="1cf36-126">في حالة تعيين المعلمة **إلزامياً** في تكوين أكواد السبب للمستودعات أو الأصناف، لا يمكن إكمال دفتر يومية الجرد وإغلاقه حتى يتم توفير كود سبب.</span><span class="sxs-lookup"><span data-stu-id="1cf36-126">If the **Mandatory** parameter is set in the configuration of reason codes for warehouses or items, the counting journal can't be completed and closed until a reason code is provided.</span></span>

<span data-ttu-id="1cf36-127">لإعداد أكواد السبب للمستودعات، استخدم الإجراء التالي:</span><span class="sxs-lookup"><span data-stu-id="1cf36-127">To set up reason codes for warehouses, use the following procedure:</span></span>

1. <span data-ttu-id="1cf36-128">انتقل إلى **إدارة المخزون > إعداد > تصنيف المخزون > مستودعات**.</span><span class="sxs-lookup"><span data-stu-id="1cf36-128">Go to **Inventory Management > Setup > Inventory breakdown > Warehouses**.</span></span>
1. <span data-ttu-id="1cf36-129">في علامة التبويب **إدارة المخزون والمستودعات**، ضمن الحقل **نهج كود سبب الجرد**، حدد أحد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="1cf36-129">On the **Inventory and warehouse management** tab, in the **Counting reason code policy** field, select one of the following options:</span></span>
    - <span data-ttu-id="1cf36-130">**فارغ**: تستخدم هذه المعلمة التي تم إعدادها للصنف لتحديد ما إذا كانت دفاتر يومية الجرد إلزامية بالنسبة للمنتج أم لا.</span><span class="sxs-lookup"><span data-stu-id="1cf36-130">**Blank** – The parameter that is set up for the item is used to determine whether counting journals are mandatory for the product.</span></span>
    - <span data-ttu-id="1cf36-131">**إلزامي**: دائماً ما يكون كود السبب مطلوباً في دفاتر يومية الجرد للمستودع.</span><span class="sxs-lookup"><span data-stu-id="1cf36-131">**Mandatory** – A reason code is always required on counting journals for the warehouse.</span></span>
    - <span data-ttu-id="1cf36-132">**اختياري**: لا يكون كود السبب مطلوباً في دفاتر يومية الجرد للمستودع.</span><span class="sxs-lookup"><span data-stu-id="1cf36-132">**Optional** – A reason code isn't required on counting journals for the warehouse.</span></span>

<span data-ttu-id="1cf36-133">لإعداد أكواد السبب للمنتجات، استخدم الإجراء التالي:</span><span class="sxs-lookup"><span data-stu-id="1cf36-133">To set up reason codes for products, use the following procedure:</span></span>

1. <span data-ttu-id="1cf36-134">انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="1cf36-134">Go to **Product information management > Products > Released products**.</span></span>
1. <span data-ttu-id="1cf36-135">في علامة التبويب **المنتج**، اختر **نهج كود سبب الجرد**، ثم حدد أحد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="1cf36-135">On the **Product** tab, select **Counting reason code policy**, and then select one of the following options:</span></span>
    - <span data-ttu-id="1cf36-136">**فارغ**: تستخدم هذه المعلمة التي تم إعدادها للمستودع لتحديد ما إذا كانت دفاتر يومية الجرد إلزامية بالنسبة للمنتج أم لا.</span><span class="sxs-lookup"><span data-stu-id="1cf36-136">**Blank** – The parameter that is set up for the warehouse is used to determine whether counting journals are mandatory for the product.</span></span>
    - <span data-ttu-id="1cf36-137">**إلزامي**: دائماً ما يكون كود السبب مطلوباً في دفاتر يومية الجرد للمنتج.</span><span class="sxs-lookup"><span data-stu-id="1cf36-137">**Mandatory** – A reason code is always required on counting journals for the product.</span></span> <span data-ttu-id="1cf36-138">يتجاوز هذا الإعداد أي إعداد كود سبب على مستوي المستودع.</span><span class="sxs-lookup"><span data-stu-id="1cf36-138">This setting overrides any reason code setting at the warehouse level.</span></span>
    - <span data-ttu-id="1cf36-139">**اختياري**: لا يكون كود السبب مطلوباً في دفاتر يومية الجرد للمنتج.</span><span class="sxs-lookup"><span data-stu-id="1cf36-139">**Optional** – A reason code isn't required on counting journals for the product.</span></span> <span data-ttu-id="1cf36-140">يتجاوز هذا الإعداد أي إعداد كود سبب على مستوي المستودع.</span><span class="sxs-lookup"><span data-stu-id="1cf36-140">This setting overrides any reason code setting at the warehouse level.</span></span>

## <a name="use-reason-codes-in-counting-journals"></a><span data-ttu-id="1cf36-141">استخدام أكواد السبب في دفاتر يومية الجرد</span><span class="sxs-lookup"><span data-stu-id="1cf36-141">Use reason codes in counting journals</span></span> 

<span data-ttu-id="1cf36-142">في دفتر يومية الجرد، يمكنك إضافة أكواد سبب لجرد الأنواع التالية:</span><span class="sxs-lookup"><span data-stu-id="1cf36-142">In a counting journal, you can add reason codes for counts of the following types:</span></span>

- <span data-ttu-id="1cf36-143">الجرد الدوري‬</span><span class="sxs-lookup"><span data-stu-id="1cf36-143">Cycle count</span></span>
- <span data-ttu-id="1cf36-144">الجرد الفوري</span><span class="sxs-lookup"><span data-stu-id="1cf36-144">Spot count</span></span>
- <span data-ttu-id="1cf36-145">جرد الحدود</span><span class="sxs-lookup"><span data-stu-id="1cf36-145">Threshold count</span></span>
- <span data-ttu-id="1cf36-146">تسوية واردة</span><span class="sxs-lookup"><span data-stu-id="1cf36-146">Adjustment in</span></span>
- <span data-ttu-id="1cf36-147">تسوية صادرة</span><span class="sxs-lookup"><span data-stu-id="1cf36-147">Adjustment out</span></span>

<span data-ttu-id="1cf36-148">تتم إضافة أكواد السبب إلى بنود دفتر اليومية في دفاتر يومية الجرد من النوع **دفتر يومية الجرد**.</span><span class="sxs-lookup"><span data-stu-id="1cf36-148">Reason codes are added to the journal lines in counting journals of the **Counting journal** type.</span></span>

1. <span data-ttu-id="1cf36-149">انتقل إلى **إدارة المخزون > إدخالات دفتر اليومية > جرد الأصناف > جرد**.</span><span class="sxs-lookup"><span data-stu-id="1cf36-149">Go to **Inventory management > Journal entries > Item counting > Counting**.</span></span>
1. <span data-ttu-id="1cf36-150">في تفاصيل البند الخاصة بدفتر يومية الجرد، في الحقل **كود سبب الجرد**، حدد أحد الخيارات.</span><span class="sxs-lookup"><span data-stu-id="1cf36-150">In the line details of the counting journal, in the **Counting reason code** field, select an option.</span></span> 

<span data-ttu-id="1cf36-151">لعرض سجل الجرد بمجرد تسجيله بواسطة أكواد السبب، انتقل إلى **إدارة المخزون > ‏‫الاستعلامات والتقارير > سجل الجرد**، ثم في الحقل **كود سبب الجرد**، قم بعرض محفوظات الجرد التي تم تسجيلها من خلال كود السبب.</span><span class="sxs-lookup"><span data-stu-id="1cf36-151">To view the counting history as it's recorded by reason codes, go to **Inventory management > Inquiries and reports > Counting history** and then, in the **Counting reason code** field, view the counting history that has been recorded through a reason code.</span></span>

## <a name="use-a-reason-code-for-a-quantity-adjustment"></a><span data-ttu-id="1cf36-152">استخدام كود سبب لتسوية كمية</span><span class="sxs-lookup"><span data-stu-id="1cf36-152">Use a reason code for a quantity adjustment</span></span> 

<span data-ttu-id="1cf36-153">لإضافة كود سبب لتسوية الكمية، استخدم الإجراء التالي:</span><span class="sxs-lookup"><span data-stu-id="1cf36-153">To add a reason code for a quantity adjustment, use the following procedure:</span></span>

1. <span data-ttu-id="1cf36-154">في الصفحة **المخزون الفعلي**، حدد **تسوية الكمية**.</span><span class="sxs-lookup"><span data-stu-id="1cf36-154">On the **On-hand inventory** page, select **Adjust quantity**.</span></span> <span data-ttu-id="1cf36-155">يمكنك فتح صفحة **المخزون الفعلي** بطرق متعددة.</span><span class="sxs-lookup"><span data-stu-id="1cf36-155">You can open the **On-hand inventory** page in several ways.</span></span> <span data-ttu-id="1cf36-156">على سبيل المثال، حدد **إدارة المخزون > الاستعلامات والتقارير > المخزون الفعلي**.</span><span class="sxs-lookup"><span data-stu-id="1cf36-156">For example, select **Inventory management > Inquiries and reports > On-hand inventory**.</span></span>
1. <span data-ttu-id="1cf36-157">حدد **تسوية الكمية**، ثم في الحقل **كود سبب الجرد**، حدد أحد أكواد السبب.</span><span class="sxs-lookup"><span data-stu-id="1cf36-157">Select **Adjust quantity** and then, in the **Counting reason code** field, select a reason code.</span></span>

