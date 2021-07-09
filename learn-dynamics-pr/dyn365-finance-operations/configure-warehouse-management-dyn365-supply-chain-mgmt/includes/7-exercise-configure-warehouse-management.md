---
ms.openlocfilehash: b8d75a82bb07c99a3cd01386ada533eeebd07bbb
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073169"
---
## <a name="scenario"></a><span data-ttu-id="79646-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="79646-101">Scenario</span></span> 
<span data-ttu-id="79646-102">بصفتك مدير المستودع في USMF، فأنت بحاجة إلى تكوين عناصر إدارة المستودعات.</span><span class="sxs-lookup"><span data-stu-id="79646-102">As the warehouse manager in USMF, you need to configure the warehouse management elements.</span></span>

## <a name="create-a-storage-dimension-group"></a><span data-ttu-id="79646-103">إنشاء مجموعة أبعاد التخزين</span><span class="sxs-lookup"><span data-stu-id="79646-103">Create a storage dimension group</span></span> 

<span data-ttu-id="79646-104">بصفتك مدير مستودع في USMF، فأنت بحاجة إلى إنشاء مجموعة أبعاد تخزين جديدة لاستخدامها مع إدارة المستودعات.</span><span class="sxs-lookup"><span data-stu-id="79646-104">As a warehouse manager in USMF, you need to create a new storage dimension group to use with warehouse management.</span></span>

1.  <span data-ttu-id="79646-105">في شركة **USMF**، انتقل إلى **إدارة معلومات المنتج > الإعداد > مجموعات الأبعاد والمتغيرات > مجموعات أبعاد التخزين**.</span><span class="sxs-lookup"><span data-stu-id="79646-105">In company **USMF**, go to **Product information management > Setup > Dimension and variant groups > Storage dimension groups**.</span></span>
2.  <span data-ttu-id="79646-106">حدد **جديد** في جزء الإجراء لإنشاء مجموعة أبعاد التخزين الجديدة.</span><span class="sxs-lookup"><span data-stu-id="79646-106">Select **New** in the Action Pane to create a new storage dimension group.</span></span>
3.  <span data-ttu-id="79646-107">اكتب **LASD** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="79646-107">Type **LASD** in the **Name** field.</span></span>
4.  <span data-ttu-id="79646-108">اكتب **أبعاد التخزين في لوس أنجلوس** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="79646-108">Type **Los Angeles storage dimension** in the **Description** field.</span></span>
5.  <span data-ttu-id="79646-109">قم بتمكين خيار **استخدام عمليات إدارة المستودعات** لتمكين إدارة المستودعات في علامة التبويب السريعة **الإعداد الخاص بالمستودع**.</span><span class="sxs-lookup"><span data-stu-id="79646-109">Enable the **Use warehouse management processes** option to enable warehouse management in the **Warehouse specific setup** FastTab.</span></span>
6.  <span data-ttu-id="79646-110">حدد **حفظ** في جزء الإجراء، وتحقق من أن أبعاد **الموقع**، و **المستودع**، و **الموقع**، و **حالة المخزون**، و **لوحة الترخيص** نشطة.</span><span class="sxs-lookup"><span data-stu-id="79646-110">Select **Save** in the Action Pane and verify that the **Site**, **Warehouse**, **Location**, **Inventory status**, and **License plate** dimensions are active.</span></span>
7.  <span data-ttu-id="79646-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79646-111">Close the page.</span></span>

## <a name="create-a-tracking-dimension-group"></a><span data-ttu-id="79646-112">إنشاء مجموعة أبعاد التعقب</span><span class="sxs-lookup"><span data-stu-id="79646-112">Create a tracking dimension group</span></span> 

<span data-ttu-id="79646-113">بصفتك مدير مستودع في USMF، أنت بحاجة إلى إنشاء مجموعة أبعاد تعقب جديدة لن تتعقب الأرقام التسلسلية أو أرقام الدُفعات.</span><span class="sxs-lookup"><span data-stu-id="79646-113">As a warehouse manager in USMF, you need to create a new tracking dimension group that will not track serial numbers or batch numbers.</span></span>

