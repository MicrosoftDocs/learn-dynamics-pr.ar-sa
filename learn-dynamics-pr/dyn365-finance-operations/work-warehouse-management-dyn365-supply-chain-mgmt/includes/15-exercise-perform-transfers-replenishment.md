---
ms.openlocfilehash: b9f6cfcde9cd5eadf5d6ca09e3b11e04378f113c
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6073861"
---
## <a name="set-up-transfer-orders"></a><span data-ttu-id="7c55f-101">إعداد أوامر التحويل</span><span class="sxs-lookup"><span data-stu-id="7c55f-101">Set up transfer orders</span></span>
 
<span data-ttu-id="7c55f-102">تحتاج إلى إجراء إعداد لأوامر التحويل في مستودع Contoso لعصير البرتقال.</span><span class="sxs-lookup"><span data-stu-id="7c55f-102">You need to perform setup for transfer orders for Contoso Orange Juice.</span></span> <span data-ttu-id="7c55f-103">للبدء، قم بإنشاء مستودع نقل وربطه، وإعداد توجيهات الموقع، وإعداد قالب عمل.</span><span class="sxs-lookup"><span data-stu-id="7c55f-103">To get started, create and link a transit warehouse, set up location directives, and set up a work template.</span></span> 

### <a name="create-transit-and-production-warehouses"></a><span data-ttu-id="7c55f-104">إنشاء مستودعات النقل والإنتاج</span><span class="sxs-lookup"><span data-stu-id="7c55f-104">Create transit and production warehouses</span></span> 

1.  <span data-ttu-id="7c55f-105">في الشركة **USP2**، افتح **إدارة المستودع > إعداد > المستودع >المستودعات**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-105">In the company **USP2**, open **Warehouse management > Setup > Warehouse > Warehouses**.</span></span>
2.  <span data-ttu-id="7c55f-106">حدد **جديد** لإنشاء مستودع جديد.</span><span class="sxs-lookup"><span data-stu-id="7c55f-106">Select **New** to create a new warehouse.</span></span>
3.  <span data-ttu-id="7c55f-107">في الحقل **المستودع**، أدخل **31**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-107">In the **Warehouse** field, enter **31**.</span></span>
4.  <span data-ttu-id="7c55f-108">في الحقل **الاسم**، أدخل **الموقع 3 - مستودع النقل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-108">In the **Name** field, enter **Site 3 - Transit Warehouse**.</span></span>
5.  <span data-ttu-id="7c55f-109">في علامة التبويب السريعة **عام**، حدد **3** في حقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-109">On the **General** FastTab, select **3** in the **Site** field.</span></span>
6.  <span data-ttu-id="7c55f-110">في الحقل **النوع**، حدد **نقل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-110">In the **Type** field, select **Transit**.</span></span>
7.  <span data-ttu-id="7c55f-111">قم بتوسيع علامة التبويب السريعة **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-111">Expand the **Warehouse** FastTab.</span></span>
8.  <span data-ttu-id="7c55f-112">قم بتعيين شريط التمرير **استخدام عمليات إدارة المستودعات** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-112">Set the **Use warehouse management processes** slider to **Yes**.</span></span>
9.  <span data-ttu-id="7c55f-113">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-113">Select **Save**.</span></span>
10. <span data-ttu-id="7c55f-114">حدد **جديد** لإنشاء مستودع جديد.</span><span class="sxs-lookup"><span data-stu-id="7c55f-114">Select **New** to create a new warehouse.</span></span>
11. <span data-ttu-id="7c55f-115">في الحقل **المستودع‏‎**، أدخل **32**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-115">In the **Warehouse** field, enter **32**.</span></span>
12. <span data-ttu-id="7c55f-116">في الحقل **الاسم**، أدخل **الموقع 3 - مستودع Prod**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-116">In the **Name** field, enter **Site 3 - Prod Warehouse**.</span></span>
13. <span data-ttu-id="7c55f-117">في علامة التبويب السريعة **عام**، حدد **3** في حقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-117">On the **General** FastTab, select **3** in the **Site** field.</span></span>
14. <span data-ttu-id="7c55f-118">قم بتوسيع علامة التبويب السريعة **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-118">Expand the **Warehouse** FastTab.</span></span>
15. <span data-ttu-id="7c55f-119">قم بتعيين شريط التمرير **استخدام عمليات إدارة المستودعات** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-119">Set the **Use warehouse management processes** slider to **Yes**.</span></span>
16. <span data-ttu-id="7c55f-120">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-120">Select **Save**.</span></span>

### <a name="set-up-a-location-directive"></a><span data-ttu-id="7c55f-121">إعداد التوجيه الخاص بالموقع</span><span class="sxs-lookup"><span data-stu-id="7c55f-121">Set up a location directive</span></span>

