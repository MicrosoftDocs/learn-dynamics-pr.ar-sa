---
ms.openlocfilehash: 442255c31d8a5efdf8a853ff98269d746d94467d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6072999"
---
## <a name="set-up-warehouse-work-policies"></a><span data-ttu-id="e11cc-101">إعداد سياسات عمل المستودع</span><span class="sxs-lookup"><span data-stu-id="e11cc-101">Set up warehouse work policies</span></span>
 
<span data-ttu-id="e11cc-102">لا تتضمن عمليات المستودع دائماً عمل المستودع.</span><span class="sxs-lookup"><span data-stu-id="e11cc-102">Warehouse processes don't always include warehouse work.</span></span> <span data-ttu-id="e11cc-103">من خلال تحديد سياسة العمل، يمكنك منع إنشاء عمل لانتقاء المواد الخام واستبعاد البضائع النهائية لمجموعة من المنتجات في مواقع محددة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-103">By defining a work policy, you can prevent the creation of work for raw material picking and put away of finished goods for a set of products at specific locations.</span></span> 

1.  <span data-ttu-id="e11cc-104">في شركة **USMF**، انتقل إلى **إدارة المستودعات > الإعداد > العمل > سياسات العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-104">In company **USMF**, go to **Warehouse management > Setup > Work > Work policies**.</span></span>

2.  <span data-ttu-id="e11cc-105">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-105">Select **New** in the Action Pane.</span></span>

3.  <span data-ttu-id="e11cc-106">في حقل **اسم سياسة العمل**، أدخل **لا يوجد عمل إبعاد**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-106">In the **Work policy name** field, type **No put-away work**.</span></span>

4.  <span data-ttu-id="e11cc-107">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-107">Select **Save**.</span></span>

5.  <span data-ttu-id="e11cc-108">حدد **إضافة** في علامة التبويب السريعة **أنواع أوامر العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-108">Select **Add** in the **Work order types** FastTab.</span></span>

6.  <span data-ttu-id="e11cc-109">في حقل **نوع أمر العمل**، حدد **إبعاد البضائع المنتهية**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-109">In the **Work order type** field, select **Finished goods put away**.</span></span>

7.  <span data-ttu-id="e11cc-110">حدد **إضافة** مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="e11cc-110">Select **Add** again.</span></span>

8.  <span data-ttu-id="e11cc-111">في حقل **نوع أمر العمل**، حدد **إبعاد المنتج المساعد والمنتج الثانوي**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-111">In the **Work order type** field, select **Co-product and by-product put away**.</span></span>

9.  <span data-ttu-id="e11cc-112">قم بتوسيع علامة التبويب السريعة **مواقع المخزون**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-112">Expand the **Inventory locations** FastTab.</span></span>

10. <span data-ttu-id="e11cc-113">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-113">Select **Add**.</span></span>

11. <span data-ttu-id="e11cc-114">في قائمة **المستودع**، حدد المستودع **51**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-114">In the **Warehouse** list, select warehouse **51**.</span></span>

12. <span data-ttu-id="e11cc-115">في حقل **الموقع**، أدخل أو حدد **001**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-115">In the **Location** field, enter or select **001**.</span></span>

13. <span data-ttu-id="e11cc-116">قم بتوسيع علامة التبويب السريعة **المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-116">Expand the **Products** FastTab.</span></span>

14. <span data-ttu-id="e11cc-117">في حقل **تحديد المنتج**، حدد **تم التحديد**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-117">In the **Product selection** field, select **Selected**.</span></span>

15. <span data-ttu-id="e11cc-118">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-118">Select **Add**.</span></span>

16. <span data-ttu-id="e11cc-119">في الحقل **رقم الصنف**، أدخل أو حدد **L0101**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-119">In the **Item number** field, enter or select **L0101**.</span></span>

17. <span data-ttu-id="e11cc-120">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-120">Select **Save** in the Action Pane.</span></span>


## <a name="create-a-work-class"></a><span data-ttu-id="e11cc-121">إنشاء درجة عمل</span><span class="sxs-lookup"><span data-stu-id="e11cc-121">Create a work class</span></span>

