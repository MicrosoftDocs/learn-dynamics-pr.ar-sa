---
ms.openlocfilehash: d65adc4985781ae74d5b8dccf385bf9b02b1d6f1
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073395"
---
<span data-ttu-id="3dd55-101">قبل البدء، تحتاج إلى إعداد معلمات الإنتاج وأسماء دفتر اليومية في وحدة التحكم في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="3dd55-101">Before starting, you need to set up production parameters and journal names in the Production control module.</span></span>

- <span data-ttu-id="3dd55-102">**المعلمات**: إعداد معلمات الإنتاج الأساسية لتحديد كيفية قيام التطبيق بمعالجة أوامر الإنتاج ومعالجتها.</span><span class="sxs-lookup"><span data-stu-id="3dd55-102">**Parameters** - Set up basic production parameters to define how the application must handle and process production orders.</span></span> <span data-ttu-id="3dd55-103">حدد كيفية إنشائها وتقديرها وجدولتها واستهلاكها.</span><span class="sxs-lookup"><span data-stu-id="3dd55-103">Define how they are created, estimated, scheduled, and consumed.</span></span> <span data-ttu-id="3dd55-104">يمكنك أيضاً تحديد نوع الملاحظات التي تريدها وكيفية إجراء محاسبة التكاليف.</span><span class="sxs-lookup"><span data-stu-id="3dd55-104">You can also select what kind of feedback you want and how cost accounting must be conducted.</span></span>
- <span data-ttu-id="3dd55-105">**أسماء دفاتر اليومية**: تحديد أسماء دفاتر يومية الإنتاج التي ترغب في استخدامها لتسجيل الحركات المستمرة وترحيلها.</span><span class="sxs-lookup"><span data-stu-id="3dd55-105">**Journal names** - Identify the production journal names that you want to use to record and post ongoing transactions.</span></span>

<span data-ttu-id="3dd55-106">تسجل دفاتر يومية أمر الإنتاج حركات الأصناف المختلفة التي تحدث عند العمل بأوامر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="3dd55-106">Production order journals record the different item transactions that occur when you work with production orders.</span></span> <span data-ttu-id="3dd55-107">إن حركات الأصناف هذه لها تأثير مباشر في السجلات المالية للشركة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-107">These item transactions have a direct effect on a company's financial records.</span></span> 

<span data-ttu-id="3dd55-108">عندما تقوم بترحيل دفتر يومية إنتاج، يتم تحويل جميع حركات الأصناف تلقائياً إلى دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="3dd55-108">When you post a production journal, all item transactions are automatically transferred to the general ledger.</span></span> <span data-ttu-id="3dd55-109">وحدة دفتر الأستاذ العام هي الموقع المركزي للبيانات والمعلومات المالية في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="3dd55-109">The General ledger module is the centralized location for financial data and information in Supply Chain Management.</span></span>

<span data-ttu-id="3dd55-110">الأنواع الأربعة لدفاتر يومية الإنتاج في Supply Chain Management هي:</span><span class="sxs-lookup"><span data-stu-id="3dd55-110">The four types of production journals in Supply Chain Management are:</span></span>

- <span data-ttu-id="3dd55-111">قائمة الانتقاء - إصدار المواد الخام إلى WIP.</span><span class="sxs-lookup"><span data-stu-id="3dd55-111">Picking list – Issue raw materials to the WIP.</span></span>
- <span data-ttu-id="3dd55-112">بطاقة المسار - الإبلاغ عن العمالة كإجماليات.</span><span class="sxs-lookup"><span data-stu-id="3dd55-112">Route card – Report labor as totals.</span></span>
- <span data-ttu-id="3dd55-113">بطاقة الوظيفة - الإبلاغ عن العمالة كتفاصيل حول أوقات البدء والتوقف.</span><span class="sxs-lookup"><span data-stu-id="3dd55-113">Job card – Report labor as details with start and stop times.</span></span>
- <span data-ttu-id="3dd55-114">الإبلاغ كمنتهٍ - استلام السلع المنتهية في المخزون والإبلاغ عن الكميات الجيدة والسيئة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-114">Report as finished – Receive finished goods into inventory and report good and bad quantities.</span></span>