1.  <span data-ttu-id="7c55f-122">افتح **إدارة المستودعات > إعداد > توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-122">Open **Warehouse management > Setup > Location directives**.</span></span>
2.  <span data-ttu-id="7c55f-123">حدد **مشكلة التحويل** في حقل **نوع أمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-123">Select **Transfer issue** in the **Work order type** field.</span></span>
3.  <span data-ttu-id="7c55f-124">في الصفحة **توجيهات الموقع**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-124">Select **New** in the **Location directives** page.</span></span>
4.  <span data-ttu-id="7c55f-125">أدخل **مشكلة التحويل** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-125">Enter **Transfer Issue** in the **Name** field.</span></span>
5.  <span data-ttu-id="7c55f-126">في علامة التبويب السريعة **توجيهات الموقع**، حدد **انتقاء** في الحقل **نوع العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-126">On the **Location directives** FastTab, select **Pick** in the **Work type** field.</span></span>
6.  <span data-ttu-id="7c55f-127">في حقل **الموقع**، حدد **3**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-127">In the **Site** field, select **3**.</span></span>
7.  <span data-ttu-id="7c55f-128">في حقل **المستودع‏‎**، حدد **30**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-128">In the **Warehouse** field, select **30**.</span></span>
8.  <span data-ttu-id="7c55f-129">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-129">Select **Save**</span></span>
8.  <span data-ttu-id="7c55f-130">حدد **جديد** ضمن علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-130">Select **New** on the **Lines** FastTab.</span></span>
9.  <span data-ttu-id="7c55f-131">تأكد أن حقل **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-131">Verify that the **Sequence number** field is **1**.</span></span>
10. <span data-ttu-id="7c55f-132">أدخل **1000** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-132">Enter **1000** in the **To quantity** field.</span></span>
11. <span data-ttu-id="7c55f-133">حدد **بلا‬** في الحقل **تحديد موقع الكمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-133">Select **None** in the **Locate quantity** field.</span></span>
12. <span data-ttu-id="7c55f-134">قم بتوسيع علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-134">Expand the **Location Directive Actions** FastTab.</span></span>
13. <span data-ttu-id="7c55f-135">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-135">Select **New**.</span></span>
14. <span data-ttu-id="7c55f-136">في حقل **الاسم**، أدخل **مجمع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-136">Enter **Bulk** in the **Name** field.</span></span>
15. <span data-ttu-id="7c55f-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-137">Select **Save**.</span></span>
16. <span data-ttu-id="7c55f-138">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-138">Select **New** in the Action Pane.</span></span>
17. <span data-ttu-id="7c55f-139">أدخل **مشكلة وضع التحويل** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-139">Enter **Transfer Issue-Put** in the **Name** field.</span></span>
18. <span data-ttu-id="7c55f-140">في **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-140">Select **Put** in the **Work type**.</span></span>
19. <span data-ttu-id="7c55f-141">في حقل **الموقع**، حدد **3**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-141">In the **Site** field, select **3**.</span></span>
20. <span data-ttu-id="7c55f-142">في حقل **المستودع‏‎**، حدد **31**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-142">In the **Warehouse** field, select **31**.</span></span>
21. <span data-ttu-id="7c55f-143">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-143">Select **Save**</span></span>
21. <span data-ttu-id="7c55f-144">حدد **جديد** ضمن علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-144">Select **New** on the **Lines** FastTab.</span></span>
22. <span data-ttu-id="7c55f-145">تأكد أن حقل **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-145">Verify that the **Sequence number** field is **1**.</span></span>
23. <span data-ttu-id="7c55f-146">أدخل **1000** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-146">Enter **1000** in the **To quantity** field.</span></span>
24. <span data-ttu-id="7c55f-147">حدد **بلا‬** في الحقل **تحديد موقع الكمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-147">Select **None** in the **Locate quantity** field.</span></span>
25. <span data-ttu-id="7c55f-148">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-148">Select **Save**</span></span>
25. <span data-ttu-id="7c55f-149">قم بتوسيع علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-149">Expand the **Location Directive Actions** FastTab.</span></span>
26. <span data-ttu-id="7c55f-150">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-150">Select **New**.</span></span>
27. <span data-ttu-id="7c55f-151">في حقل **الاسم**، أدخل **مجمع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-151">Enter **Bulk** in the **Name** field.</span></span>
28. <span data-ttu-id="7c55f-152">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-152">Select **Save**.</span></span>
29. <span data-ttu-id="7c55f-153">في الجزء الأيمن، حدد **استلام إيصال التحويل** في الحقل **نوع أمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-153">In the left-hand pane, select **Transfer Receipt** in the **Work order type** field.</span></span>
30. <span data-ttu-id="7c55f-154">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-154">Select **New** in the Action Pane.</span></span>
31. <span data-ttu-id="7c55f-155">أدخل **مشكلة التحويل** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-155">Enter **Transfer Issue** in the **Name** field.</span></span>
32. <span data-ttu-id="7c55f-156">في الحقل **نوع العمل**، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-156">Select **Pick** in the **Work type** field.</span></span>
33. <span data-ttu-id="7c55f-157">في حقل **الموقع**، حدد **3**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-157">In the **Site** field, select **3**.</span></span>
34. <span data-ttu-id="7c55f-158">في حقل **المستودع‏‎**، حدد **31**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-158">In the **Warehouse** field, select **31**.</span></span>
35. <span data-ttu-id="7c55f-159">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-159">Select **Save**</span></span>
35. <span data-ttu-id="7c55f-160">حدد **جديد** ضمن علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-160">Select **New** on the **Lines** FastTab.</span></span>
36. <span data-ttu-id="7c55f-161">تأكد أن حقل **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-161">Verify that the **Sequence number** field is **1**.</span></span>
37. <span data-ttu-id="7c55f-162">أدخل **1000** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-162">Enter **1000** in the **To quantity** field.</span></span>
38. <span data-ttu-id="7c55f-163">حدد **بلا‬** في الحقل **تحديد موقع الكمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-163">Select **None** in the **Locate quantity** field.</span></span>
39. <span data-ttu-id="7c55f-164">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-164">Select **Save**</span></span>
39. <span data-ttu-id="7c55f-165">قم بتوسيع علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-165">Expand the **Location Directive Actions** FastTab.</span></span>
40. <span data-ttu-id="7c55f-166">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-166">Select **New**.</span></span>
41. <span data-ttu-id="7c55f-167">في حقل **الاسم**، أدخل **مجمع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-167">Enter **Bulk** in the **Name** field.</span></span>
42. <span data-ttu-id="7c55f-168">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-168">Select **Save**.</span></span>
43. <span data-ttu-id="7c55f-169">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-169">Select **New** in the Action Pane.</span></span>
44. <span data-ttu-id="7c55f-170">أدخل **مشكلة وضع التحويل** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-170">Enter **Transfer Issue-Put** in the **Name** field.</span></span>
45. <span data-ttu-id="7c55f-171">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-171">Select **Put** in the **Work type** field.</span></span>
46. <span data-ttu-id="7c55f-172">في حقل **الموقع**، حدد **3**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-172">In the **Site** field, select **3**.</span></span>
47. <span data-ttu-id="7c55f-173">حدد **32** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-173">In the **Warehouse** field, select **32**.</span></span>
48. <span data-ttu-id="7c55f-174">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-174">Select **Save**</span></span>
48. <span data-ttu-id="7c55f-175">ضمن علامة التبويب السريعة **البنود**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-175">Select **New** in the **Lines** FastTab.</span></span>
49. <span data-ttu-id="7c55f-176">تأكد أن حقل **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-176">Verify that the **Sequence number** field is **1**.</span></span>
50. <span data-ttu-id="7c55f-177">أدخل **1000** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-177">Enter **1000** in the **To quantity** field.</span></span>
51. <span data-ttu-id="7c55f-178">حدد **بلا‬** في الحقل **تحديد موقع الكمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-178">Select **None** in the **Locate quantity** field.</span></span>
52. <span data-ttu-id="7c55f-179">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-179">Select **Save**</span></span>
52. <span data-ttu-id="7c55f-180">قم بتوسيع علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-180">Expand the **Location Directive Actions** FastTab.</span></span>
53. <span data-ttu-id="7c55f-181">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-181">Select **New**.</span></span>
54. <span data-ttu-id="7c55f-182">في حقل **الاسم**، أدخل **مجمع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-182">Enter **Bulk** in the **Name** field.</span></span>
55. <span data-ttu-id="7c55f-183">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-183">Select **Save**.</span></span>

