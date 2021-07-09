---
ms.openlocfilehash: 749dafb876cd628713fd10e1dfbc87b3de5a815a
ms.sourcegitcommit: d9d731bb071133aa102da6c7c602825acae008a2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2021
ms.locfileid: "6073713"
---
<span data-ttu-id="8f416-101">يساعد التعهد بالأمر في التعهد بتواريخ التسليم لعملائك بشكل موثوق به ويمنحك المرونة بحيث تتمكّن من الوفاء بالتسليم في هذه التواريخ.</span><span class="sxs-lookup"><span data-stu-id="8f416-101">Order promising helps you reliably promise delivery dates to your customers and gives you flexibility so that you can meet those dates.</span></span>

<span data-ttu-id="8f416-102">يحسب التعهد بالأمر أول مواعيد شحن واستلام متاحة وهي تستند إلى طريقة التحكم في تواريخ التسليم وعدد أيام النقل.</span><span class="sxs-lookup"><span data-stu-id="8f416-102">Order promising calculates the earliest ship and receipt dates and is based on the delivery date control method and transport days.</span></span> 

<span data-ttu-id="8f416-103">استناداً إلى نوع التحكم في تاريخ التسليم في بند أمر المبيعات، يحسب Supply Chain Management أول تاريخ تسليم متاح ويملأ **تاريخ الشحن المطلوب** و **‏‫‏‏تاريخ الاستلام المطلوب‬**.</span><span class="sxs-lookup"><span data-stu-id="8f416-103">Based on the delivery date control type on the sales order line, Supply Chain Management calculates the earliest delivery date and populates the **Requested ship date** and the **Requested receipt date**.</span></span>
<span data-ttu-id="8f416-104">**تاريخ الشحن المطلوب** هو أول تاريخ يمكن للشركة إرسال كمية البند الكاملة للمنتج من المستودع المحدد في البند.</span><span class="sxs-lookup"><span data-stu-id="8f416-104">The **Requested ship date** is the earliest date that the company is able to dispatch the product's full line quantity from the warehouse that is specified on the line.</span></span> <span data-ttu-id="8f416-105">**تاريخ الاستلام المطلوب** هو أول تاريخ يمكن توقُّع تسليم كمية البند الكاملة للمنتج فيه إلى عنوان العميل.</span><span class="sxs-lookup"><span data-stu-id="8f416-105">The **Requested receipt date** is the earliest date that the product's full line quantity can be expected to be delivered to the customer's address.</span></span>

<span data-ttu-id="8f416-106">توضح الصورة التالية الأنواع الخمسة للتحكم بتاريخ التسليم.</span><span class="sxs-lookup"><span data-stu-id="8f416-106">The five delivery date control types are shown in the following image.</span></span>

![رسم تخطيطي يوضح الطرق المختلفة للتعهد بالأمر.](../media/order-promising-methods.png)

### <a name="none"></a><span data-ttu-id="8f416-108">بلا</span><span class="sxs-lookup"><span data-stu-id="8f416-108">None</span></span>

<span data-ttu-id="8f416-109">توضح الصورة التالية أثر التعهد بالأمر في حالة تعيين التحكم في تاريخ التسليم على **بلا**.</span><span class="sxs-lookup"><span data-stu-id="8f416-109">The following image shows the impact of order promising if the delivery date control is set to **None**.</span></span> <span data-ttu-id="8f416-110">تفترض ميزة التعهد بالأمر أن المخزون متوفر دائماً وأن شحنة الأمر يمكن التعهد بها في يوم تسجيل الأمر.</span><span class="sxs-lookup"><span data-stu-id="8f416-110">Order promising assumes that stock is always available and order shipment can be promised on the day that the order is taken.</span></span>

![رسم تخطيطي للعملية التي تتضمن المراحل: "الإدخال" و"الشحن" و"النقل" و"الاستلام".](../media/none-1.png)

### <a name="sales-lead-time"></a><span data-ttu-id="8f416-112">الحد الأدنى لوقت الإنتاج لوقت المبيعات</span><span class="sxs-lookup"><span data-stu-id="8f416-112">Sales lead time</span></span>