<span data-ttu-id="e11cc-122">استعداداً لإعداد الجهاز المحمول للمستودع الخاص بك، يُطلب منك إعداد فصل عمل، والذي ستسميه أوامر الشراء، والتي ستحتوي على أنواع مواقع الإيداع لباب الدفع ومجمع وحزمة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-122">In preparation for setting up the mobile device for your warehouse, you are asked to set up a work class, which you will name Purch-Orders, which will have the Put location types of Bay-door, Bulk, and Pack.</span></span>


1.  <span data-ttu-id="e11cc-123">افتح **إدارة المستودعات > إعداد > العمل > فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-123">Open **Warehouse management > Setup > Work > Work classes**.</span></span>

2.  <span data-ttu-id="e11cc-124">حدد **جديد** في جزء الإجراء لإنشاء فئة عمل.</span><span class="sxs-lookup"><span data-stu-id="e11cc-124">Select **New** in the Action Pane to create a work class.</span></span>

3.  <span data-ttu-id="e11cc-125">في حقل **معرف فئة العمل**، أدخل **أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-125">In the **Work class ID** field, enter **Purch-Orde**.</span></span>

4.  <span data-ttu-id="e11cc-126">بالنسبة إلى **الوصف**، أدخل **أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-126">For **Description**, enter **Purchase Orders**.</span></span>

5.  <span data-ttu-id="e11cc-127">بالنسبة إلى **نوع أمر العمل**، حدد **أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-127">For **Work order type**, select **Purchase orders**.</span></span>

6.  <span data-ttu-id="e11cc-128">في علامة التبويب السريعة **أنواع مواقع الإيداع الصالحة**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-128">On the **Valid put location types** FastTab, select **New**.</span></span>

7.  <span data-ttu-id="e11cc-129">حدد **باب الدفع**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-129">Select **BAYDOOR**.</span></span>

8.  <span data-ttu-id="e11cc-130">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-130">Select **New**.</span></span>

9.  <span data-ttu-id="e11cc-131">حدد **مجمع**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-131">Select **Bulk**.</span></span>

10. <span data-ttu-id="e11cc-132">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-132">Select **New**.</span></span>

11. <span data-ttu-id="e11cc-133">حدد **حزمة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-133">Select **Pack**.</span></span>

12. <span data-ttu-id="e11cc-134">انقر على **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-134">Click **Save** in the Action Pane.</span></span>


## <a name="create-a-mobile-device-menu-item-and-menu"></a><span data-ttu-id="e11cc-135">إنشاء صنف قائمة الجهاز المحمول والقائمة</span><span class="sxs-lookup"><span data-stu-id="e11cc-135">Create a mobile device menu item and menu</span></span> 

<span data-ttu-id="e11cc-136">وبصفتك مدير المستودع، يجب تكوين خيارات الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-136">As Warehouse manager, you must configure the mobile device options.</span></span> <span data-ttu-id="e11cc-137">ستقوم بإعداد وظيفتين: استلام أمر الشراء وإبعاد أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-137">You will be setting up two functions: Purchase order receive and Purchase order put away.</span></span> <span data-ttu-id="e11cc-138">ستضيف بعد ذلك الوظائف إلى قائمة الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-138">You will then add the functions to your Mobile device menu.</span></span>

### <a name="set-up-mobile-device-menu-items"></a><span data-ttu-id="e11cc-139">إعداد أصناف قوائم الأجهزة المحمولة</span><span class="sxs-lookup"><span data-stu-id="e11cc-139">Set up mobile device menu items</span></span>

1.  <span data-ttu-id="e11cc-140">افتح **إدارة المستودعات > إعداد > الجهاز المحمول > أصناف قوائم الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-140">Open **Warehouse management > Setup > Mobile device > Mobile device menu items**.</span></span>

2.  <span data-ttu-id="e11cc-141">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-141">Select **New** in the Action Pane.</span></span>

3.  <span data-ttu-id="e11cc-142">بالنسبة إلى **اسم صنف القائمة**، أدخل **استلام أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-142">For **Menu item name**, enter **PO Receive**.</span></span>

