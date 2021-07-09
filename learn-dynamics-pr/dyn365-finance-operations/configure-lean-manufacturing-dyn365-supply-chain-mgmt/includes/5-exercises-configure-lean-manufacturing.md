---
ms.openlocfilehash: 3ac3b06883f201e88effebaf41b2ed12ec8bd039
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073543"
---
## <a name="before-you-begin"></a><span data-ttu-id="c0de0-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="c0de0-101">Before you begin</span></span>
<span data-ttu-id="c0de0-102">للحصول على أقصى استفادة من هذه التدريبات، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية في Supply Chain Management والتي يتم تثبيتها باستخدام Lifecycle Services ‏(LCS).</span><span class="sxs-lookup"><span data-stu-id="c0de0-102">To get the most benefit from these exercises, we recommend that you have the standard sample data available in Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

 
## <a name="exercise---create-a-value-stream"></a><span data-ttu-id="c0de0-103">تدريب - إنشاء تدفق قيم</span><span class="sxs-lookup"><span data-stu-id="c0de0-103">Exercise - Create a value stream</span></span> 

<span data-ttu-id="c0de0-104">بعد تعريف تدفق قيم lean manufacturing وتعيينه لشركة **USMF**، عليك إنشاء تدفق قيم في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="c0de0-104">After defining and mapping the lean manufacturing value stream for the **USMF** company, you must create the value stream in Supply Chain Management.</span></span>

1.  <span data-ttu-id="c0de0-105">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفق الإنتاج محدود الفاقد > تدفقات القيم**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-105">Go to **Production control > Setup > Lean production flow > Value streams**.</span></span>

2.  <span data-ttu-id="c0de0-106">حدد **جديد** في جزء الإجراءات لإنشاء تدفق قيم جديد.</span><span class="sxs-lookup"><span data-stu-id="c0de0-106">Select **New** in the Action Pane to create a new value stream.</span></span>

3.  <span data-ttu-id="c0de0-107">أدخل التفاصيل التالية لتدفق القيم الجديد:</span><span class="sxs-lookup"><span data-stu-id="c0de0-107">Enter the following details for the new value stream:</span></span>

    -   <span data-ttu-id="c0de0-108">**الاسم**:‏ SeaLeanVS</span><span class="sxs-lookup"><span data-stu-id="c0de0-108">**Name**: SeaLeanVS</span></span>

    -   <span data-ttu-id="c0de0-109">**اسم البحث**:‏ SeaLeanVS</span><span class="sxs-lookup"><span data-stu-id="c0de0-109">**Search name**: SeaLeanVS</span></span>

    -   <span data-ttu-id="c0de0-110">**المدير**:‏ Jodi Christiansen</span><span class="sxs-lookup"><span data-stu-id="c0de0-110">**Manager**: Jodi Christiansen</span></span>

4.  <span data-ttu-id="c0de0-111">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-111">Select **Save**.</span></span>


## <a name="exercise---create-a-production-flow"></a><span data-ttu-id="c0de0-112">تدريب - إنشاء تدفق إنتاج</span><span class="sxs-lookup"><span data-stu-id="c0de0-112">Exercise - Create a production flow</span></span> 

<span data-ttu-id="c0de0-113">بصفتك مشرف طابق (صالة) الإنتاج، تتوفّر لك مجموعة منطقية للقدرة الإنتاجية لخلية العمل بسلوك مشابه للقدرة الإنتاجية لخلايا العمل المستخدمة في نموذج تدفق إنتاج مكبر صوت السيارة.</span><span class="sxs-lookup"><span data-stu-id="c0de0-113">As the production (shop) floor supervisor, you have a logical grouping of work cell capacity with similar behavior in capacity load for the work cells that are used to model the Car Speaker production flow.</span></span>

<span data-ttu-id="c0de0-114">عليك إنشاء تدفق إنتاج جديد (SeaPFModel) لوضع نموذج لعملية دهان أغطية مكبرات صوت السيارات.</span><span class="sxs-lookup"><span data-stu-id="c0de0-114">You must create a new production flow (SeaPFModel) to model the process of painting the covers for the car speakers.</span></span> <span data-ttu-id="c0de0-115">سيتم حساب القدرة الإنتاجية وحمل العمل لتدفق الإنتاج بكميات المنتج المنتجة (الإنتاجية).</span><span class="sxs-lookup"><span data-stu-id="c0de0-115">The capacity and load of the production flow will be measured in quantities of product that are produced (throughput).</span></span>

<span data-ttu-id="c0de0-116">سيتم تعريف دورة تدفق الإنتاج هذه كيوم واحد، عدد الأيام المستخدمة في التخطيط التلقائي (دورة EPE يوم واحد (**1**)).</span><span class="sxs-lookup"><span data-stu-id="c0de0-116">The cycle for this production flow will be defined as one day, the number of days that are used in automatic planning (EPE cycle is **1** day).</span></span> <span data-ttu-id="c0de0-117">سيتم استخدام طريقة جدولة كانبان **إضافة** في حالة عدم توفر قدرة إنتاجية خلال الفترات المطلوبة؛ نوع فترة التخطيط هو **اليوم** والحد الزمني للتخطيط هو **10**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-117">The **Add** method of kanban scheduling will be used if no capacity is available during the required periods; the planning period type is **Day** and the planning time fence is **10**.</span></span>

1.  <span data-ttu-id="c0de0-118">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفق الإنتاج محدود الفاقد > نماذج تدفق الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-118">Go to **Production control > Setup > Lean production flow > Production flow models**.</span></span>

2.  <span data-ttu-id="c0de0-119">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="c0de0-119">Select **New** in the Action Pane.</span></span>

