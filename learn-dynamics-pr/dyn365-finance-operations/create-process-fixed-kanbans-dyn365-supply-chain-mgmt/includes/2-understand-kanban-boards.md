---
ms.openlocfilehash: de97c5faf7231695eed7ef629ec8a4a9645d66e2
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073801"
---
## <a name="process-actions"></a><span data-ttu-id="67686-101">إجراءات المعالجة</span><span class="sxs-lookup"><span data-stu-id="67686-101">Process actions</span></span>

<span data-ttu-id="67686-102">لا يمكن تنفيذ إجراءات المعالجة من التحضير والبدء والإكمال إلا عندما يتم التخطيط لوظيفة معالجة.</span><span class="sxs-lookup"><span data-stu-id="67686-102">The process actions of prepare, start, and complete can only be performed when a process job is planned.</span></span> <span data-ttu-id="67686-103">يجب أن تحتوي وظائف المعالجة التي لم يتم التخطيط لها بشكل صريح على الحقل **كمية التخطيط التلقائي** في صفحة **قاعدة كانبان** الذي تم تعيينه بالقيمة **1**.</span><span class="sxs-lookup"><span data-stu-id="67686-103">Process jobs that are not explicitly planned must have the **Automatic planning quantity** field on the **Kanban rule** page set to **1**.</span></span> <span data-ttu-id="67686-104">يتم تخطيط كافة وظائف المعالجة غير المخططة المرتبطة بهذه القاعدة تلقائياً عند إنشائها، ويمكن الآن إعدادها أو بدؤها أو إكمالها.</span><span class="sxs-lookup"><span data-stu-id="67686-104">All unplanned process jobs that are related to this rule are automatically planned when they are created and can now be prepared, started, or completed.</span></span>

## <a name="automatic-planning-of-kanbans"></a><span data-ttu-id="67686-105">التخطيط التلقائي لبطاقات كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-105">Automatic planning of kanbans</span></span>

<span data-ttu-id="67686-106">يتم تحديد معلمات القدرة الإنتاجية للتخطيط التلقائي لجدولة كانبان في قاعدة كانبان ونموذج تدفق الإنتاج محدود الفاقد المرتبط بالقدرة الإنتاجية لخلية العمل.</span><span class="sxs-lookup"><span data-stu-id="67686-106">The capacity parameters for automatic planning of the kanban schedule are defined on the kanban rule and Lean production flow model that are linked to the work cell capacity.</span></span>

<span data-ttu-id="67686-107">يتم تخطيط وظائف معالجة كانبان تلقائياً عند وصول عدد الوظائف غير المخطط لها المرتبطة بقاعدة كانبان إلى كمية التخطيط التلقائي.</span><span class="sxs-lookup"><span data-stu-id="67686-107">Kanban process jobs are automatically planned when the number of unplanned jobs that are related to the kanban rule reaches the automatic planning quantity.</span></span> <span data-ttu-id="67686-108">أي قيمة تبلغ 1 أو أكبر موضوعة في هذا الحقل ستؤدي إلى تخطيط وظائف كانبان تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="67686-108">Any value of 1 or greater that is placed in this field will cause the kanbans to automatically plan.</span></span> <span data-ttu-id="67686-109">إذا كانت كمية التخطيط التلقائي أكبر من 1، يتم تخطيط بطاقات كانبان التي تم تشغيلها معاً بشكل تسلسلي.</span><span class="sxs-lookup"><span data-stu-id="67686-109">If the automatic planning quantity is greater than 1, the kanbans that are triggered together are planned sequentially.</span></span>

## <a name="planning-period-fence"></a><span data-ttu-id="67686-110">الحد الزمني للتخطيط</span><span class="sxs-lookup"><span data-stu-id="67686-110">Planning period fence</span></span>

<span data-ttu-id="67686-111">عندما يكون الحد الزمني للتخطيط في نموذج تدفق الإنتاج هو 1، تتم إضافة وظائف كانبان إلى نهاية فترة التخطيط لجدول خلية العمل.</span><span class="sxs-lookup"><span data-stu-id="67686-111">When the planning period fence in the production flow model is 1, the kanban jobs are added to the end of the planning period of the work cell schedule.</span></span> <span data-ttu-id="67686-112">إذا تم تحميل فترة واحدة، فسيتم فتح الفترة التالية تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="67686-112">If one period is loaded, the next period is opened automatically.</span></span> <span data-ttu-id="67686-113">يمكنك تعيين وظائف كانبان كأولوية من خلال تعيينها على هذا النحو في لوحة جدول الكانبان.</span><span class="sxs-lookup"><span data-stu-id="67686-113">You can set the kanbans as priority by designating them as such on the Kanban schedule board.</span></span>