4.  <span data-ttu-id="e11cc-143">بالنسبة إلى **العنوان**، أدخل **استلام أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-143">For **Title**, enter **PO Receive**.</span></span>

5.  <span data-ttu-id="e11cc-144">بالنسبة إلى **الوضع**، حدد **العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-144">For **Mode**, select **Work**.</span></span>

6.  <span data-ttu-id="e11cc-145">قم بتعيين شريط التمرير **‏‫استخدام العمل الموجود‬** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-145">Set the **Use existing work** slider to **No**.</span></span>

7.  <span data-ttu-id="e11cc-146">في علامة التبويب السريعة **عام**، في **عملية إنشاء العمل**، حدد **استلام بنود أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-146">On the **General** FastTab, on **Work creation process**, select **Purchase order line receiving**.</span></span>

8.  <span data-ttu-id="e11cc-147">حدد **تجميع لوحات الترخيص** في حقل **سياسة تجميع لوحات الترخيص**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-147">Select **License plate grouping** in the **License plate grouping policy** field.</span></span>

9.  <span data-ttu-id="e11cc-148">قم بتعيين شريط التمرير **إنشاء لوحة الترخيص** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-148">Set the **Generate license plate** slider to **Yes**.</span></span>

10. <span data-ttu-id="e11cc-149">قم بتعيين جميع أشرطة التمرير الأخرى إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-149">Set all other sliders to **No**.</span></span>

11. <span data-ttu-id="e11cc-150">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-150">Select **Save** in the Action Pane.</span></span>

12. <span data-ttu-id="e11cc-151">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-151">Select **New** in the Action Pane.</span></span>

13. <span data-ttu-id="e11cc-152">بالنسبة إلى **اسم صنف القائمة**، أدخل **إبعاد أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-152">For **Menu item name**, enter **PO Put away**.</span></span>

14. <span data-ttu-id="e11cc-153">بالنسبة إلى **العنوان**، أدخل **إبعاد أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-153">For **Title**, enter **PO Put away**.</span></span>

15. <span data-ttu-id="e11cc-154">بالنسبة إلى **الوضع**، حدد **العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-154">For **Mode**, select **Work**.</span></span>

16. <span data-ttu-id="e11cc-155">قم بتعيين شريط التمرير **‏‫استخدام العمل الموجود‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-155">Set the **Use existing work** slider to **Yes**.</span></span>

17. <span data-ttu-id="e11cc-156">في علامة التبويب السريعة **عام**، في حقل **تم التوجيه بواسطة**، حدد **تجميع المستخدمين**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-156">On the **General** FastTab, in the **Directed by** field, select **User grouping**.</span></span>

18. <span data-ttu-id="e11cc-157">قم بتعيين شريط التمرير **إبعاد المجموعة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-157">Set the **Group put away** slider to **Yes**.</span></span>

19. <span data-ttu-id="e11cc-158">قم بتعيين جميع أشرطة التمرير المتبقية إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-158">Set all remaining sliders to **No**.</span></span>

20. <span data-ttu-id="e11cc-159">في علامة التبويب السريعة **فئات العمل**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-159">On **Work classes** FastTab, select **New**.</span></span>

21. <span data-ttu-id="e11cc-160">بالنسبة إلى **معرف فئة العمل**، حدد **أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-160">For **Work class ID**, select **Purch-Orde**.</span></span>

22. <span data-ttu-id="e11cc-161">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-161">Select **Save** in the Action Pane.</span></span>

23. <span data-ttu-id="e11cc-162">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-162">Close the page.</span></span>

### <a name="set-up-a-mobile-device-menu"></a><span data-ttu-id="e11cc-163">إعداد قائمة الأجهزة المحمولة</span><span class="sxs-lookup"><span data-stu-id="e11cc-163">Set up a mobile device menu</span></span>

1.  <span data-ttu-id="e11cc-164">افتح **إدارة المستودعات > إعداد > الجهاز المحمول > قائمة الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-164">Open **Warehouse management > Setup > Mobile device > Mobile device menu**.</span></span>

