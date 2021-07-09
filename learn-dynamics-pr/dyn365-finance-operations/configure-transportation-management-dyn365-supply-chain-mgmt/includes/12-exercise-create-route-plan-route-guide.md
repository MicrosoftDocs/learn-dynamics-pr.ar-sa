---
ms.openlocfilehash: f59fad3680928fea36ae4f2c605a727516635ad3
ms.sourcegitcommit: b9be1fa219842266c6aecd648ba283550b2f271f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/21/2020
ms.locfileid: "6073567"
---
## <a name="scenario---create-a-route-plan"></a><span data-ttu-id="300dc-101">السيناريو - إنشاء خطة توجيه</span><span class="sxs-lookup"><span data-stu-id="300dc-101">Scenario - Create a route plan</span></span>

<span data-ttu-id="300dc-102">كعضو في فريق مشروع إدارة سلاسل التوريد لدورات العمل الوطنية، فإنك بحاجة إلى تكوين خطة توجيه جديدة من جورجيا إلى لوس أنجلوس والولايات المتحدة الأمريكية.</span><span class="sxs-lookup"><span data-stu-id="300dc-102">As a member of the Supply Chain Management project team for Adventure works cycles, you need to configure a new route plan from Georgia, US to Los Angeles, US.</span></span> <span data-ttu-id="300dc-103">ستحتاج أيضاً إلى إنشاء مركز جديد للمستودعات في جورجيا ولوس أنجلوس.</span><span class="sxs-lookup"><span data-stu-id="300dc-103">You will also need to create a new hub for the warehouses at Georgia and Los Angeles.</span></span> 

### <a name="create-a-new-route-plan-named-ga-to-la"></a><span data-ttu-id="300dc-104">قم بإنشاء خطة توجيه جديدة باسم "GA إلى LA"</span><span class="sxs-lookup"><span data-stu-id="300dc-104">Create a new route plan named "GA to LA"</span></span>

1.  <span data-ttu-id="300dc-105">في **USMF**، افتح **إدارة النقل > إعداد > التوجيه > خطط التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="300dc-105">In **USMF**, open **Transportation management > Setup > Routing > Route plans**.</span></span>
2.  <span data-ttu-id="300dc-106">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="300dc-106">Select **New**.</span></span>
3.  <span data-ttu-id="300dc-107">في الحقل **خطة التوجيه**، أدخل **GA إلى LA**.</span><span class="sxs-lookup"><span data-stu-id="300dc-107">In the **Route plan** field, enter **GA to LA**.</span></span>
4.  <span data-ttu-id="300dc-108">في الحقل **الاسم**، أدخل **جورجيا إلى لوس أنجلوس**.</span><span class="sxs-lookup"><span data-stu-id="300dc-108">In the **Name** field, enter **Georgia to Los Angeles**.</span></span>
5.  <span data-ttu-id="300dc-109">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="300dc-109">Close the page.</span></span>

### <a name="create-new-hubs-for-georgia-and-los-angeles"></a><span data-ttu-id="300dc-110">إنشاء مراكز جديدة لجورجيا ولوس أنجلوس</span><span class="sxs-lookup"><span data-stu-id="300dc-110">Create new hubs for Georgia and Los Angeles</span></span>