<span data-ttu-id="67686-114">عند تحديد أكثر من فترة واحدة في نموذج تدفق الإنتاج، يتم تحديد آخر فترة بدء ممكنة لكل وظيفة كانبان بالمعادلة التالية:</span><span class="sxs-lookup"><span data-stu-id="67686-114">When more than one period is defined in the production flow model, the latest possible start period is determined for each kanban job by the following formula:</span></span>

> <span data-ttu-id="67686-115">**تاريخ البدء = تاريخ الاستحقاق - دورة EPE**</span><span class="sxs-lookup"><span data-stu-id="67686-115">**Start date = due date - EPECycle**</span></span>

<span data-ttu-id="67686-116">يتم تكوين دورة EPE في نموذج تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="67686-116">The EPECycle is configured in the production flow model.</span></span>

## <a name="capacity-shortage-reaction"></a><span data-ttu-id="67686-117">الاستجابة للعجز في القدرة الإنتاجية</span><span class="sxs-lookup"><span data-stu-id="67686-117">Capacity shortage reaction</span></span>

<span data-ttu-id="67686-118">إذا كان تاريخ البدء المحسوب واقعاً في الماضي، فسيتم تعيين تاريخ البدء على اليوم.</span><span class="sxs-lookup"><span data-stu-id="67686-118">If the calculated start date is in the past, the start date is set to today.</span></span> <span data-ttu-id="67686-119">يقوم التخطيط التلقائي بمحاولة تحميل وظائف كانبان في الفترة المرتبطة بهذا التاريخ.</span><span class="sxs-lookup"><span data-stu-id="67686-119">Automatic planning tries to load the kanban jobs on the period that is related to this date.</span></span> <span data-ttu-id="67686-120">إذا لم تكن هذه المعالجة ممكنة، فسيتم التخطيط التلقائي وفقاً لإعداد ‏‫الاستجابة للعجز في القدرة الإنتاجية‬ في نموذج تدفق الإنتاج محدود الفاقد.</span><span class="sxs-lookup"><span data-stu-id="67686-120">If this process is not possible, automatic planning proceeds according to the capacity shortage reaction setting in the Lean production flow model.</span></span> <span data-ttu-id="67686-121">تتمثل الإعدادات الممكنة للاستجابة للعجز في القدرة الإنتاجية‬ فيما يلي:</span><span class="sxs-lookup"><span data-stu-id="67686-121">The possible capacity shortage reaction settings are:</span></span>

-   <span data-ttu-id="67686-122">**تأجيل** - يتم تأجيل الوظيفة حتى يوم توفر الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="67686-122">**Postpone** - The job is postponed until the day that throughput becomes available.</span></span>

-   <span data-ttu-id="67686-123">**إلغاء** - يتم إلغاء التخطيط التلقائي لوظيفة كانبان، وتظهر رسالة تشير إلى أنه لا يمكن التخطيط للوظيفة.</span><span class="sxs-lookup"><span data-stu-id="67686-123">**Cancel** - Automatic planning of the kanban job is canceled and a message displays indicating that the job could not be planned.</span></span>

-   <span data-ttu-id="67686-124">**إضافة إلى الفترة المطلوبة** - تتم إضافة الوظيفة إلى الفترة المجدولة للتاريخ المطلوب.</span><span class="sxs-lookup"><span data-stu-id="67686-124">**Add to the requested period** - The job is added to the scheduled period of the required date.</span></span> <span data-ttu-id="67686-125">وتكون النتيجة هي زيادة تحميل خلية العمل خلال الفترة المجدولة.</span><span class="sxs-lookup"><span data-stu-id="67686-125">The result is that the work cell is overloaded during the scheduled period.</span></span>

-   <span data-ttu-id="67686-126">**توزيع** - يتم توزيع بطاقات كانبان لحدث واحد على فترات الإنتاج المتاحة، بدءاً من أول فترة متاحة.</span><span class="sxs-lookup"><span data-stu-id="67686-126">**Distribute** - Kanbans of a single event are distributed to the available production periods, starting with the first available period.</span></span>

<span data-ttu-id="67686-127">إن المثال على الاستجابة للعجز في القدرة الإنتاجية سيكون كالآتي: إذا كانت كمية التخطيط التلقائي هي 3، فسيبحث التخطيط التلقائي عن فترة ذات قدرة إنتاجية كافية لبطاقات كانبان الثلاث التي تم تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="67686-127">An example of a capacity shortage reaction would be if the automatic planning quantity is 3, the automatic planning looks for a period that has enough capacity for the three triggered kanbans.</span></span>

## <a name="distribute-method"></a><span data-ttu-id="67686-128">أسلوب التوزيع</span><span class="sxs-lookup"><span data-stu-id="67686-128">Distribute method</span></span>