### <a name="set-up-work-classes"></a><span data-ttu-id="7c55f-184">إعداد فئات العمل</span><span class="sxs-lookup"><span data-stu-id="7c55f-184">Set up Work classes</span></span>

1.  <span data-ttu-id="7c55f-185">انتقل إلى **إدارة المستودعات > إعداد > العمل > فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-185">Go to **Warehouse management > Setup > Work > Work classes**.</span></span>
2.  <span data-ttu-id="7c55f-186">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-186">Select **New**.</span></span>
3.   <span data-ttu-id="7c55f-187">في الحقل **معرّف فئة العمل**، أدخل **تحويل 2**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-187">In the **Work class ID** field, enter **Transfer2**.</span></span>
4.   <span data-ttu-id="7c55f-188">في حقل **الوصف**، أدخل **‏‫تحويل‬**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-188">In the **Description** field, enter **Transfer**.</span></span>
5.   <span data-ttu-id="7c55f-189">في حقل **نوع أمر العمل**، حدد **مشكلة التحويل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-189">In the **Work order type** field, select **Transfer issue**.</span></span>
6.   <span data-ttu-id="7c55f-190">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-190">Select **Save**.</span></span>
7.   <span data-ttu-id="7c55f-191">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-191">Close the page.</span></span>

### <a name="set-up-a-location-profile"></a><span data-ttu-id="7c55f-192">إعداد ملف تعريف الموقع</span><span class="sxs-lookup"><span data-stu-id="7c55f-192">Set up a Location profile</span></span>
1.  <span data-ttu-id="7c55f-193">انتقل إلى **إدارة المستودعات > إعداد > المستودع‬‏‫ > ملفات تعريف الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-193">Go to **Warehouse management > Setup > Warehouse > Location profiles**.</span></span>
2.  <span data-ttu-id="7c55f-194">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-194">Select **New**.</span></span>
3.  <span data-ttu-id="7c55f-195">في حقل **معرّف ملف تعريف الموقع**، أدخل **PRODIN**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-195">In the **Location profile ID** field, enter **PRODIN**.</span></span>
4.  <span data-ttu-id="7c55f-196">في حقل **الاسم**، أدخل **الإنتاج في**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-196">In the **Name** field, enter **Production in**.</span></span>
5.  <span data-ttu-id="7c55f-197">في علامة التبويب السريعة **عام**، حدد **مجمع** في حقل **تنسيق الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-197">In the **General** FastTab, in the **Location format** field, select **BULK**.</span></span>
6.  <span data-ttu-id="7c55f-198">في حقل **نوع الموقع**، حدد **مجمع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-198">In the **Location type** field, select **BULK**.</span></span>
7.  <span data-ttu-id="7c55f-199">حدد **نعم** في حقل **‬‏‫استخدام تعقب لوحة الترخيص**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-199">In the **Use license plate tracking** field, select **Yes**.</span></span>
8.  <span data-ttu-id="7c55f-200">في الحقل **السماح بالأصناف المختلطة**، حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-200">In the **Allow mixed items** field, select **Yes**.</span></span>
9.  <span data-ttu-id="7c55f-201">في الحقل **السماح بحالات المخزون المختلطة**، حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-201">In the **Allow mixed inventory statuses** field, select **Yes**.</span></span>
10. <span data-ttu-id="7c55f-202">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-202">Close the page.</span></span> 


### <a name="set-up-a-work-template"></a><span data-ttu-id="7c55f-203">إعداد قالب عمل</span><span class="sxs-lookup"><span data-stu-id="7c55f-203">Set up a work template</span></span>

1.  <span data-ttu-id="7c55f-204">افتح **إدارة المستودعات > إعداد > العمل > قوالب العمل**</span><span class="sxs-lookup"><span data-stu-id="7c55f-204">Open **Warehouse management > Setup > Work > Work templates**.</span></span>
2.  <span data-ttu-id="7c55f-205">في حقل **نوع أمر العمل**، حدد **مشكلة التحويل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-205">In the **Work order type** field, select **Transfer issue**.</span></span>
3.  <span data-ttu-id="7c55f-206">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-206">Select **New**.</span></span>
 
    > [!NOTE]
    > <span data-ttu-id="7c55f-207">تظهر هذه الصفحة أخطاء بسبب الحقول المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-207">This page throws errors because of required fields.</span></span> <span data-ttu-id="7c55f-208">وبمجرد إدخال كافة المعلومات بشكل صحيح، يتم حل الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-208">Once all information is correctly entered, the errors are resolved.</span></span> <span data-ttu-id="7c55f-209">قم بإغلاق الخطأ ثم **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-209">Simply close the error and **Save**.</span></span>

