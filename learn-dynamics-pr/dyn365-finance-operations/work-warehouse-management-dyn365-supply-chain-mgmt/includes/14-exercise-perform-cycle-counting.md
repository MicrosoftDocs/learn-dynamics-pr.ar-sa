---
ms.openlocfilehash: e69d4f67a4e5550872ca4632a1402c7eeb0d0d17
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073015"
---
## <a name="set-up-cycle-counting"></a><span data-ttu-id="298e1-101">إعداد الجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="298e1-101">Set up cycle counting</span></span>

<span data-ttu-id="298e1-102">بصفتك مدير مستودع، قم بإعداد الجرد الدوري للجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="298e1-102">As a warehouse manager, set up a cycle count for the mobile device.</span></span>


### <a name="set-up-a-cycle-counting-adjustment-type"></a><span data-ttu-id="298e1-103">إعداد نوع تسوية الجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="298e1-103">Set up a cycle counting adjustment type</span></span>

1.  <span data-ttu-id="298e1-104">في **USMF**، افتح **إدارة المستودعات‬ > إعداد > المخزون > أنواع التسوية**.</span><span class="sxs-lookup"><span data-stu-id="298e1-104">In **USMF**, Open **Warehouse management > Setup > Inventory > Adjustment types**.</span></span>

2.  <span data-ttu-id="298e1-105">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-105">Select **New**.</span></span>

3.  <span data-ttu-id="298e1-106">في الحقل **أنواع تعديلات المخزون**، أدخل **جرد دوري جديد**.</span><span class="sxs-lookup"><span data-stu-id="298e1-106">In the **Inventory adjustment types** field, enter **New Cycle Count**.</span></span>

4.  <span data-ttu-id="298e1-107">في حقل **الوصف**، أدخل **جرد دوري جديد**.</span><span class="sxs-lookup"><span data-stu-id="298e1-107">In the **Description** field, enter **New Cycle Count**.</span></span>

5.  <span data-ttu-id="298e1-108">في الحقل **الاسم**، حدد **ICnt**</span><span class="sxs-lookup"><span data-stu-id="298e1-108">In the **Name** field, select **ICnt**.</span></span>

6.  <span data-ttu-id="298e1-109">اضغط على المفتاح **Tab** واستخدم شريط المسافات لتحديد خانة الاختيار **إزالة الحجوزات**.</span><span class="sxs-lookup"><span data-stu-id="298e1-109">Press the **Tab** key and use the space bar  to select the **Remove reservations** check box.</span></span>


### <a name="set-up-warehouse-management-parameters-for-cycle-counting"></a><span data-ttu-id="298e1-110">إعداد معلمات إدارة المستودعات للجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="298e1-110">Set up warehouse management parameters for cycle counting</span></span>

1.  <span data-ttu-id="298e1-111">افتح **إدارة المستودعات > إعداد > معلمات إدارة المستودعات**.</span><span class="sxs-lookup"><span data-stu-id="298e1-111">Open **Warehouse management > Setup > Warehouse management parameters**.</span></span>

2.  <span data-ttu-id="298e1-112">حدد علامة التبويب **الجرد الدوري** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="298e1-112">Select the **Cycle counting** tab on the left pane.</span></span>

3.  <span data-ttu-id="298e1-113">في الحقل **رمز نوع تسوية الجرد الدوري الافتراضي**، حدد **جرد دوري جديد**.</span><span class="sxs-lookup"><span data-stu-id="298e1-113">In the **Default cycle counting adjustment type code** field, select **New Cycle Count**.</span></span>

4.  <span data-ttu-id="298e1-114">في الحقل **معرّف حساب فئة عمل الجرد الدوري الافتراضي**، حدد **CCount**.</span><span class="sxs-lookup"><span data-stu-id="298e1-114">In the **Default cycle count work class ID** field, select **CCount**.</span></span>