2.  <span data-ttu-id="e11cc-165">حدد **الوارد** في شريط القائمة اليسرى، وحدد **تحرير** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-165">Select **Inbound** in the left menu bar and select **Edit** in the Action Pane.</span></span>

3.  <span data-ttu-id="e11cc-166">في جزء **القوائم المتوفرة وأصناف القوائم**، حدد **استلام أمر الشراء** وحدد سهم الاتجاه الصحيح.</span><span class="sxs-lookup"><span data-stu-id="e11cc-166">In the **AVAILABLE MENUS AND MENU ITEMS** pane, select **PO Receive** and select the right directional arrow.</span></span>

4.  <span data-ttu-id="e11cc-167">في جزء **القوائم المتوفرة وأصناف القوائم**، حدد **إبعاد أمر الشراء** وحدد سهم الاتجاه الصحيح.</span><span class="sxs-lookup"><span data-stu-id="e11cc-167">In the **AVAILABLE MENUS AND MENU ITEMS** pane, select **PO Put away** and select the right directional arrow.</span></span>

5.  <span data-ttu-id="e11cc-168">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-168">Select **Save**.</span></span>

6.  <span data-ttu-id="e11cc-169">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-169">Close the page.</span></span>


## <a name="create-mobile-device-users"></a><span data-ttu-id="e11cc-170">إنشاء مستخدمي الأجهزة المحمولة</span><span class="sxs-lookup"><span data-stu-id="e11cc-170">Create mobile device users</span></span> 

<span data-ttu-id="e11cc-171">وبصفتك مدير المستودع، يجب تكوين مستخدمي الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-171">As Warehouse manager, you must configure the mobile device users.</span></span> <span data-ttu-id="e11cc-172">أضف Ted Howard كعامل بمعرف مستخدم واسم مستخدم كـ *thoward* مع مستودع افتراضي 62.</span><span class="sxs-lookup"><span data-stu-id="e11cc-172">Add Ted Howard as a worker with a User ID and User name as *thoward* with a default warehouse of 62.</span></span> <span data-ttu-id="e11cc-173">ستكون كلمة المرور 1234 على الجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="e11cc-173">The password will be 1234 on the mobile device.</span></span>

1.  <span data-ttu-id="e11cc-174">افتح **إدارة المستودعات > إعداد > العامل**</span><span class="sxs-lookup"><span data-stu-id="e11cc-174">Open **Warehouse management > Setup > Worker**.</span></span>

2.  <span data-ttu-id="e11cc-175">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-175">Select **New** in the Action Pane.</span></span>

3.  <span data-ttu-id="e11cc-176">في حقل القائمة المنسدلة **العامل**، حدد **Ted Howard** ثم انقر على **تحديد**</span><span class="sxs-lookup"><span data-stu-id="e11cc-176">In the **Worker** dropdown field, select **Ted Howard** then click **Select**</span></span>

4.  <span data-ttu-id="e11cc-177">ضمن علامة التبويب السريعة **المستخدمين**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-177">On the **Users** FastTab, select **New**.</span></span>

5.  <span data-ttu-id="e11cc-178">بالنسبة إلى **معرف المستخدم**، أدخل **thoward**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-178">For **User ID**, enter **thoward**.</span></span>

6.  <span data-ttu-id="e11cc-179">بالنسبة إلى **اسم المستخدم**، أدخل **thoward**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-179">For **User name**, enter **thoward**.</span></span>

7.  <span data-ttu-id="e11cc-180">بالنسبة إلى **المستودع الافتراضي**، حدد **62**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-180">For **Default warehouse**, select **62**.</span></span>

8.  <span data-ttu-id="e11cc-181">بالنسبة **لاسم القائمة**، حدد **أساسي**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-181">For **Menu name**, select **Main**.</span></span>

9.  <span data-ttu-id="e11cc-182">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-182">Select **Save** in the Action Pane.</span></span>

10. <span data-ttu-id="e11cc-183">بالنسبة إلى **كلمة المرور**، أدخل **1234**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-183">For **Password**, enter **1234**.</span></span>