3.  <span data-ttu-id="c0de0-120">في حقل **نموذج تدفق الإنتاج**، أدخل **SeaPFModel**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-120">In the **Production flow model** field, enter **SeaPFModel**.</span></span>

4.  <span data-ttu-id="c0de0-121">في حقل **نوع النموذج**، أدخل **الإنتاجية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-121">In the **Model type** field, enter **Throughput**.</span></span>

5.  <span data-ttu-id="c0de0-122">في **دورة EPE** في حقل **الأيام**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-122">In the **EPE Cycle** in the **Days** field, enter **1**.</span></span>

6.  <span data-ttu-id="c0de0-123">في حقل **نوع فترة التخطيط**، حدد **اليوم**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-123">In the **Planning period type** field, select **Day**.</span></span>

7.  <span data-ttu-id="c0de0-124">في حقل **الحد الزمني للتخطيط**، أدخل **10**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-124">In the **Planning time fence** field, enter **10**.</span></span>

8.  <span data-ttu-id="c0de0-125">في القائمة المنسدلة **الاستجابة للعجز في القدرة الإنتاجية**، حدد **تأجيل**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-125">In the **Capacity shortage reaction** drop-down menu, select **Postpone**.</span></span>

9. <span data-ttu-id="c0de0-126">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-126">Select **Save**.</span></span>

### <a name="create-a-production-flow"></a><span data-ttu-id="c0de0-127">إنشاء تدفق إنتاج</span><span class="sxs-lookup"><span data-stu-id="c0de0-127">Create a production flow</span></span>

<span data-ttu-id="c0de0-128">عليك أيضاً إنشاء إصدار تدفق إنتاج لتدفق إنتاج الكتاب الإلكتروني لشركة USMF وإعداد الوقت اللازم لإنتاج وحدة من المنتج وأزمنة الدورات كجزء من التكوين.</span><span class="sxs-lookup"><span data-stu-id="c0de0-128">You must also create a production flow version for the USMF eBook production flow and set up the takt and cycle times as part of the configuration.</span></span>

<span data-ttu-id="c0de0-129">تفاصيل تدفق الإنتاج:</span><span class="sxs-lookup"><span data-stu-id="c0de0-129">Details for the production flow:</span></span>

| <span data-ttu-id="c0de0-130">الحقل</span><span class="sxs-lookup"><span data-stu-id="c0de0-130">Field</span></span>                               | <span data-ttu-id="c0de0-131">التفاصيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-131">Details</span></span>               |
|-------------------------------------|-----------------------|
| <span data-ttu-id="c0de0-132">الاسم</span><span class="sxs-lookup"><span data-stu-id="c0de0-132">Name</span></span>                                | <span data-ttu-id="c0de0-133">eBookProdFlow</span><span class="sxs-lookup"><span data-stu-id="c0de0-133">eBookProdFlow</span></span>         |
| <span data-ttu-id="c0de0-134">الوصف</span><span class="sxs-lookup"><span data-stu-id="c0de0-134">Description</span></span>                         | <span data-ttu-id="c0de0-135">تدفق إنتاج الكتاب الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="c0de0-135">eBook Production Flow</span></span> |
| <span data-ttu-id="c0de0-136">الكيان القانوني</span><span class="sxs-lookup"><span data-stu-id="c0de0-136">Legal entity</span></span>                        | <span data-ttu-id="c0de0-137">USMF</span><span class="sxs-lookup"><span data-stu-id="c0de0-137">USMF</span></span>                  |
| <span data-ttu-id="c0de0-138">تدفق القيم</span><span class="sxs-lookup"><span data-stu-id="c0de0-138">Value stream</span></span>                        | <span data-ttu-id="c0de0-139">SeaLeanVS</span><span class="sxs-lookup"><span data-stu-id="c0de0-139">SeaLeanVS</span></span>             |
| <span data-ttu-id="c0de0-140">مجموعة الإنتاج</span><span class="sxs-lookup"><span data-stu-id="c0de0-140">Production group</span></span>                    | <span data-ttu-id="c0de0-141">10</span><span class="sxs-lookup"><span data-stu-id="c0de0-141">10</span></span>                    |
| <span data-ttu-id="c0de0-142">لكل وحدة قياس دورة</span><span class="sxs-lookup"><span data-stu-id="c0de0-142">Per cycle unit of measure</span></span>           | <span data-ttu-id="c0de0-143">القطع</span><span class="sxs-lookup"><span data-stu-id="c0de0-143">pcs</span></span>                   |
| <span data-ttu-id="c0de0-144">الكمية لكل دورة</span><span class="sxs-lookup"><span data-stu-id="c0de0-144">Quantity per cycle</span></span>                  | <span data-ttu-id="c0de0-145">1</span><span class="sxs-lookup"><span data-stu-id="c0de0-145">1</span></span>                     |
| <span data-ttu-id="c0de0-146">متوسط الوقت اللازم لإنتاج وحدة من المنتج</span><span class="sxs-lookup"><span data-stu-id="c0de0-146">Average takt time</span></span>                   | <span data-ttu-id="c0de0-147">1</span><span class="sxs-lookup"><span data-stu-id="c0de0-147">1</span></span>                     |
| <span data-ttu-id="c0de0-148">الحد الأدنى للوقت اللازم لإنتاج وحدة من المنتج</span><span class="sxs-lookup"><span data-stu-id="c0de0-148">Minimum takt time</span></span>                   | <span data-ttu-id="c0de0-149">1</span><span class="sxs-lookup"><span data-stu-id="c0de0-149">1</span></span>                     |
| <span data-ttu-id="c0de0-150">الحد الأقصى للوقت اللازم لإنتاج وحدة من المنتج</span><span class="sxs-lookup"><span data-stu-id="c0de0-150">Maximum takt time</span></span>                   | <span data-ttu-id="c0de0-151">2</span><span class="sxs-lookup"><span data-stu-id="c0de0-151">2</span></span>                     |
| <span data-ttu-id="c0de0-152">فترة زمن الدورة الفعلي (بالأيام)</span><span class="sxs-lookup"><span data-stu-id="c0de0-152">Period for actual cycle time (days)</span></span> | <span data-ttu-id="c0de0-153">1</span><span class="sxs-lookup"><span data-stu-id="c0de0-153">1</span></span>                     |