<span data-ttu-id="8f416-113">توضح الصورة التالية أثر التعهد بالأمر في حالة تعيين التحكم في تاريخ التسليم على **‏‫الحد الأدنى لوقت الإنتاج لوقت المبيعات‬**.</span><span class="sxs-lookup"><span data-stu-id="8f416-113">The following image shows the impact of order promising if the delivery date control is set to **Sales lead time**.</span></span> <span data-ttu-id="8f416-114">‏‫الحد الأدنى لوقت الإنتاج لوقت المبيعات‬ هو الوقت بين إنشاء أمر المبيعات وشحن الأصناف.</span><span class="sxs-lookup"><span data-stu-id="8f416-114">Sales lead time is the time between creation of the sales order and shipment of the items.</span></span> <span data-ttu-id="8f416-115">يعتمد حساب تاريخ التسليم على عدد افتراضي من الأيام ولا يضع في الاعتبار مدى توفر المخزون أو الطلب المعروف أو التوريد المخطط.</span><span class="sxs-lookup"><span data-stu-id="8f416-115">The delivery date calculation is based on a default number of days and does not consider stock availability, known demand, or planned supply.</span></span> <span data-ttu-id="8f416-116">يمكنك تعريف ‏‫الحد الأدنى لوقت الإنتاج لأحد المواقع.</span><span class="sxs-lookup"><span data-stu-id="8f416-116">You can define the lead time for a site.</span></span> <span data-ttu-id="8f416-117">في حالة عدم تحديد الحد الأدنى لوقت الإنتاج لموقع معيّن، يتم استخدام الإعداد الافتراضي للصنف.</span><span class="sxs-lookup"><span data-stu-id="8f416-117">If no site-specific lead time is defined, the default setting for the item is used.</span></span>

<span data-ttu-id="8f416-118">يفترض التعهد بالأمر أن المخزون متاح خارج الحد الأدنى لوقت الإنتاج ويمكن التعهد بشحن الأمر بصرف النظر عن مدى التوفّر الفعلي.</span><span class="sxs-lookup"><span data-stu-id="8f416-118">Order promising assumes that stock is available beyond the lead time and order shipment can be promised regardless of the actual availability.</span></span>

![رسم تخطيطي للعملية التي تتضمن المراحل: "الإدخال" و"‏‏الحد الأدنى لوقت الإنتاج لوقت المبيعات الثابت" و"الشحن" و"النقل" و"الاستلام".](../media/sales-lead-time.png)

### <a name="available-to-promise-atp"></a><span data-ttu-id="8f416-120">متوفر حسب التعهد (ATP)</span><span class="sxs-lookup"><span data-stu-id="8f416-120">Available-to-promise (ATP)</span></span> 

<span data-ttu-id="8f416-121">ATP هو كمية الصنف المتوفرة والتي يمكن التعهد بها للعميل في تاريخ محدد.</span><span class="sxs-lookup"><span data-stu-id="8f416-121">ATP is the quantity of an item that is available and can be promised to a customer on a specific date.</span></span> <span data-ttu-id="8f416-122">يشمل حساب ATP المخزون الذي لم يتم الالتزام به و‏‫الحد الأدنى لوقت الإنتاج‬ وعمليات الاستلام المخططة والإصدارات.</span><span class="sxs-lookup"><span data-stu-id="8f416-122">The ATP calculation includes uncommitted inventory, lead times, planned receipts, and issues.</span></span>

<span data-ttu-id="8f416-123">يشمل ATP الميزات التالية:</span><span class="sxs-lookup"><span data-stu-id="8f416-123">ATP has the following features:</span></span>

-   <span data-ttu-id="8f416-124">تعتمد تعهدات التسليم على البيانات في الوقت الفعلي.</span><span class="sxs-lookup"><span data-stu-id="8f416-124">Delivery promises are based on real-time data.</span></span>

-   <span data-ttu-id="8f416-125">يستبعد أو يحد من الحجوزات حيث يضع في الاعتبار أوامر المبيعات التي تم إدخالها بالفعل (تم التعهد بها أو لم يتم تنفيذها).</span><span class="sxs-lookup"><span data-stu-id="8f416-125">Eliminates or reduces reservations as it considers sales order that are already entered (promised and unfulfilled).</span></span>

-   <span data-ttu-id="8f416-126">يمكن ضبطه بهامش وقت.</span><span class="sxs-lookup"><span data-stu-id="8f416-126">Can be fine-tuned with margin time.</span></span>

-   <span data-ttu-id="8f416-127">يضع في الاعتبار تقويمات العمل للأعمال التجارية إلى جانب تقويمات شركات النقل والعملاء.</span><span class="sxs-lookup"><span data-stu-id="8f416-127">Considers business's working calendars as well as carriers' and customers' calendars.</span></span>