1.  <span data-ttu-id="300dc-111">افتح **إدارة النقل > إعداد > التوجيه > أصول الموزّعات**.</span><span class="sxs-lookup"><span data-stu-id="300dc-111">Open **Transportation management > Setup > Routing > Hub masters**.</span></span>
2.  <span data-ttu-id="300dc-112">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="300dc-112">Select **New** on the Action Pane.</span></span>
3.  <span data-ttu-id="300dc-113">في الحقل **المركز**، أدخل **جورجيا 3**.</span><span class="sxs-lookup"><span data-stu-id="300dc-113">In the **Hub** field, enter **Georgia 3**.</span></span>
4.  <span data-ttu-id="300dc-114">في الحقل **الاسم**، أدخل **Savannah GA**.</span><span class="sxs-lookup"><span data-stu-id="300dc-114">In the **Name** field, enter **Savannah GA**.</span></span>
5.  <span data-ttu-id="300dc-115">قم بتوسيع علامة التبويب السريعة **الرموز**.</span><span class="sxs-lookup"><span data-stu-id="300dc-115">Expand the **Codes** FastTab.</span></span>
6.  <span data-ttu-id="300dc-116">في حقل **نوع المركز**، حدد **مركز**.</span><span class="sxs-lookup"><span data-stu-id="300dc-116">In the **Hub type** field, select **Hub**.</span></span>
7.  <span data-ttu-id="300dc-117">في حقل **السعر الرئيسي**، حدد **TruckRateMaster**.</span><span class="sxs-lookup"><span data-stu-id="300dc-117">In the **Rate master** field, select **TruckRateMaster**.</span></span>
8.  <span data-ttu-id="300dc-118">قم بتوسيع علامة التبويب السريعة **تواريخ السريان**.</span><span class="sxs-lookup"><span data-stu-id="300dc-118">Expand the **Effective dates** FastTab.</span></span>
9.  <span data-ttu-id="300dc-119">في حقل **تاريخ ووقت البدء الساري**، حدد **اليوم**.</span><span class="sxs-lookup"><span data-stu-id="300dc-119">In the **Effective start date and time** field, select **Today**.</span></span>
10. <span data-ttu-id="300dc-120">في الحقل **تاريخ ووقت الانتهاء الساري**، حدد شهراً من تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="300dc-120">In the **Effective end date and time** field, select a month from today's date.</span></span>
11. <span data-ttu-id="300dc-121">قم بتوسيع علامة التبويب السريعة **العنوان**.</span><span class="sxs-lookup"><span data-stu-id="300dc-121">Expand the **Address** FastTab.</span></span>
12. <span data-ttu-id="300dc-122">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="300dc-122">Select **Add**.</span></span>
13. <span data-ttu-id="300dc-123">في الحقل **الاسم أو الوصف**، أدخل **جورجيا 3**.</span><span class="sxs-lookup"><span data-stu-id="300dc-123">In the **Name or description** field, enter **Georgia 3**.</span></span>
14. <span data-ttu-id="300dc-124">في حقل **الرمز البريدي**، أدخل **31302**.</span><span class="sxs-lookup"><span data-stu-id="300dc-124">In the **Zip/postal code** field, enter **31302**.</span></span>
15. <span data-ttu-id="300dc-125">في حقل **الشارع**، أدخل **123 ABC Street**.</span><span class="sxs-lookup"><span data-stu-id="300dc-125">In the **Street** field, enter **123 ABC Street**.</span></span>
16. <span data-ttu-id="300dc-126">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="300dc-126">Select **OK**.</span></span>
17. <span data-ttu-id="300dc-127">حدد **جديد** في جزء الإجراءات لإنشاء سجل آخر.</span><span class="sxs-lookup"><span data-stu-id="300dc-127">Select **New** on the Action Pane to create another record.</span></span>
18. <span data-ttu-id="300dc-128">في الحقل **المركز**، أدخل **لوس أنجلوس 2**.</span><span class="sxs-lookup"><span data-stu-id="300dc-128">In the **Hub** field, enter **Los Angeles 2**.</span></span>
19. <span data-ttu-id="300dc-129">في الحقل **الاسم**، أدخل **لوس أنجلوس، كاليفورنيا 2**.</span><span class="sxs-lookup"><span data-stu-id="300dc-129">In the **Name** field, enter **Los Angeles CA 2**.</span></span>
20. <span data-ttu-id="300dc-130">قم بتوسيع علامة التبويب السريعة **الرموز**.</span><span class="sxs-lookup"><span data-stu-id="300dc-130">Expand the **Codes** FastTab.</span></span>
21. <span data-ttu-id="300dc-131">في حقل **نوع المركز**، حدد **مركز**.</span><span class="sxs-lookup"><span data-stu-id="300dc-131">In the **Hub type** field, select **Hub**.</span></span>
22. <span data-ttu-id="300dc-132">في حقل **السعر الرئيسي**، حدد **TruckRateMaster**.</span><span class="sxs-lookup"><span data-stu-id="300dc-132">In the **Rate master** field, select **TruckRateMaster**.</span></span>
23. <span data-ttu-id="300dc-133">قم بتوسيع علامة التبويب السريعة **تواريخ السريان**.</span><span class="sxs-lookup"><span data-stu-id="300dc-133">Expand the **Effective dates** FastTab.</span></span>
24. <span data-ttu-id="300dc-134">في حقل **تاريخ ووقت البدء الساري**، حدد **اليوم**.</span><span class="sxs-lookup"><span data-stu-id="300dc-134">In the **Effective start date and time** field, select **Today**.</span></span>
25. <span data-ttu-id="300dc-135">في الحقل **تاريخ ووقت الانتهاء الساري**، حدد شهراً من تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="300dc-135">In the **Effective end date and time** field, select a month from today's date.</span></span>
26. <span data-ttu-id="300dc-136">قم بتوسيع علامة التبويب السريعة **العنوان**.</span><span class="sxs-lookup"><span data-stu-id="300dc-136">Expand the **Address** FastTab.</span></span>
27. <span data-ttu-id="300dc-137">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="300dc-137">Select **Add**.</span></span>
28. <span data-ttu-id="300dc-138">في الحقل **الاسم أو الوصف**، أدخل **لوس أنجلوس 2**.</span><span class="sxs-lookup"><span data-stu-id="300dc-138">In the **Name or description** field, enter **Los Angeles 2**.</span></span>
29. <span data-ttu-id="300dc-139">في حقل **الرمز البريدي**، أدخل **90001**.</span><span class="sxs-lookup"><span data-stu-id="300dc-139">In the **Zip/postal code** field, enter **90001**.</span></span>
30. <span data-ttu-id="300dc-140">في حقل **الشارع**، أدخل **987 XYZ Avenue**.</span><span class="sxs-lookup"><span data-stu-id="300dc-140">In the **Street** field, enter **987 XYZ Avenue**.</span></span>
31. <span data-ttu-id="300dc-141">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="300dc-141">Select **OK**.</span></span>
32. <span data-ttu-id="300dc-142">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="300dc-142">Select **Save** on the Action Pane.</span></span>
32. <span data-ttu-id="300dc-143">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="300dc-143">Close the page.</span></span>

