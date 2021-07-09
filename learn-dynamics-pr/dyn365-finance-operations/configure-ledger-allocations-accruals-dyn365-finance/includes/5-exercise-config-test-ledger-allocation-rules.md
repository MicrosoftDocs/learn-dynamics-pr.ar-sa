---
ms.openlocfilehash: 5c8b16234c886653e68d9b6f7731ad564d804a59
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070600"
---
<span data-ttu-id="0a6b7-101">تحتاج إلى تكوين قواعد توزيع دفتر الأستاذ واختبارها في USMF.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-101">You need to configure and test ledger allocation rules in USMF.</span></span> <span data-ttu-id="0a6b7-102">يطلب المحاسب أن تقوم بإنشاء ثلاثة حسابات دفتر أستاذ جديدة لتوزيع الحركات المرحلة بالتساوي إلى أبعاد مالية مختلفة، استناداً إلى قاعدة للفترة الحالية.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-102">The accountant requests that you create three new ledger accounts to allocate posted transactions equally to different financial dimensions, based on a rule for the current period.</span></span>

## <a name="create-main-accounts"></a><span data-ttu-id="0a6b7-103">إنشاء حسابات رئيسية</span><span class="sxs-lookup"><span data-stu-id="0a6b7-103">Create main accounts</span></span> 

1.  <span data-ttu-id="0a6b7-104">انتقل إلى **دفتر الأستاذ العام > دليل الحسابات > الحسابات > الحسابات الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-104">Go to **General ledger > Chart of accounts > Accounts > Main accounts**.</span></span>
2.  <span data-ttu-id="0a6b7-105">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-105">Select **New**.</span></span>
3.  <span data-ttu-id="0a6b7-106">في حقل **الحساب الرئيسي**، اكتب "100001"</span><span class="sxs-lookup"><span data-stu-id="0a6b7-106">In the **Main account** field, type '100001'</span></span>
4.  <span data-ttu-id="0a6b7-107">في حقل **الاسم**، اكتب "الحساب الموزع 1".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-107">In the **Name** field, type 'Allocated Account 1'.</span></span>
5.  <span data-ttu-id="0a6b7-108">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-108">Select **New**.</span></span>
6.  <span data-ttu-id="0a6b7-109">في حقل **الحساب الرئيسي**، اكتب "100002"</span><span class="sxs-lookup"><span data-stu-id="0a6b7-109">In the **Main account** field, type '100002'</span></span>
7.  <span data-ttu-id="0a6b7-110">في حقل **الاسم**، اكتب "الحساب الموزع 2".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-110">In the **Name** field, type 'Allocated Account 2'.</span></span>
8.  <span data-ttu-id="0a6b7-111">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-111">Select **New**.</span></span>
9.  <span data-ttu-id="0a6b7-112">في حقل **الحساب الرئيسي**، اكتب "100003"</span><span class="sxs-lookup"><span data-stu-id="0a6b7-112">In the **Main account** field, type '100003'</span></span>
10. <span data-ttu-id="0a6b7-113">في حقل **الاسم**، اكتب "الحساب المقابل الموزع".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-113">In the **Name** field, type 'Allocated Offset Account'.</span></span>
11. <span data-ttu-id="0a6b7-114">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-114">Close the page.</span></span>

## <a name="create-date-intervals-for-the-current-period"></a><span data-ttu-id="0a6b7-115">إنشاء فترات تاريخ للفترة الحالية</span><span class="sxs-lookup"><span data-stu-id="0a6b7-115">Create date intervals for the current period</span></span> 

1.  <span data-ttu-id="0a6b7-116">انتقل إلى **دفتر الأستاذ العام > إعداد دفتر الأستاذ > فترات التاريخ**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-116">Go to **General ledger > Ledger setup > Date intervals**.</span></span>
1.  <span data-ttu-id="0a6b7-117">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-117">Select **New**.</span></span>
2.  <span data-ttu-id="0a6b7-118">في حقل **كود الفاصل الزمني**، اكتب "CurPeriod".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-118">In the **Date interval code** field, type 'CurPeriod'.</span></span>
3.  <span data-ttu-id="0a6b7-119">في حقل **الوصف**، اكتب "الفترة الحالية".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-119">In the **Description** field, type 'Current Period'.</span></span>
4.  <span data-ttu-id="0a6b7-120">في **نوع فترة من تاريخ**، حدد **الفترة**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-120">In the **From date period type** field, select **Period**.</span></span>
5.  <span data-ttu-id="0a6b7-121">في الحقل **بدء/نهاية من تاريخ**، حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-121">In the **From date Start/End** field, select **Start**.</span></span>
6.  <span data-ttu-id="0a6b7-122">في الحقل **نوع فترة إلى تاريخ**، حدد **الفترة**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-122">In the **To date period type** field, select **Period**.</span></span>
7.  <span data-ttu-id="0a6b7-123">في الحقل **بدء/نهاية إلى تاريخ**، حدد **نهاية**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-123">In the **To date Start/End** field, select **End**.</span></span>
8.  <span data-ttu-id="0a6b7-124">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-124">Close the page.</span></span>

