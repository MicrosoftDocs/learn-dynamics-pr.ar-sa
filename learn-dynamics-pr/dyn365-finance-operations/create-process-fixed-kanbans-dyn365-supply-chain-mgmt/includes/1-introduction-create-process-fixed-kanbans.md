---
ms.openlocfilehash: 8de82610badd7d88d143582e668290815c7f9184
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073785"
---
<span data-ttu-id="adf4f-101">في Dynamics 365 Supply Chain Management، يتم تنفيذ كانبان كإطار عمل لتخطيط وتتبع ومعالجة التصنيع والتزويد، استناداً إلى إشارات السحب.</span><span class="sxs-lookup"><span data-stu-id="adf4f-101">In Dynamics 365 Supply Chain Management, a kanban is implemented as a framework to plan, track, and process manufacturing and replenishment, based on pull signals.</span></span>

## <a name="kanban-replenishment-strategies"></a><span data-ttu-id="adf4f-102">استراتيجيات تزويد كانبان</span><span class="sxs-lookup"><span data-stu-id="adf4f-102">Kanban replenishment strategies</span></span>

<span data-ttu-id="adf4f-103">استراتيجيات التزويد المختلفة في كانبان عبارة عن كانبان للكميات الثابتة وبطاقات كانبان المجدولة وبطاقات كانبان للحدث.</span><span class="sxs-lookup"><span data-stu-id="adf4f-103">The various kanban replenishment strategies are fixed quantity kanbans, scheduled kanbans, and event kanbans.</span></span> <span data-ttu-id="adf4f-104">تُستخدم هذه الاستراتيجيات للتعامل مع سيناريوهات التصنيع والتزويد الشائعة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-104">These strategies are used to handle common manufacturing and replenishment scenarios.</span></span>

<span data-ttu-id="adf4f-105">توضح الوحدات التالية الغرض من استراتيجيات تزويد موارد كانبان المختلفة لتشغيل إشارات سحب كانبان والفائدة التي يمكن أن تقدمها هذه الآليات لمؤسسات Lean.</span><span class="sxs-lookup"><span data-stu-id="adf4f-105">The next units demonstrate the purpose of the various kanban replenishment strategies for triggering kanban pull signals and the benefit that those mechanisms can offer to Lean organizations.</span></span>

<span data-ttu-id="adf4f-106">استراتيجيات التزويد هي:</span><span class="sxs-lookup"><span data-stu-id="adf4f-106">The replenishment strategies are:</span></span>

-   <span data-ttu-id="adf4f-107">**ثابتة** - عادةً ما تُستخدم هذه الاستراتيجية في سيناريوهات التصنيع حسب المخزون.</span><span class="sxs-lookup"><span data-stu-id="adf4f-107">**Fixed** - Typically, this strategy is used in make-to-stock scenarios.</span></span>

-   <span data-ttu-id="adf4f-108">**مجدولة** - تُستخدم هذه الاستراتيجية في سيناريوهات التصنيع حسب المخزون.</span><span class="sxs-lookup"><span data-stu-id="adf4f-108">**Scheduled** - This strategy is used in make-to-stock scenarios.</span></span>

-   <span data-ttu-id="adf4f-109">**الحدث** - تُستخدم هذه الاستراتيجية عادةً في سيناريوهات حسب الطلب.</span><span class="sxs-lookup"><span data-stu-id="adf4f-109">**Event** - This strategy is typically used in make-to-order scenarios.</span></span>

<span data-ttu-id="adf4f-110">يُعد كانبان جزءاً أساسياً من نظام سحب التوريد، وهو عنصر حاسم في الإنتاج/التوريد الخاص بمؤسسات lean.</span><span class="sxs-lookup"><span data-stu-id="adf4f-110">A kanban is an essential part of a pull system of supply, which is a critical element of lean production/supply.</span></span> <span data-ttu-id="adf4f-111">عندما يتم استهلاك كانبان، يجب أن يتم تمريره (تشغيله) إلى مصدر التوريد لتزويده.</span><span class="sxs-lookup"><span data-stu-id="adf4f-111">When a kanban has been consumed, it should be passed (triggered) to the source of supply to replenish it.</span></span> <span data-ttu-id="adf4f-112">يتم تحديد مصدر التوريد هذا من خلال أنشطة تدفق الإنتاج التي يرتبط بها كانبان.</span><span class="sxs-lookup"><span data-stu-id="adf4f-112">This source of supply is defined through the production flow activities to which the kanban is linked.</span></span>