5.  <span data-ttu-id="298e1-115">في الحقل **أولوية عمل الجرد الدوري الافتراضي**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="298e1-115">In the **Default cycle count work priority** field, enter **1**.</span></span>
    <span data-ttu-id="298e1-116">تغير هذه الخطوة أولوية عمل الجرد الدوري مقارنة بأنواع العمل الأخرى الموجودة في المستودع.</span><span class="sxs-lookup"><span data-stu-id="298e1-116">This step changes the priority of cycle counting work compared to other types of work in the warehouse.</span></span> <span data-ttu-id="298e1-117">وبإدخال رقم أقل من الرقم الخاص بأنواع العمل الأخرى، فإنك تقوم برفع أولوية عمل الجرد الدوري.</span><span class="sxs-lookup"><span data-stu-id="298e1-117">By entering a number that is lower than the number for other types of work, you raise the priority of the cycle counting work.</span></span>

### <a name="set-up-a-spot-cycle-counting-menu-item"></a><span data-ttu-id="298e1-118">إعداد صنف قائمة الجرد الدوري الفوري</span><span class="sxs-lookup"><span data-stu-id="298e1-118">Set up a spot cycle counting menu item</span></span>

1.  <span data-ttu-id="298e1-119">افتح **إدارة المستودعات > إعداد > الجهاز المحمول > أصناف قوائم الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="298e1-119">Open **Warehouse management > Setup > Mobile device > Mobile device menu items**.</span></span>

2.  <span data-ttu-id="298e1-120">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-120">Select **New**.</span></span>

3.  <span data-ttu-id="298e1-121">في الحقل **اسم صنف القائمة**، أدخل **الجرد الدوري الفوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-121">In the **Menu item name** field, enter **Spot Cycle Count**.</span></span>

4.  <span data-ttu-id="298e1-122">في الحقل **العنوان**، أدخل **الجرد الدوري الفوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-122">In the **Title** field, enter **Spot Cycle Count**.</span></span>

5.  <span data-ttu-id="298e1-123">حدد **عمل** في الحقل **الوضع‬‏‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-123">Select **Work** in the **Mode** field.</span></span>

6.  <span data-ttu-id="298e1-124">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-124">Select **Save**.</span></span>
7.  <span data-ttu-id="298e1-125">قد تتلقي رسالة تحذير **يجب تحديد عملية إنشاء العمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-125">You may receive a warning message **Work creation process must be specified**.</span></span>

7.  <span data-ttu-id="298e1-126">قم بتعيين شريط التمرير **‏‫استخدام العمل الموجود‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="298e1-126">Set the **Use existing work** slider to **Yes**.</span></span>

8.  <span data-ttu-id="298e1-127">قم بتعيين شريط التمرير **عرض حالة المخزون** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="298e1-127">Set the **Display inventory status** slider to **Yes**.</span></span>

9.  <span data-ttu-id="298e1-128">حدد **تجميع النظام** في حقل **تم التوجيه بواسطة**.</span><span class="sxs-lookup"><span data-stu-id="298e1-128">Select **System directed** in the **Directed by** field.</span></span>

10. <span data-ttu-id="298e1-129">قم بتوسيع علامة التبويب السريعة **فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-129">Expand the **Work classes** FastTab.</span></span>

11. <span data-ttu-id="298e1-130">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-130">Select **New**.</span></span>

12. <span data-ttu-id="298e1-131">حدد **CCount** في الحقل **معرّف فئة العمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-131">Select **CCount** in the **Work class ID** field.</span></span>

13. <span data-ttu-id="298e1-132">حدد **الجرد الدوري** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="298e1-132">Select **Cycle Counting** in the Action Pane.</span></span>

14. <span data-ttu-id="298e1-133">في الصفحة **الجرد الدوري للجهاز المحمول**، أدخل **2** في الحقل **عدد المحاولات**.</span><span class="sxs-lookup"><span data-stu-id="298e1-133">On the **Mobile device cycle counting** page, enter **2** in the **Number of attempts** field.</span></span>

15. <span data-ttu-id="298e1-134">حدد **موافق** لإغلاق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="298e1-134">Select **OK** to close the page.</span></span>

16. <span data-ttu-id="298e1-135">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-135">Select **Save**.</span></span>


### <a name="add-the-spot-cycle-count-menu-item-to-the-mobile-device-menu"></a><span data-ttu-id="298e1-136">إضافة صنف قائمة الجرد الدوري الفوري‬ إلى قائمة الجهاز المحمول</span><span class="sxs-lookup"><span data-stu-id="298e1-136">Add the Spot cycle count menu item to the mobile device menu</span></span>