1.  <span data-ttu-id="79646-114">افتح **إدارة معلومات المنتج > الإعداد > مجموعات الأبعاد والمتغيرات > مجموعات أبعاد التعقب**.</span><span class="sxs-lookup"><span data-stu-id="79646-114">Open **Product information management > Setup > Dimension and variant groups > Tracking dimension groups**.</span></span>
2.  <span data-ttu-id="79646-115">حدد **جديد** في جزء الإجراء لإنشاء مجموعة أبعاد تعقب جديدة.</span><span class="sxs-lookup"><span data-stu-id="79646-115">Select **New** in the Action Pane to create a new Tracking dimension group.</span></span>
3.  <span data-ttu-id="79646-116">اكتب **LABT** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="79646-116">Type **LABT** in the **Name** field.</span></span>
4.  <span data-ttu-id="79646-117">اكتب **تعقب الدُفعات في لوس أنجلوس** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="79646-117">Type **Los Angeles batch tracking** in the **Description** field.</span></span>
5.  <span data-ttu-id="79646-118">تأكد من تحديد **لا شيء** في حقل **التقاط الرقم التسلسلي** في علامة التبويب السريعة **الأرقام التسلسلية**.</span><span class="sxs-lookup"><span data-stu-id="79646-118">Ensure that  **None** is selected in the **Capture serial number** field in the **Serial numbers** FastTab.</span></span>
6.  <span data-ttu-id="79646-119">حدد **حفظ** في جزء الإجراءات وستظهر أبعاد التعقب في علامة التبويب السريعة **أبعاد التعقب**.</span><span class="sxs-lookup"><span data-stu-id="79646-119">Select **Save** in the Action Pane and the Tracking dimensions will appear in the **Tracking dimensions** FastTab.</span></span>
6.  <span data-ttu-id="79646-120">تأكد من عدم تحديد خانة الاختيار **نشط** لأبعاد **رقم الدُفعة**، و **الرقم التسلسلي** و **المالك**.</span><span class="sxs-lookup"><span data-stu-id="79646-120">Ensure that the **Active** check box is not selected for **Batch number**, **Serial number** and **Owner** dimensions.</span></span>
7.  <span data-ttu-id="79646-121">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79646-121">Close the page.</span></span>



## <a name="create-a-warehouse-and-assign-a-name-and-site"></a><span data-ttu-id="79646-122">إنشاء مستودع وتعيين اسم وموقع</span><span class="sxs-lookup"><span data-stu-id="79646-122">Create a warehouse and assign a name and site</span></span> 

<span data-ttu-id="79646-123">بصفتك مدير مستودع في USMF، أنت بحاجة إلى تكوين مستودع جديد يسمى "MainDC" في الموقع 1 للاستخدام داخل الشركة USP2.</span><span class="sxs-lookup"><span data-stu-id="79646-123">As a warehouse manager in USMF, you need to configure a new warehouse named "MainDC" in Site 1 for use within company USP2.</span></span>

1.  <span data-ttu-id="79646-124">افتح **إدارة المستودعات > الإعداد > المستودع > المستودعات**.</span><span class="sxs-lookup"><span data-stu-id="79646-124">Open **Warehouse management > Setup > Warehouse > Warehouses**.</span></span>
2.  <span data-ttu-id="79646-125">حدد **جديد** لإنشاء مستودع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-125">Select **New** to create a new warehouse.</span></span>
3.  <span data-ttu-id="79646-126">اكتب **MainDC** للمستودع.</span><span class="sxs-lookup"><span data-stu-id="79646-126">Type **MainDC** for the warehouse.</span></span>
4.  <span data-ttu-id="79646-127">حدد **الموقع 1** لربط المستودع به.</span><span class="sxs-lookup"><span data-stu-id="79646-127">Select **Site 1** to relate the warehouse to.</span></span>

## <a name="assign-warehouse-management-attributes"></a><span data-ttu-id="79646-128">تعيين سمات إدارة المستودعات</span><span class="sxs-lookup"><span data-stu-id="79646-128">Assign warehouse management attributes</span></span>