<span data-ttu-id="adf4f-113">ترتبط قواعد كانبان في Supply Chain Management بتدفقات الإنتاج باعتبارها الأساس الذي يحدد أنشطة كانبان.</span><span class="sxs-lookup"><span data-stu-id="adf4f-113">Kanban rules in Supply Chain Management are tied to production flows as the foundation that defines the activities of a kanban.</span></span> <span data-ttu-id="adf4f-114">يمكن إعداد قواعد كانبان لدعم مجموعة متنوعة من سيناريوهات التجهيز للمخزون والتصنيع حسب الطلب.</span><span class="sxs-lookup"><span data-stu-id="adf4f-114">Kanban rules can be set up to support a variety of make-to-stock and make-to-order scenarios.</span></span>

## <a name="kanban-types"></a><span data-ttu-id="adf4f-115">أنواع كانبان</span><span class="sxs-lookup"><span data-stu-id="adf4f-115">Kanban types</span></span>

<span data-ttu-id="adf4f-116">نوعا كانبان هما **التصنيع** و **السحب**.</span><span class="sxs-lookup"><span data-stu-id="adf4f-116">The two kanban types are **Manufacturing** and **Withdrawal**.</span></span> <span data-ttu-id="adf4f-117">تُستخدم أنواع كانبان هذه لتصنيع المواد ونقلها في عملية الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="adf4f-117">These kanban types are used to manufacture and transfer materials in the production process.</span></span>


## <a name="manufacturing-kanban"></a><span data-ttu-id="adf4f-118">كانبان التصنيع</span><span class="sxs-lookup"><span data-stu-id="adf4f-118">Manufacturing kanban</span></span>

<span data-ttu-id="adf4f-119">يتم تعيين كانبان من نوع التصنيع لعملية تقوم بإضافة قيمة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-119">A kanban of the type Manufacturing is assigned to a process that adds value.</span></span> <span data-ttu-id="adf4f-120">يرتبط كانبان بنشاط تدفق إنتاج، وبالتالي مجموعة موارد لها دور خلية عمل.</span><span class="sxs-lookup"><span data-stu-id="adf4f-120">The kanban is linked to a production flow activity and thus a resource group with the role of a work cell.</span></span> <span data-ttu-id="adf4f-121">ترتبط بطاقات كانبان التصنيع بنشاط عملية واحد على الأقل.</span><span class="sxs-lookup"><span data-stu-id="adf4f-121">Manufacturing kanbans relate to at least one process activity.</span></span>

<span data-ttu-id="adf4f-122">يجب أن يكون النشاط الأول لكانبان التصنيع عبارة عن نشاط عملية.</span><span class="sxs-lookup"><span data-stu-id="adf4f-122">The first activity of a manufacturing kanban must be a process activity.</span></span>
<span data-ttu-id="adf4f-123">يمكن أن يتبع نشاط العملية عملية نقل أو نشاط عملية آخر، مما يسمح لكانبان بتوسيع أنشطة متعددة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-123">A process activity can be followed by a transfer or another process activity, allowing a kanban to span multiple activities.</span></span>

<span data-ttu-id="adf4f-124">يتم أيضاً تصميم أنشطة التعاقد من الباطن على أنها أنشطة واستخدام بطاقات كانبان التصنيع للمعالجة التي تحدث عند المورد.</span><span class="sxs-lookup"><span data-stu-id="adf4f-124">Subcontracting activities are also modeled as activities and use manufacturing kanbans for the processing that occurs at the vendor.</span></span>