1.  <span data-ttu-id="298e1-137">افتح **إدارة المستودعات > إعداد > الجهاز المحمول > قائمة الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="298e1-137">Open **Warehouse management > Setup > Mobile device > Mobile device menu**.</span></span>

2.  <span data-ttu-id="298e1-138">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="298e1-138">Select **Edit**.</span></span>

3.  <span data-ttu-id="298e1-139">حدد **وارد‬** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="298e1-139">Select **Inbound** in the left-hand pane.</span></span>

3.  <span data-ttu-id="298e1-140">في القسم **قوائم الجهاز المحمول**، حدد **الجرد الدوري الفوري** من قائمة **القوائم المتوفرة وأصناف القائمة**.</span><span class="sxs-lookup"><span data-stu-id="298e1-140">In the **Mobile device menus** section, select **Spot Cycle Count** from the **Available menus and menu items** list.</span></span>

4.  <span data-ttu-id="298e1-141">حدد سهم الاتجاه الأيسر لإضافة صنف القائمة إلى قائمة **بنية القائمة**.</span><span class="sxs-lookup"><span data-stu-id="298e1-141">Select the right directional arrow to add the menu item to the **Menu structure** list.</span></span>

5.  <span data-ttu-id="298e1-142">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-142">Select **Save**.</span></span>


### <a name="enable-the-mobile-device"></a><span data-ttu-id="298e1-143">تمكين الجهاز المحمول</span><span class="sxs-lookup"><span data-stu-id="298e1-143">Enable the mobile device</span></span>

1.  <span data-ttu-id="298e1-144">انتقل إلى **إدارة المستودعات > إعداد > الجهاز المحمول > عناصر قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="298e1-144">Go to **Warehouse management > Setup > Mobile device > Mobile device menu items**.</span></span>

2.  <span data-ttu-id="298e1-145">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-145">Select **New**.</span></span>

3.  <span data-ttu-id="298e1-146">في حقل **اسم صنف القائمة**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-146">In the **Menu item name** field, enter a value.</span></span>

4.  <span data-ttu-id="298e1-147">يرجى إدخال قيمة في حقل **العنوان**.</span><span class="sxs-lookup"><span data-stu-id="298e1-147">In the **Title** field, enter a value.</span></span>

5.  <span data-ttu-id="298e1-148">في حقل **الوضع‬**، حدد **عمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-148">In the **Mode** field, select **Work**.</span></span>

6.  <span data-ttu-id="298e1-149">قم بتعيين خيار **‏‫استخدام العمل الموجود‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="298e1-149">Set the **Use existing work** option to **Yes**.</span></span> <span data-ttu-id="298e1-150">عند تعيين هذا الخيار إلى **نعم**، سيقوم النظام بالبحث عن العمل الموجود عند استخدام صنف القائمة الخاص بالجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="298e1-150">When you set this option to **Yes**, the system will look for existing work when the mobile device menu item is used.</span></span>

7.  <span data-ttu-id="298e1-151">في حقل **تم التوجيه بواسطة**، حدد **تجميع النظام**.</span><span class="sxs-lookup"><span data-stu-id="298e1-151">In the **Directed by** field, select **System directed**.</span></span> <span data-ttu-id="298e1-152">سيتم توجيه عامل المستودع لعمل مفتوح موجود ضمن فئات العمل المحددة.</span><span class="sxs-lookup"><span data-stu-id="298e1-152">The warehouse worker will be directed to open work that is in defined work classes.</span></span> 

8.  <span data-ttu-id="298e1-153">قم بتوسيع قسم **‎‏‫تفاصيل العمل** أو طيه.</span><span class="sxs-lookup"><span data-stu-id="298e1-153">Expand or collapse the **Work classes** section.</span></span>


### <a name="create-work-classes"></a><span data-ttu-id="298e1-154">إنشاء فئات العمل</span><span class="sxs-lookup"><span data-stu-id="298e1-154">Create work classes</span></span>