4.  <span data-ttu-id="7c55f-210">أدخل **مشكلة أمر التحويل** في حقل **قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-210">Enter **Transfer Order Issue** in the **Work template** field.</span></span>
5.  <span data-ttu-id="7c55f-211">أدخل **مشكلة التحويل** في حقل **وصف قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-211">Enter **Transfer Issue** in the **Work template description** field.</span></span>
6.  <span data-ttu-id="7c55f-212">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-212">Select **Save**.</span></span>
7.  <span data-ttu-id="7c55f-213">حدد **جديد** في منطقة **تفاصيل قالب العمل**</span><span class="sxs-lookup"><span data-stu-id="7c55f-213">Select **New** in the **Work Template Details** area.</span></span>
8.  <span data-ttu-id="7c55f-214">في الحقل **نوع العمل**، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-214">Select **Pick** in the **Work type** field.</span></span>
9.  <span data-ttu-id="7c55f-215">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-215">Select the **Mandatory** check box.</span></span>
10. <span data-ttu-id="7c55f-216">حدد **Transfer2** في حقل **معرّف فئة العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-216">Select **Transfer2** in the **Work class ID** field.</span></span>
11. <span data-ttu-id="7c55f-217">حدد **جديد** في منطقة **تفاصيل قالب العمل**</span><span class="sxs-lookup"><span data-stu-id="7c55f-217">Select **New** in the **Work Template Details** area.</span></span>
12. <span data-ttu-id="7c55f-218">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-218">Select **Put** in the **Work type** field.</span></span>
13. <span data-ttu-id="7c55f-219">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-219">Select the **Mandatory** check box.</span></span>
14. <span data-ttu-id="7c55f-220">حدد **Transfer2** في حقل **معرّف فئة العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-220">Select **Transfer2** in the **Work class ID** field.</span></span>
15. <span data-ttu-id="7c55f-221">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-221">Select **Save**.</span></span>
16. <span data-ttu-id="7c55f-222">تأكد من تحديد خانة الاختيار **صالح‬** في علامة التبويب **نظرة عامة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-222">Verify that the **Valid** check box on the **Overview** tab is now selected.</span></span>
17. <span data-ttu-id="7c55f-223">حدد **إيصال استلام التحويل** في حقل **نوع أمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-223">In the **Work order type** field, select **Transfer receipt**.</span></span>
18. <span data-ttu-id="7c55f-224">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-224">Select **New** in the Action Pane.</span></span>
19. <span data-ttu-id="7c55f-225">في الحقل **قالب العمل**، أدخل **32 حتى الاستلام**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-225">Enter **32 TO Receipt** in the **Work template** field.</span></span>
20. <span data-ttu-id="7c55f-226">أدخل **مشكلة التحويل** في حقل **وصف قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-226">Enter **Transfer Issue** in the **Work template description** field.</span></span>
21. <span data-ttu-id="7c55f-227">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-227">Select **Save**.</span></span>
22. <span data-ttu-id="7c55f-228">حدد **جديد** في منطقة **تفاصيل قالب العمل**</span><span class="sxs-lookup"><span data-stu-id="7c55f-228">Select **New** in the **Work Template Details** area.</span></span>
23. <span data-ttu-id="7c55f-229">في الحقل **نوع العمل**، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-229">Select **Pick** in the **Work type** field.</span></span>
24. <span data-ttu-id="7c55f-230">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-230">Select the **Mandatory** check box.</span></span>
25. <span data-ttu-id="7c55f-231">في الحقل **معرّف فئة العمل**، أدخل **تحويل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-231">Select **Transfer** in the **Work class ID** field.</span></span>
26. <span data-ttu-id="7c55f-232">حدد **جديد** في منطقة **تفاصيل قالب العمل**</span><span class="sxs-lookup"><span data-stu-id="7c55f-232">Select **New** in the **Work Template Details** area.</span></span>
27. <span data-ttu-id="7c55f-233">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-233">Select **Put** in the **Work type** field.</span></span>
28. <span data-ttu-id="7c55f-234">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-234">Select the **Mandatory** check box.</span></span>
29. <span data-ttu-id="7c55f-235">في الحقل **معرّف فئة العمل**، أدخل **تحويل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-235">Select **Transfer** in the **Work class ID** field.</span></span>
30. <span data-ttu-id="7c55f-236">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-236">Select **Save**.</span></span>
31. <span data-ttu-id="7c55f-237">تأكد من تحديد خانة الاختيار **صالح**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-237">Verify that the **Valid** check box is now selected.</span></span>
32. <span data-ttu-id="7c55f-238">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="7c55f-238">Close the pages.</span></span>


## <a name="set-up-replenishment"></a><span data-ttu-id="7c55f-239">إعداد التزويد</span><span class="sxs-lookup"><span data-stu-id="7c55f-239">Set up replenishment</span></span>

<span data-ttu-id="7c55f-240">لقد تمت مطالبتك بإجراء إعداد التزويد للمستودع 30 من مستودعات Contoso لعصير البرتقال.</span><span class="sxs-lookup"><span data-stu-id="7c55f-240">You have been asked to perform the replenishment setup for Warehouse 30 for Contoso Orange Juice.</span></span>

### <a name="set-up-mobile-device-menu-items-and-menu"></a><span data-ttu-id="7c55f-241">إعداد قوائم وأصناف قوائم الأجهزة المحمولة</span><span class="sxs-lookup"><span data-stu-id="7c55f-241">Set up mobile device menu items and menu</span></span>