11. <span data-ttu-id="e11cc-184">بالنسبة إلى **تأكيد كلمة المرور**، أدخل **1234**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-184">For **Confirm password**, enter **1234**.</span></span>

12. <span data-ttu-id="e11cc-185">حدد **تعيين كلمة المرور**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-185">Select **Set password**.</span></span>

13. <span data-ttu-id="e11cc-186">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-186">Close the page.</span></span>


## <a name="set-up-a-mobile-device-menu-item-for-completing-work-of-the-purchase-order-type"></a><span data-ttu-id="e11cc-187">قم بإعداد عنصر قائمة جهاز محمول لإكمال عمل نوع أمر الشراء</span><span class="sxs-lookup"><span data-stu-id="e11cc-187">Set up a mobile device menu item for completing work of the Purchase order type</span></span>

<span data-ttu-id="e11cc-188">بصفتك مدير مستودع، تحتاج إلى إنشاء صنف قائمة يُستخدم لأداء عمل من نوع أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-188">As a warehouse manager, you need to create a menu item that is used for performing work of the Purchase order type.</span></span> <span data-ttu-id="e11cc-189">تحدد فئة العمل المرتبطة بصنف القائمة العمل الصالح.</span><span class="sxs-lookup"><span data-stu-id="e11cc-189">The work class that's associated with the menu item determines which work is valid.</span></span>

### <a name="create-a-mobile-device-menu-item"></a><span data-ttu-id="e11cc-190">إنشاء صنف قائمة الجهاز المحمول</span><span class="sxs-lookup"><span data-stu-id="e11cc-190">Create a mobile device menu item</span></span>

1.  <span data-ttu-id="e11cc-191">انتقل إلى **إدارة المستودعات > إعداد > الجهاز المحمول > عناصر قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-191">Go to **Warehouse management > Setup > Mobile device > Mobile device menu items**.</span></span>

2.  <span data-ttu-id="e11cc-192">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-192">Select **New**.</span></span>

3.  <span data-ttu-id="e11cc-193">في حقل **اسم صنف القائمة**، أدخل قيمة فريدة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-193">In the **Menu item name** field, enter a unique value.</span></span> <span data-ttu-id="e11cc-194">على سبيل المثال، يمكنك إدخال **POMove**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-194">For example, you could type **POMove**.</span></span> <span data-ttu-id="e11cc-195">تذكر القيمة، فستحتاج إليها لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="e11cc-195">Remember the value, you'll need it later.</span></span>

4.  <span data-ttu-id="e11cc-196">في حقل **العنوان**، أدخل **نقل أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-196">In the **Title** field, type **PO Move**.</span></span> <span data-ttu-id="e11cc-197">هذا هو العنوان الذي سيتم عرضه على الجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="e11cc-197">This is the title that will be displayed on the mobile device.</span></span>

5.  <span data-ttu-id="e11cc-198">في حقل **الوضع‬**، حدد **عمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-198">In the **Mode** field, select **Work**.</span></span>

6.  <span data-ttu-id="e11cc-199">حدد **نعم** في حقل **استخدام العمل القائم**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-199">Select **Yes** in the **Use existing work** field.</span></span>

7.  <span data-ttu-id="e11cc-200">حدد **نعم** في حقل **عرض حالة المخزون**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-200">Select **Yes** in the **Display inventory status** field.</span></span>

8.  <span data-ttu-id="e11cc-201">في حقل **تم التوجيه بواسطة**، حدد **تجميع النظام**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-201">In the **Directed by** field, select **System grouping**.</span></span> <span data-ttu-id="e11cc-202">عند تحديد شيء ما في حقل **تم التوجيه بواسطة**، تظهر الحقول الإضافية في قسم **عام** في هذه الصفحة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-202">When you select something in the **Directed by** field, additional fields appear in the **General** section on this page.</span></span> <span data-ttu-id="e11cc-203">تعتمد الحقول التي تظهر على ما قمت بتحديده.</span><span class="sxs-lookup"><span data-stu-id="e11cc-203">The fields that appear depend on what you selected.</span></span> <span data-ttu-id="e11cc-204">عند تحديد **تجميع النظام**، تتم إضافة حقلين جديدين.</span><span class="sxs-lookup"><span data-stu-id="e11cc-204">When you select **System grouping**, two new fields are added.</span></span>