## <a name="create-an-allocation-journal-name"></a><span data-ttu-id="0a6b7-125">إنشاء اسم دفتر يومية توزيع</span><span class="sxs-lookup"><span data-stu-id="0a6b7-125">Create an allocation journal name</span></span> 

1.  <span data-ttu-id="0a6b7-126">انتقل إلى **دفتر الأستاذ العام > إعداد دفتر اليومية > أسماء دفاتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-126">Go to **General ledger > Journal setup > Journal names**.</span></span>
2.  <span data-ttu-id="0a6b7-127">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-127">Select **New**.</span></span>
3.  <span data-ttu-id="0a6b7-128">في حقل **الاسم**، اكتب "**AllocDemo**".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-128">In the **Name** field, type '**AllocDemo**'.</span></span>
4.  <span data-ttu-id="0a6b7-129">في حقل **الوصف**، اكتب "**دفاتر يومية التوزيع**".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-129">In the **Description** field, type '**Allocation Journals**'.</span></span>
5.  <span data-ttu-id="0a6b7-130">في حقل **نوع دفتر اليومية**، حدد **التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-130">In the **Journal type** field, select **Allocation**.</span></span>
6.  <span data-ttu-id="0a6b7-131">في حقل **سلسلة الإيصال**، أدخل قيمة أو حددها.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-131">In the **Voucher series** field, enter or select a value.</span></span>
7.  <span data-ttu-id="0a6b7-132">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-132">Close the page.</span></span>


## <a name="create-an-allocation-rule"></a><span data-ttu-id="0a6b7-133">إنشاء قاعدة توزيع</span><span class="sxs-lookup"><span data-stu-id="0a6b7-133">Create an allocation rule</span></span> 

1.  <span data-ttu-id="0a6b7-134">انتقل إلى **دفتر الأستاذ العام > توزيعات > قواعد توزيع دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-134">Go to **General ledger > Allocations > Ledger allocation rules**.</span></span>
2.  <span data-ttu-id="0a6b7-135">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-135">Select **New**.</span></span>
3.  <span data-ttu-id="0a6b7-136">في حقل **الوصف**، اكتب "**العرض التوضيحي‬ لتوزيع Adventure Works CyclesRent**".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-136">In the **Description** field, type '**Adventure Works CyclesRent Allocation Demo**'.</span></span>
4.  <span data-ttu-id="0a6b7-137">حدد علامة التبويب **عام**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-137">Select the **General** tab.</span></span>
5.  <span data-ttu-id="0a6b7-138">حدد **نعم** في الحقل **نشط**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-138">Select **Yes** in the **Active** field.</span></span>
6.  <span data-ttu-id="0a6b7-139">في حقل **أسلوب التوزيع**، حدد **بالتساوي**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-139">In the **Allocation method** field, select **Equally**.</span></span>
7.  <span data-ttu-id="0a6b7-140">في حقل **اسم دفتر اليومية**، أدخل **AllocDemo‎** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-140">In the **Journal name** field, enter or select **AllocDemo**.</span></span> 
8.  <span data-ttu-id="0a6b7-141">في حقل **كود الفاصل الزمني**، أدخل **CurPeriod** أو حدده، ثم اضغط على المفتاح Tab.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-141">In the **Date interval code** field, enter or select **CurPeriod**, and then press the Tab key.</span></span>
9.  <span data-ttu-id="0a6b7-142">حدد **مصدر**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-142">Select **Source**.</span></span>
10. <span data-ttu-id="0a6b7-143">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-143">Select **New**.</span></span>
11. <span data-ttu-id="0a6b7-144">في الحقل **معايير المصدر**، أدخل **601511‎** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-144">In the **Source criteria** field, enter or select **601511**.</span></span> 
12. <span data-ttu-id="0a6b7-145">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-145">Select **New**.</span></span>
13. <span data-ttu-id="0a6b7-146">في الحقل **إعداد الحقل**، حدد **البُعد المالي**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-146">In the **Field setting** field, select **Financial dimension**.</span></span>
14. <span data-ttu-id="0a6b7-147">في حقل **الاسم**، أدخل **القسم‎** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-147">In the **Name** field, enter or select **Department**.</span></span> 
15. <span data-ttu-id="0a6b7-148">في الحقل **معايير المصدر**، أدخل **024‎** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-148">In the **Source criteria** field, enter or select **024**.</span></span>
16. <span data-ttu-id="0a6b7-149">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-149">Close the page.</span></span>
17. <span data-ttu-id="0a6b7-150">حدد **الوجهة**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-150">Select **Destination**.</span></span>
18. <span data-ttu-id="0a6b7-151">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-151">Select **New**.</span></span>
19. <span data-ttu-id="0a6b7-152">في حقل **إلى الحساب**، حدد القيم "100001".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-152">In the **To account** field, specify the values '100001'.</span></span>
20. <span data-ttu-id="0a6b7-153">في حقل **القسم**، أدخل **023** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-153">In the **Department** field, enter or select **023**.</span></span> 
21. <span data-ttu-id="0a6b7-154">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-154">Select **New**.</span></span>
22. <span data-ttu-id="0a6b7-155">في حقل **إلى الحساب**، حدد القيم "100002".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-155">In the **To account** field, specify the values '100002'.</span></span>
23. <span data-ttu-id="0a6b7-156">في حقل **القسم**، أدخل **026** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-156">In the **Department** field, enter or select **026**.</span></span> 
24. <span data-ttu-id="0a6b7-157">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-157">Close all pages.</span></span>