-   <span data-ttu-id="8f416-128">يتطلب أداء عالي الجودة للتسليم من المورّدين.</span><span class="sxs-lookup"><span data-stu-id="8f416-128">Requires high delivery performance from suppliers.</span></span>

-   <span data-ttu-id="8f416-129">لا يتطلب تشغيل التخطيط ويستخدم التوريد الحالي.</span><span class="sxs-lookup"><span data-stu-id="8f416-129">Does not require a planning run and uses already existing supply.</span></span>

-   <span data-ttu-id="8f416-130">ملائم لصناعة التوزيع وشركات التصنيع للتخزين.</span><span class="sxs-lookup"><span data-stu-id="8f416-130">Good fit for distribution industry and make-to-stock manufacturers.</span></span>

-   <span data-ttu-id="8f416-131">يدعم التجارة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="8f416-131">Supports intercompany trade.</span></span>

<span data-ttu-id="8f416-132">تعرض الصورة التالية حساب ATP.</span><span class="sxs-lookup"><span data-stu-id="8f416-132">The following image shows the calculation of ATP.</span></span> <span data-ttu-id="8f416-133">يفحص المخزون والتوريد اللذين لم يتم الالتزام بهما والطلب الذي تم الالتزام به.</span><span class="sxs-lookup"><span data-stu-id="8f416-133">It checks uncommitted stock, supply, and committed demand.</span></span>

![‏‫رسم تخطيطي للعملية التي تتضمن المراحل: "الإدخال" و"A T P" و"الشحن" و"النقل" و"الاستلام".‬](../media/atp-1.png)

### <a name="atp--issue-margin"></a><span data-ttu-id="8f416-135">ATP + هامش الإصدار</span><span class="sxs-lookup"><span data-stu-id="8f416-135">ATP + issue margin</span></span>

<span data-ttu-id="8f416-136">أول تاريخ شحن يساوي تاريخ ATP زائد هامش إصدار الصنف.</span><span class="sxs-lookup"><span data-stu-id="8f416-136">The earliest ship date is equal to the ATP date plus the issue margin for the item.</span></span> <span data-ttu-id="8f416-137">هامش الإصدار هو الوقت المطلوب لتحضير الأصناف للشحن.</span><span class="sxs-lookup"><span data-stu-id="8f416-137">The issue margin is the time that is required to prepare the items for shipment.</span></span>

<span data-ttu-id="8f416-138">تعرض الصورة التالية حساب ATP + هامش الإصدار.</span><span class="sxs-lookup"><span data-stu-id="8f416-138">The following image shows the calculation of the ATP + issue margin.</span></span> <span data-ttu-id="8f416-139">ويفحص المخزون والتوريد اللذين لم يتم الالتزام بهما والطلب الذي تم الالتزام به وهامش ثابت بالأيام.</span><span class="sxs-lookup"><span data-stu-id="8f416-139">It checks uncommitted stock, supply, committed demand, and a fixed margin in days.</span></span>

![‏‫رسم تخطيطي للعملية التي تتضمن المراحل: "الإدخال" و"A T P" و"الإصدار" و"الشحن" و"النقل" و"الاستلام".‬](../media/atp-issue-margin.png)

### <a name="capable-to-promise-ctp"></a><span data-ttu-id="8f416-141">المتاح للتعهد (CTP)</span><span class="sxs-lookup"><span data-stu-id="8f416-141">Capable-to-promise (CTP)</span></span> 

<span data-ttu-id="8f416-142">CTP هو عندما يستند التعهد بالأمر إلى خطة ديناميكية (عملية تحديد إجمالي المكونات المطلوبة‬ لبند أمر المبيعات) والتحقق من مدى التوفر ومكونات ‏‫الحد الأدنى لوقت الإنتاج في BOM ووقت المعالجة في مسارات المنتج النهائي.</span><span class="sxs-lookup"><span data-stu-id="8f416-142">CTP is when order promising is based on a dynamic plan (sales order line explosion), checking availability and lead time components in the BOM and process time in the routes of the finished product.</span></span>

![‏‫رسم تخطيطي للعملية التي تتضمن المراحل: "الإدخال" و"C T P" و"الشحن" و"النقل" و"الاستلام".‬](../media/ctp-1.png)