<span data-ttu-id="67686-129">إذا كانت القدرة الإنتاجية التي يتم طلبها بواسطة بطاقات كانبان التي تم تشغيلها أعلى من القدرة الإنتاجية اليومية للخلية، فسيتم تطبيق أسلوب *التوزيع* تلقائياً (لأنه لم يتم العثور على أجزاء مجانية إطلاقاً).</span><span class="sxs-lookup"><span data-stu-id="67686-129">If the capacity that is requested by the triggered kanbans is higher than the daily capacity of the cell, the *distribute* method is applied automatically (because a free slot could never be found).</span></span>

<span data-ttu-id="67686-130">بدءاً من الفترة المرتبطة بتاريخ البدء، تتم مراجعة الفترات من خلال الانتقال للخلف في الوقت حتى الفترة الفعلية (اليوم).</span><span class="sxs-lookup"><span data-stu-id="67686-130">Starting from the period that is related to the start date, the periods are checked, going backward in time, until the actual period (today).</span></span> <span data-ttu-id="67686-131">إذا لم يتم العثور على فترة زمنية قبل تاريخ الاستحقاق، فسيستمر البحث بعد تاريخ الاستحقاق ويستمر في المستقبل ما لم يتم العثور على فترة ذات قدرة إنتاجية كافية.</span><span class="sxs-lookup"><span data-stu-id="67686-131">If no slot can be found before the due date, the search continues after the due date and continues in the future unless a period with enough capacity can be found.</span></span>

<span data-ttu-id="67686-132">يحدد الحد الزمني للتخطيط عدد الفترات المتاحة للتخطيط، بدءاً من الفترة المرتبطة باليوم الفعلي.</span><span class="sxs-lookup"><span data-stu-id="67686-132">The planning period fence defines the number of available periods for planning, starting from the period that is related to the actual day.</span></span> <span data-ttu-id="67686-133">في حالة عدم العثور على قدرة إنتاجية متوفرة لإدراجها في كافة الفترات المتاحة، فسيتم إلغاء التخطيط التلقائي ويتم عرض رسالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="67686-133">If no available capacity can be found to slot in all available periods, automatic planning is canceled and an error message is displayed.</span></span>

## <a name="loading-kanban-jobs-on-the-kanban-schedule"></a><span data-ttu-id="67686-134">تحميل وظائف كانبان على جدول كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-134">Loading kanban jobs on the Kanban schedule</span></span> 

<span data-ttu-id="67686-135">يتكون جدول كانبان لكل خلية عمل من فترات تتوافق مع الإعدادات في نموذج تدفق الإنتاج محدود الفاقد.</span><span class="sxs-lookup"><span data-stu-id="67686-135">The Kanban schedule for each work cell consists of periods that correspond to the settings in the Lean production flow model.</span></span> <span data-ttu-id="67686-136">قد تكون الفترات يومية أو أسبوعية.</span><span class="sxs-lookup"><span data-stu-id="67686-136">The periods can be daily or weekly.</span></span>

<span data-ttu-id="67686-137">يتم تحديد مدى توفر كل فترة بالساعات من خلال وقت العمل للفترة المخصصة للتقويم.</span><span class="sxs-lookup"><span data-stu-id="67686-137">The availability of each period in hours is defined by the working time of the period that is assigned to the calendar.</span></span> <span data-ttu-id="67686-138">إذا كان نموذج القدرة الإنتاجية هو **الإنتاجية**، وكان نوع الفترة هو **يوم عمل قياسي**، فسيتم حساب القدرة على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="67686-138">If the capacity model is **throughput** and the period type is **standard work day**, the capacity is calculated as follows:</span></span>

> <span data-ttu-id="67686-139">**القدرة = الإنتاجية (يوم قياسي) × وقت العمل (الفترة) ÷ طول اليوم القياسي (التقويم)**</span><span class="sxs-lookup"><span data-stu-id="67686-139">**capacity = throughput (standard day) \* working time (period) ÷ length of standard day (calendar)**</span></span>

<span data-ttu-id="67686-140">يتم حساب حمل العمل لكل بطاقة كانبان استناداً إلى نسبة الإنتاجية للصنف المرتبط بخلية العمل في إعداد مجموعة الجداول محدودة الفاقد.</span><span class="sxs-lookup"><span data-stu-id="67686-140">The load of each kanban is calculated depending on the throughput ratio of the item that is related to the work cell in the lean schedule group setup.</span></span> <span data-ttu-id="67686-141">يعتمد الحساب على نموذج القدرة الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="67686-141">The calculation depends on the capacity model.</span></span>

<span data-ttu-id="67686-142">بالنسبة لصافي الإنتاجية، يتم حساب حمل العمل على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="67686-142">For throughput, the load is calculated as:</span></span>