<span data-ttu-id="3dd55-115">تتضمن العديد من مكونات رؤوس دفاتر اليومية التي يمكنك وضعها في الاعتبار ما يلي:</span><span class="sxs-lookup"><span data-stu-id="3dd55-115">Several components of journal headers that you can consider include:</span></span>

- <span data-ttu-id="3dd55-116">دفتر اليومية (الرأس):</span><span class="sxs-lookup"><span data-stu-id="3dd55-116">Journal (header):</span></span>
    - <span data-ttu-id="3dd55-117">النوع - التحكم في نوع دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="3dd55-117">Type – Controls the type of journal.</span></span>
    - <span data-ttu-id="3dd55-118">الاسم – التحكم في الإيصال والرقم والسلوك.</span><span class="sxs-lookup"><span data-stu-id="3dd55-118">Name – Controls the voucher, number, and behavior.</span></span>
- <span data-ttu-id="3dd55-119">الرقم – توفير معرف فريد.</span><span class="sxs-lookup"><span data-stu-id="3dd55-119">Number – Provides a unique identifier.</span></span>

<span data-ttu-id="3dd55-120">تشتمل بنود دفتر اليومية على ميزات مميزة مختلفة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-120">Journal lines have different distinct features.</span></span> <span data-ttu-id="3dd55-121">يمكن أن تختلف حسب نوع دفتر اليومية، ويمكن استخدامها لتسجيل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="3dd55-121">They can differ by journal type, and can be used to record the following:</span></span>
- <span data-ttu-id="3dd55-122">المواد والكميات</span><span class="sxs-lookup"><span data-stu-id="3dd55-122">Materials and quantities</span></span>
- <span data-ttu-id="3dd55-123">العمليات والوقت المستغرق</span><span class="sxs-lookup"><span data-stu-id="3dd55-123">Operations and time spent</span></span>
- <span data-ttu-id="3dd55-124">الكميات الجيدة والسيئة</span><span class="sxs-lookup"><span data-stu-id="3dd55-124">Good and bad quantities</span></span>

<span data-ttu-id="3dd55-125">بالإضافة إلى إعداد معلمات التحكم في الإنتاج على مستوى الشركة، يمكنك تكوين معلمات التحكم في الإنتاج بشكل فريد حسب الموقع.</span><span class="sxs-lookup"><span data-stu-id="3dd55-125">In addition to setting up the production control parameters at the company level, you can configure the production control parameters uniquely by site.</span></span> <span data-ttu-id="3dd55-126">إذا لم يكن الموقع يحتوي على معلمات معينة له على وجه التحديد، تستخدم Supply Chain Management المعلمات التي تم تكوينها من قِبل الشركة لهذا الموقع.</span><span class="sxs-lookup"><span data-stu-id="3dd55-126">If a site does not specifically have parameters assigned to it, Supply Chain Management uses the company configured parameters for that site.</span></span>

## <a name="allocation-keys"></a><span data-ttu-id="3dd55-127">مفاتيح التوزيع</span><span class="sxs-lookup"><span data-stu-id="3dd55-127">Allocation keys</span></span> 

<span data-ttu-id="3dd55-128">إذا بدأ موظف أكثر من وظيفة واحدة في صفحة **تسجيل الوظائف**، فإنه يُشار إليها باسم مجموعة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-128">If an employee starts more than one job on the **Job registration** page, it is referred to as a bundle.</span></span> 

<span data-ttu-id="3dd55-129">تُستخدم مفاتيح التوزيع لتحديد كيف وأي الوظائف المجمعة أو التسجيلات المجمعة تعمل في منطقة معينة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-129">Allocation keys are used to define how, and which, bundled jobs or bundled registrations work within a specific area.</span></span> <span data-ttu-id="3dd55-130">يمكن توزيع الوقت المستغرق في الوظائف المجمعة للوظائف الفردية بطرق مختلفة باستخدام مفاتيح التوزيع هذه.</span><span class="sxs-lookup"><span data-stu-id="3dd55-130">The time spent on bundled jobs can be allocated to the individual jobs in different ways by using those allocation keys.</span></span>

<span data-ttu-id="3dd55-131">تتكون مفاتيح التوزيع من المكونات التالية:</span><span class="sxs-lookup"><span data-stu-id="3dd55-131">Allocation keys consist of the following components:</span></span>