1.  <span data-ttu-id="79646-129">قم بتوسيع علامة التبويب السريعة **التخطيط الرئيسي** وحدد "إنتاج" **التقويم** للمستودع.</span><span class="sxs-lookup"><span data-stu-id="79646-129">Expand the **Master planning** FastTab and select the **Calendar** "Production" for the warehouse.</span></span>
2.  <span data-ttu-id="79646-130">قم بتوسيع علامة التبويب السريعة **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="79646-130">Expand the **Warehouse** FastTab.</span></span>
3.  <span data-ttu-id="79646-131">قم بتعيين شريط التمرير **استخدام عمليات إدارة المستودعات** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-131">Set the **Use warehouse management processes** slider to **yes**.</span></span>
4.  <span data-ttu-id="79646-132">قم بتعيين شريط التمرير **السماح بتحركات لوحة الترخيص أثناء الجرد الدوري** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-132">Set the **Allow license plate moves during cycle counting** slider to **yes**.</span></span>
5.  <span data-ttu-id="79646-133">قم بتعيين شريط التمرير **إنقاص بند التحميل** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-133">Set the **Decrement load line** slider to **yes**.</span></span>
6.  <span data-ttu-id="79646-134">حدد **حفظ** وأغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79646-134">Select **Save** and close the page.</span></span>

## <a name="create-location-types"></a><span data-ttu-id="79646-135">إنشاء أنواع المواقع</span><span class="sxs-lookup"><span data-stu-id="79646-135">Create location types</span></span> 

<span data-ttu-id="79646-136">بصفتك مدير مستودع في USMF، أنت بحاجة إلى إنشاء أنواع مواقع جديدة للمستودع، والتي ستطلق عليها اسم "RCV" و"PICKING" و"FRESH".</span><span class="sxs-lookup"><span data-stu-id="79646-136">As a warehouse manager in USMF, you need to create new location types for the warehouse, which you will name "RCV," "PICKING," and "FRESH."</span></span>

1.  <span data-ttu-id="79646-137">افتح **إدارة المستودعات > الإعداد > المستودع > أنواع المواقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-137">Open **Warehouse management > Setup > Warehouse > Location types**.</span></span>
2.  <span data-ttu-id="79646-138">حدد **جديد** لإنشاء نوع موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-138">Select **New** to create a new location type.</span></span>
3.  <span data-ttu-id="79646-139">اكتب **انتقاء** كمعرف في حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-139">Type **PICKING** as the identifier in the **Location type** field.</span></span>
4.  <span data-ttu-id="79646-140">اكتب **انتقاء** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="79646-140">Type **Picking** in the **Description** field.</span></span>
5.  <span data-ttu-id="79646-141">حدد **جديد** لإنشاء نوع موقع جديد آخر.</span><span class="sxs-lookup"><span data-stu-id="79646-141">Select **New** to create another new location type.</span></span>
6.  <span data-ttu-id="79646-142">اكتب **RCV** كمعرف في حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-142">Type **RCV** as the identifier in the **Location type** field.</span></span>
7.  <span data-ttu-id="79646-143">اكتب **استلام** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="79646-143">Type **Receiving** in the **Description** field.</span></span>
8.  <span data-ttu-id="79646-144">حدد **جديد** لإنشاء نوع موقع جديد آخر.</span><span class="sxs-lookup"><span data-stu-id="79646-144">Select **New** to create another new location type.</span></span>
9.  <span data-ttu-id="79646-145">اكتب **تحديث** كمعرف في حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-145">Type **FRESH** as the identifier in the **Location type** field.</span></span>
10. <span data-ttu-id="79646-146">اكتب **تحديث** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="79646-146">Type **Fresh** in the **Description** field.</span></span>
11. <span data-ttu-id="79646-147">حدد **حفظ** وأغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79646-147">Select **Save** and close the page.</span></span>

## <a name="create-location-formats-and-add-segments"></a><span data-ttu-id="79646-148">إنشاء تنسيقات الموقع وإضافة الشرائح</span><span class="sxs-lookup"><span data-stu-id="79646-148">Create location formats and add segments</span></span>

<span data-ttu-id="79646-149">بصفتك مدير مستودع في USMF، أنت بحاجة إلى إنشاء تنسيق موقع جديد لـ Aisle-Rack-Shelf وRack-Shelf.</span><span class="sxs-lookup"><span data-stu-id="79646-149">As a warehouse manager in USMF, you need to create a new location format for Aisle-Rack-Shelf, and Rack-Shelf.</span></span>