1.  <span data-ttu-id="c0de0-154">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفق الإنتاج محدود الفاقد > تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-154">Go to **Production control > Setup > Lean production flow > Production flows**.</span></span>

2.  <span data-ttu-id="c0de0-155">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="c0de0-155">Select **New** on the Action Pane.</span></span> <span data-ttu-id="c0de0-156">يتم إنشاء سجل تدفق إنتاج جديد.</span><span class="sxs-lookup"><span data-stu-id="c0de0-156">A new production flow record is created.</span></span>

3.  <span data-ttu-id="c0de0-157">في حقل **الاسم**، أدخل **eBookProdFlow**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-157">In the **Name** field, enter **eBookProdFlow**.</span></span>

4.  <span data-ttu-id="c0de0-158">في حقل **الوصف**، أدخل **‏‫تدفق إنتاج الكتاب الإلكتروني‬**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-158">In the **Description** field, enter **eBook Production Flow**.</span></span>

5.  <span data-ttu-id="c0de0-159">في حقل **الكيان القانوني**، حدد **USMF**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-159">In the **Legal entity** field, select **USMF**.</span></span>

6.  <span data-ttu-id="c0de0-160">في حقل **تدفق القيم**، حدد **SeaLeanVS**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-160">In the **Value stream** field, select **SeaLeanVS**.</span></span>

7.  <span data-ttu-id="c0de0-161">في حقل **مجموعة الإنتاج**، حدد **10**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-161">In the **Production group** field, select **10**.</span></span>

8.  <span data-ttu-id="c0de0-162">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-162">Select **Save**.</span></span>

9.  <span data-ttu-id="c0de0-163">في علامة التبويب السريعة **الإصدارات**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-163">On the **Versions** FastTab, select **Add**.</span></span>

10. <span data-ttu-id="c0de0-164">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-164">Select **OK**.</span></span>


### <a name="configure-the-takt-requirements-for-the-new-production-flow-version"></a><span data-ttu-id="c0de0-165">تكوين متطلبات إنتاج وحدة من المنتج لإصدار تدفق الإنتاج الجديد</span><span class="sxs-lookup"><span data-stu-id="c0de0-165">Configure the takt requirements for the new production flow version</span></span>

1.  <span data-ttu-id="c0de0-166">قم بتوسيع علامتَي التبويب السريعتَين **الإصدارات** و **تفاصيل الإصدار**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-166">Expand the **Versions** and **Version details** FastTabs.</span></span>

2.  <span data-ttu-id="c0de0-167">في حقل **لكل وحدة قياس دورة**، حدد **أجزاء**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-167">In the **Per cycle unit of measure** field, select **pcs**.</span></span>

3.  <span data-ttu-id="c0de0-168">في حقل **الكمية لكل دورة**، أدخِل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-168">In the **Quantity per cycle** field, enter **1**.</span></span>

4.  <span data-ttu-id="c0de0-169">في حقل **متوسط الوقت اللازم لإنتاج وحدة من المنتج**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-169">In the **Average takt time** field, enter **1**.</span></span>

5.  <span data-ttu-id="c0de0-170">في حقل **الحد الأدنى للوقت اللازم لإنتاج وحدة من المنتج**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-170">In the **Minimum takt time** field, enter **1**.</span></span>

6.  <span data-ttu-id="c0de0-171">في حقل **الحد الأقصى للوقت اللازم لإنتاج وحدة من المنتج**، أدخل **2**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-171">In the **Maximum takt time** field, enter **2**.</span></span>

7.  <span data-ttu-id="c0de0-172">في حقل **فترة زمن الدورة الفعلي (بالأيام)**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-172">In the **Period for actual cycle time (days)** field, enter **1**.</span></span>

8.  <span data-ttu-id="c0de0-173">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="c0de0-173">Select **Save** on the Action Pane.</span></span>

9.  <span data-ttu-id="c0de0-174">قم بملاحظة أن حقل **حالة الخطة**، في علامة التبويب السريعة **الإصدارات** معيّن على **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-174">Observe that the **Plan status** field, in the **Versions** FastTab is set to **Draft**.</span></span>

10. <span data-ttu-id="c0de0-175">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="c0de0-175">Close all pages.</span></span>


## <a name="exercise---create-a-process-activity"></a><span data-ttu-id="c0de0-176">تدريب - إنشاء نشاط عملية</span><span class="sxs-lookup"><span data-stu-id="c0de0-176">Exercise - Create a process activity</span></span> 

