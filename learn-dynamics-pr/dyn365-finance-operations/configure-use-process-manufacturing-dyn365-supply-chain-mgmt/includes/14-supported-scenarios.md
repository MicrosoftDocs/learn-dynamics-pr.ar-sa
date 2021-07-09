---
ms.openlocfilehash: 4e8777ae1f902f8cbacf02c58a265a69d351ec47
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073161"
---
<span data-ttu-id="93933-101">لا تدعم جميع مهام سير العمل معالجة منتجات وزن التعبئة مع إدارة المستودع.</span><span class="sxs-lookup"><span data-stu-id="93933-101">Not all workflows support catch weight product processing with warehouse management.</span></span> <span data-ttu-id="93933-102">تنطبق القيود التالية:</span><span class="sxs-lookup"><span data-stu-id="93933-102">The following restrictions apply:</span></span>

-   <span data-ttu-id="93933-103">بالنسبة لمنتجات وزن التعبئة، لا يمكن تغيير مجموعة أبعاد التخزين للأصناف (بحيث يمكن استخدام عمليات إدارة المستودع لها).</span><span class="sxs-lookup"><span data-stu-id="93933-103">For catch weight products, the storage dimension group for items can't be changed (so that warehouse management processes can be used for them).</span></span>

-   <span data-ttu-id="93933-104">لا يمكن إنشاء أصناف وزن التعبئة لأصناف المعادلة فقط.</span><span class="sxs-lookup"><span data-stu-id="93933-104">Catch weight items can only be created for formula items.</span></span>

-   <span data-ttu-id="93933-105">لا يمكن ربط منتجات وزن التعبئة بمجموعة أبعاد تعقب حيث يكون مالك البُعد عبارة عن مستخدم نشط.</span><span class="sxs-lookup"><span data-stu-id="93933-105">Catch weight products can't be associated with a tracking dimension group where the dimension owner is an active user.</span></span>

-   <span data-ttu-id="93933-106">لا يمكن إنشاء صنف وزن التعبئة لمنتج من نوع الخدمة.</span><span class="sxs-lookup"><span data-stu-id="93933-106">It is not possible to create a catch weight item for a product of the Service type.</span></span>

-   <span data-ttu-id="93933-107">يجب أن تكون منتجات وزن التعبئة منتجات مخزّنة عن طريق تعيينها إلى مجموعة نماذج الصنف مع تحديد خانة الاختيار **‬‏‫منتج مخزّن**.</span><span class="sxs-lookup"><span data-stu-id="93933-107">Catch weight products must be stocked products by assigning it to an item model group with the **Stocked product** check box selected.</span></span>

-   <span data-ttu-id="93933-108">لا يمكن استخدام منتجات وزن التعبئة مع وظيفة تسجيل التسلسلات قبل الاستهلاك.</span><span class="sxs-lookup"><span data-stu-id="93933-108">Catch weight products can't be used together with the functionality for registering serials before consumption.</span></span>

-   <span data-ttu-id="93933-109">لا يمكن استخدام منتجات وزن التعبئة الممكنة للمتغير مع وظيفة تحويل وحدات القياس المتغيرة.</span><span class="sxs-lookup"><span data-stu-id="93933-109">Catch weight products that are variant-enabled can't be used together with the functionality for converting variant units of measure.</span></span>

-   <span data-ttu-id="93933-110">لا يمكن تحديد منتجات وزن التعبئة كـ "مجموعة منتجات" للبيع بالتجزئة.</span><span class="sxs-lookup"><span data-stu-id="93933-110">Catch weight products can't be selected as a retail "product kit."</span></span>

-   <span data-ttu-id="93933-111">لا يمكن استخدام منتجات وزن التعبئة إلا مع مجموعة تسلسل وحدة تحتوي على وحدات معالجة وزن التعبئة ولها وحدة وزن التعبئة كأقل تسلسل.</span><span class="sxs-lookup"><span data-stu-id="93933-111">Catch weight products can be used only with a unit sequence group that has catch weight handling units and that has the catch weight unit as the lowest sequence.</span></span>

-   <span data-ttu-id="93933-112">بالنسبة لمنتجات وزن التعبئة، يمكن تحويل وحدة المخزون إلى وحدة وزن التعبئة فقط إذا كان التحويل ينتج كمية اسمية تزيد عن كمية واحدة.</span><span class="sxs-lookup"><span data-stu-id="93933-112">For catch weight products, the inventory unit can be converted to the catch weight unit only if the conversion produces a nominal quantity that is more than one.</span></span>