9.  <span data-ttu-id="e11cc-205">في حقل **تجميع النظام**، حدد **WorkPoolId**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-205">In the **System grouping field** field, select **WorkPoolId**.</span></span> <span data-ttu-id="e11cc-206">عندما يقوم عمال المستودع بفتح صنف القائمة هذا، سيطلب منك فحص معرف وعاء العمل.</span><span class="sxs-lookup"><span data-stu-id="e11cc-206">When warehouse workers open this menu item, they'll be asked to scan a Work pool ID.</span></span> <span data-ttu-id="e11cc-207">سيتم دفع جميع أوامر العمل التي تحتوي على معرف وعاء العمل هذا وبنود أمر العمل المفتوحة مع إحدى فئات العمل المضافة إلى عنصر القائمة هذا إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="e11cc-207">All work orders with this Work pool ID and open work order lines with one of the work classes added to this menu item will be pushed to the user.</span></span>

10. <span data-ttu-id="e11cc-208">في حقل **تسمية تجميع النظام**، أدخل **وعاء العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-208">In the **System grouping label** field, type **Work pool**.</span></span> <span data-ttu-id="e11cc-209">هذا هو النص الذي يتم عرضه للمستخدم على الجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="e11cc-209">This is the text that is displayed to the user on the mobile device.</span></span>

11. <span data-ttu-id="e11cc-210">حدد **نعم** في حقل **تجاوز لوحة الترخيص أثناء الإيداع**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-210">Select **Yes** in the **Override license plate during put** field.</span></span>
    <span data-ttu-id="e11cc-211">يسمح هذا الخيار لعمال المستودعات بتجاوز لوحة الترخيص المستهدفة عند وضع الأصناف في موقع تتحكم فيه لوحة الترخيص.</span><span class="sxs-lookup"><span data-stu-id="e11cc-211">This option allows warehouse workers to override the target license plate when items are put down on a license plate-controlled location.</span></span>

12. <span data-ttu-id="e11cc-212">حدد **نعم** في حقل **إبعاد المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-212">Select **Yes** in the **Group put away** field.</span></span> <span data-ttu-id="e11cc-213">إذا كانت جميع بنود الوضع في أمر العمل تشترك في نفس الموقع، فسيتلقى المستخدم تعليمة وضع واحدة مجمعة لجميع البنود.</span><span class="sxs-lookup"><span data-stu-id="e11cc-213">If all Put lines on the work order share the same location, the user will receive one combined Put instruction for all lines.</span></span>

13. <span data-ttu-id="e11cc-214">قم بتوسيع القسم **فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-214">Expand the **Work classes** section.</span></span>

14. <span data-ttu-id="e11cc-215">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-215">Select **New**.</span></span>

15. <span data-ttu-id="e11cc-216">في حقل **معرف فئة العمل**، حدد **شراء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-216">In the **Work class ID** field, select **Purchase**.</span></span> <span data-ttu-id="e11cc-217">تقوم فئة العمل بتقييد العمل الذي يمكن استخدام صنف القائمة من أجله.</span><span class="sxs-lookup"><span data-stu-id="e11cc-217">The work class restricts the work that the menu item can be used for.</span></span> <span data-ttu-id="e11cc-218">في هذه الحالة، سيتم استخدامه لبنود أمر العمل المفتوحة التي تحتوي على معرف فئة عمل الشراء.</span><span class="sxs-lookup"><span data-stu-id="e11cc-218">In this case, it will be used for open work order lines that have the Purchase work class ID.</span></span>

16. <span data-ttu-id="e11cc-219">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-219">Select **Save**.</span></span>


### <a name="set-up-work-confirmation"></a><span data-ttu-id="e11cc-220">إعداد تأكيد العمل</span><span class="sxs-lookup"><span data-stu-id="e11cc-220">Set up work confirmation</span></span>

