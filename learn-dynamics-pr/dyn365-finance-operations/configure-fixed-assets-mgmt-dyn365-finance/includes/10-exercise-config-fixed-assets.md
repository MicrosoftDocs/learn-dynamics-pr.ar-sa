---
ms.openlocfilehash: 82b99e5975395d6fc4ce2a76b6963af23a9f773b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070718"
---
## <a name="scenario"></a><span data-ttu-id="358c0-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="358c0-101">Scenario</span></span> 

<span data-ttu-id="358c0-102">باستخدام دور المحاسب، ستقوم بإعداد ملفات تعريف ترحيل الأصول الثابتة وأنواع الحركات المتعددة.</span><span class="sxs-lookup"><span data-stu-id="358c0-102">Using the Accountant role, you will set up fixed asset posting profiles and multiple transaction types.</span></span>  <span data-ttu-id="358c0-103">والأمثلة الموضحة في المعمل خاصة بملف تعريف الترحيل الأساسي، رغم أنه يجب إنشاء ملفات تعريف الترحيل لمخطط محدد للحسابات ومتطلبات التقارير المالية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="358c0-103">Examples given in the lab are for a basic posting profile, though posting profiles must be created for your specific chart of accounts and financial reporting requirements.</span></span>


## <a name="set-up-fixed-asset-posting-profiles"></a><span data-ttu-id="358c0-104">إعداد ملفات تعريف ترحيل الأصول الثابتة</span><span class="sxs-lookup"><span data-stu-id="358c0-104">Set up fixed asset posting profiles</span></span>

1.  <span data-ttu-id="358c0-105">في الشركة **USMF**، انتقل إلى **الأصول الثابتة > إعداد > ملفات تعريف ترحيل الأصول الثابتة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-105">In the **USMF** company, go to **Fixed assets > Setup > Fixed asset posting profiles**.</span></span>
2.  <span data-ttu-id="358c0-106">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="358c0-106">Select **New**.</span></span>
3.  <span data-ttu-id="358c0-107">في الحقل **ملف تعريف الترحيل**، اكتب **FAPP**.</span><span class="sxs-lookup"><span data-stu-id="358c0-107">In the **Posting profile** field, type **FAPP.**</span></span>
4.  <span data-ttu-id="358c0-108">في الحقل **الوصف**، اكتب **ملف تعريف ترحيل الأصول الثابتة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-108">In the **Description** field, type **Fixed asset posting profile**.</span></span> 

    <span data-ttu-id="358c0-109">ستحتاج إلى إنشاء ملف تعريف ترحيل لكل نوع حركة أصل ثابت ستستخدمه عند التعامل مع الأصول الثابتة.</span><span class="sxs-lookup"><span data-stu-id="358c0-109">You will need to create a posting profile for each fixed asset transaction type that you will be using when working with fixed assets.</span></span> <span data-ttu-id="358c0-110">ابدأ بنوع حركة **الاستحواذ**.</span><span class="sxs-lookup"><span data-stu-id="358c0-110">Start with the **Acquisition** transaction type.</span></span>

5.  <span data-ttu-id="358c0-111">حدد **إضافة** ضمن **حسابات دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="358c0-111">Select **Add** under **Ledger accounts**.</span></span>

6.  <span data-ttu-id="358c0-112">في الحقل **الدفتر**، أدخل **SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-112">In the **Book** field, enter **SLLR**.</span></span>
    
    <span data-ttu-id="358c0-113">يسمح لك الحقل **التجميعات** بتحديد ملف تعريف الترحيل وصولاً إلى "الجدول" (إعداد حساب واحد لكل أصل ثابت) أو "المجموعة" (إعداد حساب واحد لكل مجموعة أصول ثابتة).</span><span class="sxs-lookup"><span data-stu-id="358c0-113">The **Groupings** field allows you to define the posting profile down to the Table (one account set up for each fixed asset) or Group (one account set up for each fixed asset group).</span></span> <span data-ttu-id="358c0-114">بالنسبة إلى هذا المعمل، يتم تعيين القيمة على **الكل** لتطبيقها على كافة الأصول الثابتة باستخدام الدفتر المحدد.</span><span class="sxs-lookup"><span data-stu-id="358c0-114">For this lab, the value is set to **All** to apply to all fixed assets with the specified book.</span></span>