-   <span data-ttu-id="93933-113">لا يدعم إعداد الرموز الشريطية لمنتجات وزن التعبئة إعداد الوزن المتغير.</span><span class="sxs-lookup"><span data-stu-id="93933-113">The setup of bar codes for catch weight products doesn't support a variable weight setup.</span></span>

### <a name="order-processing"></a><span data-ttu-id="93933-114">معالجة الأوامر</span><span class="sxs-lookup"><span data-stu-id="93933-114">Order processing</span></span>
<span data-ttu-id="93933-115">تنطبق القيود التالية على سير عمل معالجة الطلبات:</span><span class="sxs-lookup"><span data-stu-id="93933-115">The following restrictions apply for order processing workflows:</span></span>

-   <span data-ttu-id="93933-116">لا يتم دعم معالجة أمر بين الشركات الشقيقة لمنتجات وزن التعبئة ما لم تكن الوحدات المناسبة لتحويل الوحدة ووزن التعبئة متوافقة بين الكيانين القانونيين في التجارة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="93933-116">Intercompany order processing for catch weight products isn't supported unless the proper unit conversion and catch weight units are compatible between the two legal entities in the intercompany trade.</span></span>

-   <span data-ttu-id="93933-117">لا تدعم عملية إنشاء إشعار الشحن المسبق (ASN/بنيات التعبئة) معلومات الوزن.</span><span class="sxs-lookup"><span data-stu-id="93933-117">The creation of advance ship notice (ASN/packing structures) doesn't support weight information.</span></span>

-   <span data-ttu-id="93933-118">يجب صيانة كمية الأمر استناداً إلى وحدة وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-118">The order quantity must be maintained based on the catch weight unit.</span></span>

### <a name="inbound-warehouse-processing"></a><span data-ttu-id="93933-119">معالجة المستودع الوارد</span><span class="sxs-lookup"><span data-stu-id="93933-119">Inbound warehouse processing</span></span>
<span data-ttu-id="93933-120">تنطبق القيود التالية على سير عمل معالجة المستودع الوارد:</span><span class="sxs-lookup"><span data-stu-id="93933-120">The following restrictions apply for inbound warehouse processing workflows:</span></span>

-   <span data-ttu-id="93933-121">يتطلب استلام لوحات الترخيص أن يتم تعيين الأوزان أثناء التسجيل نظراً لأن معلومات الوزن غير مدعومة كجزء من إشعار الشحن المسبق.</span><span class="sxs-lookup"><span data-stu-id="93933-121">Receiving license plates requires that weights are assigned during registration because weight information isn't supported as part of the advance ship notice.</span></span> <span data-ttu-id="93933-122">عند استخدام عمليات علامة وزن التعبئة، يجب تعيين رقم العلامة يدوياً لكل وحدة وزن تعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-122">When catch weight tag processes are used, the tag number must be manually assigned for each catch weight unit.</span></span>

-   <span data-ttu-id="93933-123">استلام لوحات الترخيص المختلطة غير مدعوم لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-123">Receiving mixed license plates isn't supported for catch weight products.</span></span>

### <a name="inventory-and-warehouse-operations"></a><span data-ttu-id="93933-124">عمليات المستودع والمخزون</span><span class="sxs-lookup"><span data-stu-id="93933-124">Inventory and warehouse operations</span></span>
<span data-ttu-id="93933-125">تنطبق القيود التالية على سير عمل عمليات المستودع والمخزون:</span><span class="sxs-lookup"><span data-stu-id="93933-125">The following restrictions apply for inventory and warehouse operations workflows:</span></span>

-   <span data-ttu-id="93933-126">لا يتم دعم الإنشاء اليدوي لأوامر العزل لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-126">Manual creation of quarantine orders isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-127">لا يتم دعم الحركة اليدوية للمخزون المرتبط بالعمل لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-127">Manual movement of inventory that is related to work isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-128">لا يتم دعم دمج لوحات الترخيص لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-128">Consolidation of license plates isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-129">لا يتم دعم التغييرات التي يتم إدخالها على حالة مخزون المستودع كجزء من مهمة دورية لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-129">Changes to the warehouse inventory status as part of a periodic task aren't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-130">لا يتم دعم التغييرات التي يتم تحديدها بواسطة استعلام في حالة المخزون لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-130">Changes to an inventory status that are defined by a query aren't supported for catch weight products.</span></span> <span data-ttu-id="93933-131">(لا يتم اعتماد التغييرات التي تم إجراؤها على حالة مخزون أمر الجودة بأي شكل.)</span><span class="sxs-lookup"><span data-stu-id="93933-131">(Changes to a quality order inventory status aren't supported either.)</span></span>