<span data-ttu-id="adf4f-125">تظهر وظائف العمليات الجديدة أو غير المخططة على لوحة جدولة كانبان ليتم جدولتها إذا لم يتم تكوينها ليتم التخطيط لها تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="adf4f-125">New or unplanned process jobs appear on the kanban schedule board to be scheduled if they have not been configured to be automatically planned.</span></span> <span data-ttu-id="adf4f-126">إذا تم تخطيط الوظائف تلقائياً، فستتم إضافتها مباشرةً إلى جدول كانبان ويمكن معالجتها مباشرةً باستخدام لوحة جدولة كانبان لوظائف المعالجة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-126">If the jobs are automatically planned, they are added directly to the kanban schedule and can be processed directly with the Kanban schedule board for process jobs.</span></span>

### <a name="planning-period-and-time-fence"></a><span data-ttu-id="adf4f-127">فتره التخطيط والحد الزمني</span><span class="sxs-lookup"><span data-stu-id="adf4f-127">Planning period and time fence</span></span>

<span data-ttu-id="adf4f-128">يتم تخطيط وظائف عملية كانبان استناداً إلى تكوين نموذج تدفق الإنتاج المرتبط بخلية العمل.</span><span class="sxs-lookup"><span data-stu-id="adf4f-128">Kanban process jobs are planned based on the configuration of the production flow model that is associated with the work cell.</span></span> <span data-ttu-id="adf4f-129">تحدد فترة التخطيط والحدود الزمنية للتخطيط التي تم تعيينها في نموذج تدفق الإنتاج فترات لوحة جدولة كانبان.</span><span class="sxs-lookup"><span data-stu-id="adf4f-129">The Planning period and Planning time fence that are set on the production flow model define the periods for the Kanban schedule board.</span></span> <span data-ttu-id="adf4f-130">يمكن أن تكون فترات التخطيط بالأيام أو الأسابيع.</span><span class="sxs-lookup"><span data-stu-id="adf4f-130">Planning periods can be either days or weeks.</span></span> <span data-ttu-id="adf4f-131">تعرض لوحة جدولة كانبان وظائف كانبان المجدولة أثناء الحد الزمني المحدد للتخطيط.</span><span class="sxs-lookup"><span data-stu-id="adf4f-131">The Kanban schedule board displays the kanban jobs that are scheduled during the defined planning time fence.</span></span> <span data-ttu-id="adf4f-132">يمكن جدولة بطاقات كانبان فقط في هذا الحد الزمني للتخطيط.</span><span class="sxs-lookup"><span data-stu-id="adf4f-132">Kanbans can only be scheduled within this planning time fence.</span></span>

### <a name="capacity-shortage-reaction"></a><span data-ttu-id="adf4f-133">الاستجابة للعجز في القدرة الإنتاجية</span><span class="sxs-lookup"><span data-stu-id="adf4f-133">Capacity shortage reaction</span></span>

<span data-ttu-id="adf4f-134">يحدد رد فعل نقص القدرة طريقة جدولة كانبان التي يجب عليك استخدامها إذا لم تتوفر القدرة أثناء الفترة المطلوبة عندما يتم تخطيط بطاقات كانبان تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="adf4f-134">The Capacity shortage reaction defines the method of kanban scheduling that you should use if no capacity is available during the required period when kanbans are automatically planned.</span></span> <span data-ttu-id="adf4f-135">يتضمن تفاعل تخزين القدرة الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="adf4f-135">The Capacity storage reaction includes the following options:</span></span>

-   <span data-ttu-id="adf4f-136">**تأجيل** - يتم تأجيل الوظيفة حتى يوم توفر الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="adf4f-136">**Postpone** - The job is postponed until the day that throughput becomes available.</span></span>

-   <span data-ttu-id="adf4f-137">**إلغاء** - تم إلغاء التخطيط التلقائي لوظيفة كانبان.</span><span class="sxs-lookup"><span data-stu-id="adf4f-137">**Cancel** - Automatic planning of the kanban job is canceled.</span></span>