1.  <span data-ttu-id="7c55f-242">افتح **إدارة المستودعات > إعداد > الجهاز المحمول > أصناف قوائم الأجهزة المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-242">Open **Warehouse management > Setup > Mobile device > Mobile device menu items**.</span></span>
2.  <span data-ttu-id="7c55f-243">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-243">Select **New**.</span></span>
3.  <span data-ttu-id="7c55f-244">أدخل **تزويد** في حقل **اسم صنف القائمة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-244">Enter **Replenishment** in the **Menu item name** field.</span></span>
4.  <span data-ttu-id="7c55f-245">في حقل **العنوان**، أدخل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-245">Enter **Replenishment** in the **Title** field.</span></span>
5.  <span data-ttu-id="7c55f-246">حدد **عمل** في الحقل **الوضع‬‏‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-246">Select **Work** in the **Mode** field.</span></span>
6.  <span data-ttu-id="7c55f-247">قم بتعيين شريط التمرير **‏‫استخدام العمل الموجود‬** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-247">Set the **Use existing work** slider to **Yes**.</span></span>
7.  <span data-ttu-id="7c55f-248">حدد **جديد** في علامة التبويب السريعة **‏‫فئات العمل‬**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-248">Select **New** on the **Work classes** FastTab.</span></span>
8.  <span data-ttu-id="7c55f-249">في رأس عمود **معرّف فئة العمل**، انقر بزر الماوس الأيمن على السهم لأسفل في الحقل وحدد **عرض التفاصيل** لفتح صفحة **فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-249">In the **Work class ID** column header, right-click the down arrow in the field and select **View details** to open the **Work classes** page.</span></span>
9.  <span data-ttu-id="7c55f-250">حدد **جديد** في صفحة **فئات العمل** ضمن جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-250">In the **Work classes** page, select **New** in the Action Pane.</span></span> 
10.  <span data-ttu-id="7c55f-251">في الحقل **معرّف فئة العمل**، أدخل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-251">In the **Work class ID** field, enter **Replenish**.</span></span>
11.  <span data-ttu-id="7c55f-252">في القائمة المنسدلة **نوع أمر العمل**، حدد **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-252">In the **Work order type** dropdown menu, select **Replenishment**.</span></span>
12.  <span data-ttu-id="7c55f-253">في حقل **الوصف**، أدخل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-253">In the **Description** field, enter **Replenishment**.</span></span>
13.  <span data-ttu-id="7c55f-254">حدد **حفظ** في جزء الإجراءات ثم أغلق صفحة **فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-254">Select **Save** in the Action Pane and close the **Work classes** page.</span></span> <span data-ttu-id="7c55f-255">يجب الرجوع إلى صفحة **أصناف قوائم الأجهزة المحمول**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-255">You should be back on the **Mobile device menu items** page.</span></span> <span data-ttu-id="7c55f-256">تأكد من أن صنف القائمة **تزويد** لا يزال محدداً.</span><span class="sxs-lookup"><span data-stu-id="7c55f-256">Ensure the new **Replenishment** menu item is still selected.</span></span>
8.  <span data-ttu-id="7c55f-257">في علامة التبويب السريعة **فئات العمل**، حدد معرّف فئة العمل **تزويد** من القائمة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-257">In the **Work classes** FastTab, select the **Replenish** Work class ID from the list.</span></span>
9.  <span data-ttu-id="7c55f-258">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-258">Close the page.</span></span>
10. <span data-ttu-id="7c55f-259">افتح **إدارة المستودعات > إعداد > الجهاز المحمول > قائمة الأجهزة المحمولة** وحدد القائمة حيث ترغب في إضافة التزويد.</span><span class="sxs-lookup"><span data-stu-id="7c55f-259">Open **Warehouse management > Setup > Mobile device > Mobile device menu** and select the menu where you would like to add replenishment.</span></span>
11. <span data-ttu-id="7c55f-260">حدد **تحرير**</span><span class="sxs-lookup"><span data-stu-id="7c55f-260">Select **Edit**</span></span>
12. <span data-ttu-id="7c55f-261">حدد صنف القائمة **تزويد** من جزء **القوائم المتوفرة وأصناف القوائم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-261">Select the **Replenishment** menu item from the **Available menus and menu items** pane.</span></span>
13. <span data-ttu-id="7c55f-262">حدد السهم الاتجاهي الأيمن لنقل **تزويد** إلى الجزء **بنية القائمة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-262">Select the right directional arrow to move **Replenishment** to the **Menu structure** pane.</span></span>
14. <span data-ttu-id="7c55f-263">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-263">Close the page.</span></span>


### <a name="set-up-a-work-template"></a><span data-ttu-id="7c55f-264">إعداد قالب عمل</span><span class="sxs-lookup"><span data-stu-id="7c55f-264">Set up a work template</span></span>

1.  <span data-ttu-id="7c55f-265">افتح **إدارة المستودعات > إعداد > العمل > قوالب العمل**</span><span class="sxs-lookup"><span data-stu-id="7c55f-265">Open **Warehouse management > Setup > Work > Work templates**.</span></span>
2.  <span data-ttu-id="7c55f-266">في الحقل **نوع أمر العمل**، حدد **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-266">In the **Work order type** field, select **Replenishment**.</span></span>
3.  <span data-ttu-id="7c55f-267">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-267">Select **New**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="7c55f-268">تظهر هذه الصفحة أخطاء بسبب الحقول المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-268">This page throws errors because of required fields.</span></span> <span data-ttu-id="7c55f-269">وبمجرد إدخال كافة المعلومات بشكل صحيح، يتم حل الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-269">Once all information is correctly entered, the errors are resolved.</span></span> <span data-ttu-id="7c55f-270">قم بإغلاق الخطأ ثم **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-270">Simply close the error and **Save**.</span></span>

4.  <span data-ttu-id="7c55f-271">أدخل **تزويد** في الحقل **قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-271">Enter **Replenish** in the **Work template** field.</span></span>
5.  <span data-ttu-id="7c55f-272">في الحقل **وصف قالب العمل**، أدخل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-272">Enter **Replenish** in the **Work template description** field.</span></span>
6.  <span data-ttu-id="7c55f-273">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-273">Select **Save**</span></span>
7.  <span data-ttu-id="7c55f-274">حدد **جديد** في القسم **تفاصيل قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-274">Select **New** in the **Work Template Details** section.</span></span>
8.  <span data-ttu-id="7c55f-275">في الحقل **نوع العمل**، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-275">Select **Pick** in the **Work type** field.</span></span>
9.  <span data-ttu-id="7c55f-276">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-276">Select the **Mandatory** check box.</span></span>
10. <span data-ttu-id="7c55f-277">في الحقل **معرّف فئة العمل**، حدد **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-277">Select **Replenish** in the **Work class ID** field.</span></span>
11. <span data-ttu-id="7c55f-278">حدد **جديد** في القسم **تفاصيل قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-278">Select **New** in the **Work Template Details** section.</span></span>
12. <span data-ttu-id="7c55f-279">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-279">Select **Put** in the **Work type** field.</span></span>
13. <span data-ttu-id="7c55f-280">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-280">Select the **Mandatory** check box.</span></span>
14. <span data-ttu-id="7c55f-281">في الحقل **معرّف فئة العمل**، حدد **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-281">Select **Replenish** in the **Work class ID** field.</span></span>
15. <span data-ttu-id="7c55f-282">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-282">Close the page.</span></span>


### <a name="set-up-a-location-directive"></a><span data-ttu-id="7c55f-283">إعداد التوجيه الخاص بالموقع</span><span class="sxs-lookup"><span data-stu-id="7c55f-283">Set up a location directive</span></span>

