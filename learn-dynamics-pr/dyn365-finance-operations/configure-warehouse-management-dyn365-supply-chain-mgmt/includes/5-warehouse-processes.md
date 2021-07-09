---
ms.openlocfilehash: b8081887c4397b05ca1194426862ae8932f82ec6
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073780"
---
<span data-ttu-id="b76da-101">كجزء من تكوين المستودع، عليك تمكين عمليات المستودع وفقاً لمتطلبات العمل التجاري.</span><span class="sxs-lookup"><span data-stu-id="b76da-101">As part of the warehouse configuration, you must enable warehouse processes according to business requirements.</span></span> <span data-ttu-id="b76da-102">أحد أهم المكونات التي يتعين عليك تكوينها هو قوالب الموجة وقوالب العمل وأوعية العمل وتوجيهات الموقع.</span><span class="sxs-lookup"><span data-stu-id="b76da-102">The most important components for you to configure are wave templates, work templates, work pools, and location directives.</span></span> 

## <a name="wave-templates"></a><span data-ttu-id="b76da-103">قوالب الموجات</span><span class="sxs-lookup"><span data-stu-id="b76da-103">Wave templates</span></span> 

<span data-ttu-id="b76da-104">قوالب الموجة، المتوفرة في **إدارة المستودعات > الإعداد > الموجات**، تساعد في تمكين عملية الإصدار إلى المستودع الصادرة.</span><span class="sxs-lookup"><span data-stu-id="b76da-104">Wave templates, found in **Warehouse management > Setup > Waves**, help enable the outbound release-to-warehouse process.</span></span> <span data-ttu-id="b76da-105">عند إصدار بنود الأمر (إما مباشرةً من المستندات المصدر، أو من خلال عمليات الوظيفة الدُفعية، أو بالأحمال التي سبق أن تم إنشاؤها)، يتم استخدام وظيفة قوالب الموجة.</span><span class="sxs-lookup"><span data-stu-id="b76da-105">When order lines are released (either directly from source documents, through batch job processes, or by loads that have already been created), the wave template functionality is used.</span></span>

<span data-ttu-id="b76da-106">يمكنك إنشاء ثلاثة أنواع من قوالب الموجة:</span><span class="sxs-lookup"><span data-stu-id="b76da-106">You can create three types of wave templates:</span></span>

-   <span data-ttu-id="b76da-107">الشحن</span><span class="sxs-lookup"><span data-stu-id="b76da-107">Shipping</span></span>
-   <span data-ttu-id="b76da-108">أمر الإنتاج</span><span class="sxs-lookup"><span data-stu-id="b76da-108">Production order</span></span>
-   <span data-ttu-id="b76da-109">كانبان</span><span class="sxs-lookup"><span data-stu-id="b76da-109">Kanban</span></span>

<span data-ttu-id="b76da-110">يمكنك استخدام المعلمات لتعريف مدى تشغيل النظام تلقائياً في معالجة العمل الصادر.</span><span class="sxs-lookup"><span data-stu-id="b76da-110">You can use parameters to define how far the system should automatically go in the outbound work processing.</span></span>

<span data-ttu-id="b76da-111">يتم تحديد قالب الموجة استناداً إلى تسلسل قوالب الموجة والمعايير المحددة في القالب.</span><span class="sxs-lookup"><span data-stu-id="b76da-111">A wave template is selected based on the wave template sequence and criteria that are specified in the template.</span></span> <span data-ttu-id="b76da-112">إذا كان القالب مدرجاً في أعلى التسلسل، يتم فحص المعايير في هذا القالب أولاً.</span><span class="sxs-lookup"><span data-stu-id="b76da-112">If a template is listed at the top of the sequence, the criteria in that template are checked first.</span></span> <span data-ttu-id="b76da-113">إذا كان من الممكن استيفاء المعايير، تتم معالجة قالب الموجة.</span><span class="sxs-lookup"><span data-stu-id="b76da-113">If the criteria can be met, the wave template is processed.</span></span>
<span data-ttu-id="b76da-114">بخلاف ذلك، يتم فحص المعايير في القالب التالي، وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="b76da-114">Otherwise, the criteria in the next template are checked, and so on.</span></span>

<span data-ttu-id="b76da-115">وبالتالي، من المفيد وضع القالب الذي يتضمن المعايير الأكثر تحديداً في أعلى قائمة تسلسل قوالب الموجة بحيث تتم معالجته أولاً.</span><span class="sxs-lookup"><span data-stu-id="b76da-115">Therefore, it's a good idea to put the template that has the most specific criteria at the top of the wave template sequence list so that it's processed first.</span></span>