> <span data-ttu-id="67686-143">**القدرة الإنتاجية = معدل الإنتاجية × كمية كانبان × عامل تصحيح الوحدة**</span><span class="sxs-lookup"><span data-stu-id="67686-143">**capacity load = throughput ratio \* Kanban quantity \* unit correction factor**</span></span>

<span data-ttu-id="67686-144">بالنسبة للساعات، يتم حساب حمل العمل على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="67686-144">For hours, the load is calculated as:</span></span>

> <span data-ttu-id="67686-145">**القدرة الإنتاجية = زمن الدورة (النشاط) × معدل الإنتاجية × تصحيح الكمية (كمية الوظائف) × عامل تصحيح الوحدة**</span><span class="sxs-lookup"><span data-stu-id="67686-145">**capacity load = cycle time (activity) \* throughput ratio \* quantity correction (job quantity) \* unit correction factor**</span></span>

<span data-ttu-id="67686-146">يُضاف حمل عمل كل بطاقة كانبان مخطط لها لكل فترة لتحديد حمل عمل الفترة.</span><span class="sxs-lookup"><span data-stu-id="67686-146">The load of each planned kanban is added for each period to determine the period's load.</span></span> <span data-ttu-id="67686-147">يتم حساب القدرة الإنتاجية لوظيفة معالجة كانبان عندما يتم تخطيط وظيفة معالجة كانبان للمرة الأولى.</span><span class="sxs-lookup"><span data-stu-id="67686-147">The capacity load of a kanban process job is calculated whenever a kanban process job is planned for the first time.</span></span>
<span data-ttu-id="67686-148">يتم استخدام عوامل تصحيح الوحدة في المثيل الذي تختلف فيه وحدة قياس الوظيفة عن وحدة قياس قدرة خلية العمل.</span><span class="sxs-lookup"><span data-stu-id="67686-148">Unit correction factors are used in the instance where a job's unit of measure is different than the unit of measure of the work cell's capacity.</span></span> <span data-ttu-id="67686-149">يتم استخدام تصحيح الكمية إذا كانت كمية الوظيفة تختلف عن كمية النشاط أو كمية زمن الدورة.</span><span class="sxs-lookup"><span data-stu-id="67686-149">The quantity correction is used if the job quantity differs from the activity quantity or the cycle time quantity.</span></span>

## <a name="lean-schedule-groups"></a><span data-ttu-id="67686-150">مجموعات الجداول محدودة الفاقد</span><span class="sxs-lookup"><span data-stu-id="67686-150">Lean schedule groups</span></span>

<span data-ttu-id="67686-151">تسمح الصفحة التي يتم الوصول إليها من خلال **إدارة معلومات المنتج > مجموعات الجداول محدودة الفاقد** للمستخدمين بإمكانية تعيين نسب الإنتاجية والألوان لجدولة كانبان للأصناف أو مجموعات الأصناف.</span><span class="sxs-lookup"><span data-stu-id="67686-151">The **Product information management > Lean manufacturing > Lean schedule groups** page allows users to assign colors and throughput ratios for kanban scheduling to items or item groups.</span></span> <span data-ttu-id="67686-152">يمكن تنفيذ هذه العملية بشكل عام أو خاص لخلية العمل.</span><span class="sxs-lookup"><span data-stu-id="67686-152">This process can be done globally or specifically for a work cell.</span></span> <span data-ttu-id="67686-153">يمكن استخدام الألوان لفهم الخصائص المختلفة للأصناف التي يتم إنتاجها في الخلية لأغراض الجدولة بشكل مرئي.</span><span class="sxs-lookup"><span data-stu-id="67686-153">The colors can be used to visually understand the different characteristics of items that are produced in the cell for scheduling purposes.</span></span>


## <a name="lean-schedule-items"></a><span data-ttu-id="67686-154">أصناف الجداول محدودة الفاقد</span><span class="sxs-lookup"><span data-stu-id="67686-154">Lean schedule items</span></span>

<span data-ttu-id="67686-155">يمكن تعيين أصناف أو مجموعات أصناف معينة إلى مجموعة جداول محدودة الفاقد بنسبة إنتاجية معينة باستخدام الصفحة **أصناف الجداول محدودة الفاقد**.</span><span class="sxs-lookup"><span data-stu-id="67686-155">Specific items or groups of items can be assigned to a Lean schedule group with a specific throughput ratio by using the **Lean schedule items** page.</span></span>

## <a name="kanban-schedule-board"></a><span data-ttu-id="67686-156">لوحة جدول الكانبان</span><span class="sxs-lookup"><span data-stu-id="67686-156">Kanban schedule board</span></span>