1.  <span data-ttu-id="7c55f-284">افتح **إدارة المستودعات > إعداد > توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-284">Open **Warehouse management > Setup > Location directives**.</span></span>
2.  <span data-ttu-id="7c55f-285">حدد **تزويد** في حقل **نوع أمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-285">Select **Replenishment** in the **Work order type** field.</span></span>
3.  <span data-ttu-id="7c55f-286">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-286">Select **New**.</span></span>
4.  <span data-ttu-id="7c55f-287">أدخل **تزويد** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-287">Enter **Replenish** in the **Name** field.</span></span>
5.  <span data-ttu-id="7c55f-288">في الحقل **نوع العمل**، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-288">Select **Pick** in the **Work type** field.</span></span>
6.  <span data-ttu-id="7c55f-289">حدد **3** في حقل **الموقع‏‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-289">Select **3** in the **Site** field.</span></span>
7.  <span data-ttu-id="7c55f-290">حدد **32** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-290">Select **32** in the **Warehouse** field.</span></span>
8.  <span data-ttu-id="7c55f-291">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-291">Select **Save**</span></span>
8.  <span data-ttu-id="7c55f-292">حدد **جديد** ضمن علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-292">Select **New** on the **Lines** FastTab.</span></span>
9.  <span data-ttu-id="7c55f-293">تأكد أن **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-293">Verify that the **Sequence number** is **1**.</span></span>
10. <span data-ttu-id="7c55f-294">أدخل **500** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-294">Enter **500** in the **To quantity** field.</span></span>
11. <span data-ttu-id="7c55f-295">في حقل **الوحدة**، أدخل **ea**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-295">Enter **ea** in the **Unit** field.</span></span>
12. <span data-ttu-id="7c55f-296">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-296">Select **Save**.</span></span>
13. <span data-ttu-id="7c55f-297">حدد **جديد** في علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-297">Select **New** on the **Location directive actions** FastTab.</span></span>
14. <span data-ttu-id="7c55f-298">أدخل **تزويد** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-298">Enter **Replenish** in the **Name** field.</span></span>
15. <span data-ttu-id="7c55f-299">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-299">Select **Save**.</span></span>
16. <span data-ttu-id="7c55f-300">حدد **تحرير استعلام** في علامة التبويب السريعة **إجراءات توجيه الموقع**، وليس في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-300">Select **Edit query** in the **Location Directive Actions** Fast Tab, not in the Action Pane.</span></span>
17. <span data-ttu-id="7c55f-301">حدد **إضافة** في صفحة **الاستعلام**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-301">Select **Add** on the **Query** page.</span></span>
18. <span data-ttu-id="7c55f-302">حدد **المواقع** في عمود **الجدول**، إذا لم يتم ملئها تلقائياً بـ **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-302">Select **Locations** in the **Table** column, if it does not automatically populate with **Locations**.</span></span>
19. <span data-ttu-id="7c55f-303">حدد **المواقع** في **الجدول المشتق**، إذا لم يتم ملئها تلقائياً بـ **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-303">Select  **Locations** in the **Derived table** if it does not automatically populate with **Locations**</span></span> 
19. <span data-ttu-id="7c55f-304">حدد **معرّف ملف تعريف الموقع** ضمن عمود **الحقل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-304">Select **Location profile ID** in the **Field** column.</span></span>
20. <span data-ttu-id="7c55f-305">حدد **مجمع** في عمود **المعايير**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-305">Select **BULK** in the **Criteria** column.</span></span>
21. <span data-ttu-id="7c55f-306">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-306">Select **OK**.</span></span>
22. <span data-ttu-id="7c55f-307">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-307">Select **New** in the Action Pane.</span></span>
23. <span data-ttu-id="7c55f-308">في حقل **الاسم**، أدخل **تزويد وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-308">Enter **Replenish Put** in the **Name** field.</span></span>
24. <span data-ttu-id="7c55f-309">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-309">Select **Put** in the **Work type** field.</span></span>
25. <span data-ttu-id="7c55f-310">حدد **3** في حقل **الموقع‏‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-310">Select **3** in the **Site** field.</span></span>
26. <span data-ttu-id="7c55f-311">حدد **32** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-311">Select **32** in the **Warehouse** field.</span></span>
27. <span data-ttu-id="7c55f-312">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-312">Select **Save**</span></span>
27. <span data-ttu-id="7c55f-313">حدد **جديد** ضمن علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-313">Select **New** on the **Lines** FastTab.</span></span>
28. <span data-ttu-id="7c55f-314">تأكد أن **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-314">Verify that the **Sequence number** is **1**.</span></span>
29. <span data-ttu-id="7c55f-315">أدخل **500** في حقل **لكل كمية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-315">Enter **500** in the **To quantity** field.</span></span>
30. <span data-ttu-id="7c55f-316">في حقل **الوحدة**، أدخل **ea**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-316">Enter **ea** in the **Unit** field.</span></span>
31. <span data-ttu-id="7c55f-317">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-317">Select **Save**.</span></span>
32. <span data-ttu-id="7c55f-318">حدد **جديد** في علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-318">Select **New** on the **Location Directive Actions** FastTab.</span></span>
33. <span data-ttu-id="7c55f-319">في حقل **الاسم**، أدخل **تزويد وضع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-319">Enter **Replenish Put** in the **Name** field.</span></span>
34. <span data-ttu-id="7c55f-320">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-320">Select **Save**.</span></span>
35. <span data-ttu-id="7c55f-321">حدد **تحرير استعلام** في علامة التبويب السريعة **إجراءات توجيه الموقع**، وليس في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7c55f-321">Select **Edit query** in the **Location Directive Actions** Fast Tab, not in the Action Pane.</span></span>
36. <span data-ttu-id="7c55f-322">حدد **إضافة** في صفحة **الاستعلام**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-322">Select **Add** on the **Query** page.</span></span>
37. <span data-ttu-id="7c55f-323">حدد **المواقع** في عمود **الجدول المشتق**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-323">Select **Locations** in the **Derived table** column.</span></span>
38. <span data-ttu-id="7c55f-324">حدد **معرّف ملف تعريف الموقع** ضمن عمود **الحقل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-324">Select **Location profile ID** in the **Field** column.</span></span>
39. <span data-ttu-id="7c55f-325">حدد **PRODIN** في عمود **المعايير**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-325">Select **PRODIN** in the **Criteria** column.</span></span>
40. <span data-ttu-id="7c55f-326">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-326">Select **OK**.</span></span>
41. <span data-ttu-id="7c55f-327">قم بإغلاق صفحة **توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-327">Close the **Location directives** page.</span></span>


