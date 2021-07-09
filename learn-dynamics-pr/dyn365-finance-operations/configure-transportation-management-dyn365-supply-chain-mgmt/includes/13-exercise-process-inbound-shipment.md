---
ms.openlocfilehash: db045fce453e5ccd374db8e909de3bb75c5761bf
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6073865"
---

## <a name="scenario"></a><span data-ttu-id="80972-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="80972-101">Scenario</span></span>

<span data-ttu-id="80972-102">في هذا المعمل، ستقوم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="80972-102">In this lab you will:</span></span>

- <span data-ttu-id="80972-103">إنشاء موزّع وخطة توجيه ودليل توجيه</span><span class="sxs-lookup"><span data-stu-id="80972-103">Create a hub, route plan, and route guide</span></span> 
- <span data-ttu-id="80972-104">بدء شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-104">Initiate an inbound shipment</span></span> 
- <span data-ttu-id="80972-105">معالجة شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-105">Process an inbound shipment</span></span> 
- <span data-ttu-id="80972-106">تأكيد شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-106">Confirm an inbound shipment</span></span> 

## <a name="prerequisite-steps"></a><span data-ttu-id="80972-107">خطوات المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="80972-107">Prerequisite steps</span></span> 

### <a name="add-a-vendor-address-for-the-ade-supply-company"></a><span data-ttu-id="80972-108">إضافة عنوان مورد لشركة Ade Supply</span><span class="sxs-lookup"><span data-stu-id="80972-108">Add a vendor address for the Ade Supply company</span></span>

1.  <span data-ttu-id="80972-109">في شركة **USMF**، افتح **الحسابات الدائنة > الموردين > كافة الموردين**.</span><span class="sxs-lookup"><span data-stu-id="80972-109">In company **USMF**, open **Accounts payable > Vendors > All vendors**.</span></span>
2.  <span data-ttu-id="80972-110">حدد المورد **1003** من قائمة الموردين.</span><span class="sxs-lookup"><span data-stu-id="80972-110">Select vendor **1003** from the list of vendors.</span></span>
3.  <span data-ttu-id="80972-111">في جزء الإجراء، حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="80972-111">On the Action Pane, select **Edit**.</span></span>
4.  <span data-ttu-id="80972-112">في علامة التبويب السريعة **العناوين**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="80972-112">In the **Addresses** FastTab, select **Add**.</span></span>
5.  <span data-ttu-id="80972-113">في الحقل **الاسم أو الوصف**، أدخل **الموقع الرئيسي لشركة Ade Supply**.</span><span class="sxs-lookup"><span data-stu-id="80972-113">In the **Name or description** field, enter **Ade Supply main location**.</span></span>
6.  <span data-ttu-id="80972-114">في حقل **الرمز البريدي**، أدخل **00210**.</span><span class="sxs-lookup"><span data-stu-id="80972-114">In the **Zip/postal code** field, enter **00210**.</span></span>
7.  <span data-ttu-id="80972-115">في حقل **الشارع**، أدخل **123 Main Street**.</span><span class="sxs-lookup"><span data-stu-id="80972-115">In the **Street** field, enter **123 Main Street**.</span></span>
8.  <span data-ttu-id="80972-116">قم بتعيين شريط التمرير **أساسي‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="80972-116">Set the **Primary** slider to **Yes**.</span></span>
9.  <span data-ttu-id="80972-117">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="80972-117">Select **OK**.</span></span>
10. <span data-ttu-id="80972-118">في علامة التبويب السريعة **الفاتورة والتسليم**، في الحقل **وضع التسليم**، حدد **Parce-STD**.</span><span class="sxs-lookup"><span data-stu-id="80972-118">In the **Invoice and delivery** FastTab, in the **Mode of delivery** field, select **Parce-STD**.</span></span>
11. <span data-ttu-id="80972-119">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="80972-119">Close the pages.</span></span>

### <a name="modify-the-cfr-terms-of-delivery"></a><span data-ttu-id="80972-120">تعديل شروط التسليم الخاصة بـ CFR</span><span class="sxs-lookup"><span data-stu-id="80972-120">Modify the CFR terms of delivery</span></span>