<span data-ttu-id="67686-157">تعرض **التحكم بالإنتاج > كانبان > لوحة جدول الكانبان** وظائف كانبان المجدولة أثناء الحد الزمني للتخطيط الذي تم تحديده في خلية العمل.</span><span class="sxs-lookup"><span data-stu-id="67686-157">The **Production control > Kanban > Kanban schedule board** displays the kanban jobs that are scheduled during the planning time fence that is defined on the work cell.</span></span> <span data-ttu-id="67686-158">يمكن جدولة بطاقات كانبان فقط في هذا الحد الزمني للتخطيط.</span><span class="sxs-lookup"><span data-stu-id="67686-158">Kanbans can only be scheduled within this planning time fence.</span></span>


## <a name="kanban-job-scheduling"></a><span data-ttu-id="67686-159">جدولة وظيفة كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-159">Kanban job scheduling</span></span>

<span data-ttu-id="67686-160">في الصفحة **التحكم بالإنتاج > كانبان > جدولة وظيفة كانبان**، في علامة التبويب **الخطة**، يمكن إعادة تعيين حالات وظائف مختلفة إلى حالات أخرى عن طريق استخدام الزر **إرجاع حالة المهمة**.</span><span class="sxs-lookup"><span data-stu-id="67686-160">On the **Production control > Kanban > Kanban job scheduling** page, on the **PLAN** tab, different job statuses can be reset to other statuses by using the **Revert job status** button.</span></span> <span data-ttu-id="67686-161">تعمل وظيفة إعادة الضبط على عكس الإجراءات التي تمت معالجتها مسبقاً للوصول إلى الحالة المتوافقة.</span><span class="sxs-lookup"><span data-stu-id="67686-161">The reset function reverses the previously processed actions to reach the correspondent status.</span></span> <span data-ttu-id="67686-162">إذا كان يجب إعادة تعيين أكثر من حالة واحدة، فسيتم تنفيذ جميع الإجراءات العكسية خطوة بخطوة.</span><span class="sxs-lookup"><span data-stu-id="67686-162">If more than one status must be reset, all reverse actions are performed step by step.</span></span>


## <a name="kanban-job-status-for-process-jobs"></a><span data-ttu-id="67686-163">حالة وظيفة كانبان لوظائف المعالجة</span><span class="sxs-lookup"><span data-stu-id="67686-163">Kanban job status for process jobs</span></span>

<span data-ttu-id="67686-164">تكون حالة وظيفة كانبان مهمة لفهم عملية التخطيط لبطاقات كانبان.</span><span class="sxs-lookup"><span data-stu-id="67686-164">The kanban job status is important for understanding the planning process for kanbans.</span></span> <span data-ttu-id="67686-165">بإمكان وظيفة كانبان من النوع "معالجة" أن تكون بالحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="67686-165">A kanban job of the Process type can have the following statuses:</span></span>

-   <span data-ttu-id="67686-166">**غير مخطط**</span><span class="sxs-lookup"><span data-stu-id="67686-166">**Not planned**</span></span>

-   <span data-ttu-id="67686-167">**مخطط**</span><span class="sxs-lookup"><span data-stu-id="67686-167">**Planned**</span></span>

-   <span data-ttu-id="67686-168">**مُعد**</span><span class="sxs-lookup"><span data-stu-id="67686-168">**Prepared**</span></span>

-   <span data-ttu-id="67686-169">**قيد التقدم**</span><span class="sxs-lookup"><span data-stu-id="67686-169">**In progress**</span></span>

-   <span data-ttu-id="67686-170">**مكتمل**</span><span class="sxs-lookup"><span data-stu-id="67686-170">**Completed**</span></span>

<span data-ttu-id="67686-171">تعرض الصورة التالية الخيارات التي يتم عرضها في صفحة **عكس حالة وظيفة الكانبان** في **التحكم بالإنتاج > كانبان > جدولة وظيفة كانبان**.</span><span class="sxs-lookup"><span data-stu-id="67686-171">The following image shows the options that are offered on the **Revert kanban job status** page in **Production control > Kanban > Kanban job scheduling**.</span></span>

![لقطة شاشة لصفحة عكس حالة وظيفة الكانبان.](../media/revert-1.png)

<span data-ttu-id="67686-173">في صفحة **التحكم بالإنتاج > كانبان > لوحة كانبان لوظائف المعالجة**، يتم تنشيط الأزرار الخاصة بمعالجة أنشطة معينة لوظيفة كانبان هذه (على سبيل المثال، **إعداد/بدء**) استناداً إلى حالة وظيفة كانبان.</span><span class="sxs-lookup"><span data-stu-id="67686-173">On the **Production control > Kanban > Kanban board for process jobs** page, the buttons for processing certain activities for that kanban job (for example, **Prepare/Start**) are activated depending on the kanban job's status.</span></span>


