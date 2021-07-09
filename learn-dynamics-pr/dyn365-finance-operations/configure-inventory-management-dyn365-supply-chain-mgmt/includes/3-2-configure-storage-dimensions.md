---
ms.openlocfilehash: d2803135bb1190b0b00be11385cfe26634e9bb25
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073674"
---
<span data-ttu-id="09915-101">تمثل أبعاد مخزون التخزين الطرق المختلفة التي يتم من خلالها تخزين الأصناف واستردادها من المخزون.</span><span class="sxs-lookup"><span data-stu-id="09915-101">Storage inventory dimensions represent the different ways in which items are stored and retrieved from inventory.</span></span> <span data-ttu-id="09915-102">وهذه تسمح بإدارة المخزون على مستوى تفصيلي.</span><span class="sxs-lookup"><span data-stu-id="09915-102">This allows for inventory to be managed at a detailed level.</span></span> <span data-ttu-id="09915-103">يعتمد نوع التفاصيل التي تنطبق على إنشاء أبعاد التخزين على احتياجات الشركة وتوقعاتها.</span><span class="sxs-lookup"><span data-stu-id="09915-103">The type of details that you apply to the creation of storage dimensions depends on your company’s needs and expectations.</span></span> <span data-ttu-id="09915-104">خذ بعين الاعتبار صلة كل بُعد، خاصة عندما يكون للأصناف احتياجات معالجة خاصة.</span><span class="sxs-lookup"><span data-stu-id="09915-104">Consider the relevance of each dimension, especially when items have special handling needs.</span></span>

<span data-ttu-id="09915-105">فيما يلي أبعاد التخزين المتوفرة في Supply Chain Management:</span><span class="sxs-lookup"><span data-stu-id="09915-105">The storage dimensions that are available in Supply Chain Management are:</span></span>

- <span data-ttu-id="09915-106">الموقع</span><span class="sxs-lookup"><span data-stu-id="09915-106">Site</span></span>
- <span data-ttu-id="09915-107">المستودع</span><span class="sxs-lookup"><span data-stu-id="09915-107">Warehouse</span></span>
- <span data-ttu-id="09915-108">الموقع</span><span class="sxs-lookup"><span data-stu-id="09915-108">Location</span></span>
- <span data-ttu-id="09915-109">حالة المخزون</span><span class="sxs-lookup"><span data-stu-id="09915-109">Inventory status</span></span>
- <span data-ttu-id="09915-110">لوحة الترخيص</span><span class="sxs-lookup"><span data-stu-id="09915-110">License plate</span></span>

<span data-ttu-id="09915-111">يجب تعيين مجموعة أبعاد تخزين لمنتج تم إصداره.</span><span class="sxs-lookup"><span data-stu-id="09915-111">A storage dimension group must be assigned to a released product.</span></span> <span data-ttu-id="09915-112">تستخدم مجموعات أبعاد التخزين في تحديد كيفية تخزين المخزون في المستودع الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="09915-112">Storage dimension groups are used to determine how inventory will be stored in your warehouse.</span></span> <span data-ttu-id="09915-113">تتضمن Supply Chain Management بعض أبعاد المخزون والخيارات التي ينبغي لك مراعاتها عند إنشاء مجموعات الأبعاد.</span><span class="sxs-lookup"><span data-stu-id="09915-113">Supply Chain Management includes some inventory dimensions and options for you to consider when creating your dimension groups.</span></span>  

<span data-ttu-id="09915-114">**إدارة معلومات المنتج > الإعداد > مجموعات الأبعاد والمتغيرات > مجموعات أبعاد التخزين**</span><span class="sxs-lookup"><span data-stu-id="09915-114">**Product information management > Setup > Dimension and variant groups > Storage dimension groups**</span></span>