<span data-ttu-id="298e1-155">الآن، ستقوم بإنشاء فئتين من فئات العمل التي سيتم استخدامها مع صنف قائمة الجهاز المحمول هذا.</span><span class="sxs-lookup"><span data-stu-id="298e1-155">Now, you will create two work classes that will be used with this mobile device menu item.</span></span> <span data-ttu-id="298e1-156">عند استخدام صنف القائمة، سيتم الاستعلام عن فئات العمل هذه، سيظهر العمل ذي الأولوية الأعلى للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="298e1-156">When the menu item is used, these work classes will be queried, and the work that has the highest priority will be shown to the user.</span></span>

1. <span data-ttu-id="298e1-157">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-157">Select **New**.</span></span>

2. <span data-ttu-id="298e1-158">في الحقل **معرّف فئة العمل**، حدد القيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-158">In the **Work class ID** field, select a value.</span></span>

3. <span data-ttu-id="298e1-159">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-159">Select **New**.</span></span>

4. <span data-ttu-id="298e1-160">في الحقل **معرّف فئة العمل**، حدد القيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-160">In the **Work class ID** field, select a value.</span></span>

5. <span data-ttu-id="298e1-161">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-161">Select **Save**.</span></span>

6. <span data-ttu-id="298e1-162">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="298e1-162">Close the page.</span></span>

7. <span data-ttu-id="298e1-163">انتقل إلى **إدارة المستودعات > إعداد > الجهاز المحمول > قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="298e1-163">Go to **Warehouse management > Setup > Mobile device > Mobile device menu**.</span></span>

8. <span data-ttu-id="298e1-164">في الشجرة، حدد صنف القائمة الذي قمت بإنشائه لتوك.</span><span class="sxs-lookup"><span data-stu-id="298e1-164">In the tree, select the menu item that you just created.</span></span>

9. <span data-ttu-id="298e1-165">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="298e1-165">Select **Edit**.</span></span>

10. <span data-ttu-id="298e1-166">حدد السهم لإضافة عنصر القائمة إلى القائمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-166">Select the arrow to add the menu item to the menu.</span></span>

11. <span data-ttu-id="298e1-167">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-167">Select **Save**.</span></span>


### <a name="create-a-counting-threshold"></a><span data-ttu-id="298e1-168">إنشاء حد جرد</span><span class="sxs-lookup"><span data-stu-id="298e1-168">Create a counting threshold</span></span>

1.  <span data-ttu-id="298e1-169">انتقل إلى **إدارة المستودعات > إعداد > الجرد الدوري > حدود الجرد الدوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-169">Go to **Warehouse management > Setup > Cycle counting > Cycle count thresholds**.</span></span>

2.  <span data-ttu-id="298e1-170">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-170">Select **New**.</span></span>

3.  <span data-ttu-id="298e1-171">في الحقلين **معرّف حد الجرد الدوري** و **الوصف**، أدخل **حد جديد**.</span><span class="sxs-lookup"><span data-stu-id="298e1-171">In the **Cycle counting threshold ID** and **Description** fields, enter **New threshold**.</span></span>

4.  <span data-ttu-id="298e1-172">قم بتعيين الخيار **إجراء الجرد الدوري على الفور** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="298e1-172">Set the **Process cycle counting immediately** option to **Yes**.</span></span>

6.  <span data-ttu-id="298e1-173">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-173">Select **Save**.</span></span>

7.  <span data-ttu-id="298e1-174">في جزء الإجراء، حدد **تحديد المواقع**.</span><span class="sxs-lookup"><span data-stu-id="298e1-174">Select **Select locations** in the Action Pane.</span></span>

8.  <span data-ttu-id="298e1-175">في الحقل **المعايير‬**، حدد **المستودع** و **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="298e1-175">In the **Criteria** fields, select the **warehouse** and **site**.</span></span>

9.  <span data-ttu-id="298e1-176">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="298e1-176">Select **OK**.</span></span>

10. <span data-ttu-id="298e1-177">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="298e1-177">Close the page.</span></span>


### <a name="create-a-cycle-counting-plan"></a><span data-ttu-id="298e1-178">إنشاء خطة للجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="298e1-178">Create a cycle counting plan</span></span>

1.  <span data-ttu-id="298e1-179">انتقل إلى **إدارة المستودعات > إعداد > الجرد الدوري > خطط الجرد الدوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-179">Go to **Warehouse management > Setup > Cycle counting > Cycle count plans**.</span></span>