-   <span data-ttu-id="adf4f-138">**إضافة إلى الفترة المطلوبة** - تتم إضافة الوظيفة إلى الفترة المجدولة للتاريخ المطلوب.</span><span class="sxs-lookup"><span data-stu-id="adf4f-138">**Add to the requested period** - The job is added to the scheduled period of the required date.</span></span> <span data-ttu-id="adf4f-139">وتكون النتيجة هي زيادة تحميل خلية العمل خلال الفترة المجدولة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-139">The result is that the work cell is overloaded during the scheduled period.</span></span>

-   <span data-ttu-id="adf4f-140">**توزيع** -يتم توزيع بطاقات كانبان لحدث واحد على فترات الإنتاج المتاحة، بدءاً من أول فترة متاحة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-140">**Distribute** - The kanbans of a single event are distributed to the available production periods, starting with the first available period.</span></span>

### <a name="schedule-board-for-process-jobs"></a><span data-ttu-id="adf4f-141">لوحة جدولة لوظائف العملية</span><span class="sxs-lookup"><span data-stu-id="adf4f-141">Schedule board for process jobs</span></span>

<span data-ttu-id="adf4f-142">بعد تخطيط وظائف كانبان، يستخدم طابق المتجر لوحة جدولة كانبان لوظائف العملية لأداء وظائف كانبان المختلفة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-142">After the kanbans have been planned, the shop floor then uses the Kanban schedule board for process jobs for performing against the various kanban jobs.</span></span>

## <a name="withdrawal-kanban"></a><span data-ttu-id="adf4f-143">كانبان السحب</span><span class="sxs-lookup"><span data-stu-id="adf4f-143">Withdrawal kanban</span></span>

<span data-ttu-id="adf4f-144">يُنشئ كانبان من النوع **السحب** وظيفة نقل تستند إلى نشاط نقل.</span><span class="sxs-lookup"><span data-stu-id="adf4f-144">A kanban with the type **Withdrawal** creates a transfer job that is based on a transfer activity.</span></span> <span data-ttu-id="adf4f-145">تُستخدم بطاقات كانبان السحب لنقل كانبان لصنف معين بين محلات السوبر ماركت والمستودعات ومواقع الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="adf4f-145">Withdrawal kanbans are used to move a kanban of a specific item between supermarkets, warehouses, and production locations.</span></span> <span data-ttu-id="adf4f-146">لا تضيف بطاقات كانبان السحب قيمة ولا يتم التخطيط لها مثل بطاقات كانبان التصنيع.</span><span class="sxs-lookup"><span data-stu-id="adf4f-146">Withdrawal kanbans do not add value and are not planned as manufacturing kanbans are.</span></span>

### <a name="schedule-board-for-transfer-jobs"></a><span data-ttu-id="adf4f-147">لوحة جدولة لوظائف النقل</span><span class="sxs-lookup"><span data-stu-id="adf4f-147">Schedule board for transfer jobs</span></span>

<span data-ttu-id="adf4f-148">يتم تنفيذ بطاقات كانبان السحب في صالة المتجر باستخدام لوحة كانبان لوظائف النقل.</span><span class="sxs-lookup"><span data-stu-id="adf4f-148">Withdrawal kanbans are implemented on the shop floor by using the Kanban board for transfer jobs.</span></span> <span data-ttu-id="adf4f-149">توفر صفحة **لوحة كانبان لوظائف النقل** للعامل الرؤية التي يحتاجها لجمع المواد لتزويد محلات السوبر ماركت الجانبية ودعم انتقاء المواد من محلات السوبر ماركت.</span><span class="sxs-lookup"><span data-stu-id="adf4f-149">The **Kanban board for transfer jobs** page provides a worker with the visibility that he or she needs to gather materials to replenish line side supermarkets and to support the picking of materials from supermarkets.</span></span> <span data-ttu-id="adf4f-150">كما يتم دعم متطلبات التتبع المادي.</span><span class="sxs-lookup"><span data-stu-id="adf4f-150">Physical traceability requirements are also supported.</span></span> 