<span data-ttu-id="c0de0-177">يجري تطوير قلم للكتاب الإلكتروني كعنصر مكمل لمجموعة مواد الكتب الإلكترونية التي تباع في شركة USMF.</span><span class="sxs-lookup"><span data-stu-id="c0de0-177">A new eBook stylus is being developed to compliment the eBook kits that are sold at USMF.</span></span> <span data-ttu-id="c0de0-178">يتم شراء القلم من مورّد خارجي وتكوينه في شركة USMF.</span><span class="sxs-lookup"><span data-stu-id="c0de0-178">The stylus is purchased from an outside vendor and configured at USMF.</span></span> <span data-ttu-id="c0de0-179">يلزم وجود نشاط للعملية لتكوين القلم ووضعه في المخزون لاستخدامه في مكان آخر.</span><span class="sxs-lookup"><span data-stu-id="c0de0-179">A process activity is needed to configure the stylus and place it in stock for use elsewhere.</span></span>

<span data-ttu-id="c0de0-180">تفاصيل نشاط العملية:</span><span class="sxs-lookup"><span data-stu-id="c0de0-180">Details for the process activity:</span></span>

| <span data-ttu-id="c0de0-181">الحقل</span><span class="sxs-lookup"><span data-stu-id="c0de0-181">Field</span></span>            | <span data-ttu-id="c0de0-182">التفاصيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-182">Details</span></span>           |
|------------------|-------------------|
| <span data-ttu-id="c0de0-183">الاسم</span><span class="sxs-lookup"><span data-stu-id="c0de0-183">Name</span></span>             | <span data-ttu-id="c0de0-184">نشاط النقل</span><span class="sxs-lookup"><span data-stu-id="c0de0-184">Transfer Activity</span></span> |
| <span data-ttu-id="c0de0-185">كمية العملية</span><span class="sxs-lookup"><span data-stu-id="c0de0-185">Process quantity</span></span> | <span data-ttu-id="c0de0-186">10 أجزاء</span><span class="sxs-lookup"><span data-stu-id="c0de0-186">10 pcs</span></span>            |
| <span data-ttu-id="c0de0-187">وحدة التشغيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-187">Operating unit</span></span>   | <span data-ttu-id="c0de0-188">LeanProduction</span><span class="sxs-lookup"><span data-stu-id="c0de0-188">LeanProduction</span></span>    |
| <span data-ttu-id="c0de0-189">خلية العمل</span><span class="sxs-lookup"><span data-stu-id="c0de0-189">Work cell</span></span>        | <span data-ttu-id="c0de0-190">1260</span><span class="sxs-lookup"><span data-stu-id="c0de0-190">1260</span></span>              |



1.  <span data-ttu-id="c0de0-191">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفقات الإنتاج محدود الفاقد >تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-191">Go to **Production Control > Setup > Lean Production Flows > Production flows**.</span></span>

2.  <span data-ttu-id="c0de0-192">افتح تدفق الإنتاج **مكبر الصوت متوسط المدى 2 PF‬‏‫**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-192">Open the **Mid Range Speaker 2 PF** production flow.</span></span>

3.  <span data-ttu-id="c0de0-193">في علامة التبويب السريعة **الإصدارات**، حدد الزر **الأنشطة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-193">On the **Versions** FastTab, select the **Activities** button.</span></span>

4.  <span data-ttu-id="c0de0-194">حدد الزر **إنشاء نشاط خطة جديد** في الجزء العلوي.</span><span class="sxs-lookup"><span data-stu-id="c0de0-194">Select the **Create new plan activity** button at the top.</span></span>

5.  <span data-ttu-id="c0de0-195">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-195">Select **Next**.</span></span>

6.  <span data-ttu-id="c0de0-196">أدخل **نشاط النقل** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-196">Enter **Transfer Activity** in the **Name** field.</span></span>

7.  <span data-ttu-id="c0de0-197">أدخل **10** في حقل **كمية العملية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-197">Enter **10** in the **Process quantity** field.</span></span>

8.  <span data-ttu-id="c0de0-198">في القائمة المنسدلة **الوحدة**، حدد **أجزاء**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-198">In the **Unit** drop-down list, select **pcs**.</span></span>

9.  <span data-ttu-id="c0de0-199">في القائمة المنسدلة **وحدة التشغيل**، حدد **‎LeanProduction**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-199">In the **Operating unit** drop-down list, select **LeanProduction**.</span></span>

10. <span data-ttu-id="c0de0-200">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-200">Select **Next**.</span></span>

11. <span data-ttu-id="c0de0-201">في القائمة المنسدلة **خلية العمل**، حدد **1260**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-201">In the **Work cell** drop-down list, select **1260**.</span></span>

12. <span data-ttu-id="c0de0-202">قم بتعيين الخيار **تحديث المخزون الفعلي عند الاستلام** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-202">Set the **Update on hand on receipt** option to **Yes**.</span></span>

13. <span data-ttu-id="c0de0-203">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-203">Select **Next**.</span></span>

14. <span data-ttu-id="c0de0-204">حدد **1260** في الحقل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-204">Select **1260** in the **Replenishing** field.</span></span>

15. <span data-ttu-id="c0de0-205">حدد **المنتج النهائي** في حقل **نوع المنتج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-205">Select **Finished product** in the **Product type** field.</span></span>

16. <span data-ttu-id="c0de0-206">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-206">Select **Next**.</span></span>

17. <span data-ttu-id="c0de0-207">حدد المستودع **13** في حقل **نقل من مستودع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-207">Select Warehouse **13** in the **Transfer from location warehouse** field.</span></span>

18. <span data-ttu-id="c0de0-208">حدد الموقع **13** في الحقل **نقل من الموقع - الموقع**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-208">Select location **13** in the **Transfer from location - location** field.</span></span>

19. <span data-ttu-id="c0de0-209">لموقع **النقل إلى**، حدد **22** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-209">For the **Transfer to** location, select **22** in the **Warehouse** field.</span></span>