2.  <span data-ttu-id="298e1-180">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-180">Select **New**.</span></span>

3.  <span data-ttu-id="298e1-181">في الحقل **معرّف خطة الجرد الدوري**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-181">In the **Cycle counting plan ID** field, enter a value.</span></span>

4.  <span data-ttu-id="298e1-182">في الحقل **الوصف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-182">In the **Description** field, enter a value.</span></span>

5.  <span data-ttu-id="298e1-183">في الحقل **العدد الأقصى للجرد الدوري**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-183">In the **Maximum number of cycle counts** field, enter a number.</span></span>

6.  <span data-ttu-id="298e1-184">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-184">Select **Save**.</span></span>

7.  <span data-ttu-id="298e1-185">في جزء الإجراء، حدد **تحديد المواقع**.</span><span class="sxs-lookup"><span data-stu-id="298e1-185">Select **Select locations** in the Action Pane.</span></span>

8.  <span data-ttu-id="298e1-186">في الحقل **المعايير‬**، حدد **المستودع** و **الموقع** للخطة.</span><span class="sxs-lookup"><span data-stu-id="298e1-186">In the **Criteria** fields, select **Warehouse** and **site** for plan.</span></span>

9.  <span data-ttu-id="298e1-187">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="298e1-187">Select **OK**.</span></span>

10. <span data-ttu-id="298e1-188">في الحقل **الأيام بين الجرد الدوري**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-188">In the **Days between cycle counting** field, enter a number.</span></span> <span data-ttu-id="298e1-189">على سبيل المثال، إذا تم تعيين الحقل **الأيام بين الجرد الدوري** إلى **5**، سيتم إنشاء عمل جرد دوري كل خمسة أيام.</span><span class="sxs-lookup"><span data-stu-id="298e1-189">For example, if the **Days between cycle counting** field is set to **5**, cycle counting work will be created every five days.</span></span> <span data-ttu-id="298e1-190">ومع ذلك، إذا تمت معالجة عمل الجرد الدوري في اليوم الثالث، فسيتم إنشاء عمل الجرد الدوري التالي بعد مرور خمسة أيام على معالجة آخر جرد دوري، أي في اليوم الثامن.</span><span class="sxs-lookup"><span data-stu-id="298e1-190">However, if cycle counting work is processed on day three, the next cycle counting work will be created five days after the last cycle counting was processed, on day eight.</span></span>

11. <span data-ttu-id="298e1-191">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-191">Select **Save**.</span></span>

12. <span data-ttu-id="298e1-192">حدد **جديد** في علامة التبويب السريعة **تحديدات منتج خطة الجرد الدوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-192">Select **New** in the **Cycle count plan product selections** FastTab.</span></span>

13. <span data-ttu-id="298e1-193">في الحقل **الرقم التسلسلي**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-193">In the **Sequence number** field, enter a number.</span></span> <span data-ttu-id="298e1-194">يكون الفرز من أصغر رقم إلى أكبر رقم.</span><span class="sxs-lookup"><span data-stu-id="298e1-194">The sort is from the smallest number to the largest number.</span></span> <span data-ttu-id="298e1-195">يجب أن تكون القيمة أكبر من صفر (0).</span><span class="sxs-lookup"><span data-stu-id="298e1-195">The value must be more than 0 (zero).</span></span>

14. <span data-ttu-id="298e1-196">في الحقل **الوصف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-196">In the **Description** field, enter a value.</span></span>

15. <span data-ttu-id="298e1-197">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-197">Select **Save**.</span></span>

16. <span data-ttu-id="298e1-198">حدد **استعلام تحديد المنتج**.</span><span class="sxs-lookup"><span data-stu-id="298e1-198">Select **Define product query**.</span></span>

17. <span data-ttu-id="298e1-199">في الحقل **المعايير**، حدد صنفاً للاستعلام.</span><span class="sxs-lookup"><span data-stu-id="298e1-199">In the **Criteria** field, select an item for the query.</span></span>

18. <span data-ttu-id="298e1-200">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="298e1-200">Select **OK**.</span></span>

19. <span data-ttu-id="298e1-201">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="298e1-201">Close the page.</span></span>