## <a name="changing-kanban-job-statuses-preconditions"></a><span data-ttu-id="67686-174">تغيير حالات وظيفة كانبان: شروط مسبقة</span><span class="sxs-lookup"><span data-stu-id="67686-174">Changing kanban job statuses: Preconditions</span></span>

<span data-ttu-id="67686-175">يتم شرح الشروط المسبقة المتنوعة والنتائج المختلفة لإعادة تعيين وظائف كانبان في الجدول التالي.</span><span class="sxs-lookup"><span data-stu-id="67686-175">The various preconditions and results of resetting kanban jobs are explained in the following table.</span></span>

| <span data-ttu-id="67686-176">حالات العكس</span><span class="sxs-lookup"><span data-stu-id="67686-176">Reversal Statuses</span></span> | <span data-ttu-id="67686-177">الشروط المسبقة</span><span class="sxs-lookup"><span data-stu-id="67686-177">Pre-Conditions</span></span> | <span data-ttu-id="67686-178">النتيجة</span><span class="sxs-lookup"><span data-stu-id="67686-178">Result</span></span> |
| :------------------- | :------------------- |:----------------|
| <span data-ttu-id="67686-179">مكتمل إلى قيد التقدم</span><span class="sxs-lookup"><span data-stu-id="67686-179">Completed to in progress</span></span> | <span data-ttu-id="67686-180">لا تتم معالجة المعاملات المالية ذات الصلة (إن وجدت).</span><span class="sxs-lookup"><span data-stu-id="67686-180">The related financial transactions (if any) are not processed.</span></span> <span data-ttu-id="67686-181">يجب أن تكون هناك حركات كافية في متناول اليد لعكس الحركات الفعلية.</span><span class="sxs-lookup"><span data-stu-id="67686-181">There must be enough transactions on hand to reverse the physical transactions.</span></span> <span data-ttu-id="67686-182">بطاقة كانبان ذات الصلة ليست بالحالة "فارغ".</span><span class="sxs-lookup"><span data-stu-id="67686-182">The related kanban is not of the Empty status.</span></span> | <span data-ttu-id="67686-183">عكس الحركات الفعلية (الاستلام والإصدارات).</span><span class="sxs-lookup"><span data-stu-id="67686-183">Reverse the physical transactions (receipt and issues).</span></span> <span data-ttu-id="67686-184">إذا كانت هذه هي آخر وظيفة في الكانبان، فأعد تعيين حالة الكانبان إلى **قيد التقدم**.</span><span class="sxs-lookup"><span data-stu-id="67686-184">If this was the last job in the kanban, reset the kanban status to **In progress**.</span></span> |
| <span data-ttu-id="67686-185">مخطط إلى غير مخطط</span><span class="sxs-lookup"><span data-stu-id="67686-185">Planned to Not planned</span></span> | <span data-ttu-id="67686-186">إذا تم تعيين كمية التخطيط التلقائي إلى **1**، فلن يتم تنفيذ هذه الخطوة على إعادة التعيين؛ وتظل الوظيفة بالحالة "مخطط".</span><span class="sxs-lookup"><span data-stu-id="67686-186">If the automatic planning quantity is assigned to **1**, this step is not performed on the reset; the job remains at a status of Planned.</span></span> | <span data-ttu-id="67686-187">يزيل تاريخ البدء المخطط له والتسلسل المرتبط به.</span><span class="sxs-lookup"><span data-stu-id="67686-187">Removes the planned starting date and the related sequence.</span></span> |
| <span data-ttu-id="67686-188">معد إلى مخطط</span><span class="sxs-lookup"><span data-stu-id="67686-188">Prepared to planned</span></span> | <span data-ttu-id="67686-189">بلا</span><span class="sxs-lookup"><span data-stu-id="67686-189">None</span></span> | <span data-ttu-id="67686-190">قم بعكس معاملات إصدار التدفق الأمامي، إن وجدت.</span><span class="sxs-lookup"><span data-stu-id="67686-190">Reverse the forward flushing issue transactions, if any.</span></span> <span data-ttu-id="67686-191">إذا كانت البطاقات المتداولة مستخدمه وكانت طريقه التعيين **يدوية**، سيتم حجز تعيين البطاقة.</span><span class="sxs-lookup"><span data-stu-id="67686-191">If the circulating cards are used and the assignment method is **Manual**, the card assignment is reversed.</span></span> <span data-ttu-id="67686-192">إذا كانت هذه هي الوظيفة الأولى في كانبان، فقم أيضاً بإعادة تعيين حالة كانبان إلى **غير مخطط**.</span><span class="sxs-lookup"><span data-stu-id="67686-192">If it is the first job of the kanban, also reset the kanban status to **Not planned**.</span></span> |
| <span data-ttu-id="67686-193">قيد التقدم إلى معد</span><span class="sxs-lookup"><span data-stu-id="67686-193">In progress to prepared</span></span> | <span data-ttu-id="67686-194">بلا</span><span class="sxs-lookup"><span data-stu-id="67686-194">None</span></span> | <span data-ttu-id="67686-195">يقوم بإعادة تعيين حالة الوظيفة إلى **معد**.</span><span class="sxs-lookup"><span data-stu-id="67686-195">Resets the job status to **Prepared**.</span></span> |