20. <span data-ttu-id="c0de0-210">حدد الموقع **01-01-2-1** في حقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-210">Select location **01-01-2-1** in the **Location** field.</span></span>

21. <span data-ttu-id="c0de0-211">حدد **الشاحن** في حقل **شحن بواسطة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-211">Select **Shipper** in the **Freighted by** field.</span></span>

22. <span data-ttu-id="c0de0-212">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-212">Select **Next**.</span></span>

23. <span data-ttu-id="c0de0-213">حدد سجل **وقت الانتظار بعد**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-213">Select the **Queue time after** record.</span></span>

24. <span data-ttu-id="c0de0-214">أدخل **4** في حقل **الوقت**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-214">Enter **4** in the **Time** field.</span></span>

25. <span data-ttu-id="c0de0-215">حدد **ساعة** في حقل **الوحدة الزمنية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-215">Select **hr** in the **Time unit** field.</span></span>

26. <span data-ttu-id="c0de0-216">أدخل **10** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-216">Enter **10** in the **Per quantity** field.</span></span>

27. <span data-ttu-id="c0de0-217">حدد سجل **وقت التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-217">Select the **Runtime** record.</span></span>

28. <span data-ttu-id="c0de0-218">أدخل **2** في حقل **الوقت**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-218">Enter **2** in the **Time** field.</span></span>

29. <span data-ttu-id="c0de0-219">حدد **ساعة** في حقل **الوحدة الزمنية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-219">Select **hr** in the **Time unit** field.</span></span>

30. <span data-ttu-id="c0de0-220">أدخل **10** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-220">Enter **10** in the **Per quantity** field.</span></span>

31. <span data-ttu-id="c0de0-221">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-221">Select **Next**.</span></span>

32. <span data-ttu-id="c0de0-222">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-222">Select **Finish**.</span></span>


## <a name="exercise---configure-process-and-transfer"></a><span data-ttu-id="c0de0-223">تدريب - تكوين العملية والنقل</span><span class="sxs-lookup"><span data-stu-id="c0de0-223">Exercise - Configure process and transfer</span></span> 

<span data-ttu-id="c0de0-224">جارٍ تطوير جهاز تحكم عن بُعد جديد لمكبر صوت السيارة كعنصر مكمل لمجموعة مواد مكبرات صوت السيارات التي تُباع في Contoso.</span><span class="sxs-lookup"><span data-stu-id="c0de0-224">A new car speaker remote is being developed to complement the car speaker kits that are sold at Contoso.</span></span> <span data-ttu-id="c0de0-225">يحتاج تدفق إنتاج CarSpeakProdFlow إلى تعديل ليتضمن نشاط نقل لنقل جهاز التحكم عن بُعد المكون إلى مستودع المكونات الكهربائية.</span><span class="sxs-lookup"><span data-stu-id="c0de0-225">The CarSpeakProdFlow production flow needs to be amended to include a transfer activity to move the configured remote to the Electrical Component warehouse.</span></span>

<span data-ttu-id="c0de0-226">تفاصيل نشاط النقل لتدفق الإنتاج:</span><span class="sxs-lookup"><span data-stu-id="c0de0-226">Details for production flow transfer activity:</span></span>


| <span data-ttu-id="c0de0-227">الحقل</span><span class="sxs-lookup"><span data-stu-id="c0de0-227">Field</span></span>                       | <span data-ttu-id="c0de0-228">التفاصيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-228">Details</span></span>                           |
|-----------------------------|-----------------------------------|
| <span data-ttu-id="c0de0-229">الاسم</span><span class="sxs-lookup"><span data-stu-id="c0de0-229">Name</span></span>                        | <span data-ttu-id="c0de0-230">RemoteTransfer</span><span class="sxs-lookup"><span data-stu-id="c0de0-230">RemoteTransfer</span></span>                    |
| <span data-ttu-id="c0de0-231">كمية العملية</span><span class="sxs-lookup"><span data-stu-id="c0de0-231">Process quantity</span></span>            | <span data-ttu-id="c0de0-232">10</span><span class="sxs-lookup"><span data-stu-id="c0de0-232">10</span></span>                                |
| <span data-ttu-id="c0de0-233">وحدة التشغيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-233">Operating unit</span></span>              | <span data-ttu-id="c0de0-234">SeaLeanVS</span><span class="sxs-lookup"><span data-stu-id="c0de0-234">SeaLeanVS</span></span>                        |
| <span data-ttu-id="c0de0-235">مجموعة موارد التزويد</span><span class="sxs-lookup"><span data-stu-id="c0de0-235">Replenishing resource group</span></span> | <span data-ttu-id="c0de0-236">1250</span><span class="sxs-lookup"><span data-stu-id="c0de0-236">1250</span></span>                              |
| <span data-ttu-id="c0de0-237">تحديث المخزون الفعلي عند الاستلام</span><span class="sxs-lookup"><span data-stu-id="c0de0-237">Update on hand on receipt</span></span>   | <span data-ttu-id="c0de0-238">نعم</span><span class="sxs-lookup"><span data-stu-id="c0de0-238">Yes</span></span>                               |
| <span data-ttu-id="c0de0-239">تحديث المخزون الفعلي عند الانتقاء</span><span class="sxs-lookup"><span data-stu-id="c0de0-239">Update on hand on pick</span></span>      | <span data-ttu-id="c0de0-240">لا</span><span class="sxs-lookup"><span data-stu-id="c0de0-240">No</span></span>                                |
| <span data-ttu-id="c0de0-241">نقل إلى</span><span class="sxs-lookup"><span data-stu-id="c0de0-241">Transfer to</span></span>                 | <span data-ttu-id="c0de0-242">المستودع 61، مخرجات الموقع</span><span class="sxs-lookup"><span data-stu-id="c0de0-242">warehouse 61, location Output</span></span> |
| <span data-ttu-id="c0de0-243">شحن بواسطة</span><span class="sxs-lookup"><span data-stu-id="c0de0-243">Freighted by</span></span>                | <span data-ttu-id="c0de0-244">الشاحن</span><span class="sxs-lookup"><span data-stu-id="c0de0-244">Shipper</span></span>                           |
| <span data-ttu-id="c0de0-245">وقت التشغيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-245">Runtime</span></span>                     | <span data-ttu-id="c0de0-246">دقيقة واحدة لكل 25 جزء</span><span class="sxs-lookup"><span data-stu-id="c0de0-246">1 min per 25 pcs</span></span>                  |