## <a name="create-and-post-general-journal-for-allocation-testing"></a><span data-ttu-id="0a6b7-158">إنشاء دفتر يومية عام وترحيله لاختبار التوزيع</span><span class="sxs-lookup"><span data-stu-id="0a6b7-158">Create and post general journal for allocation testing</span></span> 

1.  <span data-ttu-id="0a6b7-159">انتقل إلى **دفتر الأستاذ العام > إدخالات دفتر اليومية > دفاتر اليومية العامة**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-159">Go to **General ledger > Journal entries > General journals**.</span></span>
2.  <span data-ttu-id="0a6b7-160">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-160">Select **New**.</span></span>
3.  <span data-ttu-id="0a6b7-161">في حقل **الاسم**، أدخل **AllocDemo‎** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-161">In the **Name** field, enter or select **AllocDemo**.</span></span>
4.  <span data-ttu-id="0a6b7-162">حدد **البنود**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-162">Select **Lines**.</span></span>
5.  <span data-ttu-id="0a6b7-163">في حقل **الحساب**، حدد القيم "‎601511-024-020-‎".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-163">In the **Account** field, specify the values '601511-024-020- '.</span></span>
6.  <span data-ttu-id="0a6b7-164">في حقل **الوصف**، اكتب "‏‫عرض توضيحي‬ للتوزيع".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-164">In the **Description** field, type 'Allocation Demo'.</span></span>
7.  <span data-ttu-id="0a6b7-165">قم بتعيين **مدين** إلى "72700".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-165">Set **Debit** to '72700'.</span></span>
8.  <span data-ttu-id="0a6b7-166">في حقل **الحساب المقابل**، حدد القيم "‎605160 -024-020-‎".</span><span class="sxs-lookup"><span data-stu-id="0a6b7-166">In the **Offset account** field, specify the values ' 605160 -024-020- '.</span></span>
9.  <span data-ttu-id="0a6b7-167">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-167">Select **Post**.</span></span>
10. <span data-ttu-id="0a6b7-168">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-168">Close all pages.</span></span>

## <a name="process-an-allocation-request-to-test-the-allocation-rule"></a><span data-ttu-id="0a6b7-169">معالجة طلب توزيع لاختبار قاعدة التوزيع</span><span class="sxs-lookup"><span data-stu-id="0a6b7-169">Process an allocation request to test the allocation rule</span></span> 

1.  <span data-ttu-id="0a6b7-170">انتقل إلى **دفتر الأستاذ العام > توزيعات > طلب توزيع العملية**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-170">Go to **General ledger > Allocations > Process allocation request**.</span></span>
2.  <span data-ttu-id="0a6b7-171">في حقل **القاعدة**، اكتب **العرض التوضيحي‬ لتوزيع Adventure Works CyclesRent**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-171">In the **Rule** field, enter or select **Adventure Works CyclesRent Allocation Demo**.</span></span>
3.  <span data-ttu-id="0a6b7-172">في الحقل **خيارات المقترح**، حدد **مقترح فقط**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-172">In the **Proposal options** field, select **Proposal only**.</span></span>
4.  <span data-ttu-id="0a6b7-173">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-173">Select **OK**.</span></span>


## <a name="verify-the-allocation-journals-created-by-processing-the-allocation-requests"></a><span data-ttu-id="0a6b7-174">تحقق من دفاتر يومية التوزيع التي تم إنشاؤها بمعالجة طلبات التوزيع</span><span class="sxs-lookup"><span data-stu-id="0a6b7-174">Verify the allocation journals created by processing the allocation requests</span></span> 

1.  <span data-ttu-id="0a6b7-175">انتقل إلى **دفتر الأستاذ العام > توزيعات > دفاتر يومية التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-175">Go to **General ledger > Allocations > Allocation journals**.</span></span>
2.  <span data-ttu-id="0a6b7-176">حدد **البنود**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-176">Select **Lines**.</span></span>
3.  <span data-ttu-id="0a6b7-177">راجع البيانات وحللها لمعرفة ما إذا كان قد تم توزيع الحركة الأصلية بالتساوي.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-177">Review and analyze data to see if the original transaction has been allocated equally.</span></span>
4.  <span data-ttu-id="0a6b7-178">انتقل إلى **تحقق من الصحة > محاكاة الترحيل**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-178">Go to **Validate > Simulate posting**.</span></span>    
5.  <span data-ttu-id="0a6b7-179">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-179">Select **Post**.</span></span>
6.  <span data-ttu-id="0a6b7-180">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="0a6b7-180">Close all pages.</span></span>