<span data-ttu-id="b76da-116">على سبيل المثال، أنت ترغب في معالجة كل العمل لشركة نقل مفضّلة اليوم وتأجيل معالجة العمل لشركات النقل الأخرى مؤقتاً.</span><span class="sxs-lookup"><span data-stu-id="b76da-116">For example, you want to process all the work for a preferred carrier today and temporarily delay processing of the work for other carriers.</span></span>
<span data-ttu-id="b76da-117">في هذه الحالة، يجب أن يكون قالب الموجة الذي يحدد العمل لشركة النقل المفضّلة هذه مدرجاً في ترتيب أعلى في التسلسل مقارنةً بالقوالب الأخرى.</span><span class="sxs-lookup"><span data-stu-id="b76da-117">In this case, the wave template that selects work for that preferred carrier should be listed higher in the sequence than other templates.</span></span>
<span data-ttu-id="b76da-118">بخلاف ذلك، قد تتم معالجة العمل لشركات النقل الأخرى قبل إكمال عمل شركة النقل المفضّلة.</span><span class="sxs-lookup"><span data-stu-id="b76da-118">Otherwise, the work for other carriers might be processed before the work for the preferred carrier is completed.</span></span>

<span data-ttu-id="b76da-119">يجب تحديد طرق معالجة الموجة في كل قالب موجة.</span><span class="sxs-lookup"><span data-stu-id="b76da-119">You must specify the wave process methods in each wave template.</span></span> <span data-ttu-id="b76da-120">تختلف الطرق المتوفرة، اعتماداً على نوع قالب الموجة.</span><span class="sxs-lookup"><span data-stu-id="b76da-120">The methods that are available vary, depending on the wave template type.</span></span>

## <a name="work-templates"></a><span data-ttu-id="b76da-121">قوالب العمل</span><span class="sxs-lookup"><span data-stu-id="b76da-121">Work templates</span></span> 

<span data-ttu-id="b76da-122">تُعرّف قوالب العمل المتوفرة في **إدارة المستودعات > الإعداد > العمل** العمل الذي يتم إجراؤه وكيفية إجرائه.</span><span class="sxs-lookup"><span data-stu-id="b76da-122">Work templates, found in **Warehouse management > Setup > Work** define what work is performed and how the work is done.</span></span>
<span data-ttu-id="b76da-123">يمكن أن تحتوي قوالب العمل أيضاً على كود توجيه يرتبط بتوجيه موقع لتحديد مكان إجراء العمل.</span><span class="sxs-lookup"><span data-stu-id="b76da-123">Work templates can also contain a directive code that links to a location directive to determine where work is performed.</span></span>

<span data-ttu-id="b76da-124">تشتمل قوالب العمل على استعلام يحدد معايير العمل.</span><span class="sxs-lookup"><span data-stu-id="b76da-124">Work templates include a query that specifies the criteria for the work.</span></span>
<span data-ttu-id="b76da-125">يجب أن يشمل كل قالب عملية انتقاء واحدة على الأقل وعملية وضع واحدة على الأقل لدفع عملية العمل الأساسية لنقل المخزون المتاح من موقع إلى آخر.</span><span class="sxs-lookup"><span data-stu-id="b76da-125">Each template must include at least one Pick operation and one Put operation to drive the basic work operation of transferring on-hand inventory from one location to another.</span></span>

<span data-ttu-id="b76da-126">إذا كان على عاملين متعددين أن يتمكنوا من معالجة العمل لبعض عمليات المستودعات لديك، قد ترغب في استخدام مفهوم *التشغيل المرحلي* للمخزون وفصل تنفيذ العمل إلى درجات عمل مختلفة.</span><span class="sxs-lookup"><span data-stu-id="b76da-126">If multiple workers must be able to process work for some of your warehouse operations, you might want to use the concept of *staging* for the inventory and separate the work implementation into different work classes.</span></span>

<span data-ttu-id="b76da-127">يُستخدم قالب العمل لإنشاء عمل المستودع ومعالجته في مراحل مختلفة من عملية إدارة المستودعات.</span><span class="sxs-lookup"><span data-stu-id="b76da-127">Work template is used to create and process warehouse work at various stages in the warehouse management process.</span></span> <span data-ttu-id="b76da-128">يجب تحديد قالب عمل صالح مثل الانتقاء - وضع في أزواج.</span><span class="sxs-lookup"><span data-stu-id="b76da-128">A valid work template should be specified as pick - put in pairs.</span></span>