1.  <span data-ttu-id="80972-121">افتح **الحسابات الدائنة > إعداد > شروط التسليم**.</span><span class="sxs-lookup"><span data-stu-id="80972-121">Open **Accounts payable > Setup > Terms of delivery**.</span></span>
2.  <span data-ttu-id="80972-122">حدد **CFR** من الجانب الأيمن.</span><span class="sxs-lookup"><span data-stu-id="80972-122">Select **CFR** from the left-hand panel.</span></span>
3.  <span data-ttu-id="80972-123">حدد **تحرير** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="80972-123">Select **Edit** on the Action Pane.</span></span>
4.  <span data-ttu-id="80972-124">في علامة التبويب السريعة **النقل**، قم بتعيين شريط التمرير **إضافة مصاريف النقل إلى أوامر مبيعات البيع بالتجزئة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="80972-124">In the **Transportation** FastTab, set the **Add transportation charges to retail sales orders** slider to **Yes**.</span></span>
5.  <span data-ttu-id="80972-125">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="80972-125">Close the page.</span></span>

## <a name="create-a-hub-route-plan-and-route-guide"></a><span data-ttu-id="80972-126">إنشاء موزّع وخطة توجيه ودليل توجيه</span><span class="sxs-lookup"><span data-stu-id="80972-126">Create a hub, route plan, and route guide</span></span> 

<span data-ttu-id="80972-127">لقد طُلب منك إنشاء موزّع لشركة Ade Supply وإنشاء خطة توجيه ودليل توجيه بين شركة Ade Supply ومستودع USMF 61.</span><span class="sxs-lookup"><span data-stu-id="80972-127">You have been asked to set up a hub for the Ade Supply company and create a route plan and guide between the Ade Supply company and USMF's warehouse 61.</span></span>

### <a name="create-a-hub-for-the-ade-supply-company"></a><span data-ttu-id="80972-128">إنشاء موزّع لشركة Ade Supply</span><span class="sxs-lookup"><span data-stu-id="80972-128">Create a hub for the Ade Supply company</span></span>

1.  <span data-ttu-id="80972-129">افتح **إدارة النقل > إعداد > التوجيه > أصول الموزّعات**.</span><span class="sxs-lookup"><span data-stu-id="80972-129">Open **Transportation management > Setup > Routing > Hub masters**.</span></span>
2.  <span data-ttu-id="80972-130">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="80972-130">Select **New** on the Action Pane.</span></span>
3.  <span data-ttu-id="80972-131">في الحقل **الموزّع**، أدخل **Ade Supply**.</span><span class="sxs-lookup"><span data-stu-id="80972-131">In the **Hub** field, enter **Ade Supply**.</span></span>
4.  <span data-ttu-id="80972-132">في الحقل **الاسم**، أدخل **Ade Supply NH**.</span><span class="sxs-lookup"><span data-stu-id="80972-132">In the **Name** field, enter **Ade Supply NH**.</span></span>
5.  <span data-ttu-id="80972-133">في علامة التبويب السريعة **الرموز**، في الحقل **انوع الموزّع**، حدد **موزّع**.</span><span class="sxs-lookup"><span data-stu-id="80972-133">In the **Codes** FastTab, in the **Hub type** field, select **Hub**.</span></span>
6.  <span data-ttu-id="80972-134">في حقل **السعر الرئيسي**، حدد **ParcelRateMaster**.</span><span class="sxs-lookup"><span data-stu-id="80972-134">In the **Rate master** field, select **ParcelRateMaster**.</span></span>
7.  <span data-ttu-id="80972-135">في علامة التبويب السريعة **العنوان**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="80972-135">In the **Address** FastTab, select **Add**.</span></span>
8.  <span data-ttu-id="80972-136">في صفحة **عنوان جديد**، أدخل **Ade Supply NH** في حقل **الاسم أو الوصف**.</span><span class="sxs-lookup"><span data-stu-id="80972-136">On the **New address** page, in the **Name or description** field, enter **Ade Supply NH**.</span></span>
9.  <span data-ttu-id="80972-137">في حقل **الرمز البريدي**، أدخل **00210**.</span><span class="sxs-lookup"><span data-stu-id="80972-137">In the **ZIP/postal code** field, enter **00210**.</span></span>
10. <span data-ttu-id="80972-138">في حقل **الشارع**، أدخل **123 Main Street**.</span><span class="sxs-lookup"><span data-stu-id="80972-138">In the **Street** field, enter **123 Main Street**.</span></span>
11. <span data-ttu-id="80972-139">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="80972-139">Select **OK**.</span></span>
12. <span data-ttu-id="80972-140">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="80972-140">Close the page.</span></span>