-   <span data-ttu-id="93933-132">بالنسبة لمنتجات وزن التعبئة، لا يمكن تغيير حالة المخزون من الصفحة **الكمية الفعلية حسب الموقع** .</span><span class="sxs-lookup"><span data-stu-id="93933-132">For catch weight products, the inventory status can't be changed from the **On-hand by location** page.</span></span>

-   <span data-ttu-id="93933-133">بالنسبة لمنتجات وزن التعبئة، لا يمكن تغيير حالة المخزون كجزء من عمل حركة تطبيق المستودع.</span><span class="sxs-lookup"><span data-stu-id="93933-133">For catch weight products, the inventory status can't be changed as part of warehouse app movement work.</span></span>

-   <span data-ttu-id="93933-134">لم يتم دعم تحميل لوحة الترخيص الخاصة بتهيئة مخزون المستودع لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-134">License plate loading to initialize warehouse stock isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-135">معالجة المخزون الفعلي السالب غير مدعومة لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-135">Handling of negative physical inventory isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-136">لا يمكن استخدام علامات المخزون لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-136">Inventory marking can't be used for catch weight products.</span></span>

### <a name="outbound-warehouse-processing"></a><span data-ttu-id="93933-137">معالجة المستودع الصادر</span><span class="sxs-lookup"><span data-stu-id="93933-137">Outbound warehouse processing</span></span>
<span data-ttu-id="93933-138">تنطبق القيود التالية على سير عمل معالجة المستودع الصادر:</span><span class="sxs-lookup"><span data-stu-id="93933-138">The following restrictions apply for outbound warehouse processing workflows:</span></span>

-   <span data-ttu-id="93933-139">لا يتم دعم وظيفة انتقاء نظام المجموعة لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-139">The functionality for cluster picking isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-140">لا يتم دعم معالجة مستودع الانتقاء والتعبئة‬ لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-140">Pick and pack warehouse processing isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-141">بالنسبة لمنتجات وزن التعبئة، يتعذّر إكمال العمل من صفحة **العمل** .</span><span class="sxs-lookup"><span data-stu-id="93933-141">For catch weight products, work can't be completed from the **Work** page.</span></span>

-   <span data-ttu-id="93933-142">بالنسبة لمنتجات وزن التعبئة، يمكن تشغيل العمل المحدد في قالب العمل تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="93933-142">For catch weight products, work that is defined in a work template can be run automatically.</span></span>

-   <span data-ttu-id="93933-143">لا يتم دعم وظيفة عكس العمل لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-143">The functionality for reversing work isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-144">بالنسبة لمنتجات وزن التعبئة، لا يتم دعم معالجة محطة التعبئة اليدوية حيث يتم إنشاء العمل بعد إغلاق الحاويات.</span><span class="sxs-lookup"><span data-stu-id="93933-144">For catch weight products, manual packing station processing where work is created after containers are closed isn't supported.</span></span>

-   <span data-ttu-id="93933-145">لا يتم دعم وظيفة مسح أجهزة الكمبيوتر باستخدام بعضها البعض لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-145">The functionality for pcs-by-pcs scanning isn't supported for catch weight products.</span></span>

### <a name="production-processing"></a><span data-ttu-id="93933-146">معالجة الإنتاج</span><span class="sxs-lookup"><span data-stu-id="93933-146">Production processing</span></span>
<span data-ttu-id="93933-147">تنطبق القيود التالية على سير عمل معالجة الإنتاج:</span><span class="sxs-lookup"><span data-stu-id="93933-147">The following restrictions apply for production processing workflows:</span></span>

-   <span data-ttu-id="93933-148">بالنسبة لمنتجات وزن التعبئة، يتم دعم أوامر الدفعة لمنتجات المعادلة فقط.</span><span class="sxs-lookup"><span data-stu-id="93933-148">For catch weight products, only batch orders for formula products are supported.</span></span>

-   <span data-ttu-id="93933-149">لا يتم دعم وظائف كانبان لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-149">Kanban functionality isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-150">بالنسبة لمنتجات وزن التعبئة، لا يمكن تسجيل الأرقام التسلسلية قبل الاستهلاك.</span><span class="sxs-lookup"><span data-stu-id="93933-150">For catch weight products, serial numbers can't be registered before consumption.</span></span>

-   <span data-ttu-id="93933-151">لا يتم دعم وظيفة عكس لوحات الترخيص لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-151">The functionality for reversing license plates isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-152">بالنسبة لمنتجات وزن التعبئة، يمكن تسجيل الإبلاغ كمنتهٍ بالرقم التسلسلي.</span><span class="sxs-lookup"><span data-stu-id="93933-152">For catch weight products, reporting as finished can be registered by serial number.</span></span>