<span data-ttu-id="b76da-129">[![لقطة شاشة لصفحة قوالب العمل في Finance and Operations.](../media/work-templates.png)](../media/work-templates.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b76da-129">[![Screenshot of the Finance and Operations Work templates page.](../media/work-templates.png)](../media/work-templates.png#lightbox)</span></span>

<span data-ttu-id="b76da-130">**‏‫تجميع قوالب الموجة** يمكن أيضاً استخدامه في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="b76da-130">**Wave template grouping** can also be used in Supply Chain Management.</span></span> <span data-ttu-id="b76da-131">فهو يتيح التجميع والتقسيم حسب الوظيفة المتاحة بالفعل في قالب الموجة.</span><span class="sxs-lookup"><span data-stu-id="b76da-131">It enables grouping and breaking by functionality already on the wave template.</span></span> <span data-ttu-id="b76da-132">يمكن أن يكون استخدام هذه الوظيفة مفيداً في المستودع حيث يتم إنشاء الموجات استناداً إلى معايير محددة لكن إنشاء الموجات تلقائياً مفضّل على الإنشاء اليدوي.</span><span class="sxs-lookup"><span data-stu-id="b76da-132">Using this functionality can be useful in a warehouse where waves are created based on specific criteria but where automatic wave creation is preferred over manual.</span></span>



### <a name="scenario"></a><span data-ttu-id="b76da-133">السيناريو</span><span class="sxs-lookup"><span data-stu-id="b76da-133">Scenario</span></span> 

<span data-ttu-id="b76da-134">يتم إنشاء أمر شراء وتأكيده وإرساله إلى المورّد.</span><span class="sxs-lookup"><span data-stu-id="b76da-134">A purchase order is created, confirmed, and sent to a vendor.</span></span> <span data-ttu-id="b76da-135">يشحن المورّد الأصناف، التي سيتم تسلمها في موقع الوارد الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="b76da-135">The vendor ships the items, which will be received in your inbound location.</span></span>

<span data-ttu-id="b76da-136">بعد ذلك، عليك انتقاء أصناف المخزون وتخزينها بعيداً في موقع معيّن يمكن أن يمثل موقع انتقاء لأمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="b76da-136">Then, you need to pick the inventory items and put them away in a specific location that might be a picking location for a sales order.</span></span>

<span data-ttu-id="b76da-137">عند إنشاء أمر المبيعات، يتم انتقاء أصناف المخزون وتخزينها في موقع للتشغيل المرحلي لتتم تعبئتها.</span><span class="sxs-lookup"><span data-stu-id="b76da-137">When the sales order is created, you pick the inventory items and put them away in a staging location to be packed.</span></span>

<span data-ttu-id="b76da-138">أخيراً، ستنتقي الأصناف المعبأة وتخزنها في موقع للصادر ليتم شحنها.</span><span class="sxs-lookup"><span data-stu-id="b76da-138">Finally, you will pick the packed items and put them away on an outbound location to be shipped.</span></span>

## <a name="work-pools"></a><span data-ttu-id="b76da-139">أوعية العمل</span><span class="sxs-lookup"><span data-stu-id="b76da-139">Work pools</span></span> 

<span data-ttu-id="b76da-140">أوعية العمل، التي توجد أيضاً في **إدارة المستودعات > الإعداد > العمل** تُستخدم لتنظيم عمل المستودع في مجموعات.</span><span class="sxs-lookup"><span data-stu-id="b76da-140">Work pools, also found in **Warehouse management > Setup > Work** are used to organize warehouse work into groups.</span></span>

<span data-ttu-id="b76da-141">على سبيل المثال، يمكنك إنشاء وعاء عمل لتصنيف العمل الذي يحدث في موقع مستودع معيّن.</span><span class="sxs-lookup"><span data-stu-id="b76da-141">For example, you can create a work pool to classify work that occurs in a specific warehouse location.</span></span>

<span data-ttu-id="b76da-142">بالنسبة إلى جميع أنواع العمل، باستثناء الجرد، يمكنك تعيين وعاء عمل إلى قالب عمل.</span><span class="sxs-lookup"><span data-stu-id="b76da-142">For all work types except counting, you can assign a work pool to a work template.</span></span>

<span data-ttu-id="b76da-143">بالنسبة إلى الجرد الدوري، يمكنك تعيين وعاء عمل في الصفحات التالية:</span><span class="sxs-lookup"><span data-stu-id="b76da-143">For cycle counting, you can assign a work pool on the following pages:</span></span>

-   <span data-ttu-id="b76da-144">خطط الجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="b76da-144">Cycle count plans</span></span>
-   <span data-ttu-id="b76da-145">حدود الجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="b76da-145">Cycle count thresholds</span></span>
-   <span data-ttu-id="b76da-146">عمل الجرد الدوري حسب الموقع</span><span class="sxs-lookup"><span data-stu-id="b76da-146">Cycle count work by location</span></span>
-   <span data-ttu-id="b76da-147">عمل الجرد الدوري حسب الصنف</span><span class="sxs-lookup"><span data-stu-id="b76da-147">Cycle count work by item</span></span>

<span data-ttu-id="b76da-148">عند استخدام قوالب العمل لإنشاء العمل، يتم تعيين وعاء العمل تلقائياً للعمل.</span><span class="sxs-lookup"><span data-stu-id="b76da-148">When you use work templates to create work, the work pool is automatically assigned to the work.</span></span>

<span data-ttu-id="b76da-149">يمكن أيضاً استخدام معرّفات وعاء العمل للحد من نوع العمل الذي يتم توجيهه إلى عامل في المستودع، بشرط أن تكون هذه الوظيفة مكونة على صنف قائمة الجهاز المحمول ذي الصلة.</span><span class="sxs-lookup"><span data-stu-id="b76da-149">Work pool IDs can also be used to limit the type of work that is directed to a warehouse worker, provided that this functionality is configured on the relevant mobile device menu item.</span></span>

<span data-ttu-id="b76da-150">بالإضافة إلى ذلك، يتمتع مديرو المستودعات الآن بالقدرة على تغيير أوعية العمل التي تم إنشاؤها للعاملين، وهذا ما يسمح للمديرين بالتفاعل بشكل أسرع مع التغييرات في صالة الإنتاج، ما يتيح لهم تبسيط العملية الفعلية إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="b76da-150">Additionally, warehouse managers now have the ability to Change work pools that have been created for workers, this allows managers to react quicker to changes on the shop floor enabling them to streamline the physical process when needed.</span></span> 

## <a name="location-directives"></a><span data-ttu-id="b76da-151">توجيهات الموقع</span><span class="sxs-lookup"><span data-stu-id="b76da-151">Location directives</span></span> 

<span data-ttu-id="b76da-152">يتم استخدام توجيهات الموقع لتوجيه حركات العمل إلى المواقع الملائمة في المستودع.</span><span class="sxs-lookup"><span data-stu-id="b76da-152">Location directives are used to direct the work transactions to the appropriate locations in the warehouse.</span></span> <span data-ttu-id="b76da-153">بمعنى آخر، فهي تُعرّف مكان الانتقاء والوضع.</span><span class="sxs-lookup"><span data-stu-id="b76da-153">In other words, they define where to pick and put.</span></span>

<span data-ttu-id="b76da-154">لتبسيط تعريف الإجراءات المقترنة بكل بند لتوجيه الموقع، استخدم أحد الاستراتيجيات المعرّفة مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="b76da-154">To simplify defining the actions that are associated with each location directive line, use one of the predefined strategies.</span></span>

<span data-ttu-id="b76da-155">على سبيل المثال، يمكنك استخدام استراتيجية *موقع فارغ بدون عمل وارد* للبحث عن المواقع الخالية في أي مستودع، أو يمكنك استخدام استراتيجية *حجز دفعة ما تنتهي صلاحيته أولاً يُصرف أولاً* لانتقاء المبيعات الصادرة.</span><span class="sxs-lookup"><span data-stu-id="b76da-155">For example, you can use the *Empty location with no incoming work* strategy to search for free locations in a warehouse, or you can use the *FEFO batch reservation* strategy for outbound sales picking.</span></span>

<span data-ttu-id="b76da-156">على سبيل المثال، في حركة أمر مبيعات، تحدد توجيهات الموقع مكان انتقاء الأصناف ومكان وضع الأصناف التي تم انتقاؤها.</span><span class="sxs-lookup"><span data-stu-id="b76da-156">For example, in a sales order transaction, a location directive determines where the items will be picked and where the picked items will be put.</span></span>

 <span data-ttu-id="b76da-157">يمكنك استخدام توجيهات الموقع لتنفيذ ما يلي:</span><span class="sxs-lookup"><span data-stu-id="b76da-157">You can use location directives to do the following:</span></span>

-   <span data-ttu-id="b76da-158">تخزين الأصناف الواردة.</span><span class="sxs-lookup"><span data-stu-id="b76da-158">Put away incoming items.</span></span>
-   <span data-ttu-id="b76da-159">انتقاء الأصناف وتشغيلها مرحلياً للحركات الصادرة.</span><span class="sxs-lookup"><span data-stu-id="b76da-159">Pick and stage items for outbound transactions.</span></span>
-   <span data-ttu-id="b76da-160">انتقاء المواد الخام ووضعها للإنتاج.</span><span class="sxs-lookup"><span data-stu-id="b76da-160">Pick and put raw materials for production.</span></span>
-   <span data-ttu-id="b76da-161">تزويد المواقع.</span><span class="sxs-lookup"><span data-stu-id="b76da-161">Replenish locations.</span></span>

<span data-ttu-id="b76da-162">يمكنك استخدام صفحة **استخدام موقع ثابت** لتعيين موقع دائم أو ثابت لصنف من المخزون.</span><span class="sxs-lookup"><span data-stu-id="b76da-162">You can use the **Fixed location usage** page to assign a permanent or fixed location to an inventory item.</span></span> <span data-ttu-id="b76da-163">يمكنك تعيين مواقع متعددة ثابتة للصنف نفسه ويمكن تعيين الموقع الثابت نفسه لأصناف متعددة.</span><span class="sxs-lookup"><span data-stu-id="b76da-163">You can assign multiple fixed locations to the same item, and multiple items can have the same fixed location assigned to them.</span></span> <span data-ttu-id="b76da-164">يتم استخدام المواقع الثابتة لإعداد توجيهات الموقع وتزويد المخزون.</span><span class="sxs-lookup"><span data-stu-id="b76da-164">Fixed locations are used to set up location directives and inventory replenishment.</span></span>

<span data-ttu-id="b76da-165">[![لقطة شاشة لصفحة استخدام الموقع الثابت.](../media/fixed-locations.png)](../media/fixed-locations.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b76da-165">[![Screenshot of the Fixed location usage page.](../media/fixed-locations.png)](../media/fixed-locations.png#lightbox)</span></span>

<span data-ttu-id="b76da-166">تتضمن توجيهات الموقع ميزات متعددة تساعد في تحديد مواقع الانتقاء والوضع لحركة المخزون:</span><span class="sxs-lookup"><span data-stu-id="b76da-166">Location directives have several features that help with identifying pick and put locations for inventory movement:</span></span>

-   <span data-ttu-id="b76da-167">**محددة للمستودع** - إذا كان لديك مستودعات متعددة تم إعدادها بشكل مماثل، يمكنك استخدام ميزة النسخ.</span><span class="sxs-lookup"><span data-stu-id="b76da-167">**They are warehouse-specific** - If you have multiple warehouses that are set up similarly, you can use the copy feature.</span></span> <span data-ttu-id="b76da-168">مع ذلك، لا يزال عليك إعداد توجيهات الموقع لكل واحد.</span><span class="sxs-lookup"><span data-stu-id="b76da-168">However, you still need to have location directives set up for each one.</span></span>
-   <span data-ttu-id="b76da-169">**هناك 16 نوعاً مختلفاً من أوامر العمل يمكنك إعداد توجيه موقع لها** - بعضها أنواع قياسية، مثل أوامر الشراء وأوامر المبيعات وإصدار النقل واستلام النقل.</span><span class="sxs-lookup"><span data-stu-id="b76da-169">**There are 16 different types of work orders for which you can set up a location directive** - Some of these are standard types, such as purchase orders, sales orders, transfer issue, and transfer receipt.</span></span> <span data-ttu-id="b76da-170">توجد أنواع أخرى من أوامر العمل كذلك.</span><span class="sxs-lookup"><span data-stu-id="b76da-170">Other types of work orders exist as well.</span></span>
    <span data-ttu-id="b76da-171">على سبيل المثال، إذا كنت تمثل شركة تصنيع، هناك أوامر عمل للبضائع المنتهية التي تم تخزينها وانتقاء المواد الخام وانتقاء كانبان.</span><span class="sxs-lookup"><span data-stu-id="b76da-171">For example, if you are a manufacturing company, there are work orders for finished goods that are put away, raw material picking, and Kanban picking.</span></span> <span data-ttu-id="b76da-172">تشمل أوامر العمل الأخرى أنواعاً متعددة من الجرد الدوري وأوامر الإرجاع والتزويد.</span><span class="sxs-lookup"><span data-stu-id="b76da-172">Other work orders include several types for cycle counting, return orders, and replenishment.</span></span>

<span data-ttu-id="b76da-173">إليك ثلاث علامات تبويب سريعة تتضمن تفاصيل حول توجيه الموقع:</span><span class="sxs-lookup"><span data-stu-id="b76da-173">Three FastTabs that include details about a location directive are:</span></span>

-   <span data-ttu-id="b76da-174">**توجيهات الموقع** - تحدد الموقع والمستودع.</span><span class="sxs-lookup"><span data-stu-id="b76da-174">**Location directives** - Specifies the site and warehouse.</span></span>
-   <span data-ttu-id="b76da-175">**البنود** - يمكنها فصل التوجيهات استناداً إلى معايير مختلفة.</span><span class="sxs-lookup"><span data-stu-id="b76da-175">**Lines** - Can separate directives based on different criteria.</span></span> <span data-ttu-id="b76da-176">على سبيل المثال، يمكنها فصل التوجيهات استناداً إلى كميات الحركة.</span><span class="sxs-lookup"><span data-stu-id="b76da-176">For example, it could separate directives based on the quantities of the transaction.</span></span> <span data-ttu-id="b76da-177">من الأمثلة، يمكن أن تستخدم توجيهاً واحداً في حالة تلقي أمر شراء يضم 1000 صنف أو أقل وآخر إذا كانت الكمية أكبر من 1000.</span><span class="sxs-lookup"><span data-stu-id="b76da-177">As another example, you can have one directive if the purchase order being received is 1,000 items or less, and another for an amount greater than 1,000.</span></span>
-   <span data-ttu-id="b76da-178">**إجراءات توجيه الموقع** - حيث يمكنك تحديد كيف يتم إجراء حركات لأصناف أو مواقع معيّنة بقدر أكبر من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="b76da-178">**Location directive actions** - Where you can specify how certain items or locations are being transacted in much greater detail.</span></span> <span data-ttu-id="b76da-179">على سبيل المثال، في حالة استلام أصناف تحتاج إلى وضعها في منطقة مبرّدة، يمكن أن ينص استعلام إجراءات توجيه الموقع على ذلك.</span><span class="sxs-lookup"><span data-stu-id="b76da-179">For example, if you are receiving items that need to be put into a refrigerated zone, the Location directive actions query can make that stipulation.</span></span>

<span data-ttu-id="b76da-180">[![لقطة شاشة لأنواع أوامر عمل توجيه الموقع.](../media/location-directives-work.png)](../media/location-directives-work.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b76da-180">[![Screenshot of the location directives work order types.](../media/location-directives-work.png)](../media/location-directives-work.png#lightbox)</span></span>

## <a name="disposition-codes"></a><span data-ttu-id="b76da-181">رموز التخلص</span><span class="sxs-lookup"><span data-stu-id="b76da-181">Disposition codes</span></span> 

<span data-ttu-id="b76da-182">رموز الإرجاع عبارة عن مجموعة من القواعد المستخدمة عند استلام أصناف تالفة.</span><span class="sxs-lookup"><span data-stu-id="b76da-182">Disposition codes are a collection of rules that are used when damaged items are received.</span></span>

![لقطة شاشة لصفحة "رموز الإرجاع".](../media/disposition-codes.png)

<span data-ttu-id="b76da-184">رمز الإرجاع، المتوفّر في **إدارة المستودعات > الإعداد > جهاز محمول**، هو حقل الغرض منه هو استخدامه في توجيه الموقع لإرجاع البضائع.</span><span class="sxs-lookup"><span data-stu-id="b76da-184">A disposition code, found in **Warehouse management > Setup > Mobile device**, is a field that is intended for use on a location directive for return merchandise.</span></span> <span data-ttu-id="b76da-185">ويصف الإجراء الذي سيتم اتخاذه عند معالجة عملية الإرجاع.</span><span class="sxs-lookup"><span data-stu-id="b76da-185">It describes what action will be taken upon processing of the return.</span></span> 

<span data-ttu-id="b76da-186">شاهد هذا الفيديو للاطّلاع على عرض توضيحي لـ **قوالب العمل** و **توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="b76da-186">Watch this video to  see a demonstration of **Work templates** and **Location directives**.</span></span>
 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4MBmY]