### <a name="create-a-route-plan-from-new-hampshire-to-washington"></a><span data-ttu-id="80972-141">إنشاء خطة طريق من نيوهامشير إلى واشنطن</span><span class="sxs-lookup"><span data-stu-id="80972-141">Create a route plan from New Hampshire to Washington</span></span>

1.  <span data-ttu-id="80972-142">افتح **إدارة النقل > إعداد > التوجيه > خطط التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="80972-142">Open **Transportation management > Setup > Routing > Route plans**.</span></span>
2.  <span data-ttu-id="80972-143">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="80972-143">Select **New** on the Action Pane.</span></span>
3.  <span data-ttu-id="80972-144">في الحقل **خطة التوجيه**، أدخل **NH إلى WA**.</span><span class="sxs-lookup"><span data-stu-id="80972-144">In the **Route plan** field, enter **NH to WA**.</span></span>
4.  <span data-ttu-id="80972-145">في الحقل **الاسم**، أدخل **نيوهامشير إلى واشنطن**.</span><span class="sxs-lookup"><span data-stu-id="80972-145">In the **Name** field, enter **New Hampshire to Washington**.</span></span>
5.  <span data-ttu-id="80972-146">من علامة التبويب السريعة **التفاصيل**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="80972-146">In the **Details** FastTab, select **New**.</span></span>
6.  <span data-ttu-id="80972-147">في الحقل **الموزّع الأصلي**، حدد **Ade Supply**.</span><span class="sxs-lookup"><span data-stu-id="80972-147">In the **Origin hub** field, select **Ade Supply**.</span></span>
7.  <span data-ttu-id="80972-148">في الحقل **الموزّع الوجهة**، حدد **Own WHS**.</span><span class="sxs-lookup"><span data-stu-id="80972-148">In the **Destination hub** field, select **Own WHS**.</span></span>
8.  <span data-ttu-id="80972-149">في حقل **شركة الشحن**، حدد **ParcelCarrier**.</span><span class="sxs-lookup"><span data-stu-id="80972-149">In the **Shipping carrier** field, select **ParcelCarrier**.</span></span>
9.  <span data-ttu-id="80972-150">في حقل **خدمة النقل**، حدد **STD**.</span><span class="sxs-lookup"><span data-stu-id="80972-150">In the **Carrier service** field, select **STD**.</span></span>
10. <span data-ttu-id="80972-151">في الحقل **المورد**، حدد **1003**.</span><span class="sxs-lookup"><span data-stu-id="80972-151">In the **Vendor** field, select **1003**.</span></span>
11. <span data-ttu-id="80972-152">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="80972-152">Close the page.</span></span>

### <a name="create-a-route-guide-from-new-hampshire-to-washington"></a><span data-ttu-id="80972-153">إنشاء دليل توجيه من نيوهامشير إلى واشنطن</span><span class="sxs-lookup"><span data-stu-id="80972-153">Create a route guide from New Hampshire to Washington</span></span>