1.  <span data-ttu-id="79646-150">افتح **إدارة المستودعات > الإعداد > المستودع > تنسيقات المواقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-150">Open **Warehouse management > Setup > Warehouse > Location formats**.</span></span>
2.  <span data-ttu-id="79646-151">حدد **جديد** لإنشاء تنسيق موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-151">Select **New** to create a new location format.</span></span>
3.  <span data-ttu-id="79646-152">اكتب **ARS** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-152">Type **ARS** in the **Location format** field.</span></span>
4.  <span data-ttu-id="79646-153">اكتب **الممر - الحامل - الرف** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="79646-153">Type **Aisle - Rack - Shelf** in the **Name** field.</span></span>
1.  <span data-ttu-id="79646-154">في علامة التبويب السريعة **التفاصيل**، سنحدد البند الأول.</span><span class="sxs-lookup"><span data-stu-id="79646-154">On the **Details** FastTab, we will specify the first line.</span></span>
2.  <span data-ttu-id="79646-155">في حقل **وصف الشريحة**، اكتب **بادئة الممر**.</span><span class="sxs-lookup"><span data-stu-id="79646-155">In the **Segment description** field, type **Aisle Prefix**.</span></span>
3.  <span data-ttu-id="79646-156">اكتب **1** في حقل **الطول**.</span><span class="sxs-lookup"><span data-stu-id="79646-156">Type **1** in the **Length** field.</span></span>
4.  <span data-ttu-id="79646-157">في علامة التبويب السريعة **التفاصيل**، حدد **جديد** لإنشاء بند ثاني.</span><span class="sxs-lookup"><span data-stu-id="79646-157">On the **Details** FastTab, select **New** to create a second line.</span></span>
5.  <span data-ttu-id="79646-158">في حقل **وصف الشريحة**، اكتب **رقم الممر**.</span><span class="sxs-lookup"><span data-stu-id="79646-158">In the **Segment description** field, type **Aisle Number**.</span></span>
6.  <span data-ttu-id="79646-159">اكتب **2** في حقل **الطول**.</span><span class="sxs-lookup"><span data-stu-id="79646-159">Type **2** in the **Length** field.</span></span>
7.  <span data-ttu-id="79646-160">في علامة التبويب السريعة **التفاصيل**، حدد **جديد** لإنشاء بند ثالث.</span><span class="sxs-lookup"><span data-stu-id="79646-160">On the **Details** FastTab, select **New** to create a third line.</span></span>
8.  <span data-ttu-id="79646-161">في حقل **وصف الشريحة**، اكتب **رقم الحامل**.</span><span class="sxs-lookup"><span data-stu-id="79646-161">In the **Segment description** field, type **Rack Number**.</span></span>
9.  <span data-ttu-id="79646-162">اكتب **2** في حقل **الطول**.</span><span class="sxs-lookup"><span data-stu-id="79646-162">Type **2** in the **Length** field.</span></span>
10. <span data-ttu-id="79646-163">في علامة التبويب السريعة **التفاصيل**، حدد **جديد** لإنشاء بند رابع.</span><span class="sxs-lookup"><span data-stu-id="79646-163">On the **Details** FastTab, select **New** to create a fourth line.</span></span>
11. <span data-ttu-id="79646-164">في حقل **وصف الشريحة**، اكتب **بادئة الرف**.</span><span class="sxs-lookup"><span data-stu-id="79646-164">In the **Segment description** field, type **Shelf Prefix**.</span></span>
12. <span data-ttu-id="79646-165">اكتب **1** في حقل **الطول**.</span><span class="sxs-lookup"><span data-stu-id="79646-165">Type **1** in the **Length** field.</span></span>
13. <span data-ttu-id="79646-166">في علامة التبويب السريعة **التفاصيل**، حدد **جديد** لإنشاء بند خامس.</span><span class="sxs-lookup"><span data-stu-id="79646-166">On the **Details** FastTab, select **New** to create a fifth line.</span></span>
14. <span data-ttu-id="79646-167">في حقل **وصف الشريحة**، اكتب **رقم الرف**.</span><span class="sxs-lookup"><span data-stu-id="79646-167">In the **Segment description** field, type **Shelf Number**.</span></span>
15. <span data-ttu-id="79646-168">اكتب **2** في حقل **الطول**.</span><span class="sxs-lookup"><span data-stu-id="79646-168">Type **2** in the **Length** field.</span></span>
16. <span data-ttu-id="79646-169">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="79646-169">Select **Save** in the Action Pane.</span></span>
16. <span data-ttu-id="79646-170">حدد **جديد** في جزء الإجراء لإنشاء تنسيق موقع ثاني.</span><span class="sxs-lookup"><span data-stu-id="79646-170">Select **New** in the Action Pane to create a second location format.</span></span>
17. <span data-ttu-id="79646-171">اكتب **RS** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-171">Type **RS** in the **Location format** field.</span></span>
18. <span data-ttu-id="79646-172">اكتب **الحامل - الرف** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="79646-172">Type **Rack - Shelf** in the **Name** field.</span></span>
19. <span data-ttu-id="79646-173">في علامة التبويب السريعة **التفاصيل**، حدد البند الأول.</span><span class="sxs-lookup"><span data-stu-id="79646-173">On the **Details** FastTab, specify the first line.</span></span>
20. <span data-ttu-id="79646-174">في حقل **وصف الشريحة**، اكتب **بادئة الحامل**.</span><span class="sxs-lookup"><span data-stu-id="79646-174">In the **Segment description** field, type **Rack Prefix**.</span></span>
21. <span data-ttu-id="79646-175">اكتب **1** في حقل **الطول**.</span><span class="sxs-lookup"><span data-stu-id="79646-175">Type **1** in the **Length** field.</span></span>
22. <span data-ttu-id="79646-176">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="79646-176">Select **Save** in the Action Pane.</span></span>
40. <span data-ttu-id="79646-177">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79646-177">Close the page.</span></span>