### <a name="add-details-to-the-route-plan"></a><span data-ttu-id="300dc-144">إضافة تفاصيل إلى خطة التوجيه</span><span class="sxs-lookup"><span data-stu-id="300dc-144">Add details to the route plan</span></span>

1.  <span data-ttu-id="300dc-145">افتح **إدارة النقل > إعداد > التوجيه > خطط التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="300dc-145">Open **Transportation management > Setup > Routing > Route plans**.</span></span>
2.  <span data-ttu-id="300dc-146">حدد خطة التوجيه **GA إلى LA**.</span><span class="sxs-lookup"><span data-stu-id="300dc-146">Select the **GA to LA** route plan.</span></span>
3.  <span data-ttu-id="300dc-147">حدد **تحرير** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="300dc-147">Select **Edit** on the Action Pane.</span></span>
3.  <span data-ttu-id="300dc-148">في علامة التبويب السريعة **التفاصيل**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="300dc-148">On the **Details** FastTab, select **New**.</span></span>
4.  <span data-ttu-id="300dc-149">في الحقل **المركز الأصلي**، حدد **جورجيا 3**.</span><span class="sxs-lookup"><span data-stu-id="300dc-149">In the **Origin hub** field, select **Georgia 3**.</span></span>
5.  <span data-ttu-id="300dc-150">في الحقل **المركز الوجهة**، حدد **لوس أنجلوس 2**.</span><span class="sxs-lookup"><span data-stu-id="300dc-150">In the **Destination hub** field, select **Los Angeles 2**.</span></span>
6.  <span data-ttu-id="300dc-151">في حقل **شركة الشحن**، حدد **ناقل عبر الشاحنات**.</span><span class="sxs-lookup"><span data-stu-id="300dc-151">In the **Shipping carrier** field, select **TruckCarrier**.</span></span>
7.  <span data-ttu-id="300dc-152">في حقل **خدمة النقل**، حدد **شاحنة**.</span><span class="sxs-lookup"><span data-stu-id="300dc-152">In the **Carrier service** field, select **Truck**.</span></span>
8.  <span data-ttu-id="300dc-153">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="300dc-153">Select **Save** on the Action Pane.</span></span>
8.  <span data-ttu-id="300dc-154">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="300dc-154">Close the page.</span></span>