1. <span data-ttu-id="e11cc-221">حدد **إعداد تأكيد العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-221">Select **Work confirmation setup**.</span></span>

2. <span data-ttu-id="e11cc-222">في الحقل **نوع العمل**، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-222">In the **Work type** field, select **Pick**.</span></span>

3. <span data-ttu-id="e11cc-223">حدد خانة الاختيار **التأكيد التلقائي**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-223">Select the **Auto confirm** check box.</span></span> <span data-ttu-id="e11cc-224">سيتم تأكيد إرشادات العمل مع انتقاء نوع العمل تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="e11cc-224">The work instruction with the work type Pick will be auto-confirmed.</span></span> <span data-ttu-id="e11cc-225">لن يتم تقديم هذه الإرشادات إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="e11cc-225">This instruction will not be presented to the user.</span></span>

4. <span data-ttu-id="e11cc-226">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-226">Select **New**.</span></span>

5. <span data-ttu-id="e11cc-227">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-227">In the **Work type** field, select **Put**.</span></span>

6. <span data-ttu-id="e11cc-228">حدد خانة الاختيار **تأكيد الموقع**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-228">Select the **Location confirmation** check box.</span></span> <span data-ttu-id="e11cc-229">سيُطلب من عامل المستودع إجراء فحص تأكيد للموقع عند وضع الصنف.</span><span class="sxs-lookup"><span data-stu-id="e11cc-229">The warehouse worker will be asked to perform a confirmation scan of the location when the item is put down.</span></span>

7. <span data-ttu-id="e11cc-230">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-230">Select **Save**.</span></span>

8. <span data-ttu-id="e11cc-231">أغلق صفحة **إعداد تأكيد العمل**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-231">Close the **Work confirmation setup** page.</span></span>

9. <span data-ttu-id="e11cc-232">أغلق صفحة **أصناف قوائم الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-232">Close the **Mobile device menu items** page.</span></span>


### <a name="add-the-menu-item-to-a-mobile-device-menu"></a><span data-ttu-id="e11cc-233">إضافة صنف القائمة إلى قائمة أجهزة محمولة</span><span class="sxs-lookup"><span data-stu-id="e11cc-233">Add the menu item to a mobile device menu</span></span>

1. <span data-ttu-id="e11cc-234">انتقل إلى **إدارة المستودعات > إعداد > الجهاز المحمول > قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-234">Go to **Warehouse management > Setup > Mobile device > Mobile device menu**.</span></span>

2. <span data-ttu-id="e11cc-235">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-235">Select **Edit**.</span></span>

3. <span data-ttu-id="e11cc-236">استخدم عامل التصفية السريع للعثور على السجلات.</span><span class="sxs-lookup"><span data-stu-id="e11cc-236">Use the Quick Filter to find records.</span></span> <span data-ttu-id="e11cc-237">على سبيل المثال، قم بالتصفية في حقل **الاسم** بقيمة *واردة*.</span><span class="sxs-lookup"><span data-stu-id="e11cc-237">For example, filter on the **Name** field with a value of *inbound*.</span></span> <span data-ttu-id="e11cc-238">تريد العثور على القائمة التي يمكنك استخدامها لأصناف القائمة الواردة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-238">You want to find the menu that you can use for inbound menu items.</span></span> <span data-ttu-id="e11cc-239">في **USMF**، تُسمى هذه **الواردة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-239">In **USMF**, this is called **Inbound**.</span></span>

4. <span data-ttu-id="e11cc-240">في الشجرة، حدد قيمة.</span><span class="sxs-lookup"><span data-stu-id="e11cc-240">In the tree, select a value.</span></span>

5. <span data-ttu-id="e11cc-241">حدد السهم الأيمن.</span><span class="sxs-lookup"><span data-stu-id="e11cc-241">Select the right arrow.</span></span>

6. <span data-ttu-id="e11cc-242">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-242">Select **Save**.</span></span>

7. <span data-ttu-id="e11cc-243">أغلق صفحة **قوائم الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="e11cc-243">Close the **Mobile device menus** page.</span></span> 
 

 