### <a name="set-up-a-wave-template"></a><span data-ttu-id="7c55f-328">إعداد قالب موجة</span><span class="sxs-lookup"><span data-stu-id="7c55f-328">Set up a wave template</span></span>

1. <span data-ttu-id="7c55f-329">افتح **إدارة المستودعات > إعداد > الموجات > قوالب الموجات**</span><span class="sxs-lookup"><span data-stu-id="7c55f-329">Open **Warehouse management > Setup > Waves > Wave templates**.</span></span>
2. <span data-ttu-id="7c55f-330">حدد **الشحن** في الحقل **نوع قالب الموجة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-330">Select **Shipping** in the **Wave template type** field.</span></span>
3. <span data-ttu-id="7c55f-331">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-331">Select **New**.</span></span>
4. <span data-ttu-id="7c55f-332">في الحقل **اسم قالب الموجة**، أدخل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-332">Enter **30 Replenish** in the **Wave template name** field.</span></span>
5. <span data-ttu-id="7c55f-333">في الحقل **وصف قالب الموجة**، أدخل **30 تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-333">Enter **30 Replenish** in the **Wave template description** field.</span></span>
6. <span data-ttu-id="7c55f-334">حدد **3** في حقل **الموقع‏‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-334">Select **3** in the **Site** field.</span></span>
7. <span data-ttu-id="7c55f-335">حدد **30** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-335">Select **30** in the **Warehouse** field.</span></span>
8. <span data-ttu-id="7c55f-336">قم بتعيين شرائط التمرير **التنفيذ التلقائي لإنشاء الموجات** و **معالجة الموجة عند الإصدار إلى المستودع** و **التنفيذ التلقائي لإصدار الموجة** و **‬‏‫التنفيذ التلقائي لإصدار عمل التزويد** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-336">Set the **Automate wave creation**, **Process wave at release to warehouse**, **Automate wave release**, and **Automate replenishment work release** sliders to **Yes**.</span></span>
9. <span data-ttu-id="7c55f-337">قم بتوسيع علامة التبويب السريعة **الأساليب** وتأكد من تحديد الأساليب **إنشاء الأحمال** و **تخصيص الموجات** و **إنشاء العمل**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-337">Expand the **Methods** FastTab and verify that the **createLoads**,  **allocateWave**, and **createWork** methods are selected.</span></span>
10. <span data-ttu-id="7c55f-338">حدد **تزويد** من الجزء **الأساليب المتبقية**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-338">Select **Replenish** from the **Remaining methods** pane.</span></span>
11. <span data-ttu-id="7c55f-339">حدد السهم الاتجاهي الأيمن لنقل **تزويد** إلى الجزء **الأساليب المحددة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-339">Select the right directional arrow to move **Replenish** to the  **Selected methods** pane.</span></span>

    > [!NOTE]
    > <span data-ttu-id="7c55f-340">إذا تلقيت خطأ مضمونه "يعتبر رمز خطوة الموجة إلزامياً"، تجاهله وتأكد من إضافة **تزويد** إلى الأساليب المحددة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-340">If you receive an error saying “Wave step code is mandatory”, ignore it and confirm that that **Replenish** has been added to the selected methods.</span></span> 

12. <span data-ttu-id="7c55f-341">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-341">Close the page.</span></span>


### <a name="set-up-a-replenishment-template"></a><span data-ttu-id="7c55f-342">إعداد قالب تزويد</span><span class="sxs-lookup"><span data-stu-id="7c55f-342">Set up a replenishment template</span></span>

1.  <span data-ttu-id="7c55f-343">افتح **إدارة المستودعات > إعداد > تزويد > قوالب التزويد**</span><span class="sxs-lookup"><span data-stu-id="7c55f-343">Open **Warehouse management > Setup > Replenishment > Replenishment templates**.</span></span>
2.  <span data-ttu-id="7c55f-344">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-344">Select **New**.</span></span>
3.  <span data-ttu-id="7c55f-345">في الحقل **قالب التزويد**، أدخل **طلب تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-345">Enter **Rep Demand** in the **Replenish template** field.</span></span>
4.  <span data-ttu-id="7c55f-346">في الحقل **الوصف**، أدخل **طلب تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-346">Enter **Replenish Demand** in the **Description** field.</span></span>
5.  <span data-ttu-id="7c55f-347">في الحقل **نوع التزويد**، حدد **طلب موجة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-347">In the **Replenishment type** field, select **Wave demand**.</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="7c55f-348">ستحتاج إلى إعداد رمز الموجة للخطوة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-348">You will need to setup a wave step code.</span></span> <span data-ttu-id="7c55f-349">في حقل البحث أعلى الشاشة، أدخل **رموز خطوة الموجة** ضمن الصفحة الظاهرة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-349">In the search field at the top, enter **wave step codes** and the page will appear.</span></span>  <span data-ttu-id="7c55f-350">في الصفحة **رموز خطوة الموجة**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-350">Select **New** in the **Wave step codes** page.</span></span> <span data-ttu-id="7c55f-351">أدخل **200** في **رمز خطوة الموجة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-351">Enter **200** in the **Wave step code**.</span></span> <span data-ttu-id="7c55f-352">في الحقل **وصف خطوة الموجة**، أدخل **تزويد**، وحدد **تزويد** في **نوع خطوة الموجة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-352">Enter **Replenish** in the **Wave step description** field, and select **Replenishment** in the **Wave step type**.</span></span> <span data-ttu-id="7c55f-353">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-353">Close the page.</span></span>