### <a name="deactivate-the-current-production-flow-version"></a><span data-ttu-id="c0de0-247">إلغاء تنشيط إصدار تدفق الإنتاج الحالي</span><span class="sxs-lookup"><span data-stu-id="c0de0-247">Deactivate the current production flow version</span></span>

1.  <span data-ttu-id="c0de0-248">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفق الإنتاج محدود الفاقد > تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-248">Go to **Production Control > Setup > Lean production flow > Production flows**.</span></span>

2.  <span data-ttu-id="c0de0-249">افتح تدفق إنتاج **تجميع مكبر الصوت القياسي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-249">Open the **Standard speaker assembly** production flow.</span></span>

3.  <span data-ttu-id="c0de0-250">في علامة التبويب السريعة **الإصدارات**، حدد الإصدار **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-250">On the **Versions** FastTab, select version **1**.</span></span>

4.  <span data-ttu-id="c0de0-251">حدد **إلغاء التنشيط**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-251">Select **Deactivate**.</span></span>

5.  <span data-ttu-id="c0de0-252">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-252">Select **OK**.</span></span> <span data-ttu-id="c0de0-253">يتم تغيير **حالة الخطة** إلى **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-253">The **Plan status** changes to **Draft**.</span></span>


### <a name="create-a-new-transfer-activity"></a><span data-ttu-id="c0de0-254">إنشاء نشاط نقل جديد</span><span class="sxs-lookup"><span data-stu-id="c0de0-254">Create a new transfer activity</span></span>

1.  <span data-ttu-id="c0de0-255">في علامة التبويب السريعة **الإصدارات**، حدد **الأنشطة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-255">On the **Versions** FastTab, select **Activities**.</span></span> <span data-ttu-id="c0de0-256">يتم فتح صفحة **أنشطة تدفق الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-256">The **Production flow activities** page opens.</span></span>

2.  <span data-ttu-id="c0de0-257">حدد **إنشاء نشاط خطة جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="c0de0-257">Select **Create new plan activity** on the Action Pane.</span></span>

3.  <span data-ttu-id="c0de0-258">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-258">Select **Next**.</span></span>

4.  <span data-ttu-id="c0de0-259">أدخل **RemoteTransfer** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-259">Enter **RemoteTransfer** in the **Name** field.</span></span>

5.  <span data-ttu-id="c0de0-260">في القائمة المنسدلة **نوع النشاط**، حدد **نقل**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-260">In the **Activity type** drop-down list, select **Transfer**.</span></span>

6.  <span data-ttu-id="c0de0-261">أدخل **10** في حقل **كمية العملية**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-261">Enter **10** in the **Process quantity** field.</span></span>

7.  <span data-ttu-id="c0de0-262">في القائمة المنسدلة **الوحدة**، حدد **أجزاء**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-262">In the **Unit** drop-down list, select **pcs**.</span></span>

8.  <span data-ttu-id="c0de0-263">في القائمة المنسدلة **وحدة التشغيل**، حدد **‎SeaLeanVS**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-263">In the **Operating unit** drop-down list, select **SeaLeanVS**.</span></span>

9.  <span data-ttu-id="c0de0-264">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-264">Select **Next**.</span></span> <span data-ttu-id="c0de0-265">يتم فتح صفحة **إنشاء نشاط نقل**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-265">The **Create transfer activity** page opens.</span></span>

10. <span data-ttu-id="c0de0-266">في القائمة المنسدلة **تزويد**، حدد **1250**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-266">In the **Replenishing** drop-down list, select **1250**.</span></span>

11. <span data-ttu-id="c0de0-267">قم بتعيين خانة الاختيار **تحديث المخزون الفعلي عند الاستلام** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-267">Set the **Update on hand on receipt** check box to **Yes**.</span></span>

12. <span data-ttu-id="c0de0-268">قم بتعيين خانة الاختيار **تحديث المخزون الفعلي عند الانتقاء** على **لا**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-268">Set the **Update on hand on pick** check box to **No**.</span></span>

13. <span data-ttu-id="c0de0-269">في حقل **نوع المنتج**، حدد **المنتج النهائي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-269">In the **Product type** field, select **Finished product**.</span></span>

14. <span data-ttu-id="c0de0-270">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-270">Select **Next**.</span></span> <span data-ttu-id="c0de0-271">يتم فتح صفحة **تعيين مواقع النقل**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-271">The **Assign transfer locations** page opens.</span></span>

15. <span data-ttu-id="c0de0-272">في مجموعة **نقل إلى موقع**، في القائمة المنسدلة **المستودع**، حدد **61**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-272">In the **Transfer to location** group, in the **Warehouse** drop-down list, select **61**.</span></span>