7.  <span data-ttu-id="358c0-115">في الحقل **الحساب الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-115">In the **Main account** field, specify **180100**.</span></span>
8.  <span data-ttu-id="358c0-116">في الحقل **الحساب** **المقابل**، حدد **300160**.</span><span class="sxs-lookup"><span data-stu-id="358c0-116">In the **Offset** **account** field, specify **300160**.</span></span> 
9.  <span data-ttu-id="358c0-117">في الحقل **نوع الحركة** من القائمة المنسدلة الموجود ضمن **حسابات دفتر الأستاذ**، حدد **تسوية الاستحواذ**.</span><span class="sxs-lookup"><span data-stu-id="358c0-117">In the drop-down **Transaction type** field under **Ledger accounts**, select **Acquisition adjustment**.</span></span>
10.  <span data-ttu-id="358c0-118">حدد **إضافة** مرة أخرى ضمن **حسابات دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="358c0-118">Select **Add** again under **Ledger accounts**.</span></span>
11.  <span data-ttu-id="358c0-119">في الحقل **الدفتر**، أدخل **SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-119">In the **Book** field, enter **SLLR**.</span></span>
12.  <span data-ttu-id="358c0-120">في الحقل **الحساب الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-120">In the **Main account** field, specify **180100**.</span></span>
13.  <span data-ttu-id="358c0-121">في الحقل **الحساب** **المقابل**، حدد **300160**.</span><span class="sxs-lookup"><span data-stu-id="358c0-121">In the **Offset** **account** field, specify  **300160**.</span></span> 
14. <span data-ttu-id="358c0-122">في الحقل **نوع الحركة**، حدد **إهلاك**.</span><span class="sxs-lookup"><span data-stu-id="358c0-122">In the **Transaction type** field, select **Depreciation**.</span></span>
15. <span data-ttu-id="358c0-123">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-123">Select **Add**.</span></span>
16. <span data-ttu-id="358c0-124">في الحقل **الدفتر**، أدخل **SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-124">In the **Book** field, enter **SLLR**.</span></span>
17. <span data-ttu-id="358c0-125">في الحقل **الحساب** **الرئيسي**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-125">In the **Main** **account** field, specify **180200**.</span></span>
18. <span data-ttu-id="358c0-126">في الحقل **الحساب المقابل**، حدد **607200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-126">In the **Offset account** field, specify **607200**.</span></span>
19. <span data-ttu-id="358c0-127">في القائمة المنسدلة **نوع الحركة**، حدد **تسوية الإهلاك**.</span><span class="sxs-lookup"><span data-stu-id="358c0-127">In the **Transaction type** dropdown menu, select **Depreciation  adjustment**.</span></span>
1. <span data-ttu-id="358c0-128">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-128">Select **Add**.</span></span>
2. <span data-ttu-id="358c0-129">في الحقل **الدفتر**، أدخل **SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-129">In the **Book** field, enter **SLLR**.</span></span>
3. <span data-ttu-id="358c0-130">في الحقل **الحساب** **الرئيسي**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-130">In the **Main** **account** field, specify **180200**.</span></span>
4. <span data-ttu-id="358c0-131">في الحقل **الحساب** **المقابل**، حدد **607200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-131">In the **Offset** **account** field, specify **607200**.</span></span>
5. <span data-ttu-id="358c0-132">في الحقل **نوع** **الحركة**، حدد **التخلص - بيع**.</span><span class="sxs-lookup"><span data-stu-id="358c0-132">In the **Transaction** **type** field, select **Disposal - sale**.</span></span>
6. <span data-ttu-id="358c0-133">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-133">Select **Add**.</span></span>
7. <span data-ttu-id="358c0-134">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-134">In the **Book** field, enter or select **SLLR**.</span></span>
8. <span data-ttu-id="358c0-135">في الحقل **الحساب** **الرئيسي**، حدد **801100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-135">In the **Main** **account** field, specify **801100**.</span></span>
9. <span data-ttu-id="358c0-136">في الحقل **الحساب** **المقابل**، حدد **801100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-136">In the **Offset** **account** field, specify **801100**.</span></span>
1. <span data-ttu-id="358c0-137">في الحقل **نوع** **الحركة**، حدد **التخلص - خردة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-137">In the **Transaction** **type** field, select **Disposal - scrap**.</span></span>
2. <span data-ttu-id="358c0-138">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-138">Select **Add**.</span></span>
3. <span data-ttu-id="358c0-139">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-139">In the **Book** field, enter or select **SLLR**.</span></span>
4. <span data-ttu-id="358c0-140">في الحقل **الحساب** **الرئيسي**، حدد **801100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-140">In the **Main** **account** field, specify **801100**.</span></span>
5. <span data-ttu-id="358c0-141">في الحقل **الحساب** **المقابل**، حدد **801100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-141">In the **Offset** **account** field, specify **801100**.</span></span>
6. <span data-ttu-id="358c0-142">قم بتوسيع علامة التبويب السريعة **التخلص**.</span><span class="sxs-lookup"><span data-stu-id="358c0-142">Expand the **Disposal** FastTab.</span></span> <span data-ttu-id="358c0-143">إعداد ملفات تعريف ترحيل التخلص لكل من البيع والخردة.</span><span class="sxs-lookup"><span data-stu-id="358c0-143">Set up disposal posting profiles for both sale and scrap.</span></span>
7. <span data-ttu-id="358c0-144">البدء بحركات بيع التخلص.</span><span class="sxs-lookup"><span data-stu-id="358c0-144">Start with disposal sale transactions.</span></span> <span data-ttu-id="358c0-145">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-145">Select **Add**.</span></span>
8. <span data-ttu-id="358c0-146">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-146">In the **Book** field, enter or select **SLLR**.</span></span>
9. <span data-ttu-id="358c0-147">في الحقل **قيمة الترحيل**، حدد **قيمة الاستحواذ**.</span><span class="sxs-lookup"><span data-stu-id="358c0-147">In the **Post** **value** field, select **Acquisition value**.</span></span>
    
    <span data-ttu-id="358c0-148">ستعالج قيمة الاستحواذ "قيم الاستحواذ وتسوية الاستحواذ" لجميع السنوات.</span><span class="sxs-lookup"><span data-stu-id="358c0-148">Acquisition value will address Acquisition and Acquisition adjustment values for all years.</span></span> <span data-ttu-id="358c0-149">يمكنك أيضاً تحديد الحسابات لأنواع الحركات هذه بشكل منفصل.</span><span class="sxs-lookup"><span data-stu-id="358c0-149">You can also define accounts for these transaction types separately.</span></span>
    
    <span data-ttu-id="358c0-150">يمكنك تحديد عملية التخلص لاستخدام حسابات مختلفة، وذلك وفقاً لما إذا كان التخلص ينتج عنه ربح أو خسارة.</span><span class="sxs-lookup"><span data-stu-id="358c0-150">You can set the disposal process to use different accounts, depending upon whether the disposal results in a gain or loss.</span></span> <span data-ttu-id="358c0-151">يتم تعيين **نوع قيمة المبيعات** على **الكل** لاستخدام الحسابات نفسها لجميع أنواع التخلص.</span><span class="sxs-lookup"><span data-stu-id="358c0-151">The **Sales value Type** is set to **All** to use the same accounts for all types of disposals.</span></span>