## <a name="create-a-dock-management-profile"></a><span data-ttu-id="79646-178">إنشاء ملف تعريف إدارة المساحات</span><span class="sxs-lookup"><span data-stu-id="79646-178">Create a dock management profile</span></span> 

<span data-ttu-id="79646-179">بصفتك مدير مستودع في USMF، أنت بحاجة إلى إعداد ملف تعريف إدارة مساحات جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-179">As a warehouse manager in USMF, you need to set up a new dock management profile.</span></span>

1.  <span data-ttu-id="79646-180">افتح **إدارة المستودعات > الإعداد > المستودع > ملفات تعريف إدارة المساحات**.</span><span class="sxs-lookup"><span data-stu-id="79646-180">Open **Warehouse management > Setup > Warehouse > Dock management profiles**.</span></span>
2.  <span data-ttu-id="79646-181">حدد **جديد** في جزء الإجراء لإنشاء ملف تعريف إدارة المساحات.</span><span class="sxs-lookup"><span data-stu-id="79646-181">Select **New** in the Action Pane to create a dock management profile.</span></span>
3.  <span data-ttu-id="79646-182">اكتب **SHIPSTAGE** في حقل **معرف ملف تعريف إدارة المساحات**.</span><span class="sxs-lookup"><span data-stu-id="79646-182">Type **SHIPSTAGE** in the **Dock management profile ID** field.</span></span>
4.  <span data-ttu-id="79646-183">اكتب **مواقع التشغيل المرحلي فريدة لكل شحنة** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="79646-183">Type **Staging locations unique per shipment** in the **Description** field.</span></span>
5.  <span data-ttu-id="79646-184">حدد **معرف الشحنة** في حقل **أنواع المخزون التي لا ينبغي أن تكون مختلطة**.</span><span class="sxs-lookup"><span data-stu-id="79646-184">Select **Shipment ID** in the **Inventory types that should not be mixed** field.</span></span>
6.  <span data-ttu-id="79646-185">اضغط على عمود **افترض موقعاً فارغاً لموجة جديدة** واستخدم شريط المسافة لتحديد خانة الاختيار.</span><span class="sxs-lookup"><span data-stu-id="79646-185">Tab to the **Assume empty location for new wave** column and use the space bar to select the check box.</span></span> <span data-ttu-id="79646-186">يضمن هذا أن الموقع فارغ قبل إضافة عناصر جديدة إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="79646-186">This ensures that the location is empty before adding new items to the location.</span></span>
7.  <span data-ttu-id="79646-187">حدد **حفظ** وأغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79646-187">Select **Save** and close the page.</span></span>