### <a name="transportation-management-processing"></a><span data-ttu-id="93933-153">معالجة إدارة النقل</span><span class="sxs-lookup"><span data-stu-id="93933-153">Transportation management processing</span></span>
<span data-ttu-id="93933-154">تنطبق القيود التالية على سير عمل معالجة إدارة النقل:</span><span class="sxs-lookup"><span data-stu-id="93933-154">The following restrictions apply for transportation management processing workflows:</span></span>

-   <span data-ttu-id="93933-155">لا يتم دعم معالجة ‏‫منضدة عمل إنشاء الأحمال‬‬ لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-155">Load building workbench processing isn't supported for catch weight products.</span></span>

-   <span data-ttu-id="93933-156">بنود طلب النقل غير مدعومة لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-156">Transport request lines aren't supported for catch weight products.</span></span>

### <a name="other-restrictions-and-behaviors"></a><span data-ttu-id="93933-157">القيود والسلوكيات الأخرى</span><span class="sxs-lookup"><span data-stu-id="93933-157">Other restrictions and behaviors</span></span>
<span data-ttu-id="93933-158">تتضمن القيود والسلوكيات الأخرى لمعالجة منتج وزن التعبئة في إدارة المستودعات ما يلي:</span><span class="sxs-lookup"><span data-stu-id="93933-158">Other restrictions and behaviors for catch weight product processing with warehouse management include:</span></span> 

-   <span data-ttu-id="93933-159">عند تسجيل علامات وزن التعبئة كجزء من معالجة تطبيق المستودع، فلن يتمكن المستخدم من إلغاء سير العمل.</span><span class="sxs-lookup"><span data-stu-id="93933-159">When catch weight tags are captured as part of warehouse app processing, the user can't cancel out of the workflow.</span></span>

-   <span data-ttu-id="93933-160">أثناء عمليات الانتقاء التي لا تتم مطالبة المستخدم فيها بتحديد أبعاد التعقب، يتم تعيين الوزن استناداً إلى متوسط الوزن.</span><span class="sxs-lookup"><span data-stu-id="93933-160">During picking processes where the user isn't prompted to identify tracking dimensions, the weight assignment is done based on the average weight.</span></span> <span data-ttu-id="93933-161">يحدث هذا السلوك عند، على سبيل المثال، يتم استخدام مجموعة من أبعاد التعقب في نفس الموقع، وبعد معالجة المستخدم الانتقاء، يتم ترك قيمة بُعد تعقب واحدة فقط في الموقع.</span><span class="sxs-lookup"><span data-stu-id="93933-161">This behavior occurs when, for example, a combination of tracking dimensions is used in the same location and, after a user processes picking, only one tracking dimension value is left in the location.</span></span>

-   <span data-ttu-id="93933-162">عند حجز المخزون لمنتج وزن التعبئة الذي تم تكوينه لعمليات إدارة المستودع، يتم الحجز استناداً إلى الحد الأدنى للوزن الذي تم تحديده، حتى إذا كانت هذه الكمية هي كمية المعالجة الأخيرة الفعلية.</span><span class="sxs-lookup"><span data-stu-id="93933-162">When inventory is reserved for a catch weight product that is configured for warehouse management processes, the reservation is done based on the minimum weight that is defined, even if this quantity is the on-hand last handling quantity.</span></span> <span data-ttu-id="93933-163">يختلف هذا السلوك عن سلوك الأصناف التي لم يتم تكوينها لعمليات إدارة المستودع.</span><span class="sxs-lookup"><span data-stu-id="93933-163">This behavior differs from the behavior for items that aren't configured for warehouse management processes.</span></span>

-   <span data-ttu-id="93933-164">لا تستخدم العمليات التي تستخدم الوزن كجزء من حسابات القدرة (حدود الموجة وفواصل العمل القصوى والحد الأقصى للحاويات وسعات تحميل الموقع وما إلى ذلك) الوزن الفعلي للمخزون.</span><span class="sxs-lookup"><span data-stu-id="93933-164">Processes that use the weight as part of capacity calculations (wave thresholds, work maximum breaks, container maximums, location load capacities, and so on) don't use the actual weight of the inventory.</span></span> <span data-ttu-id="93933-165">وبدلاً من ذلك، تعتمد العمليات على وزن المعالجة الفعلي الذي تم تحديده للمنتج.</span><span class="sxs-lookup"><span data-stu-id="93933-165">Instead, the processes are based on the physical handling weight that is defined for the product.</span></span>

-   <span data-ttu-id="93933-166">بشكل عام، لا يتم دعم وظائف البيع بالتجزئة لمنتجات وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="93933-166">In general, retail functionality isn't supported for catch weight products.</span></span>