6.   <span data-ttu-id="7c55f-354">قم بالرجوع إلى **قوالب التزويد** وحدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-354">Return to the **Replenishment templates** and select **Edit**.</span></span>
6.  <span data-ttu-id="7c55f-355">حدد **200** في **رمز خطوة الموجة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-355">Select **200** in the **Wave step code** field.</span></span>
7.  <span data-ttu-id="7c55f-356">حدد **جديد** في القسم **تفاصيل قالب التزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-356">In the **Replenishment Template Details** section, select **New**.</span></span>
8.  <span data-ttu-id="7c55f-357">في حقل **الرقم التسلسلي**، أدخِل **1**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-357">In the **Sequence number** field, enter **1**.</span></span>
9.  <span data-ttu-id="7c55f-358">في الحقل **الوصف**، أدخل **طلب**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-358">In the **Description** field, enter **Demand**.</span></span>
10. <span data-ttu-id="7c55f-359">في حقل **وحدة التزويد**، أدخل **ea**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-359">In the **Replenishment unit** field, enter **ea**.</span></span>
11. <span data-ttu-id="7c55f-360">في الحقل **قالب العمل**، أدخل **تزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-360">In the **Work template** field, select **Replenish**.</span></span>
12. <span data-ttu-id="7c55f-361">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="7c55f-361">Select **Save**</span></span>
12. <span data-ttu-id="7c55f-362">حدد **تحديد المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-362">Select **Select products**.</span></span>
13. <span data-ttu-id="7c55f-363">في الصفحة **استعلام المنتج**، أدخل **P9500** في الحقل **المعايير**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-363">On the **Product query** page, enter **P9500** in the **Criteria** field.</span></span>
14. <span data-ttu-id="7c55f-364">حدد **موافق**</span><span class="sxs-lookup"><span data-stu-id="7c55f-364">Select **OK**</span></span>
15. <span data-ttu-id="7c55f-365">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-365">Close the page.</span></span>
14. <span data-ttu-id="7c55f-366">افتح **إدارة المستودعات > إعداد > الموجات > قوالب الموجات**</span><span class="sxs-lookup"><span data-stu-id="7c55f-366">Open **Warehouse management > Setup > Waves > Wave templates**.</span></span>
15. <span data-ttu-id="7c55f-367">حدد **30 تزويد** من قائمة قوالب الموجات.</span><span class="sxs-lookup"><span data-stu-id="7c55f-367">Select **30 Replenish** from the list of wave templates.</span></span>
16. <span data-ttu-id="7c55f-368">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-368">Select **Edit**.</span></span>
17. <span data-ttu-id="7c55f-369">في الجزء **الأساليب المحددة**، حدد الأسلوب تزويد وادخل **200** في الحقل **رمز خطوة الموجة**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-369">In the **Selected Methods** pane, select the replenish method and enter **200** in the **Wave step code** field.</span></span>
18. <span data-ttu-id="7c55f-370">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-370">Select **Save**.</span></span>
19. <span data-ttu-id="7c55f-371">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-371">Close the page.</span></span>


## <a name="run-replenishment-for-a-load-demand"></a><span data-ttu-id="7c55f-372">تشغيل التزويد لطلب التحميل</span><span class="sxs-lookup"><span data-stu-id="7c55f-372">Run replenishment for a load demand</span></span>

<span data-ttu-id="7c55f-373">لقد تمت مطالبتك بتشغيل التزويد لطلب تحميل مستودع Contoso لعصير البرتقال، مرة واحدة في كل يوم من أيام العمل للأسابيع الستة القادمة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-373">You have been asked to run replenishment for a load demand for Contoso Orange Juice, once a day on every workday for the next six weeks.</span></span> <span data-ttu-id="7c55f-374">يستخدم في إعداد عمليات التزويد المتكرر.</span><span class="sxs-lookup"><span data-stu-id="7c55f-374">Set up the recurring replenishment.</span></span>

1.  <span data-ttu-id="7c55f-375">افتح **إدارة المستودعات > تزويد > ‏‫تزويد طلب الحمل‬**</span><span class="sxs-lookup"><span data-stu-id="7c55f-375">Open **Warehouse management > Replenishment > Load demand replenishment**.</span></span>
2.  <span data-ttu-id="7c55f-376">في الصفحة **تزويد طلب الحمل**، حدد **طلب تزويد** في الحقل **قالب التزويد**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-376">On the **Load demand replenishment** page, select **Rep Demand** in the **Replenish template** field.</span></span>
3.  <span data-ttu-id="7c55f-377">قم بتوسيع علامة التبويب السريعة **تشغيل في الخلفية**</span><span class="sxs-lookup"><span data-stu-id="7c55f-377">Expand the **Run in the background** FastTab.</span></span>
4.  <span data-ttu-id="7c55f-378">قم بتعيين شريط التمرير **معالجة الدفعة**، إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-378">Set the **Batch processing** slider to **Yes**.</span></span>
5.  <span data-ttu-id="7c55f-379">حدد علامة التبويب **التكرار‬**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-379">Select the **Recurrence** tab.</span></span>
6.  <span data-ttu-id="7c55f-380">في الصفحة **تحديد التكرار**، أدخل تاريخ اليوم في الحقل **تاريخ البدء**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-380">On the **Define recurrence** page, enter today's date in the **Start date** field.</span></span>
7.  <span data-ttu-id="7c55f-381">في حقل **وقت البدء**، أدخل **7:00 مساءً**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-381">In the **Start time** field, enter **7:00 PM**.</span></span>
8.  <span data-ttu-id="7c55f-382">حدد زر **الانتهاء في** وأدخل تاريخ ستة أسابيع من تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="7c55f-382">Select the **End by** button and enter a date six weeks from today's date.</span></span>
9.  <span data-ttu-id="7c55f-383">في الجزء **نمط التكرار**، حدد الزر **الأيام**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-383">In the **Recurrence Pattern** area, select the **Days** button.</span></span>
10. <span data-ttu-id="7c55f-384">حدد الزر **كل يوم من أيام الأسبوع**.</span><span class="sxs-lookup"><span data-stu-id="7c55f-384">Select the **Every weekday** button.</span></span>
11. <span data-ttu-id="7c55f-385">حدد **موافق** مرتين.</span><span class="sxs-lookup"><span data-stu-id="7c55f-385">Select **OK** twice.</span></span>
12. <span data-ttu-id="7c55f-386">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7c55f-386">Close the page.</span></span> 