## <a name="delivery-alternatives"></a><span data-ttu-id="8f416-144">بدائل التسليم</span><span class="sxs-lookup"><span data-stu-id="8f416-144">Delivery alternatives</span></span>

<span data-ttu-id="8f416-145">يمكن أن يستخدم مسجلو أوامر المبيعات صفحة **بدائل التسليم** لمعرفة خيارات تنفيذ الأوامر البديلة.</span><span class="sxs-lookup"><span data-stu-id="8f416-145">Sales order takers can use the **Delivery alternatives** page to discover alternative order fulfillment options.</span></span>

<span data-ttu-id="8f416-146">يوفر تخطيط صفحة **بدائل التسليم** نظرة عامة على جميع الخيارات البديلة.</span><span class="sxs-lookup"><span data-stu-id="8f416-146">The **Delivery alternatives** page layout gives an overview of all alternative options.</span></span> <span data-ttu-id="8f416-147">كما يتيح لمسجلي الأوامر البحث خارج الشركة الحالية عن فرص للتنفيذ.</span><span class="sxs-lookup"><span data-stu-id="8f416-147">It also lets order takers look beyond the current company for fulfillment opportunities.</span></span> <span data-ttu-id="8f416-148">في هذه الصفحة، يمكن أن يطلع مسجّلو الأوامر على الفرص بين الشركات الشقيقة والفرص من المورّدين الخارجيين.</span><span class="sxs-lookup"><span data-stu-id="8f416-148">On this page, order takers can view both intercompany opportunities and opportunities from external vendors.</span></span> <span data-ttu-id="8f416-149">من خلال فرز الخيارات حسب تاريخ التسليم، يمكن أن يطّلع مسجلو أوامر المبيعات على قائمة ذكية تتضمن بدائل التسليم.</span><span class="sxs-lookup"><span data-stu-id="8f416-149">By sorting the options by delivery date, sales order takers can view an intelligent list of delivery alternatives.</span></span> <span data-ttu-id="8f416-150">بالإضافة إلى ذلك، تساعدهم المعلمات على إدارة عمليات التسليم المقترحة بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="8f416-150">In addition, parameters help them better manage the suggested deliveries.</span></span> <span data-ttu-id="8f416-151">ولأن وقت النقل يمكن أن يؤثر في تواريخ التسليم، يمكن أن يستكشف مسجلو أوامر المبيعات خيارات النقل المختلفة التي تقدمها شركات النقل.</span><span class="sxs-lookup"><span data-stu-id="8f416-151">Because transport time can affect delivery dates, sales order takers can explore the various transportation choices that carriers offer.</span></span>

<span data-ttu-id="8f416-152">يجب وضع بدائل التسليم التالية في الاعتبار:</span><span class="sxs-lookup"><span data-stu-id="8f416-152">Consider the following delivery alternatives:</span></span>

-   <span data-ttu-id="8f416-153">التوصيات التي يحسبها البرنامج لأول تاريخ تسليم استناداً إلى:</span><span class="sxs-lookup"><span data-stu-id="8f416-153">Program-calculated recommendations for the earliest delivery date based on:</span></span>

    -   <span data-ttu-id="8f416-154">التوفر في جميع المواقع</span><span class="sxs-lookup"><span data-stu-id="8f416-154">Availability across sites</span></span>

    -   <span data-ttu-id="8f416-155">التوفر للمتغيرات</span><span class="sxs-lookup"><span data-stu-id="8f416-155">Availability for variants</span></span>

    -   <span data-ttu-id="8f416-156">الكمية الجزئية</span><span class="sxs-lookup"><span data-stu-id="8f416-156">Partial quantity</span></span>

    -   <span data-ttu-id="8f416-157">خيارات النقل البديلة</span><span class="sxs-lookup"><span data-stu-id="8f416-157">Alternative transportation options</span></span>

-   <span data-ttu-id="8f416-158">التوريد من مورّدين خارجيين أو من خلال الشركات الشقيقة أو توزيع البضائع أو كتسليم مباشر</span><span class="sxs-lookup"><span data-stu-id="8f416-158">Sourcing from external vendor or through intercompany, cross-docking, or as direct delivery</span></span>

-   <span data-ttu-id="8f416-159">تحليلات حول الطلب والتوريد الحاليَين لاستعراض احتمال إعادة التوزيع والتعجيل</span><span class="sxs-lookup"><span data-stu-id="8f416-159">Insights into existing demand and supply to potentially reallocate and expedite</span></span>