<span data-ttu-id="67686-196">بعد إعادة التعيين إلى حالة معينة، لا يتم تشغيل التخطيط التلقائي تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="67686-196">After a reset to a specific status, the automatic planning is not automatically launched.</span></span> <span data-ttu-id="67686-197">إذا كان يجب تشغيل التخطيط التلقائي مرة أخرى لكانبان، يجب بدء التخطيط التلقائي يدوياً لقاعدة كانبان.</span><span class="sxs-lookup"><span data-stu-id="67686-197">If automatic planning should be run again for the kanban, automatic planning needs to be started manually for the kanban rule.</span></span>

<span data-ttu-id="67686-198">تتوفر لديك أيضاً الخيارات التالية عند تغيير حالة وظيفة كانبان:</span><span class="sxs-lookup"><span data-stu-id="67686-198">You also have the following options when changing a kanban job's status:</span></span>

-   <span data-ttu-id="67686-199">**تخطيط شجرة تثبيت السعر بالكامل** - عند التخطيط لوظيفة كانبان ذات أنشطة متعددة، يخطط هذا الخيار لوظائف كانبان المتبقية في المراحل التمهيدية.</span><span class="sxs-lookup"><span data-stu-id="67686-199">**Plan entire pegging tree** - When planning a kanban job with multiple activities, this option plans the remaining upstream kanban jobs.</span></span>

-   <span data-ttu-id="67686-200">**استخدام قاعدة كانبان البديلة** - يستخدم قاعدة كانبان بديلة للإيفاء بالمتطلبات المحددة.</span><span class="sxs-lookup"><span data-stu-id="67686-200">**Use alternative kanban rule** - Uses an alternative kanban rule to fulfill selected requirements.</span></span> <span data-ttu-id="67686-201">يستخدم هذا الخيار حيث يمكن للمنتج المرور خلال نشاط بديل.</span><span class="sxs-lookup"><span data-stu-id="67686-201">This option is used where a product can go through alternate activity.</span></span>

-   <span data-ttu-id="67686-202">**حالة توريد شجرة تثبيت السعر** - يتحقق من حالة التوريد لجميع وظائف كانبان ذات المستوى الأدنى في شجرة تثبيت السعر.</span><span class="sxs-lookup"><span data-stu-id="67686-202">**Pegging tree supply status** - Checks the supply status of all lower-level kanbans in the pegging tree.</span></span>

## <a name="kanban-printing"></a><span data-ttu-id="67686-203">طباعة كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-203">Kanban printing</span></span>

<span data-ttu-id="67686-204">لا يلزم طباعة بطاقات كانبان وقوائم الانتقاء، ولكن يمكن استخدامها للإشارة إلى العمليات الواقعة في صالة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="67686-204">The printing of kanban cards and pick lists is not required but can be used to signal processes on the production floor.</span></span> <span data-ttu-id="67686-205">يوفر Supply Chain Management عدة سيناريوهات لطباعة قوائم الانتقاء وبطاقات كانبان:</span><span class="sxs-lookup"><span data-stu-id="67686-205">Supply Chain Management offers several scenarios for printing pick lists and kanban cards:</span></span>

-   <span data-ttu-id="67686-206">طباعة البطاقات المتداولة عند إنشاء البطاقات المتداولة</span><span class="sxs-lookup"><span data-stu-id="67686-206">Printing of circulating cards on creation of the circulating cards</span></span>

-   <span data-ttu-id="67686-207">الطباعة اليدوية لبطاقات كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-207">Manual printing of kanban cards</span></span>

-   <span data-ttu-id="67686-208">الطباعة التلقائية لبطاقات كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-208">Automatic printing of kanban cards</span></span>

-   <span data-ttu-id="67686-209">الطباعة اليدوية لقوائم الانتقاء</span><span class="sxs-lookup"><span data-stu-id="67686-209">Manual printing of pick lists</span></span>

-   <span data-ttu-id="67686-210">الطباعة التلقائية لقوائم الانتقاء مع بطاقة كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-210">Automatic printing of pick lists with the kanban card</span></span>

-   <span data-ttu-id="67686-211">تحديد الأولوية على بطاقات كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-211">Priority designation on kanban cards</span></span>