## <a name="fixed-quantity-kanban"></a><span data-ttu-id="adf4f-151">كانبان الكمية الثابتة</span><span class="sxs-lookup"><span data-stu-id="adf4f-151">Fixed quantity kanban</span></span>

<span data-ttu-id="adf4f-152">تتعلق قاعدة كانبان الكمية الثابتة بعدد ثابت من وحدات معالجة المواد؛ بمعنى أن أعداد بطاقات كانبان النشطة ثابتة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-152">A fixed quantity kanban rule relates to a fixed number of handling units; meaning, the numbers of active kanbans are constant.</span></span> <span data-ttu-id="adf4f-153">عندما يتم استهلاك منتجات كانبان وإفراغ وحدات معالجة المواد يدوياً، يتم إنشاء كانبان جديد من نفس النوع.</span><span class="sxs-lookup"><span data-stu-id="adf4f-153">Whenever the products of a kanban are consumed and handling units are manually emptied, a new kanban of the same type is created.</span></span>

<span data-ttu-id="adf4f-154">يجب حساب الكمية الثابتة، وهي عدد بطاقات كانبان في التدفق، بناءً على الطلب القديم والمستقبلي ومعامل الخدمة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-154">The Fixed quantity, which is the number of kanbans in the flow, should be calculated based on historical and future demand and service factor.</span></span>

<span data-ttu-id="adf4f-155">إذا كانت الكمية منخفضة جداً، فإنك تخاطر بنفاد المخزون لتلبية الطلب، وإذا كانت عالية جداً، فهناك خطر تكوين المخزون.</span><span class="sxs-lookup"><span data-stu-id="adf4f-155">If the quantity is too low, you risk running out of stock to meet demand, and if it is too high, then there is a risk for building up stock.</span></span>

<span data-ttu-id="adf4f-156">انتقل إلى **التحكم بالإنتاج > مهام دورية > حساب كمية كانبان > حساب كمية كانبان** لوظيفة عملية يمكن أن تساعدك على حساب كمية كانبان الثابتة.</span><span class="sxs-lookup"><span data-stu-id="adf4f-156">Go to **Production control > Periodic tasks > Kanban quantity calculation > Calculate kanban quantity** for a process job that can help you calculate the fixed kanban quantity.</span></span>

<span data-ttu-id="adf4f-157">تعتمد وظيفة عملية حساب كمية كانبان على نهج حساب كمية كانبان.</span><span class="sxs-lookup"><span data-stu-id="adf4f-157">The Calculate kanban quantity process job is based on the Kanban quantity calculation policy.</span></span> <span data-ttu-id="adf4f-158">يمكنك تعيين سياسات حساب كمية كانبان لكل قاعدة كانبان.</span><span class="sxs-lookup"><span data-stu-id="adf4f-158">You can assign the Kanban quantity calculation policies for each kanban rule.</span></span>

<span data-ttu-id="adf4f-159">**التحكم بالإنتاج > مهام دورية > حساب كمية كانبان > قواعد كانبان**</span><span class="sxs-lookup"><span data-stu-id="adf4f-159">**Production control > Periodic tasks > Kanban quantity calculation > Kanban rules**</span></span>

![لقطة شاشة لحقل سياسات حساب كمية كانبان.](../media/calculate-kanban-quantity-2.png)

<span data-ttu-id="adf4f-161">غالباً ما يتم استخدام كانبان الكمية الثابتة مع البطاقات المتداولة الثابتة ولكن يمكن استخدامها أيضاً مع بطاقات الاستخدام الواحد.</span><span class="sxs-lookup"><span data-stu-id="adf4f-161">Fixed quantity kanbans are often used with fixed circulating cards but can also be used with single use cards.</span></span> <span data-ttu-id="adf4f-162">يعتبر كانبان الكمية الثابتة أحد سيناريوهات التصنيع للتخزين.</span><span class="sxs-lookup"><span data-stu-id="adf4f-162">A fixed quantity kanban is a make-to-stock scenario.</span></span> 