-   <span data-ttu-id="8f416-160">دعم جميع طرق التحكم في تاريخ التسليم</span><span class="sxs-lookup"><span data-stu-id="8f416-160">Support for all delivery date control methods</span></span>

## <a name="delivery-control-defaults"></a><span data-ttu-id="8f416-161">الإعدادات الافتراضية للتحكم في التسليم</span><span class="sxs-lookup"><span data-stu-id="8f416-161">Delivery control defaults</span></span>

<span data-ttu-id="8f416-162">في صفحة **معلمات الحسابات المدينة**، يمكنك ضبط الإعدادات الافتراضية للتحكم في التسليم.</span><span class="sxs-lookup"><span data-stu-id="8f416-162">On the **Accounts receivable parameters** page, you can set up defaults for delivery control.</span></span>

<span data-ttu-id="8f416-163">[![لقطة شاشة لصفحة معلمات الحسابات المدينة والتي تعرض علامة التبويب السريعة للتحكم في التسليم.](../media/ar-parameters-2.png)](../media/ar-parameters-2.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="8f416-163">[![Screenshot of the  Accounts receivable parameters page, showing the delivery control FastTab.](../media/ar-parameters-2.png)](../media/ar-parameters-2.png#lightbox)</span></span>

<span data-ttu-id="8f416-164">يمكنك أيضاً إعداد التعهد بالأمر لأحد المنتجات عن طريق الانتقال إلى صفحة **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="8f416-164">You can also set up the order promising of a product by going to **Product information management > Products > Released products** page.</span></span>

### <a name="atp-time-fence"></a><span data-ttu-id="8f416-165">الحد الزمني لـ ATP</span><span class="sxs-lookup"><span data-stu-id="8f416-165">ATP time fence</span></span>

<span data-ttu-id="8f416-166">يمكنك حساب ATP باستخدام ‏‫فترة الحد الزمني لـ ATP (بالأيام) إذا حددت طريقة حساب ATP في حقل **‏‏التحكم في تاريخ التسليم**.</span><span class="sxs-lookup"><span data-stu-id="8f416-166">Calculate ATP by using the ATP time fence period (in days) if you selected the ATP calculation method in the **Delivery date control** field.</span></span>

### <a name="atp-backward-demand-time-fence"></a><span data-ttu-id="8f416-167">الحد الزمني لطلب تراجع ATP</span><span class="sxs-lookup"><span data-stu-id="8f416-167">ATP backward demand time fence</span></span>

<span data-ttu-id="8f416-168">أدخل عدد الأيام، بدايةً من اليوم بشكل تنازلي، والذي سيتم فيه وضع الطلب المتأخر (لإصدارات المخزون) في الاعتبار عند حساب تواريخ التسليم المبكرة المتوفرة للمخزون.</span><span class="sxs-lookup"><span data-stu-id="8f416-168">Enter the number of days backward from today that past due demand (that is, inventory issues) will be considered when you are calculating the earliest available delivery dates for inventory.</span></span> <span data-ttu-id="8f416-169">على سبيل المثال، إذا أدخلت **0**، لا يتم وضع أي طلب متأخر في الاعتبار.</span><span class="sxs-lookup"><span data-stu-id="8f416-169">For example, if you enter **0**, no past due demand will be considered.</span></span> <span data-ttu-id="8f416-170">إذا أدخلت **1**، سيتم وضع طلب الأمس في الاعتبار.</span><span class="sxs-lookup"><span data-stu-id="8f416-170">If you enter **1**, yesterday's demand will be considered.</span></span>

### <a name="atp-backward-supply-time-fence"></a><span data-ttu-id="8f416-171">الحد الزمني لتوفير تراجع ATP</span><span class="sxs-lookup"><span data-stu-id="8f416-171">ATP backward supply time fence</span></span>

<span data-ttu-id="8f416-172">أدخل عدد الأيام، بدايةً من اليوم بشكل تنازلي، والذي سيتم فيه وضع التوريد المتأخر (لعمليات استلام المخزون) في الاعتبار عند حساب تواريخ التسليم المبكرة المتوفرة للمخزون.</span><span class="sxs-lookup"><span data-stu-id="8f416-172">Enter the number of days backward from today that past due supply (that is, inventory receipts) will be considered when you are calculating the earliest available delivery dates for inventory.</span></span> <span data-ttu-id="8f416-173">على سبيل المثال، إذا أدخلت **0**، لا يتم وضع أي توريد متأخر في الاعتبار.</span><span class="sxs-lookup"><span data-stu-id="8f416-173">For example, if you enter **0**, no past due supply will be considered.</span></span> <span data-ttu-id="8f416-174">أما إذا أدخلت **1**، يتم وضع توريد الأمس في الاعتبار.</span><span class="sxs-lookup"><span data-stu-id="8f416-174">If you enter **1**, yesterday's supply will be considered.</span></span>

### <a name="atp-delayed-demand-offset-time"></a><span data-ttu-id="8f416-175">الوقت المقابل للطلب المتأخر لـ ATP</span><span class="sxs-lookup"><span data-stu-id="8f416-175">ATP delayed demand offset time</span></span>

<span data-ttu-id="8f416-176">عدد الأيام المستقبلية بدءاً من اليوم الذي سيعتبر فيه أن الطلب المتأخر لإصدارات المخزون يشتمل على تاريخ التسليم الخاص به.</span><span class="sxs-lookup"><span data-stu-id="8f416-176">The number of days into the future from today when past due demand on inventory issues will be considered as having its delivery date.</span></span> <span data-ttu-id="8f416-177">على سبيل المثال، إذا أدخلت **0**، فستعتبر الأصناف المشتملة على تاريخ تسليم متأخر مسلمة اليوم.</span><span class="sxs-lookup"><span data-stu-id="8f416-177">For example, if you enter **0**, items with a past due delivery date will be considered as delivered today.</span></span> <span data-ttu-id="8f416-178">أما إذا أدخلت **1**، فستعتبر الأصناف المشتملة على تاريخ تسليم متأخر مسلمة غداً.</span><span class="sxs-lookup"><span data-stu-id="8f416-178">If you enter **1**, items with a past due delivery date will be considered as delivered tomorrow.</span></span>

### <a name="atp-delayed-supply-offset-time"></a><span data-ttu-id="8f416-179">الوقت المقابل للتوفير المتأخر لـ ATP</span><span class="sxs-lookup"><span data-stu-id="8f416-179">ATP delayed supply offset time</span></span>

<span data-ttu-id="8f416-180">عدد الأيام المستقبلية بدءاً من اليوم الذي ستعتبر فيه الأصناف في إيصالات استلام المخزون المتأخرة مستلمة.</span><span class="sxs-lookup"><span data-stu-id="8f416-180">The number of days into the future from today when items on past due inventory receipts will be considered as received.</span></span> <span data-ttu-id="8f416-181">على سبيل المثال، إذا أدخلت **0**، فسيتم اعتبار أن الصنف تم استلامه اليوم.</span><span class="sxs-lookup"><span data-stu-id="8f416-181">For example, if you enter **0**, the item will be considered as received today.</span></span> <span data-ttu-id="8f416-182">أما إذا أدخلت **1**، فسيتم اعتبار أن الصنف يتم استلامه غداً.</span><span class="sxs-lookup"><span data-stu-id="8f416-182">If you enter **1**, the item will be considered as received tomorrow.</span></span>

### <a name="atp-incl-planned-orders"></a><span data-ttu-id="8f416-183">ATP شاملاً</span><span class="sxs-lookup"><span data-stu-id="8f416-183">ATP incl.</span></span> <span data-ttu-id="8f416-184">الأوامر المخططة</span><span class="sxs-lookup"><span data-stu-id="8f416-184">planned orders</span></span>

<span data-ttu-id="8f416-185">يجب تضمين الأوامر المخططة في حسابات ATP إذا حددت طريقة حساب ATP في حقل **التحكم في تاريخ التسليم**.</span><span class="sxs-lookup"><span data-stu-id="8f416-185">Include planned orders in ATP calculations if you selected the ATP calculation method in the **Delivery date control** field.</span></span>

## <a name="atp-calculations"></a><span data-ttu-id="8f416-186">حسابات ATP</span><span class="sxs-lookup"><span data-stu-id="8f416-186">ATP calculations</span></span>

<span data-ttu-id="8f416-187">يتم حساب كمية ATP باستخدام طريقة "ATP تراكمي مع نظرة مستقبلية".</span><span class="sxs-lookup"><span data-stu-id="8f416-187">The ATP quantity is calculated by using the "cumulative ATP with look-ahead" method.</span></span> <span data-ttu-id="8f416-188">الفائدة الأساسية لطريقة حساب ATP هذه هي أنها يمكن أن تعالج حالات يكون فيها مجموع الإصدارات بين عمليات الاستلام أكبر من أحدث عملية استلام (على سبيل المثال، في حالة ضرورة استخدام كمية من عملية استلام سابقة لاستيفاء أحد المتطلبات).</span><span class="sxs-lookup"><span data-stu-id="8f416-188">The main advantage of this ATP calculation method is that it can handle cases where the sum of issues among receipts is more than the latest receipt (for example, when a quantity from an earlier receipt must be used to meet a requirement).</span></span>

<span data-ttu-id="8f416-189">تشمل طريقة الحساب "ATP تراكمي مع نظرة مستقبلية" جميع الإصدارات حتى تتجاوز الكمية التراكمية المطلوب تسلمها الكمية التراكمية المطلوب إصدارها.</span><span class="sxs-lookup"><span data-stu-id="8f416-189">The "cumulative ATP with look-ahead" calculation method includes all issues until the cumulative quantity to receive exceeds the cumulative quantity to issue.</span></span> <span data-ttu-id="8f416-190">وبالتالي، تقيّم طريقة حساب ATP إمكانية استخدام جزء من الكمية من فترة سابقة في فترة لاحقة.</span><span class="sxs-lookup"><span data-stu-id="8f416-190">Therefore, this ATP calculation method evaluates whether some of the quantity from an earlier period can be used in a later period.</span></span>

<span data-ttu-id="8f416-191">كمية ATP هي رصيد المخزون غير الملتزم به في الفترة الأولى.</span><span class="sxs-lookup"><span data-stu-id="8f416-191">The ATP quantity is the uncommitted inventory balance in the first period.</span></span> <span data-ttu-id="8f416-192">وعادة ما يتم حسابها لكل فترة تتم فيها جدولة عملية استلام.</span><span class="sxs-lookup"><span data-stu-id="8f416-192">Typically, it's calculated for each period in which a receipt is scheduled.</span></span> <span data-ttu-id="8f416-193">يحسب البرنامج فترة ATP بالأيام ويحسب التاريخ الحالي كأول تاريخ لكمية ATP.</span><span class="sxs-lookup"><span data-stu-id="8f416-193">The program calculates the ATP period in days and calculates the current date as the first date for the ATP quantity.</span></span> <span data-ttu-id="8f416-194">في الفترة الأولى، يشمل ATP المخزون الفعلي بدون أوامر العملاء التي حل موعد تسليمها أو فات.</span><span class="sxs-lookup"><span data-stu-id="8f416-194">In the first period, ATP includes on-hand inventory minus customer orders that are due and overdue.</span></span>

<span data-ttu-id="8f416-195">يتم حساب ATP باستخدام المعادلة التالية:</span><span class="sxs-lookup"><span data-stu-id="8f416-195">ATP is calculated by using the following formula:</span></span>

<span data-ttu-id="8f416-196">*ATP = ATP للفترة السابقة + عمليات الاستلام للفترة الحالية - الإصدارات للفترة الحالية - الكمية الصافية للإصدار لكل فترة مستقبلية إلى الفترة التي يتجاوز فيها مجموع عمليات الاستلام لجميع الفترات المستقبلية، إلى الفترة المستقبلية وبما في ذلك هذه الفترة نفسها، مجموع الإصدارات إلى الفترة المستقبلية وبما في ذلك هذه الفترة.*</span><span class="sxs-lookup"><span data-stu-id="8f416-196">*ATP = ATP for the previous period + Receipts for the current period - Issues for the current period - Net issue quantity for each future period until the period when the sum of receipts for all future periods, up to and including the future period, exceeds the sum of issues up to and including the future period.*</span></span>

<span data-ttu-id="8f416-197">عندما لا تتوفّر إصدارات أو عمليات استلام لوضعها في الاعتبار، تعتبر كمية ATP للتواريخ التالية كأحدث كمية ATP محتسبة.</span><span class="sxs-lookup"><span data-stu-id="8f416-197">When no more issues or receipts are left to consider, the ATP quantity for the following dates is the same as the latest calculated ATP quantity.</span></span>

<span data-ttu-id="8f416-198">إذا لم يتم توفير جميع الأبعاد المستخدمة لأحد الأصناف عند اكتمال فحص ATP، فلا يزال بالإمكان تحديدها في الإصدار وعمليات الاستلام.</span><span class="sxs-lookup"><span data-stu-id="8f416-198">If not all the dimensions that are used for an item are given when the ATP check is completed, they can still be specified on the issue and receipts.</span></span> <span data-ttu-id="8f416-199">في هذه الحالة، في حساب ATP، يجب تجميع عمليات الاستلام والإصدارات في الأبعاد الحالية للحد من عدد بنود الاستلام والإصدار المستخدمة في حساب ATP.</span><span class="sxs-lookup"><span data-stu-id="8f416-199">In this case, in the ATP calculation, the receipts and issues must be aggregated to the existing dimensions to reduce the number of receipt and issue lines that are used in the ATP calculation.</span></span>

<span data-ttu-id="8f416-200">كمية ATP المعروضة دائماً أكبر من أو تساوي 0 (صفر).</span><span class="sxs-lookup"><span data-stu-id="8f416-200">The ATP quantity that is shown is always greater than or equal to 0 (zero).</span></span> <span data-ttu-id="8f416-201">إذا كان ناتج العملية الحسابية كمية ATP سلبية (على سبيل المثال، إذا كانت الكمية التي تم التعهد بها سابقاً تتجاوز الكمية المتوفرة)، يعيّن البرنامج الكمية تلقائياً على **0**.</span><span class="sxs-lookup"><span data-stu-id="8f416-201">If the calculation returns a negative ATP quantity (for example, if the quantity that was previously promised exceeds the available quantity), the program automatically sets the quantity to **0**.</span></span>

<span data-ttu-id="8f416-202">يتحكم حقل **‏‫الحد الزمني لطلب تراجع ATP‬** في طول الفترة السابقة التي يبحث فيها عن أوامر الطلب أو إصدارات المخزون المتأخرة.</span><span class="sxs-lookup"><span data-stu-id="8f416-202">The **ATP backward demand time fence** field controls how far back in time to look for delayed demand orders or inventory issues.</span></span>

<span data-ttu-id="8f416-203">يتحكم حقل **‏‫‏الحد الزمني لتوفير تراجع ATP‬** ‏‎في طول الفترة السابقة التي يتم البحث فيها عن أوامر التوريد أو عمليات استلام المخزون المتأخرة.</span><span class="sxs-lookup"><span data-stu-id="8f416-203">The **ATP backward supply time fence** field controls how far back in time to look for delayed supply orders or inventory receipts.</span></span> <span data-ttu-id="8f416-204">على سبيل المثال، في حالة وضع الأوامر المتأخرة بمقدار سبعة أيام فقط في الاعتبار في حساب ATP، يجب تعيين الحقلين على **7**.</span><span class="sxs-lookup"><span data-stu-id="8f416-204">For example, if orders that are delayed by only seven days should be considered in the ATP calculation, both fields should be set to **7**.</span></span>

<span data-ttu-id="8f416-205">يتحكم الحقلان **‏الوقت المقابل للطلب المتأخر لـ ATP** وأيضاً **‏الوقت المقابل للتوفير المتأخر لـ ATP‬** في حالات وضع الطلب أو التوريد المتأخر في الاعتبار في حساب ATP.</span><span class="sxs-lookup"><span data-stu-id="8f416-205">The **ATP delayed demand offset time** and **ATP delayed supply offset time** fields control when the delayed demand or supply will be considered in the ATP calculation.</span></span> <span data-ttu-id="8f416-206">على سبيل المثال، في حالة وضع التوريد والطلب المتأخرَين في الاعتبار في حساب ATP بعد غد، يجب تعيين الحقلين على **2**.</span><span class="sxs-lookup"><span data-stu-id="8f416-206">For example, if the delayed supply and demand should be considered in the ATP calculation the day after tomorrow, both fields should be set to **2**.</span></span> <span data-ttu-id="8f416-207">القيمة **2** تعني أن كمية أحد الأصناف في أمر شراء متأخر التي يجب وضعها في الاعتبار في حساب ATP سيتم عرضها كمتوفرة بعد يومين من التاريخ الحالي.</span><span class="sxs-lookup"><span data-stu-id="8f416-207">A value of **2** means that the quantity of an item on a delayed purchase order that should be considered in the ATP calculation will be shown as available two days after the current date.</span></span>