<span data-ttu-id="09915-115">[![لقطة شاشة لصفحة مجموعات أبعاد التخزين.](../media/storage-dimension-groups.png)](../media/storage-dimension-groups.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="09915-115">[![Screenshot of the Storage dimension groups page.](../media/storage-dimension-groups.png)](../media/storage-dimension-groups.png#lightbox)</span></span>

<span data-ttu-id="09915-116">قد تتضمن بعض الأمثلة المتطلبات التالية:</span><span class="sxs-lookup"><span data-stu-id="09915-116">Some examples might include the following requirements:</span></span>

- <span data-ttu-id="09915-117">يجب المحافظة على منتجات الألبان باردة.</span><span class="sxs-lookup"><span data-stu-id="09915-117">Dairy foods must be kept cool.</span></span>
- <span data-ttu-id="09915-118">ويجب أن يكون من السهل تعريف البضائع الصيدلية.</span><span class="sxs-lookup"><span data-stu-id="09915-118">Pharmaceutical goods must be easily identifiable.</span></span>
- <span data-ttu-id="09915-119">يجب الاحتفاظ بالأيس كريم مجمداً.</span><span class="sxs-lookup"><span data-stu-id="09915-119">Ice cream must be kept frozen.</span></span>

### <a name="scenario"></a><span data-ttu-id="09915-120">السيناريو</span><span class="sxs-lookup"><span data-stu-id="09915-120">Scenario</span></span> 

<span data-ttu-id="09915-121">لدى إحدى شركات الدراجات عدة منشآت لتخزين أجزاء الدراجات وتصنيعها.</span><span class="sxs-lookup"><span data-stu-id="09915-121">A bicycle company has several facilities that store and manufacture bicycle parts.</span></span> <span data-ttu-id="09915-122">في كل منشأة، يتم تخزين مسننات من 10 سرعات في صندوق واحد، ويتم تخزين المسننات من 12 سرعة في صندوق آخر.</span><span class="sxs-lookup"><span data-stu-id="09915-122">At each facility, 10-speed sprockets are stored in one bin, and 12-speed sprockets are stored in another bin.</span></span> <span data-ttu-id="09915-123">ومع ذلك، نظرا لأن يتم تحديد أحجام إطار الدراجات بسهولة، فإنه لا يتم فصلها في المستودع.</span><span class="sxs-lookup"><span data-stu-id="09915-123">However, because bicycle frame sizes are easily determined, they are not separated in the warehouse.</span></span> <span data-ttu-id="09915-124">يتم تخزين إطارات الرئيسية والفرعية في نفس الحوامل.</span><span class="sxs-lookup"><span data-stu-id="09915-124">Adult and children's frames are stored in the same racks.</span></span> <span data-ttu-id="09915-125">وترغب الشركة في ضمان الاحتفاظ بجرد دقيق للمخزون لكافة الأجزاء.</span><span class="sxs-lookup"><span data-stu-id="09915-125">The company wants to ensure that an accurate count of inventory is kept for all parts.</span></span>

## <a name="mandatory"></a><span data-ttu-id="09915-126">إلزامي</span><span class="sxs-lookup"><span data-stu-id="09915-126">Mandatory</span></span> 

<span data-ttu-id="09915-127">حدد شريط التمرير **إلزامي** في صفحة **مجموعات أبعاد التخزين** لجعل البُعد إلزامياً.</span><span class="sxs-lookup"><span data-stu-id="09915-127">Select the **Mandatory** slider on the **Storage dimension groups** page to make the dimension mandatory.</span></span> <span data-ttu-id="09915-128">يظهر البُعد الإلزامي على كافة دفاتر اليومية والحركات، ويجب عليك تحديد قيمة بُعد عند إنشاء إدخال.</span><span class="sxs-lookup"><span data-stu-id="09915-128">A mandatory dimension appears on all journals and transactions, and you must specify a dimension value when creating an entry.</span></span> 

<span data-ttu-id="09915-129">يتم تطبيق القواعد التالية:</span><span class="sxs-lookup"><span data-stu-id="09915-129">The following rules apply:</span></span> 

- <span data-ttu-id="09915-130">تكون أبعاد المنتج إلزامية دائماً.</span><span class="sxs-lookup"><span data-stu-id="09915-130">Product dimensions are always mandatory.</span></span>
- <span data-ttu-id="09915-131">عندما تكون وظيفة المواقع المتعددة نشطة، يكون بُعد تخزين الموقع إلزامياً.</span><span class="sxs-lookup"><span data-stu-id="09915-131">When the multi-site functionality is active, the site storage dimension is mandatory.</span></span>
- <span data-ttu-id="09915-132">يعتبر تعيين بُعد تخزين المستودع كإلزامي أمراً اختيارياً.</span><span class="sxs-lookup"><span data-stu-id="09915-132">It is optional whether the warehouse storage dimension is mandatory.</span></span>
- <span data-ttu-id="09915-133">لا يمكنك تحديد أبعاد المخزون المتبقية كإلزامية.</span><span class="sxs-lookup"><span data-stu-id="09915-133">You cannot specify the remaining inventory dimensions as mandatory.</span></span>

## <a name="primary-stocking"></a><span data-ttu-id="09915-134">المخزون الأساسي</span><span class="sxs-lookup"><span data-stu-id="09915-134">Primary stocking</span></span> 

<span data-ttu-id="09915-135">لإعداد أبعاد المخزون كمخزون أساسي، في صفحة **مجموعات أبعاد التخزين**، حدد شريط التمرير **المخزون الأساسي**.</span><span class="sxs-lookup"><span data-stu-id="09915-135">To set up inventory dimensions as primary stocking, on the **Storage dimension groups** page, select the **Primary stocking** slider.</span></span> <span data-ttu-id="09915-136">(إذا كنت ترغب في أن يكون هو المخزون الثانوي، فلا تقم بتحريك شريط التمرير.)</span><span class="sxs-lookup"><span data-stu-id="09915-136">(If you want it to be secondary stocking, do not move the slider.)</span></span>

<span data-ttu-id="09915-137">سيظهر بُعد المخزون الأساسي تلقائياً في صفحتي **المتاح** و **الحجز**.</span><span class="sxs-lookup"><span data-stu-id="09915-137">A primary stocking dimension will appear automatically on the **On-hand** and **Reservation** pages.</span></span> <span data-ttu-id="09915-138">ويؤثر ذلك على كيفية إعادة حجز الأصناف المطلوبة بناء على إيصالات الأصناف الفعلية.</span><span class="sxs-lookup"><span data-stu-id="09915-138">This affects how ordered items are re-reserved upon physical item receipts.</span></span> <span data-ttu-id="09915-139">يتم تطبيق القواعد التالية:</span><span class="sxs-lookup"><span data-stu-id="09915-139">The following rules apply:</span></span>

- <span data-ttu-id="09915-140">يجب تحديد البُعد عندما تقوم فعلياً بتحديث عمليات استلام الأصناف أو الإصدارات.</span><span class="sxs-lookup"><span data-stu-id="09915-140">The dimension must be specified when you are physically updating item receipts or issues.</span></span>
- <span data-ttu-id="09915-141">عند تنشيط الحجز التلقائي، يتم حجز الأصناف وفقاً للبُعد المحدد، شريطة أن يتم تحديد البُعد أيضاً لحركة الصنف الفعلية.</span><span class="sxs-lookup"><span data-stu-id="09915-141">When automatic reservation is active, items are reserved according to the selected dimension, provided that the dimension is also specified for the actual item transaction.</span></span> <span data-ttu-id="09915-142">وهذا يعني أنه في حالة تحديد المستودع في بند أمر المبيعات، وتم تحديد المخزون الأساسي، يقوم الحجز التلقائي بحجز الأصناف في هذا المستودع فقط.</span><span class="sxs-lookup"><span data-stu-id="09915-142">This means that if the warehouse is specified on a sales order line, and primary stocking is specified, automatic reservation only reserves items at this warehouse.</span></span>
- <span data-ttu-id="09915-143">ولا تتم إعادة حجز عمليات الحجز المطلوبة بناء على عملية الاستلام الفعلية.</span><span class="sxs-lookup"><span data-stu-id="09915-143">Ordered reservations are not re-reserved upon physical receipt.</span></span> <span data-ttu-id="09915-144">إذا تم حجز بند أمر مبيعات بالمستودع أ والموقع 1، وتم تعيين المستودع إلى المخزون الأساسي وتعيين الموقع إلى المخزون الثانوي، فلن يتم تلقائياً إعادة حجز بند أمر المبيعات إذا تغيّر المستودع عند تحديث عمليات الاستلام فعلياً.</span><span class="sxs-lookup"><span data-stu-id="09915-144">If a sales order line is reserved at warehouse A and location 1, and warehouse is set to primary stocking and location is set to secondary stocking, the sales order line does not automatically re-reserve if the warehouse is changed when the receipt is physically updated.</span></span> <span data-ttu-id="09915-145">إذا تغير الموقع إلى 2، سيقوم بند الأمر تلقائياً بإعادة الحجز للموقع 2.</span><span class="sxs-lookup"><span data-stu-id="09915-145">If the location changes to 2, the order line automatically re-reserves for location 2.</span></span>

## <a name="blank-receipt-allowed-and-blank-issue-allowed"></a><span data-ttu-id="09915-146">السماح بالإيصال الفارغ والسماح بالإصدار الفارغ</span><span class="sxs-lookup"><span data-stu-id="09915-146">Blank receipt allowed and Blank issue allowed</span></span> 

<span data-ttu-id="09915-147">حدد خانتي الاختيار **مسموح بالإيصال الفارغ** أو **مسموح بالإصدار الفارغ** في صفحة **مجموعات أبعاد التخزين** لتطبيق النتائج التالية:</span><span class="sxs-lookup"><span data-stu-id="09915-147">Select the **Blank receipt allowed** or **Blank issue allowed** check boxes on the **Storage dimension groups** page to apply the following results:</span></span>

- <span data-ttu-id="09915-148">**مسموح بالإيصال الفارغ** - في حالة عدم تحديد البعد كمخزون أساسي، فإن تحديد خانة الاختيار هذه يؤدي إلى ترك مواصفات البُعد عند تحديث عمليات الاستلام الفعلية.</span><span class="sxs-lookup"><span data-stu-id="09915-148">**Blank receipt allowed** - If you do not select the dimension as primary stocking, selecting this check box leaves out the specification of the dimension when physical receipts are updated.</span></span> <span data-ttu-id="09915-149">تعتبر هذه الوظيفة مفيدة، على سبيل المثال، عندما لا يتم تحديد رقم الشحنة/المسلسل عند الإدخال ولكن مع القيام بذلك للانتقاء والإخراج.</span><span class="sxs-lookup"><span data-stu-id="09915-149">This functionality is useful, for example, when you are not specifying the serial/lot number upon input but doing so for picking and output.</span></span>
- <span data-ttu-id="09915-150">**مسموح الإصدار الفارغ** - في حالة عدم تعليم البُعد كبعد منتج أو كمخزون أساسي، فإن تحديد هذا الحقل يؤدي إلى ترك مواصفات البُعد عند تحديث عمليات الإصدار الفعلية.</span><span class="sxs-lookup"><span data-stu-id="09915-150">**Blank issue allowed** - If the dimension is not marked as a product dimension, or as primary stocking, selecting this field leaves out the specification of the dimension when you are updating physical issues.</span></span>

## <a name="physical-inventory"></a><span data-ttu-id="09915-151">المخزون الفعلي</span><span class="sxs-lookup"><span data-stu-id="09915-151">Physical inventory</span></span> 

<span data-ttu-id="09915-152">حدد خانة الاختيار **المخزون الفعلي** لتحديد إدخال البُعد في المخزون الفعلي عندما يقوم النظام بالتحقق مما إذا كان الصنف متوفراً في المخزون أم لا.</span><span class="sxs-lookup"><span data-stu-id="09915-152">Select the **Physical inventory** check box to specify that the dimension is entered into the on-hand inventory when the system checks whether the item is available in inventory.</span></span>

## <a name="financial-inventory"></a><span data-ttu-id="09915-153">المخزون المالي</span><span class="sxs-lookup"><span data-stu-id="09915-153">Financial inventory</span></span> 

<span data-ttu-id="09915-154">حدد خانة الاختيار **المخزون المالي** للإشارة إلى أن هذا البعد جزء من المخزون المالي.</span><span class="sxs-lookup"><span data-stu-id="09915-154">Select the **Financial inventory** check box to indicate that this dimension is part of the financial inventory.</span></span> 

<span data-ttu-id="09915-155">تكون المعلمة في مهمة إذا كنت لا تعمل بمخزون سالب مالياً مع التحديث المالي لإصدارات الأصناف، على سبيل المثال، تحديث الفاتورة في الوحدة النمطية للحسابات المدينة.</span><span class="sxs-lookup"><span data-stu-id="09915-155">The parameter is of significance if you are not operating with financially negative inventory with the financial update of item issues, for example, invoice-updating in the Accounts receivable module.</span></span> <span data-ttu-id="09915-156">يفحص النظام المخزون الفعلي المالي تبعاً لإصدارات الأصناف وفقاً لنفس المنطق الموضح في الموضوع المتعلق بالمخزون الفعلي.</span><span class="sxs-lookup"><span data-stu-id="09915-156">The system checks the financial on-hand inventory upon item issues according to the same logic that was described in the topic concerning Physical inventory.</span></span>

<span data-ttu-id="09915-157">تحدد **معلمة المخزون المالي** أيضاً كيفية حساب استهلاك الصنف عند تحديث الفاتورة وإقفال المخزون ومحاسبة التكاليف لقيمة التكلفة.</span><span class="sxs-lookup"><span data-stu-id="09915-157">The **Financial inventory** parameter also determines how item consumption is calculated upon invoice updating, inventory closing, and cost accounting of the cost value.</span></span>

## <a name="coverage-plan-by-dimension"></a><span data-ttu-id="09915-158">خطة التغطية حسب البُعد</span><span class="sxs-lookup"><span data-stu-id="09915-158">Coverage plan by dimension</span></span> 

<span data-ttu-id="09915-159">حدد خانة الاختيار **خطة التغطية حسب البعد** في صفحة **مجموعات أبعاد التخزين** لإكمال خطة التغطية للصنف بشكل فردي، بدلاً من إكمالها كمجموعة.</span><span class="sxs-lookup"><span data-stu-id="09915-159">Select the **Coverage plan by dimension** check box on the **Storage dimension groups** page to complete the coverage plan for the item individually, instead of as a group.</span></span>

## <a name="for-purchase-price"></a><span data-ttu-id="09915-160">لسعر الشراء</span><span class="sxs-lookup"><span data-stu-id="09915-160">For purchase price</span></span>

<span data-ttu-id="09915-161">عند تحديد خانة الاختيار **لسعر الشراء** في صفحة **مجموعات أبعاد التخزين**، يعتمد البحث عن أسعار الشراء على القواعد التالية:</span><span class="sxs-lookup"><span data-stu-id="09915-161">When you select the **For purchase price** check box on the **Storage dimension groups** page, the search for purchase prices is based on the following rules:</span></span>

- <span data-ttu-id="09915-162">البحث عن السعر لكل صنف ولأبعاد المنتج وأبعاد التخزين</span><span class="sxs-lookup"><span data-stu-id="09915-162">Search price for each item, product dimensions, and storage dimensions</span></span>
- <span data-ttu-id="09915-163">البحث عن السعر لكل صنف ولأبعاد المنتج (أبعاد التخزين تكون فارغة)</span><span class="sxs-lookup"><span data-stu-id="09915-163">Search price for each item and product dimensions (storage dimensions are blank)</span></span>
- <span data-ttu-id="09915-164">البحث عن السعر لكل صنف (كل من أبعاد المنتج وأبعاد التخزين تكون فارغة)</span><span class="sxs-lookup"><span data-stu-id="09915-164">Search price for each item (both product dimensions and storage dimensions are blank)</span></span>


## <a name="for-sales-prices"></a><span data-ttu-id="09915-165">لأسعار البيع</span><span class="sxs-lookup"><span data-stu-id="09915-165">For sales prices</span></span>

<span data-ttu-id="09915-166">عند تحديد خانة الاختيار **لسعر البيع** في صفحة **مجموعات أبعاد التخزين**، يعتمد البحث عن أسعار البيع على القواعد التالية:</span><span class="sxs-lookup"><span data-stu-id="09915-166">When you select the **For sales prices** check box on the **Storage dimension groups** page, the search for sales prices is based on the following rules:</span></span>

- <span data-ttu-id="09915-167">البحث عن السعر لكل صنف ولأبعاد المنتج وأبعاد التخزين</span><span class="sxs-lookup"><span data-stu-id="09915-167">Search price for each item, product dimensions, and storage dimensions</span></span>
- <span data-ttu-id="09915-168">البحث عن السعر لكل صنف ولأبعاد المنتج (أبعاد التخزين تكون فارغة)</span><span class="sxs-lookup"><span data-stu-id="09915-168">Search price for each item and product dimensions (storage dimensions are blank)</span></span>
- <span data-ttu-id="09915-169">البحث عن السعر لكل صنف (كل من أبعاد المنتج وأبعاد التخزين تكون فارغة)</span><span class="sxs-lookup"><span data-stu-id="09915-169">Search price for each item (both product dimensions and storage dimensions are blank)</span></span>