1.  <span data-ttu-id="80972-154">افتح **إدارة النقل > إعداد > التوجيه > دلائل التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="80972-154">Open **Transportation management > Setup > Routing > Route guides**.</span></span>
2.  <span data-ttu-id="80972-155">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="80972-155">Select **New** on the Action Pane.</span></span>
3.  <span data-ttu-id="80972-156">في الحقل **دليل التوجيه**، أدخل **NH إلى WA**.</span><span class="sxs-lookup"><span data-stu-id="80972-156">In the **Routing guide** field, enter **NH to WA**.</span></span>
4.  <span data-ttu-id="80972-157">في الحقل **الاسم**، أدخل **نيوهامشير إلى واشنطن**.</span><span class="sxs-lookup"><span data-stu-id="80972-157">In the **Name** field, enter **New Hampshire to Washington**.</span></span>
5.  <span data-ttu-id="80972-158">في علامة التبويب السريعة **المنشأ‬**، في الحقل **الرمز البريدي**، أدخل **00210**.</span><span class="sxs-lookup"><span data-stu-id="80972-158">In the **Origin** FastTab, in the **ZIP/postal code** field, enter **00210**.</span></span>
6.  <span data-ttu-id="80972-159">في علامة التبويب السريعة **الوجهة**، في الحقل **الرمز البريدي**، أدخل **98052**.</span><span class="sxs-lookup"><span data-stu-id="80972-159">In the **Destination** FastTab, in the **ZIP/postal code to** field, enter **98052**.</span></span>
7.  <span data-ttu-id="80972-160">في علامة التبويب السريعة **النتيجة**، في الحقل **خطة التوجيه**، حدد **NH إلى WA**.</span><span class="sxs-lookup"><span data-stu-id="80972-160">In the **Result** FastTab, in the **Route plan** field, select **NH to WA**.</span></span>
8.  <span data-ttu-id="80972-161">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="80972-161">Close the page.</span></span>

## <a name="initiate-an-inbound-shipment"></a><span data-ttu-id="80972-162">بدء شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-162">Initiate an inbound shipment</span></span> 

<span data-ttu-id="80972-163">تمت مطالبتك بإنشاء أمر شراء جديد لعدد 10 مكبرات الصوت المصغرة إلى من شركة Ade Supply.</span><span class="sxs-lookup"><span data-stu-id="80972-163">You have been asked to create a new purchase order for 10 mini-speakers from the Ade Supply company.</span></span> <span data-ttu-id="80972-164">بعد إنشاء أمر الشراء، ستحتاج إلى إنشاء شحنة واردة ثم تصنيف المتجر للتحميل الداخلي للعثور على معدل النقل الأوفر سعراً.</span><span class="sxs-lookup"><span data-stu-id="80972-164">After creating the purchase order, you will need to create an inbound shipment and then rate shop for the inbound load to find the cheapest transportation rate.</span></span>

### <a name="create-a-new-purchase-order"></a><span data-ttu-id="80972-165">إنشاء أمر شراء جديد</span><span class="sxs-lookup"><span data-stu-id="80972-165">Create a new purchase order</span></span>

1.  <span data-ttu-id="80972-166">افتح **الحسابات الدائنة > أوامر الشراء > كافة أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="80972-166">Open **Accounts payable > Purchase orders > All purchase orders**.</span></span>
2.  <span data-ttu-id="80972-167">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="80972-167">Select **New** on the Action Pane.</span></span>
3.  <span data-ttu-id="80972-168">في الصفحة **إنشاء أمر شراء**، في الحقل **حساب المورد**، حدد **1003**.</span><span class="sxs-lookup"><span data-stu-id="80972-168">On the **Create purchase order** page, in the **Vendor account** field, select **1003**.</span></span>
4.  <span data-ttu-id="80972-169">في علامة التبويب السريعة **عام**، حدد **6** في حقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="80972-169">In the **General** FastTab, in the **Site** field, select **6**.</span></span>
5.  <span data-ttu-id="80972-170">حدد **61** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="80972-170">In the **Warehouse** field, select **61**.</span></span>
6.  <span data-ttu-id="80972-171">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="80972-171">Select **OK**.</span></span>
7.  <span data-ttu-id="80972-172">تحت علامة التبويب السريعة **بنود أمر الشراء**، في حقل **رقم الصنف**، حدد **L0101**.</span><span class="sxs-lookup"><span data-stu-id="80972-172">In the **Purchase order lines** FastTab, in the **Item number** field, enter **L0101**.</span></span>
8.  <span data-ttu-id="80972-173">في حقل **الكمية**، أدخِل **10**.</span><span class="sxs-lookup"><span data-stu-id="80972-173">In the **Quantity** field, enter **10**.</span></span>
9.  <span data-ttu-id="80972-174">في حقل **سعر الوحدة**، أدخِل **50**.</span><span class="sxs-lookup"><span data-stu-id="80972-174">In the **Unit price** field, enter **50**.</span></span>
10. <span data-ttu-id="80972-175">في علامة التبويب **شراء** في جزء الإجراء، حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="80972-175">In the **Purchase** tab on the Action Pane, select **Confirm**.</span></span>
11. <span data-ttu-id="80972-176">حدد **موافق** في النافذة المنبثقة التي تظهر.</span><span class="sxs-lookup"><span data-stu-id="80972-176">Select **OK** in the pop-up window that appears.</span></span>