## <a name="define-the-partial-location-cycle-counting-process"></a><span data-ttu-id="298e1-202">تحديد ‬‏‫عملية الجرد الدوري الجزئي للمواقع‫</span><span class="sxs-lookup"><span data-stu-id="298e1-202">Define the partial location cycle counting process</span></span>

<span data-ttu-id="298e1-203">عند استخدام خطط الجرد الدوري لإنشاء عمل الجرد، يمكنك إرشاد عمليات الجرد الفعلية وذلك من خلال طلب حساب المنتجات الخاصة ومتغيرات المنتج فقط بدلاً من كافة المخزون الفعلي في الموقع.</span><span class="sxs-lookup"><span data-stu-id="298e1-203">When you use cycle count plans to create counting work, you can guide the actual counting operations by requesting that only specific products and product variants be counted instead of all on-hand inventory at the location.</span></span> <span data-ttu-id="298e1-204">ومن خلال تصفية منتجات محددة، يمكن لمدير المستودع تقليل الحد الزائد للمراجعة، والمساعدة على منع حدوث أخطاء في التوحيد، وتوفير الوقت.</span><span class="sxs-lookup"><span data-stu-id="298e1-204">By filtering on specific products, the warehouse manager can reduce review overhead, help prevent consolidation mistakes, and save time.</span></span>  

<span data-ttu-id="298e1-205">يمكنك الانتقال عبر هذا الإجراء في شركة البيانات التجريبية **USMF** أو استخدام البيانات الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="298e1-205">You can go through this procedure in the **USMF** demo data company or in your own data.</span></span>

### <a name="create-a-cycle-counting-work-template"></a><span data-ttu-id="298e1-206">إنشاء قالب عمل جرد دوري</span><span class="sxs-lookup"><span data-stu-id="298e1-206">Create a cycle counting work template</span></span>

1.  <span data-ttu-id="298e1-207">انتقل إلى **إدارة المستودعات > إعداد > العمل > قوالب العمل**</span><span class="sxs-lookup"><span data-stu-id="298e1-207">Go to **Warehouse management > Setup > Work > Work templates**.</span></span>

2.  <span data-ttu-id="298e1-208">حدد **جرد دوري** في حقل **نوع أمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-208">In the **Work order type** field, select **Cycle counting**.</span></span>

3.  <span data-ttu-id="298e1-209">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-209">Select **New**.</span></span>

4.  <span data-ttu-id="298e1-210">في الحقل **الرقم التسلسلي**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-210">In the **Sequence number** field, enter a number.</span></span> <span data-ttu-id="298e1-211">يكون ترتيب الفرز من أصغر رقم إلى أكبر رقم.</span><span class="sxs-lookup"><span data-stu-id="298e1-211">The sort order is from the smallest number to the largest number.</span></span> <span data-ttu-id="298e1-212">يجب أن تكون القيمة أكبر من صفر (0).</span><span class="sxs-lookup"><span data-stu-id="298e1-212">The value must be more than 0 (zero).</span></span>

1.  <span data-ttu-id="298e1-213">في الحقل **قالب العمل**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-213">In the **Work template** field, enter a value.</span></span>

2.  <span data-ttu-id="298e1-214">في الحقل **وصف قالب العمل**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-214">In the **Work template description** field, enter a value.</span></span>

3.  <span data-ttu-id="298e1-215">في الحقل **معرّف مجموعة العمل**، حدد أو أدخل القيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-215">In the **Work pool ID** field, enter or select a value.</span></span>

4.  <span data-ttu-id="298e1-216">في حقل **أولوية العمل**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-216">In the **Work priority** field, enter a number.</span></span>

5.  <span data-ttu-id="298e1-217">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-217">Select **Save**.</span></span>

6.  <span data-ttu-id="298e1-218">حدد **جديد** في القسم **تفاصيل قالب العمل**</span><span class="sxs-lookup"><span data-stu-id="298e1-218">Select **New** in the **Work template details** section</span></span>

7.  <span data-ttu-id="298e1-219">في الحقل **نوع العمل**، حدد **جرد**.</span><span class="sxs-lookup"><span data-stu-id="298e1-219">In the **Work type** field, select **Counting**.</span></span>

8.  <span data-ttu-id="298e1-220">في الحقل **معرّف فئة العمل**، حدد أو أدخل القيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-220">In the **Work class ID** field, enter or select a value.</span></span>