10. <span data-ttu-id="358c0-152">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-152">In the **Main** **account** field, specify **180100.**</span></span>
11. <span data-ttu-id="358c0-153">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-153">In the **Offset** **account** field, specify **180200.**</span></span>
12. <span data-ttu-id="358c0-154">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-154">Select **Add**.</span></span>
13. <span data-ttu-id="358c0-155">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-155">In the **Book** field, enter or select **SLLR**.</span></span>
14. <span data-ttu-id="358c0-156">في الحقل **قيمة الترحيل**، حدد **الإهلاك (السنوات السابقة)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-156">In the **Post value** field, select **Depreciation (prior years)**.</span></span>
15. <span data-ttu-id="358c0-157">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-157">In the **Main** **account** field, specify **180100**.</span></span>
16. <span data-ttu-id="358c0-158">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-158">In the **Offset** **account** field, specify **180200.**</span></span>
17. <span data-ttu-id="358c0-159">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-159">Select **Add**.</span></span>
18. <span data-ttu-id="358c0-160">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-160">In the **Book** field, enter or select **SLLR**.</span></span>
19. <span data-ttu-id="358c0-161">في الحقل **قيمة** **الترحيل**، حدد **الإهلاك (السنة الحالية)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-161">In the **Post** **value** field, select **Depreciation (this year)**.</span></span>
20. <span data-ttu-id="358c0-162">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-162">In the **Main** **account** field, specify **180100**.</span></span>
21. <span data-ttu-id="358c0-163">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-163">In the **Offset** **account** field, specify **180200.**</span></span>
22. <span data-ttu-id="358c0-164">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-164">Select **Add**.</span></span>
23. <span data-ttu-id="358c0-165">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-165">In the **Book** field, enter or select **SLLR**.</span></span>
24. <span data-ttu-id="358c0-166">في الحقل **قيمة الترحيل**، حدد **تسويات الإهلاك (السنوات السابقة)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-166">In the **Post value** field, select **Depreciation adjustments  (prior years)**.</span></span>
25. <span data-ttu-id="358c0-167">في الحقل **الحساب الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-167">In the **Main account** field, specify **180100**.</span></span>
26. <span data-ttu-id="358c0-168">في الحقل **الحساب المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-168">In the **Offset account** field, specify **180200**.</span></span>
27. <span data-ttu-id="358c0-169">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-169">Select **Add**.</span></span>
28. <span data-ttu-id="358c0-170">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-170">In the **Book** field, enter or select **SLLR**.</span></span>
29. <span data-ttu-id="358c0-171">في الحقل **قيمة الترحيل**، حدد **تسويات الإهلاك (السنة الحالية)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-171">In the **Post value** field, select **Depreciation adjustments  (this year)**.</span></span>
30. <span data-ttu-id="358c0-172">في الحقل **الحساب الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-172">In the **Main account** field, specify **180100**.</span></span>
31. <span data-ttu-id="358c0-173">في الحقل **الحساب المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-173">In the **Offset account** field, specify **180200**.</span></span>
32. <span data-ttu-id="358c0-174">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-174">Select **Add**.</span></span>
33. <span data-ttu-id="358c0-175">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-175">In the **Book** field, enter or select **SLLR**.</span></span>
34. <span data-ttu-id="358c0-176">في الحقل **قيمة الترحيل**، حدد **صافي القيمة الدفترية**.</span><span class="sxs-lookup"><span data-stu-id="358c0-176">In the **Post** **value** field, select **Net book value**.</span></span>
35. <span data-ttu-id="358c0-177">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-177">In the **Main** **account** field, specify **180100**.</span></span>
36. <span data-ttu-id="358c0-178">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-178">In the **Offset** **account** field, specify **180200**.</span></span>
37. <span data-ttu-id="358c0-179">في الحقل **البيع** أو **الخردة**، حدد **الخردة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-179">In the **Sale** or **scrap** field, select **Scrap**.</span></span>
38. <span data-ttu-id="358c0-180">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-180">Select **Add**.</span></span>
39. <span data-ttu-id="358c0-181">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-181">In the **Book** field, enter or select **SLLR**.</span></span>
40. <span data-ttu-id="358c0-182">في الحقل **قيمة الترحيل**، حدد **قيمة الاستحواذ**.</span><span class="sxs-lookup"><span data-stu-id="358c0-182">In the **Post value** field, select **Acquisition value**.</span></span>
41. <span data-ttu-id="358c0-183">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-183">In the **Main** **account** field, specify **180100**.</span></span>
42. <span data-ttu-id="358c0-184">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-184">In the **Offset** **account** field, specify **180200**.</span></span>
43. <span data-ttu-id="358c0-185">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-185">Select **Add**.</span></span>
44. <span data-ttu-id="358c0-186">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-186">In the **Book** field, enter or select **SLLR**.</span></span>
45. <span data-ttu-id="358c0-187">في الحقل **قيمة الترحيل**، حدد **الإهلاك (السنوات السابقة)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-187">In the **Post value** field, select **Depreciation (prior years)**.</span></span>
46. <span data-ttu-id="358c0-188">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-188">In the **Main** **account** field, specify **180100**.</span></span>
47. <span data-ttu-id="358c0-189">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-189">In the **Offset** **account** field, specify **180200**.</span></span>
48. <span data-ttu-id="358c0-190">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-190">Select **Add**.</span></span>
49. <span data-ttu-id="358c0-191">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-191">In the **Book** field, enter or select **SLLR**.</span></span>
50. <span data-ttu-id="358c0-192">في الحقل **قيمة الترحيل**، حدد **الإهلاك (السنة الحالية)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-192">In the **Post value** field, select **Depreciation (this year)**.</span></span>
51. <span data-ttu-id="358c0-193">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-193">In the **Main** **account** field, specify **180100**.</span></span>
52. <span data-ttu-id="358c0-194">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-194">In the **Offset** **account** field, specify **180200.**</span></span>
53. <span data-ttu-id="358c0-195">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-195">Select **Add**.</span></span>
54. <span data-ttu-id="358c0-196">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-196">In the **Book** field, enter or select **SLLR**.</span></span>
55. <span data-ttu-id="358c0-197">في الحقل **قيمة الترحيل**، حدد **تسويات الإهلاك (السنوات السابقة)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-197">In the **Post value** field, select **Depreciation adjustments  (prior years)**.</span></span>
56. <span data-ttu-id="358c0-198">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-198">In the **Main** **account** field, specify **180100**.</span></span>
57. <span data-ttu-id="358c0-199">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-199">In the **Offset** **account** field, specify **180200**.</span></span>
58. <span data-ttu-id="358c0-200">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-200">Select **Add**.</span></span>
59. <span data-ttu-id="358c0-201">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-201">In the **Book** field, enter or select **SLLR**.</span></span>
60. <span data-ttu-id="358c0-202">في الحقل **قيمة الترحيل**، حدد **تسويات الإهلاك (السنة الحالية)**.</span><span class="sxs-lookup"><span data-stu-id="358c0-202">In the **Post value** field, select **Depreciation adjustments (this  year)**.</span></span>
61. <span data-ttu-id="358c0-203">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-203">In the **Main** **account** field, specify **180100**.</span></span>
62. <span data-ttu-id="358c0-204">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-204">In the **Offset** **account** field, specify **180200**.</span></span>
63. <span data-ttu-id="358c0-205">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="358c0-205">Select **Add**.</span></span>
64. <span data-ttu-id="358c0-206">في الحقل **الدفتر**، أدخل أو حدد **‎SLLR**.</span><span class="sxs-lookup"><span data-stu-id="358c0-206">In the **Book** field, enter or select **SLLR**.</span></span>
65. <span data-ttu-id="358c0-207">في الحقل **قيمة الترحيل**، حدد **صافي القيمة الدفترية**.</span><span class="sxs-lookup"><span data-stu-id="358c0-207">In the **Post value** field, select **Net book value**.</span></span>
66. <span data-ttu-id="358c0-208">في الحقل **الحساب** **الرئيسي**، حدد **180100**.</span><span class="sxs-lookup"><span data-stu-id="358c0-208">In the **Main** **account** field, specify **180100**.</span></span>
67. <span data-ttu-id="358c0-209">في الحقل **الحساب** **المقابل**، حدد **180200**.</span><span class="sxs-lookup"><span data-stu-id="358c0-209">In the **Offset** **account** field, specify **180200**.</span></span>
68. <span data-ttu-id="358c0-210">انقر على **حفظ** في حالة اكتمال جميع التحديثات.</span><span class="sxs-lookup"><span data-stu-id="358c0-210">Click **Save** when all the updates are complete.</span></span>

## <a name="go-to-the-next-lab-instructions-from-the-lab-environment"></a><span data-ttu-id="358c0-211">الانتقال إلى إرشادات المعمل التالية من بيئة المعمل</span><span class="sxs-lookup"><span data-stu-id="358c0-211">Go to the next lab instructions from the lab environment</span></span>
 
<span data-ttu-id="358c0-212">حدد الزر **التالي** في الركن الأيسر السفلي من الشريط الجانبي.</span><span class="sxs-lookup"><span data-stu-id="358c0-212">Select the **Next** button in the bottom-right corner of the side bar.</span></span> 