- <span data-ttu-id="3dd55-132">المواقع</span><span class="sxs-lookup"><span data-stu-id="3dd55-132">Sites</span></span>
- <span data-ttu-id="3dd55-133">وحدات الإنتاج</span><span class="sxs-lookup"><span data-stu-id="3dd55-133">Production units</span></span>
- <span data-ttu-id="3dd55-134">الموارد</span><span class="sxs-lookup"><span data-stu-id="3dd55-134">Resources</span></span>
- <span data-ttu-id="3dd55-135">أنواع الموارد</span><span class="sxs-lookup"><span data-stu-id="3dd55-135">Resource types</span></span>
- <span data-ttu-id="3dd55-136">نوع المجموعة</span><span class="sxs-lookup"><span data-stu-id="3dd55-136">Bundle type</span></span>


<span data-ttu-id="3dd55-137">إذا قمت بتجميع الوظائف، فأنت بحاجة إلى توضيح وتحديد كيفية توزيع إجمالي الوقت المسجل لجميع الوظائف لكل وظيفة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-137">If you bundle jobs, you need to define and determine how the total registered time for all jobs should be allocated for each job.</span></span> <span data-ttu-id="3dd55-138">يمكنك تحديد التوزيع عن طريق تحديد أحد الخيارات التالية في الحقل **نوع المجموعة** في الصفحة **مفاتيح التوزيع**:</span><span class="sxs-lookup"><span data-stu-id="3dd55-138">You can define the allocation by selecting one of the following options in the **Bundle type** field on the **Allocation keys** page:</span></span> 

- <span data-ttu-id="3dd55-139">**التقدير** – يتم تقسيم الوقت بين الوظائف بناءً على الوقت المقدر للوظائف.</span><span class="sxs-lookup"><span data-stu-id="3dd55-139">**Estimation** – Time is divided between the jobs based on the estimated time for the jobs.</span></span> 
- <span data-ttu-id="3dd55-140">**الوظائف** – يتم تقسيم الوقت وفقاً لإجمالي الوظائف المجمعة ومقدار الوقت المستغرق في إنهاء جميع الوظائف.</span><span class="sxs-lookup"><span data-stu-id="3dd55-140">**Jobs** – Time is divided according to total jobs that are bundled and how much time was spent finishing all the jobs.</span></span> 
- <span data-ttu-id="3dd55-141">**الوقت الصافي** – يتم تقسيم الوقت بالتساوي بين الوظائف الموجودة في المجموعة في أي وقت.</span><span class="sxs-lookup"><span data-stu-id="3dd55-141">**Net time** – Time is divided equally between the jobs that are in the bundle at any time.</span></span> 
- <span data-ttu-id="3dd55-142">**الوقت الحقيقي** – يتم توزيع وقت الوظيفة الفعلي.</span><span class="sxs-lookup"><span data-stu-id="3dd55-142">**Real time** – Actual job time is allocated.</span></span> <span data-ttu-id="3dd55-143">يمكن حساب التكلفة على أساس تكلفة الرواتب الفعلية.</span><span class="sxs-lookup"><span data-stu-id="3dd55-143">The cost can be calculated based on the actual payroll cost.</span></span>

## <a name="production-pools"></a><span data-ttu-id="3dd55-144">مجموعات الإنتاج</span><span class="sxs-lookup"><span data-stu-id="3dd55-144">Production pools</span></span> 

<span data-ttu-id="3dd55-145">تجمع أوعية الإنتاج أوامر الإنتاج في فئات ذات خصائص مشتركة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-145">Production pools group production orders into categories with shared characteristics.</span></span> <span data-ttu-id="3dd55-146">يمكن تعيين أمر إنتاج لوعاء إنتاج.</span><span class="sxs-lookup"><span data-stu-id="3dd55-146">A production order can be assigned to a production pool.</span></span> <span data-ttu-id="3dd55-147">عند إنشاء أمر إنتاج، يمكنك تعيينه لوعاء إنتاج محدد.</span><span class="sxs-lookup"><span data-stu-id="3dd55-147">When you create a production order, you can assign it to a specific production pool.</span></span> <span data-ttu-id="3dd55-148">يمكنك أيضاً تعيين وعاء إنتاج لمنتج مُصدر وبما أن جميع المنتجات مطلوبة للحصول على ملف تعريف الترحيل الخاص بها بواسطة مجموعة الصنف، فسوف تقوم بترحيل الحركات إلى أوامر الوعاء.</span><span class="sxs-lookup"><span data-stu-id="3dd55-148">You can also assign a production pool to a Released product and since all products are required to have their posting profile by the item group, it will post transactions to the orders for the pool.</span></span>