9.  <span data-ttu-id="298e1-221">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-221">Select **Save**.</span></span>

10. <span data-ttu-id="298e1-222">حدد **فواصل بند العمل** في علامة التبويب السريعة **تفاصيل قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-222">Select **Work line breaks** in the **Work template details** fast tab.</span></span>

11. <span data-ttu-id="298e1-223">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-223">Select **New**.</span></span>

12. <span data-ttu-id="298e1-224">في الحقل **الرقم التسلسلي**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-224">In the **Sequence number** field, enter a number.</span></span> <span data-ttu-id="298e1-225">يكون ترتيب الفرز من أصغر رقم إلى أكبر رقم.</span><span class="sxs-lookup"><span data-stu-id="298e1-225">The sort order is from the smallest number to the largest number.</span></span> <span data-ttu-id="298e1-226">يجب أن تكون القيمة أكبر من صفر (0).</span><span class="sxs-lookup"><span data-stu-id="298e1-226">The value must be more than 0 (zero).</span></span>

13. <span data-ttu-id="298e1-227">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-227">Select **Save**.</span></span>

14. <span data-ttu-id="298e1-228">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="298e1-228">Close all pages.</span></span>


### <a name="create-a-cycle-counting-plan"></a><span data-ttu-id="298e1-229">إنشاء خطة للجرد الدوري</span><span class="sxs-lookup"><span data-stu-id="298e1-229">Create a cycle counting plan</span></span>

1.  <span data-ttu-id="298e1-230">انتقل إلى **إدارة المستودعات > إعداد > الجرد الدوري > خطط الجرد الدوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-230">Go to **Warehouse management > Setup > Cycle counting > Cycle count plans**.</span></span>

2.  <span data-ttu-id="298e1-231">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="298e1-231">Select **New**.</span></span>

3.  <span data-ttu-id="298e1-232">في الحقل **معرّف خطة الجرد الدوري**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-232">In the **Cycle counting plan ID** field, enter a value.</span></span>

4.  <span data-ttu-id="298e1-233">في الحقل **الوصف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-233">In the **Description** field, enter a value.</span></span>

5.  <span data-ttu-id="298e1-234">في الحقل **العدد الأقصى للجرد الدوري**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-234">In the **Maximum number of cycle counts** field, enter a number.</span></span>

6.  <span data-ttu-id="298e1-235">حدد **جرد دوري** في حقل **قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="298e1-235">In the **Work template** field, select **cycle counting**.</span></span>

7.  <span data-ttu-id="298e1-236">حدد **جديد** في علامة التبويب السريعة **تحديدات منتج خطة الجرد الدوري**.</span><span class="sxs-lookup"><span data-stu-id="298e1-236">Select **New** in the **Cycle count plan product selections** FastTab.</span></span>

8.  <span data-ttu-id="298e1-237">في الحقل **الرقم التسلسلي**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="298e1-237">In the **Sequence number** field, enter a number.</span></span> <span data-ttu-id="298e1-238">يكون ترتيب الفرز من أصغر رقم إلى أكبر رقم.</span><span class="sxs-lookup"><span data-stu-id="298e1-238">The sort order is from the smallest number to the largest number.</span></span> <span data-ttu-id="298e1-239">يجب أن تكون القيمة أكبر من صفر (0).</span><span class="sxs-lookup"><span data-stu-id="298e1-239">The value must be more than 0 (zero).</span></span>

1.  <span data-ttu-id="298e1-240">في الحقل **الوصف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="298e1-240">In the **Description** field, enter a value.</span></span>

2.  <span data-ttu-id="298e1-241">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="298e1-241">Select **Save**.</span></span>

3.  <span data-ttu-id="298e1-242">حدد **استعلام تحديد المنتج**.</span><span class="sxs-lookup"><span data-stu-id="298e1-242">Select **Define product query**.</span></span>

4.  <span data-ttu-id="298e1-243">في حقل **المعايير**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="298e1-243">In the **Criteria** field, enter or select a value.</span></span>

5.  <span data-ttu-id="298e1-244">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="298e1-244">Select **OK**.</span></span>

6.  <span data-ttu-id="298e1-245">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="298e1-245">Close the page.</span></span> 