16. <span data-ttu-id="c0de0-273">في القائمة المنسدلة **الموقع**، حدد أول موقع مدرج: **01A01R1S1B**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-273">In the **Location** drop-down list, select the first location listed: **01A01R1S1B**.</span></span>

17. <span data-ttu-id="c0de0-274">في القائمة المنسدلة **شحن بواسطة**، حدد **الشاحن**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-274">In the **Freighted by** drop-down list, select **Shipper**.</span></span>

18. <span data-ttu-id="c0de0-275">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-275">Select **Next**.</span></span> <span data-ttu-id="c0de0-276">يتم فتح صفحة **تعيين وقت النشاط**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-276">The **Assign activity time** page opens.</span></span>

19. <span data-ttu-id="c0de0-277">في حقل **الوقت** لصف **وقت التشغيل**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-277">In the **Time** field for the **Runtime** row, enter **1**.</span></span>

20. <span data-ttu-id="c0de0-278">في القائمة المنسدلة المجاورة **الوحدة الزمنية**، حدد **دقيقة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-278">In the adjacent **Time unit** drop-down list, select **min**.</span></span>

21. <span data-ttu-id="c0de0-279">في حقل **لكل كمية**، أدخل **25** جزءاً.</span><span class="sxs-lookup"><span data-stu-id="c0de0-279">In the **Per quantity** field, enter **25** pcs.</span></span>

22. <span data-ttu-id="c0de0-280">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-280">Select **Next**.</span></span> <span data-ttu-id="c0de0-281">يتم فتح الصفحة **تأكيد التحديد**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-281">The **Confirm selection** page opens.</span></span>

23. <span data-ttu-id="c0de0-282">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-282">Select **Finish**.</span></span> <span data-ttu-id="c0de0-283">يتم إغلاق المعالج ويظهر نشاط تدفق إنتاج جديداً في القائمة.</span><span class="sxs-lookup"><span data-stu-id="c0de0-283">The wizard closes and a new production flow activity appears in the list.</span></span>

24. <span data-ttu-id="c0de0-284">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="c0de0-284">Select **Save** on the Action Pane.</span></span>


### <a name="create-the-predecessor-and-successor-relationship-between-the-process-and-transfer-activity-with-no-constraints"></a><span data-ttu-id="c0de0-285">قم بإنشاء العلاقة السابقة واللاحقة بين العملية ونشاط النقل بدون قيود</span><span class="sxs-lookup"><span data-stu-id="c0de0-285">Create the predecessor and successor relationship between the process and transfer activity with no constraints</span></span>

1.  <span data-ttu-id="c0de0-286">قم بتمييز النشاط **RemoteTransfer** وعلى علامة التبويب **العناصر اللاحقة**، حدد الارتباط **إضافة عنصر لاحق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-286">Highlight the **RemoteTransfer** activity and on the **Successors** tab, select the **Add successor** link.</span></span>

2.  <span data-ttu-id="c0de0-287">حدد **نشاط العنصر اللاحق** لـ **RemoteTransfer**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-287">Select the **Successor Activity** of **RemoteTransfer**.</span></span>

3.  <span data-ttu-id="c0de0-288">أدخل **نسبة زمن الدورة** **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-288">Enter the **Cycle time ratio** of **1**.</span></span>

4.  <span data-ttu-id="c0de0-289">حدد الزر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-289">Select the **OK** button.</span></span>

5.  <span data-ttu-id="c0de0-290">أغلق صفحة **أنشطة تدفق الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-290">Close the **Production flow activities** page.</span></span>

6.  <span data-ttu-id="c0de0-291">في علامة التبويب السريعة **الإصدارات**، حدد زر القائمة **تنشيط > تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-291">On the **Versions** FastTab, select the **Activation > Activate** menu button.</span></span>

7.  <span data-ttu-id="c0de0-292">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-292">Select **OK**.</span></span> <span data-ttu-id="c0de0-293">يتم تغيير **حالة الخطة** إلى **نشطة.**</span><span class="sxs-lookup"><span data-stu-id="c0de0-293">The **Plan status** changes to **Active.**</span></span>


## <a name="exercise---create-activity-relations"></a><span data-ttu-id="c0de0-294">تدريب - إنشاء علاقات الأنشطة</span><span class="sxs-lookup"><span data-stu-id="c0de0-294">Exercise - Create activity relations</span></span>

<span data-ttu-id="c0de0-295">يحتاج Pierre إلى مراجعة تدفق إنتاج مكبر الصوت متوسط المدى 2 PF حتى يصبح العنصر اللاحق لنشاط النقل\_W12\_إلى\_W11 هو العملية\_النشاط\_نشاط واحد.</span><span class="sxs-lookup"><span data-stu-id="c0de0-295">Pierre needs to revise the Mid-Range Speaker 2 PF production flow to have the Transfer\_W12\_to\_W11 activity succeeded by the Process\_Activity\_1 activity.</span></span>

<span data-ttu-id="c0de0-296">تفاصيل علاقات نشاط النقل لتدفق الإنتاج:</span><span class="sxs-lookup"><span data-stu-id="c0de0-296">Details for production flow transfer activity relations:</span></span>

| <span data-ttu-id="c0de0-297">الحقل</span><span class="sxs-lookup"><span data-stu-id="c0de0-297">Field</span></span>            | <span data-ttu-id="c0de0-298">التفاصيل</span><span class="sxs-lookup"><span data-stu-id="c0de0-298">Details</span></span> |
|------------------|---------|
| <span data-ttu-id="c0de0-299">القيد</span><span class="sxs-lookup"><span data-stu-id="c0de0-299">Constraint</span></span>       | <span data-ttu-id="c0de0-300">ساعة واحدة</span><span class="sxs-lookup"><span data-stu-id="c0de0-300">1 hour</span></span>  |
| <span data-ttu-id="c0de0-301">نسبة زمن الدورة</span><span class="sxs-lookup"><span data-stu-id="c0de0-301">Cycle time ratio</span></span> | <span data-ttu-id="c0de0-302">2</span><span class="sxs-lookup"><span data-stu-id="c0de0-302">2</span></span>       |