### <a name="create-an-inbound-shipment"></a><span data-ttu-id="80972-177">إنشاء شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-177">Create an inbound shipment</span></span>

1.  <span data-ttu-id="80972-178">في علامة التبويب **المستودع** في جزء الإجراء، حدد **منضدة عمل تخطيط التحميل**.</span><span class="sxs-lookup"><span data-stu-id="80972-178">On the **Warehouse** tab on the Action Pane, select **Load planning workbench**.</span></span>
2.  <span data-ttu-id="80972-179">حدد عمود علامة الاختيار لبند أمر الشراء الذي قمت بإنشائه للتو.</span><span class="sxs-lookup"><span data-stu-id="80972-179">Select the check mark column for the purchase order line that you just created.</span></span>
3.  <span data-ttu-id="80972-180">في علامة التبويب **العرض والطلب** في جزء الإجراء، حدد **إلى تحميل جديد‬**.</span><span class="sxs-lookup"><span data-stu-id="80972-180">On the **Supply and demand** tab on the Action Pane, select **To new load**.</span></span>
4.  <span data-ttu-id="80972-181">في الصفحة **مهمة قالب التحميل**، في الحقل **معرّف قالب التحميل**، حدد **قالب تحميل Stnd**.</span><span class="sxs-lookup"><span data-stu-id="80972-181">On the **Load template assignment** page, in the **Load template ID** field, select **Stnd Load template**.</span></span>
5.  <span data-ttu-id="80972-182">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="80972-182">Select **OK**.</span></span>

### <a name="set-up-the-rate-shop-for-the-inbound-load"></a><span data-ttu-id="80972-183">إعداد متجر الأسعار للتحميل الوارد</span><span class="sxs-lookup"><span data-stu-id="80972-183">Set up the rate shop for the inbound load</span></span>

1.  <span data-ttu-id="80972-184">في علامة التبويب **التحميلات** من **‬‏‫منضدة عمل تخطيط التحميل**، حدد **منضدة عمل الأسعار والمسارات** من القائمة المنسدلة **الأسعار والمسارات**.</span><span class="sxs-lookup"><span data-stu-id="80972-184">On the **Loads** tab of the **Load planning workbench**, select **Rate route workbench** from the **Rating and routing** drop-down menu.</span></span>
2.  <span data-ttu-id="80972-185">في جزء الإجراءات **منضدة عمل الأسعار والمسارات**، حدد **سعر التسوق**.</span><span class="sxs-lookup"><span data-stu-id="80972-185">On the Action Pane of the **Rate route workbench**, select **Rate shop**.</span></span>
3.  <span data-ttu-id="80972-186">من علامة التبويب السريعة **نتائج المسار**، قم بإلغاء تحديد خانة الاختيار **إخفاء الاستثناءات**.</span><span class="sxs-lookup"><span data-stu-id="80972-186">On the **Route results** FastTab, clear the **Hide exceptions** check box.</span></span>
4.  <span data-ttu-id="80972-187">في جزء الإجراء، حدد **المسار مع السعر**.</span><span class="sxs-lookup"><span data-stu-id="80972-187">On the Action Pane, select **Route with rate**.</span></span>
5.  <span data-ttu-id="80972-188">حدد **نتيجة المسار** للبند **Wh 61 to Cust 003 004 019** لدليل التوجيه.</span><span class="sxs-lookup"><span data-stu-id="80972-188">Select the **Route result** for the **Wh 61 to Cust 003 004 019** line for the route guide.</span></span>
5.  <span data-ttu-id="80972-189">حدد **تعيين**.</span><span class="sxs-lookup"><span data-stu-id="80972-189">Select **Assign**.</span></span>