## <a name="create-new-location-profiles"></a><span data-ttu-id="79646-188">إنشاء ملفات تعريف مواقع جديدة</span><span class="sxs-lookup"><span data-stu-id="79646-188">Create new location profiles</span></span> 

<span data-ttu-id="79646-189">بصفتك مدير مستودع في USMF، أنت بحاجة إلى إنشاء ملفات تعريف موقع جديدة للانتقاء والتشغيل المرحلي والاستلام والتجميع والحديثة.</span><span class="sxs-lookup"><span data-stu-id="79646-189">As a warehouse manager in USMF, you need to create new location profiles for picking, staging, receiving, bulk, and fresh.</span></span>

1.  <span data-ttu-id="79646-190">افتح **إدارة المستودعات > الإعداد > المستودع > ملفات تعريف المواقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-190">Open **Warehouse management > Setup > Warehouse > Location profiles**.</span></span>
2.  <span data-ttu-id="79646-191">حدد **جديد** في جزء الإجراء لإنشاء ملف تعريف موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-191">Select **New** in the Action Pane to create a new Location profile.</span></span>
3.  <span data-ttu-id="79646-192">في حقل **معرف ملف تعريف الموقع**، أدخل **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="79646-192">In the **Location profile ID** field, enter **PICKING**.</span></span>
4.  <span data-ttu-id="79646-193">في الحقل **الاسم**، أدخل **مواقع الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="79646-193">In the **Name** field, enter **Picking Locations**.</span></span>
5.  <span data-ttu-id="79646-194">في علامة التبويب السريعة **عام**، حدد **ARS** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-194">On the **General** FastTab, select **ARS** in the **Location format** field.</span></span>
6.  <span data-ttu-id="79646-195">في علامة التبويب السريعة **عام**، حدد **انتقاء** من حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-195">On the **General** FastTab, select **Picking** from the **Location type** field.</span></span>
7.  <span data-ttu-id="79646-196">قم بتعيين شريط التمرير **استخدام تعقب لوحة الترخيص** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-196">Set the **Use license plate tracking** slider to **yes**.</span></span>
8.  <span data-ttu-id="79646-197">قم بتعيين شريط التمرير **السماح بالعناصر المختلطة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-197">Set the **Allow mixed items** slider to **yes**.</span></span>
9.  <span data-ttu-id="79646-198">قم بتعيين شريط التمرير **السماح بالجرد الدوري** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-198">Set the **Allow cycle counting** slider to **yes**.</span></span>
10. <span data-ttu-id="79646-199">حدد **جديد** لإنشاء ملف تعريف موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-199">Select **New** to create a new Location profile.</span></span>
11. <span data-ttu-id="79646-200">في **معرف ملف تعريف الموقع**، أدخل **التشغيل المرحلي**.</span><span class="sxs-lookup"><span data-stu-id="79646-200">In the **Location profile ID**, enter **STAGING**.</span></span>
12. <span data-ttu-id="79646-201">في حقل **الاسم**، أدخل **مواقع التشغيل المرحلي**.</span><span class="sxs-lookup"><span data-stu-id="79646-201">In the **Name** field, enter **Staging locations**.</span></span>
13. <span data-ttu-id="79646-202">في علامة التبويب السريعة **عام**، حدد **باب الدفع** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-202">On the **General** FastTab, select **Baydoor** in the **Location format** field.</span></span>
14. <span data-ttu-id="79646-203">في علامة التبويب السريعة **عام**، حدد **المرحلة** في حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-203">On the **General** FastTab, select **Stage** in the **Location type** field.</span></span>
15. <span data-ttu-id="79646-204">قم بتعيين شريط التمرير **استخدام تعقب لوحة الترخيص** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-204">Set the **Use license plate tracking** slider to **yes**.</span></span>
16. <span data-ttu-id="79646-205">قم بتعيين شريط التمرير **السماح بالعناصر المختلطة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-205">Set the **Allow mixed items** slider to **yes**.</span></span>
17. <span data-ttu-id="79646-206">حدد **جديد** لإنشاء ملف تعريف موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-206">Select **New** to create a new Location profile.</span></span>
18. <span data-ttu-id="79646-207">في حقل **معرف ملف تعريف الموقع**، أدخل **استلام**.</span><span class="sxs-lookup"><span data-stu-id="79646-207">In the **Location profile ID** field, enter **RECEIVING**.</span></span>
19. <span data-ttu-id="79646-208">في حقل **الاسم**، أدخل **مواقع الاستلام**.</span><span class="sxs-lookup"><span data-stu-id="79646-208">In the **Name** field, enter **Receiving locations**.</span></span>
20. <span data-ttu-id="79646-209">في علامة التبويب السريعة **عام**، حدد **باب الدفع** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-209">On the **General** FastTab, select **Baydoor** in the **Location format** field.</span></span>
21. <span data-ttu-id="79646-210">في علامة التبويب السريعة **عام**، حدد **استلام** في حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-210">On the **General** FastTab, select **Recv** in the **Location type** field.</span></span>
22. <span data-ttu-id="79646-211">قم بتعيين شريط التمرير **استخدام تعقب لوحة الترخيص** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-211">Set the **Use license plate tracking** slider to **yes**.</span></span>
23. <span data-ttu-id="79646-212">قم بتعيين شريط التمرير **السماح بالعناصر المختلطة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-212">Set the **Allow mixed items** slider to **yes**.</span></span>
24. <span data-ttu-id="79646-213">حدد **جديد** لإنشاء ملف تعريف موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-213">Select **New** to create a new Location profile.</span></span>
25. <span data-ttu-id="79646-214">في حقل **معرف ملف تعريف الموقع**، أدخل **العمليات المجمعة‬**.</span><span class="sxs-lookup"><span data-stu-id="79646-214">In the **Location profile ID** field, enter **BULK-OS**.</span></span>
26. <span data-ttu-id="79646-215">في حقل **الاسم**، أدخِل **التكدس المجمع**.</span><span class="sxs-lookup"><span data-stu-id="79646-215">In the **Name** field, enter **Bulk Overstock**.</span></span>
27. <span data-ttu-id="79646-216">في علامة التبويب السريعة **عام**، حدد **RS** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-216">On the **General** FastTab, select **RS** in the **Location format** field.</span></span>
28. <span data-ttu-id="79646-217">قم بتعيين شريط التمرير **استخدام تعقب لوحة الترخيص** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-217">Set the **Use license plate tracking** slider to **yes**.</span></span>
29. <span data-ttu-id="79646-218">قم بتعيين شريط التمرير **السماح بالعناصر المختلطة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-218">Set the **Allow mixed items** slider to **yes**.</span></span>
30. <span data-ttu-id="79646-219">حدد **جديد** لإنشاء ملف تعريف موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="79646-219">Select **New** to create a new Location profile.</span></span>
31. <span data-ttu-id="79646-220">في حقل **معرف ملف تعريف الموقع**، أدخل **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="79646-220">In the **Location profile ID** field, enter **FRESH**.</span></span>
32. <span data-ttu-id="79646-221">في حقل **الاسم**، أدخل **مواقع التحديث**.</span><span class="sxs-lookup"><span data-stu-id="79646-221">In the **Name** field, enter **Fresh locations**.</span></span>
33. <span data-ttu-id="79646-222">في علامة التبويب السريعة **عام**، حدد **ARS** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-222">On the **General** FastTab, select **ARS** in the **Location format** field.</span></span>
34. <span data-ttu-id="79646-223">في علامة التبويب السريعة **عام**، حدد **تحديث** في حقل **نوع الموقع**.</span><span class="sxs-lookup"><span data-stu-id="79646-223">On the **General** FastTab, select **Fresh** in the **Location type** field.</span></span>
35. <span data-ttu-id="79646-224">قم بتعيين شريط التمرير **استخدام تعقب لوحة الترخيص** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-224">Set the **Use license plate tracking** slider to **yes**.</span></span>
36. <span data-ttu-id="79646-225">قم بتعيين شريط التمرير **السماح بالعناصر المختلطة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79646-225">Set the **Allow mixed items** slider to **yes**.</span></span>
37. <span data-ttu-id="79646-226">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="79646-226">Close the pages.</span></span>