### <a name="add-a-successor-to-the-production-flow-activity"></a><span data-ttu-id="c0de0-303">إضافة عنصر لاحق إلى نشاط تدفق الإنتاج</span><span class="sxs-lookup"><span data-stu-id="c0de0-303">Add a successor to the production flow activity</span></span>

1.  <span data-ttu-id="c0de0-304">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفق الإنتاج محدود الفاقد > تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-304">Go to **Production control > Setup > Lean production flow > Production flows**.</span></span>

2.  <span data-ttu-id="c0de0-305">حدد **الاسم** لتدفق الإنتاج **مكبر الصوت متوسط المدى 2 PF**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-305">Select the **Name** of the **Mid-Range Speaker 2 PF** production flow.</span></span>

3.  <span data-ttu-id="c0de0-306">في علامة التبويب السريعة **الإصدارات**، حدد **الأنشطة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-306">On the **Versions** FastTab, select **Activities**.</span></span>

4.  <span data-ttu-id="c0de0-307">في القائمة على اليمين، حدد النشاط **00074-النقل من المستودع 13 إلى 51**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-307">In the list on the left, select the **00074-Transfer from Warehouse 13 to 51** activity.</span></span>

5.  <span data-ttu-id="c0de0-308">في علامة التبويب السريعة **العناصر اللاحقة**، حدد **إضافة عنصر لاحق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-308">On the **Successors** FastTab, select **Add successor**.</span></span> <span data-ttu-id="c0de0-309">يتم فتح مربع الحوار **إنشاء علاقة نشاط**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-309">The **Create activity relation** dialog box opens.</span></span>

6.  <span data-ttu-id="c0de0-310">في مجموعة **العنصر اللاحق**، في القائمة المنسدلة **النشاط**، حدد النشاط **000082**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-310">In the **Successor** group, in the **Activity** drop-down list, select Activity **000082**.</span></span>

7.  <span data-ttu-id="c0de0-311">حدد خانة الاختيار **القيد**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-311">Select the **Constraint** check box.</span></span>

8.  <span data-ttu-id="c0de0-312">في حقل **قيمة القيد**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-312">In the **Constraint value** field, enter **1**.</span></span>

9.  <span data-ttu-id="c0de0-313">في القائمة المنسدلة **الوحدات**، حدد **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-313">In the **Units** drop-down list, select **hr**.</span></span>

10. <span data-ttu-id="c0de0-314">في حقل **نسبة زمن الدورة**، أدخل **2**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-314">In the **Cycle time ratio** field, enter **2**.</span></span>

11. <span data-ttu-id="c0de0-315">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-315">Select **OK**.</span></span>

12. <span data-ttu-id="c0de0-316">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="c0de0-316">Select **Save** on the Action Pane.</span></span>

13. <span data-ttu-id="c0de0-317">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="c0de0-317">Close the pages.</span></span>


## <a name="exercise---perform-validation-and-activation"></a><span data-ttu-id="c0de0-318">تدريب - إجراء التحقق من الصحة والتنشيط</span><span class="sxs-lookup"><span data-stu-id="c0de0-318">Exercise - Perform validation and activation</span></span> 

<span data-ttu-id="c0de0-319">يحتاج Pierre إلى التحقق من صحة تدفق إنتاج مكبر الصوت متوسط المدى 2 PF، الإصدار الثاني، للتأكد من أن التغييرات قد تم تنفيذها بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="c0de0-319">Pierre needs to validate the Mid-Range Speaker 2 PF production flow, Version 2, to confirm that the changes have been correctly implemented.</span></span>

1.  <span data-ttu-id="c0de0-320">انتقل إلى **التحكم بالإنتاج > الإعداد > تدفق الإنتاج محدود الفاقد > تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-320">Go to **Production control > Setup > Lean production flow > Production flows**.</span></span> <span data-ttu-id="c0de0-321">يتم فتح النموذج **تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-321">The **Production flows** form opens.</span></span>

2.  <span data-ttu-id="c0de0-322">حدد **الاسم** لتدفق الإنتاج **مكبر الصوت متوسط المدى 2 PF**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-322">Select the **Name** of the **Mid-Range Speaker 2 PF** production flow.</span></span> <span data-ttu-id="c0de0-323">يتم فتح النموذج **تدفقات الإنتاج** لتدفق الإنتاج المحدد.</span><span class="sxs-lookup"><span data-stu-id="c0de0-323">The **Production flows** form for the selected production flow opens.</span></span>

3.  <span data-ttu-id="c0de0-324">في علامة التبويب السريعة **الإصدارات**، حدد الإصدار **1**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-324">On the **Versions** FastTab, select version **1**.</span></span>

4.  <span data-ttu-id="c0de0-325">حدد **التحقق من الصحة**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-325">Select **Validate**.</span></span> <span data-ttu-id="c0de0-326">يتم فتح مربع الحوار **التحقق من صحة تدفق الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-326">The **Validate production flow** dialog box opens.</span></span>

5.  <span data-ttu-id="c0de0-327">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0de0-327">Select **OK**.</span></span>

6.  <span data-ttu-id="c0de0-328">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="c0de0-328">Close the pages.</span></span>
 