## <a name="process-an-inbound-shipment"></a><span data-ttu-id="80972-190">معالجة شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-190">Process an inbound shipment</span></span> 

<span data-ttu-id="80972-191">والآن بعد إنشاء الشحنة الواردة وتصنيفها، يجب جدولة موعد لشحنة مكبرات الصوت المصغرة.</span><span class="sxs-lookup"><span data-stu-id="80972-191">Now that the inbound shipment has been created and rated, you need to schedule an appointment for the mini-speaker shipment.</span></span> <span data-ttu-id="80972-192">قد تم مطالبتك بتسجيل موعد بدء السائق Tim Smith وإنهائه.</span><span class="sxs-lookup"><span data-stu-id="80972-192">You've also been asked to check the driver, Tim Smith, in and out of the appointment.</span></span>

### <a name="schedule-an-appointment"></a><span data-ttu-id="80972-193">جدولة موعد</span><span class="sxs-lookup"><span data-stu-id="80972-193">Schedule an appointment</span></span> 

1.  <span data-ttu-id="80972-194">افتح **إدارة النقل > تخطيط > التحميلات > كافة التحميلات**.</span><span class="sxs-lookup"><span data-stu-id="80972-194">Open **Transportation management > Planning > Loads > All loads**.</span></span>
2.  <span data-ttu-id="80972-195">في علامة التبويب **التحميلات**، حدد معرّف التحميل لأمر الشراء الذي قمت بإنشائه سابقاً.</span><span class="sxs-lookup"><span data-stu-id="80972-195">On the **Loads** tab, select the load ID for the purchase order that you created earlier.</span></span>
3.  <span data-ttu-id="80972-196">حدد **جدولة المواعيد** من القائمة المنسدلة **نقل**.</span><span class="sxs-lookup"><span data-stu-id="80972-196">Select **Appointment scheduling** from the **Transportation** drop-down menu.</span></span>
4.  <span data-ttu-id="80972-197">في الصفحة **جدولة المواعيد**، حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="80972-197">On the **Appointment scheduling** page, select **New** on the Action Pane.</span></span>
5.  <span data-ttu-id="80972-198">في علامة التبويب السريعة **تفاصيل الموعد**، في الحقل **قاعدة الموعد**، حدد **المساحات الداخلية 61**.</span><span class="sxs-lookup"><span data-stu-id="80972-198">On the **Appointment details** FastTab, in the **Appointment rule** field, select **Inbound docks 61**.</span></span>
6.  <span data-ttu-id="80972-199">في جزء الإجراء، حدد القائمة المنسدلة **حالة التحديث** ثم حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="80972-199">On the Action Pane, select the **Update status** drop-down menu and then select **Firm**.</span></span> <span data-ttu-id="80972-200">قد تحتاج إلى تحديث الصفحة لتمكين خيار **حالة التحديث**.</span><span class="sxs-lookup"><span data-stu-id="80972-200">You may have to refresh the page to enable the **Update status** option.</span></span> <span data-ttu-id="80972-201">إذا كانت القائمة **حالة التحديث** ما زالت معطلة، فقم بالرجوع إلى الصفحة السابقة وإعادة تحديد **جدولة المواعيد** من القائمة المنسدلة **النقل** ثم قم بتحديد **تأكيد** من القائمة المنسدلة **حالة التحديث**.</span><span class="sxs-lookup"><span data-stu-id="80972-201">If the **Update status** menu is still disabled, go back to the previous page and reselect **Appointment scheduling** from the **Transportation** drop-down menu and then select **Firm** from the **Update status** drop-down menu.</span></span> 
  