## <a name="scenario---create-a-route-guide"></a><span data-ttu-id="300dc-155">السيناريو - إنشاء دليل توجيه</span><span class="sxs-lookup"><span data-stu-id="300dc-155">Scenario - Create a route guide</span></span> 

<span data-ttu-id="300dc-156">كعضو في فريق مشروع إدارة سلاسل التوريد لدورات العمل الوطنية، فإنك بحاجة إلى تكوين دليل توجيهي جديد من جورجيا إلى لوس أنجلوس والولايات المتحدة الأمريكية.</span><span class="sxs-lookup"><span data-stu-id="300dc-156">As a member of the Supply Chain Management project team for Adventure Works Cycles, you need to configure a new routing guide for Georgia to Los Angeles.</span></span> <span data-ttu-id="300dc-157">وينبغي أن يؤدي دليل التوجيه في نهاية المطاف إلى أن تكون النتيجة هي الناقل عبر الشاحنات، مع خدمة النقل باستخدام شاحنة.</span><span class="sxs-lookup"><span data-stu-id="300dc-157">The routing guide should ultimately lead to the result being the TruckCarrier shipping carrier, with the Truck carrier service.</span></span>

### <a name="create-a-new-route-guide-named-ga-to-la"></a><span data-ttu-id="300dc-158">قم بإنشاء دليل توجيه جديد باسم "GA إلى LA"</span><span class="sxs-lookup"><span data-stu-id="300dc-158">Create a new route guide named "GA to LA"</span></span>

1.  <span data-ttu-id="300dc-159">في **USMF**، افتح **إدارة النقل > إعداد > التوجيه > دلائل التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="300dc-159">In **USMF**, open **Transportation management > Setup > Routing > Route guides**.</span></span>
2.  <span data-ttu-id="300dc-160">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="300dc-160">Select **New** on the Action Pane.</span></span>
3.  <span data-ttu-id="300dc-161">في الحقل **دليل التوجيه**، أدخل **GA إلى LA**.</span><span class="sxs-lookup"><span data-stu-id="300dc-161">In the **Routing guide** field, enter **GA to LA**.</span></span>
4.  <span data-ttu-id="300dc-162">في الحقل **الاسم**، أدخل **جورجيا إلى لوس أنجلوس**.</span><span class="sxs-lookup"><span data-stu-id="300dc-162">In the **Name** field, enter **Georgia to Los Angeles**.</span></span>

### <a name="add-information-origin-destination-and-result-entities-to-the-routing-guide"></a><span data-ttu-id="300dc-163">إضافة معلومات وكيانات الأصل والوجهة والنتيجة إلى دليل التوجيه</span><span class="sxs-lookup"><span data-stu-id="300dc-163">Add Information, Origin, Destination, and Result entities to the routing guide</span></span>