<span data-ttu-id="3dd55-149">فيما يلي أمثلة على السيناريوهات حيث يمكن استخدام أوعية الإنتاج لتجميع:</span><span class="sxs-lookup"><span data-stu-id="3dd55-149">The following are example scenarios where production pools can be used to group:</span></span>
- <span data-ttu-id="3dd55-150">الأوامر الجاهزة لإنتاجها</span><span class="sxs-lookup"><span data-stu-id="3dd55-150">Orders that are ready to be produced</span></span>
- <span data-ttu-id="3dd55-151">الأوامر المتعاقد عليها من الباطن التي لم يتم تسليمها</span><span class="sxs-lookup"><span data-stu-id="3dd55-151">Subcontracted orders that are missing deliveries</span></span>
- <span data-ttu-id="3dd55-152">عمليات الإنتاج العادية</span><span class="sxs-lookup"><span data-stu-id="3dd55-152">Regular productions</span></span>
- <span data-ttu-id="3dd55-153">الأوامر المفتقدة إلى المواد</span><span class="sxs-lookup"><span data-stu-id="3dd55-153">Orders that are missing materials</span></span>
- <span data-ttu-id="3dd55-154">الأوامر التي تأخرت بسبب عطل في الجهاز</span><span class="sxs-lookup"><span data-stu-id="3dd55-154">Orders that are delayed because of machine failure</span></span>
- <span data-ttu-id="3dd55-155">الأوامر الجاهزة للإصدار أو البدء أو الجدولة</span><span class="sxs-lookup"><span data-stu-id="3dd55-155">Orders that are ready for release, start, or scheduling</span></span>

### <a name="example-1"></a><span data-ttu-id="3dd55-156">المثال 1</span><span class="sxs-lookup"><span data-stu-id="3dd55-156">Example 1</span></span> 

<span data-ttu-id="3dd55-157">يمكنك تجميع أوامر التعاقد من الباطن التي تفتقد لعمليات التسليم أو عمليات الإنتاج أو الأوامر التي تفتقد للمواد أو الأوامر التي تأخرت بسبب نوع من تعطل الجهاز أو الأوامر الجاهزة للإصدار أو البدء أو الجدولة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-157">You can group subcontracted orders that are missing deliveries, production runs, orders that are missing materials, orders that are delayed because of some kind of machine failure, or orders that are ready for release, start, or for scheduling.</span></span>  

### <a name="example-2"></a><span data-ttu-id="3dd55-158">المثال 2</span><span class="sxs-lookup"><span data-stu-id="3dd55-158">Example 2</span></span> 

<span data-ttu-id="3dd55-159">يمكنك إنشاء أوعية إنتاج للأوامر ذات الأولوية القصوى أو التي لها حالة إنتاج واحدة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-159">You can create production pools for orders that are top priority or that have one production status.</span></span> <span data-ttu-id="3dd55-160">يمكنك أيضاً تعيين وعاء إنتاج لمنتج مُصدر لتحديد الطريقة المستخدمة لترحيل الحركات للأوامر الموجودة في الوعاء.</span><span class="sxs-lookup"><span data-stu-id="3dd55-160">You can also assign a production pool to a Released product to define the method that is used to post transactions for the orders in the pool.</span></span>

### <a name="example-3"></a><span data-ttu-id="3dd55-161">المثال 3</span><span class="sxs-lookup"><span data-stu-id="3dd55-161">Example 3</span></span> 
<span data-ttu-id="3dd55-162">يمكن استخدام وعاء الإنتاج إذا كنت تريد تعيين أشخاص يتمتعون بمهارات خاصة لإجراء عملية أمر إنتاج، مثل أولئك الذين يمكنهم إنجاز المهمة في المواقف الصعبة.</span><span class="sxs-lookup"><span data-stu-id="3dd55-162">A production pool can be used if you want to assign people who are specifically skilled for an operation of a production order, such as those who can get the job done in difficult situations.</span></span>