### <a name="check-in-the-driver"></a><span data-ttu-id="80972-202">تسجيل وصول السائق</span><span class="sxs-lookup"><span data-stu-id="80972-202">Check in the driver</span></span>

1.  <span data-ttu-id="80972-203">في جزء الإجراء، حدد مفتاح السهم لأسفل **حالة التحديث** ثم حدد **تسجيل وصول السائق**.</span><span class="sxs-lookup"><span data-stu-id="80972-203">On the Action Pane, select the **Update status** drop-down arrow and then select **Driver check-in**.</span></span>
2.  <span data-ttu-id="80972-204">في الصفحة **تفاصيل تسجيل وصول السائق**، في الحقل **اسم السائق**، أدخل **Tim Smith**.</span><span class="sxs-lookup"><span data-stu-id="80972-204">On the **Driver check-in details** page, in the **Driver name** field, enter **Tim Smith**.</span></span>
3.  <span data-ttu-id="80972-205">في الحقل **رخصة السائق**، أدخل **123**.</span><span class="sxs-lookup"><span data-stu-id="80972-205">In the **Driver license** field, enter **123**.</span></span>
4.  <span data-ttu-id="80972-206">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="80972-206">Select **OK**.</span></span>
5.  <span data-ttu-id="80972-207">قم بإغلاق الصفحة **جدولة المواعيد**.</span><span class="sxs-lookup"><span data-stu-id="80972-207">Close the **Appointment scheduling** page.</span></span>

### <a name="check-out-the-driver"></a><span data-ttu-id="80972-208">تسجيل انتهاء السائق</span><span class="sxs-lookup"><span data-stu-id="80972-208">Check out the driver</span></span>

1.  <span data-ttu-id="80972-209">في علامة التبويب **النقل**، ضمن القسم **المواعيد**، حدد **جدولة المواعيد**.</span><span class="sxs-lookup"><span data-stu-id="80972-209">On the **Transportation** tab, under the **APPOINTMENTS** section, select **Appointment scheduling**.</span></span>
2.  <span data-ttu-id="80972-210">في جزء الإجراء، حدد القائمة المنسدلة **حالة التحديث** ثم حدد **تسجيل انتهاء السائق**.</span><span class="sxs-lookup"><span data-stu-id="80972-210">On the Action Pane, select the **Update status** drop-down arrow and select **Driver check-out**.</span></span>
3.  <span data-ttu-id="80972-211">في الصفحة **معلومات السائق**، حدد **موافق** لقبول المعلومات الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="80972-211">On **The driver's information** page, select **OK** to accept the default information.</span></span>
4.  <span data-ttu-id="80972-212">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="80972-212">Close the page.</span></span>

## <a name="confirm-an-inbound-shipment"></a><span data-ttu-id="80972-213">تأكيد شحنة واردة</span><span class="sxs-lookup"><span data-stu-id="80972-213">Confirm an inbound shipment</span></span> 

<span data-ttu-id="80972-214">تحتاج الآن إلى تأكيد الشحنة الواردة.</span><span class="sxs-lookup"><span data-stu-id="80972-214">You now need to confirm the inbound shipment.</span></span>

1.  <span data-ttu-id="80972-215">افتح **إدارة النقل > تخطيط > التحميلات > كافة التحميلات**.</span><span class="sxs-lookup"><span data-stu-id="80972-215">Open **Transportation management > Planning > Loads > All loads**.</span></span>
3.  <span data-ttu-id="80972-216">حدد **معرّف التحميل** الخاص بالتحميل.</span><span class="sxs-lookup"><span data-stu-id="80972-216">Select the **Load ID** of the load.</span></span>
4.  <span data-ttu-id="80972-217">في الصفحة **تفاصيل التحميل**، حدد علامة التبويب **الشحن والاستلام** في جزء الإجراء، ثم حدد **الشحنة الواردة** في منطقة **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="80972-217">In the **Load details** page, select the **Ship and receive** tab on the Action Pane, and then select **Inbound shipment** in the **Confirm** area.</span></span>
5.  <span data-ttu-id="80972-218">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="80972-218">Close the page.</span></span>