1.  <span data-ttu-id="300dc-164">قم بتوسيع علامة التبويب السريعة **معلومات**.</span><span class="sxs-lookup"><span data-stu-id="300dc-164">Expand the **Information** FastTab.</span></span>
2.  <span data-ttu-id="300dc-165">في الحقل **الاتجاه**، حدد **صادر**.</span><span class="sxs-lookup"><span data-stu-id="300dc-165">In the **Direction** field, select **Outbound**.</span></span>
3.  <span data-ttu-id="300dc-166">قم بتعيين مؤشر التمرير **نشط** على الموضع **نعم**.</span><span class="sxs-lookup"><span data-stu-id="300dc-166">Set the **Active** slider to the **Yes** position.</span></span>
4.  <span data-ttu-id="300dc-167">في حقل **تاريخ ووقت البدء الساري**، حدد **اليوم**.</span><span class="sxs-lookup"><span data-stu-id="300dc-167">In the **Effective start date and time** field, select **Today**.</span></span>
5.  <span data-ttu-id="300dc-168">في الحقل **تاريخ ووقت الانتهاء الساري**، حدد شهراً من تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="300dc-168">In the **Effective end date and time** field, select a month from today's date.</span></span>
6.  <span data-ttu-id="300dc-169">قم بتوسيع علامة التبويب السريعة **الأصل**.</span><span class="sxs-lookup"><span data-stu-id="300dc-169">Expand the **Origin** FastTab.</span></span>
7.  <span data-ttu-id="300dc-170">في حقل **الرمز البريدي**، أدخل **31302**.</span><span class="sxs-lookup"><span data-stu-id="300dc-170">In the **Zip/postal code** field, enter **31302**.</span></span>
8.  <span data-ttu-id="300dc-171">في الحقل **المركز**، حدد **لوس أنجلوس 2**.</span><span class="sxs-lookup"><span data-stu-id="300dc-171">In the **Hub** field, select **Los Angeles 2**.</span></span>
9.  <span data-ttu-id="300dc-172">في الحقل **البلد/المنطقة**، أدخل **الولايات المتحدة الأمريكية**.</span><span class="sxs-lookup"><span data-stu-id="300dc-172">In the **Country/region** field, enter **USA**.</span></span>
10. <span data-ttu-id="300dc-173">قم بتوسيع علامة التبويب السريعة **الوجهة**.</span><span class="sxs-lookup"><span data-stu-id="300dc-173">Expand the **Destination** FastTab.</span></span>
11. <span data-ttu-id="300dc-174">في حقل **الرمز البريدي للمرسل**، أدخل **31302**.</span><span class="sxs-lookup"><span data-stu-id="300dc-174">In the **Zip/postal code from** field, enter **31302**.</span></span>
12. <span data-ttu-id="300dc-175">في حقل **الرمز البريدي للمستلم**، أدخل **90001**.</span><span class="sxs-lookup"><span data-stu-id="300dc-175">In the **Zip/postal code to** field, enter **90001**.</span></span>
13. <span data-ttu-id="300dc-176">في الحقل **المركز**، حدد **جورجيا 3**.</span><span class="sxs-lookup"><span data-stu-id="300dc-176">In the **Hub** field, select **Georgia 3**.</span></span>
14. <span data-ttu-id="300dc-177">في الحقل **البلد/المنطقة**، أدخل **الولايات المتحدة الأمريكية**.</span><span class="sxs-lookup"><span data-stu-id="300dc-177">In the **Country/region** field, enter **USA**.</span></span>
15. <span data-ttu-id="300dc-178">قم بتوسيع علامة التبويب السريعة **النتيجة**.</span><span class="sxs-lookup"><span data-stu-id="300dc-178">Expand the **Result** FastTab.</span></span>
16. <span data-ttu-id="300dc-179">في حقل **شركة الشحن**، حدد **ناقل عبر الشاحنات**.</span><span class="sxs-lookup"><span data-stu-id="300dc-179">In the **Shipping carrier** field, select **TruckCarrier**.</span></span>
17. <span data-ttu-id="300dc-180">في حقل **خدمة النقل**، حدد **شاحنة**.</span><span class="sxs-lookup"><span data-stu-id="300dc-180">In the **Carrier service** field, select **Truck**.</span></span>