<span data-ttu-id="67686-212">يمكنك استخدام بطاقات كانبان المطبوعة لمسح تقدم كانبان والإبلاغ عنه باستخدام لوحات جدول الكانبان.</span><span class="sxs-lookup"><span data-stu-id="67686-212">You can use the printed kanban cards to scan and report the progress of a kanban by using the Kanban schedule boards.</span></span>

<span data-ttu-id="67686-213">[![لقطة شاشة لبطاقة كانبان المطبوعة.](../media/print-1.png)](../media/print-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="67686-213">[![A screenshot of the printed kanban card.](../media/print-1.png)](../media/print-1.png#lightbox)</span></span>

<span data-ttu-id="67686-214">يمكن أن تتم الطباعة اليدوية لبطاقات كانبان من أي من الصفحات التالية:</span><span class="sxs-lookup"><span data-stu-id="67686-214">The manual printing of kanban cards can occur from any of the following pages:</span></span>

-   <span data-ttu-id="67686-215">لوحة كانبان لوظائف المعالجة</span><span class="sxs-lookup"><span data-stu-id="67686-215">Kanban board for process jobs</span></span>

-   <span data-ttu-id="67686-216">لوحة كانبان لمهام التحويل</span><span class="sxs-lookup"><span data-stu-id="67686-216">Kanban board for transfer jobs</span></span>

-   <span data-ttu-id="67686-217">جدولة وظيفة كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-217">Kanban job scheduling</span></span>

-   <span data-ttu-id="67686-218">قواعد كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-218">Kanban rules</span></span> 

-   <span data-ttu-id="67686-219">تفاصيل كانبان</span><span class="sxs-lookup"><span data-stu-id="67686-219">Kanban details</span></span> 

## <a name="automatic-printing-of-kanban-cards-and-pick-lists"></a><span data-ttu-id="67686-220">الطباعة التلقائية لبطاقات كانبان وقوائم الانتقاء</span><span class="sxs-lookup"><span data-stu-id="67686-220">Automatic printing of kanban cards and pick lists</span></span>

<span data-ttu-id="67686-221">في بعض الحالات، قد ترغب في طباعة بطاقات كانبان تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="67686-221">In some cases, you might want to automatically print the kanban cards.</span></span> <span data-ttu-id="67686-222">يمكن إعداد بطاقات كانبان لطباعتها تلقائياً عندما يصل كانبان إلى حالة معينة.</span><span class="sxs-lookup"><span data-stu-id="67686-222">Kanban cards can be set up to automatically print when a kanban reaches a specific status.</span></span>

<span data-ttu-id="67686-223">لتغيير هذه الإعدادات، انتقل إلى: **إدارة معلومات المنتج > Lean manufacturing> قواعد كانبان**.</span><span class="sxs-lookup"><span data-stu-id="67686-223">To change these settings, go to: **Product information Management > Lean manufacturing > Kanban rules**.</span></span>

<span data-ttu-id="67686-224">تتمثل الخيارات الموجودة على صفحة **قواعد كانبان** فيما يلي:</span><span class="sxs-lookup"><span data-stu-id="67686-224">The options on the **Kanban rules** page are:</span></span>

-   <span data-ttu-id="67686-225">**بلا**</span><span class="sxs-lookup"><span data-stu-id="67686-225">**None**</span></span>

-   <span data-ttu-id="67686-226">**إنشاء**</span><span class="sxs-lookup"><span data-stu-id="67686-226">**Creation**</span></span>

-   <span data-ttu-id="67686-227">**تخطيط**</span><span class="sxs-lookup"><span data-stu-id="67686-227">**Plan**</span></span>

-   <span data-ttu-id="67686-228">**إعداد**</span><span class="sxs-lookup"><span data-stu-id="67686-228">**Prepare**</span></span>

-   <span data-ttu-id="67686-229">**البدء**</span><span class="sxs-lookup"><span data-stu-id="67686-229">**Start**</span></span>

-   <span data-ttu-id="67686-230">**استلام**</span><span class="sxs-lookup"><span data-stu-id="67686-230">**Receive**</span></span>

<span data-ttu-id="67686-231">عندما يصل كانبان إلى الحالة المحددة التي تم إعدادها في صفحة **قاعدة كانبان**، تتم طباعة بطاقة كانبان تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="67686-231">When a kanban reaches the specified status that was set up on the **Kanban rule** page, the kanban card will automatically print.</span></span> <span data-ttu-id="67686-232">عند الرغبة، يمكنك طباعة قائمة انتقاء في نفس الوقت.</span><span class="sxs-lookup"><span data-stu-id="67686-232">If desired, you could print a pick list at the same time.</span></span> 
