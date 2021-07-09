---
ms.openlocfilehash: c8215e444665e29b9ed3a16665142efb26177afc
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070900"
---
## <a name="scenario"></a><span data-ttu-id="ea606-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="ea606-101">Scenario</span></span>
<span data-ttu-id="ea606-102">تحتاج إلى إعداد محاسبة بين الشركات الشقيقة بين **USP2** و **USMF** واستخدامها.</span><span class="sxs-lookup"><span data-stu-id="ea606-102">You need to set up and use intercompany accounting between **USP2** and **USMF**.</span></span> <span data-ttu-id="ea606-103">تستخدم هاتان الشركتان مخطط الحسابات نفسه.</span><span class="sxs-lookup"><span data-stu-id="ea606-103">These companies are using the same chart of accounts.</span></span> <span data-ttu-id="ea606-104">وستقوم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="ea606-104">You will:</span></span> 

1.  <span data-ttu-id="ea606-105">تكوين المحاسبة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="ea606-105">Configure intercompany accounting.</span></span>
2.  <span data-ttu-id="ea606-106">استخدام محاسبة بين الشركات الشقيقة مع دفاتر يومية عامة.</span><span class="sxs-lookup"><span data-stu-id="ea606-106">Use intercompany accounting with general journals.</span></span> 
3.  <span data-ttu-id="ea606-107">استخدام سجلات المراجعة للتحقق من الترحيل المحاسبي بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="ea606-107">Use audit trails to verify the intercompany accounting posting.</span></span>

## <a name="configure-intercompany-accounting"></a><span data-ttu-id="ea606-108">تكوين المحاسبة بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="ea606-108">Configure intercompany accounting</span></span> 

1.  <span data-ttu-id="ea606-109">تغيِّر الشركة إلى **USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-109">Change company to **USP2**.</span></span>
2.  <span data-ttu-id="ea606-110">انتقل إلى **دفتر الأستاذ العام > دليل الحسابات > الحسابات > الحسابات الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="ea606-110">Go to **General ledger > Chart of accounts > Accounts > Main accounts**.</span></span>
3.  <span data-ttu-id="ea606-111">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ea606-111">Select **New**.</span></span>
4.  <span data-ttu-id="ea606-112">في الحقل **الحساب الرئيسي**، أدخل **100100**.</span><span class="sxs-lookup"><span data-stu-id="ea606-112">In the **Main account** field, enter **100100**.</span></span>
5.  <span data-ttu-id="ea606-113">في حقل **الاسم**، أدخل **مستحق لـ USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-113">In the **Name** field, enter **Due to USMF**.</span></span>
6.  <span data-ttu-id="ea606-114">في الحقل **نوع الحساب الرئيسي**، حدد **ميزانية عمومية**.</span><span class="sxs-lookup"><span data-stu-id="ea606-114">In the **Main account type** field, select **Balance sheet**.</span></span>
7.  <span data-ttu-id="ea606-115">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea606-115">Select **Save**.</span></span>
7.  <span data-ttu-id="ea606-116">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ea606-116">Select **New**.</span></span>
8.  <span data-ttu-id="ea606-117">في الحقل **الحساب الرئيسي**، أدخل **100101**.</span><span class="sxs-lookup"><span data-stu-id="ea606-117">In the **Main account** field, enter **100101**.</span></span>
9.  <span data-ttu-id="ea606-118">في حقل **الاسم**، أدخل **مستحق من USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-118">In the **Name** field, enter **Due from USMF**.</span></span>
10. <span data-ttu-id="ea606-119">في الحقل **نوع الحساب الرئيسي**، حدد **ميزانية عمومية**.</span><span class="sxs-lookup"><span data-stu-id="ea606-119">In the **Main account type** field, select **Balance sheet**.</span></span>
11. <span data-ttu-id="ea606-120">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea606-120">Select **Save**.</span></span>
12. <span data-ttu-id="ea606-121">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea606-121">Close the page.</span></span>
13. <span data-ttu-id="ea606-122">تغيِّر الشركة إلى **USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-122">Change company to **USMF**.</span></span>
14. <span data-ttu-id="ea606-123">انتقل إلى **دفتر الأستاذ العام > دليل الحسابات > الحسابات > الحسابات الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="ea606-123">Go to **General ledger > Chart of accounts > Accounts > Main accounts**.</span></span>
15. <span data-ttu-id="ea606-124">تحقق من أن الحسابين اللذين قمت بإنشائهما في الخطوتين 4 و9 مدرجين مع اعتبار أن الشركتين تشتركان في مخطط الحساب نفسه.</span><span class="sxs-lookup"><span data-stu-id="ea606-124">Verify the two accounts that you created in the steps 4 and 9 are listed considering that the two companies are sharing the same chart of account.</span></span>
16. <span data-ttu-id="ea606-125">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ea606-125">Select **New**.</span></span>
17. <span data-ttu-id="ea606-126">في الحقل **الحساب الرئيسي**، أدخل **100106**.</span><span class="sxs-lookup"><span data-stu-id="ea606-126">In the **Main account** field, enter **100106**.</span></span>
18. <span data-ttu-id="ea606-127">في حقل **الاسم**، أدخل **مستحق لـ USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-127">In the **Name** field, enter **Due to USP2**.</span></span>
19. <span data-ttu-id="ea606-128">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea606-128">Select **Save**.</span></span>
19. <span data-ttu-id="ea606-129">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ea606-129">Select **New**.</span></span>
20. <span data-ttu-id="ea606-130">في الحقل **الحساب الرئيسي**، أدخل **100107**.</span><span class="sxs-lookup"><span data-stu-id="ea606-130">In the **Main account** field, enter **100107**.</span></span>
21. <span data-ttu-id="ea606-131">في حقل **الاسم**، أدخل **مستحق من USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-131">In the **Name** field, enter **Due from USP2**.</span></span>
22. <span data-ttu-id="ea606-132">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea606-132">Select **Save**.</span></span>
22. <span data-ttu-id="ea606-133">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea606-133">Close the page.</span></span>
23. <span data-ttu-id="ea606-134">انتقل إلى **دفتر الأستاذ العام > إعداد الترحيل > محاسبة بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="ea606-134">Go to **General ledger > Posting setup > Intercompany accounting**.</span></span>
24. <span data-ttu-id="ea606-135">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ea606-135">Select **New**.</span></span>
25. <span data-ttu-id="ea606-136">في حقل **الشركة المصدر**، حدد **USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-136">In the **Originating company** field, select **USMF**.</span></span>
26. <span data-ttu-id="ea606-137">في حقل **حساب مدين**، حدد **100107 مستحق من USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-137">In the **Debit account** field, select **100107 Due from USP2**.</span></span>
27. <span data-ttu-id="ea606-138">في حقل **حساب دائن**، حدد **100106 مستحق لـ USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-138">In the **Credit account** field, select **100106 Due to USP2**.</span></span>
28. <span data-ttu-id="ea606-139">في حقل **الشركة الوجهة**، حدد **USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-139">In the **Destination company** field, select **USP2**.</span></span>
29. <span data-ttu-id="ea606-140">في حقل **حساب مدين**، حدد **100100 مستحق لـ USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-140">In the **Debit account** field, select **100100 Due to USMF**.</span></span>
30. <span data-ttu-id="ea606-141">في حقل **حساب دائن**، حدد **100101 مستحق من USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-141">In the **Credit account** field, select **100101 Due from USMF**.</span></span>
31. <span data-ttu-id="ea606-142">في حقل **دفتر اليومية**، حدد **التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="ea606-142">In the **Journal** field, select **Allocation**.</span></span>
32. <span data-ttu-id="ea606-143">حدد **إنشاء علاقة التبادلية**.</span><span class="sxs-lookup"><span data-stu-id="ea606-143">Select **Create reciprocal relationship**.</span></span>
34. <span data-ttu-id="ea606-144">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea606-144">Select **Save**.</span></span>
35. <span data-ttu-id="ea606-145">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea606-145">Close the page.</span></span>


## <a name="use-intercompany-accounting-with-general-journals"></a><span data-ttu-id="ea606-146">استخدام محاسبة بين الشركات الشقيقة مع دفاتر يومية عامة</span><span class="sxs-lookup"><span data-stu-id="ea606-146">Use intercompany accounting with general journals</span></span> 

1.  <span data-ttu-id="ea606-147">انتقل إلى **دفتر الأستاذ العام > إدخالات دفتر اليومية > دفاتر اليومية العامة**.</span><span class="sxs-lookup"><span data-stu-id="ea606-147">Go to **General ledger > Journal entries > Global general journals**.</span></span>
2.  <span data-ttu-id="ea606-148">حدد **دفتر يومية جديد** لفتح مربع الحوار المنسدل.</span><span class="sxs-lookup"><span data-stu-id="ea606-148">Select **New journal** to open the drop-down dialog.</span></span>
3.  <span data-ttu-id="ea606-149">في الحقل **الشركة**، حدد **USMF**.</span><span class="sxs-lookup"><span data-stu-id="ea606-149">In the **Company** field, select **USMF**.</span></span>
4.  <span data-ttu-id="ea606-150">في حقل **الاسم**، حدد **GenJrn‎** (دفتر اليومية العام).</span><span class="sxs-lookup"><span data-stu-id="ea606-150">In the **Name** field, select **GenJrn** (General Journal).</span></span>
5.  <span data-ttu-id="ea606-151">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ea606-151">Select **OK**.</span></span>
6.  <span data-ttu-id="ea606-152">حدد دفتر اليومية الجديد الذي أنشأته للتو (00629)، ثم حدد **السطور**.</span><span class="sxs-lookup"><span data-stu-id="ea606-152">Select the new journal that you just created (00629), and then select **Lines**.</span></span>
7.  <span data-ttu-id="ea606-153">في عمود **نوع الحساب**، حدد **البنك**.</span><span class="sxs-lookup"><span data-stu-id="ea606-153">In the **Account type** column, select **Bank**.</span></span>
8.  <span data-ttu-id="ea606-154">في حقل **الحساب**، حدد القيم **USMF OPER**.</span><span class="sxs-lookup"><span data-stu-id="ea606-154">In the **Account** column, specify the values **USMF OPER**.</span></span>
9.  <span data-ttu-id="ea606-155">في عمود **الوصف**، أدخل **تحويل**.</span><span class="sxs-lookup"><span data-stu-id="ea606-155">In the **Description** column, enter **Wire**.</span></span>
10. <span data-ttu-id="ea606-156">قم بتعيين **دائن** إلى **1000000**.</span><span class="sxs-lookup"><span data-stu-id="ea606-156">Set **Credit** to **1000000**.</span></span>
11. <span data-ttu-id="ea606-157">في حقل **الشركة المقابلة**، حدد **USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-157">In the **Offset company** field, select **USP2**.</span></span>
12. <span data-ttu-id="ea606-158">في حقل **نوع حساب مقابل**، حدد **دفتر الأستاذ** للحساب.</span><span class="sxs-lookup"><span data-stu-id="ea606-158">In the **Offset account type** field, select  account **Ledger**.</span></span>
13. <span data-ttu-id="ea606-159">في حقل **الحساب المقابل**، حدد حساباً مقابلاً مثل **110110-069-023**.</span><span class="sxs-lookup"><span data-stu-id="ea606-159">In the **Offset account** field, select an offset account such as **110110-069-023**.</span></span>
14. <span data-ttu-id="ea606-160">حدد **استعلامات** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="ea606-160">Select **Inquiries** in the Action Pane.</span></span> 
15. <span data-ttu-id="ea606-161">حدد **التحكم في الرصيد**، ثم اعرض النتائج.</span><span class="sxs-lookup"><span data-stu-id="ea606-161">Select **Balance control**, and then view the results.</span></span>
17. <span data-ttu-id="ea606-162">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="ea606-162">Select **Close**.</span></span>
18. <span data-ttu-id="ea606-163">حدد **تحقق من الصحة > تحقق من الصحة** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="ea606-163">Select **Validate > Validate** in the Action Pane.</span></span>
20. <span data-ttu-id="ea606-164">في جزء الإجراء، حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="ea606-164">In the Action Pane select **Post**.</span></span> <span data-ttu-id="ea606-165">في القائمة المنسدلة لشريط المعلومات "اكتملت العملية"، سترى أنه تم ترحيل إيصالين، بواقع واحد لكل شركة.</span><span class="sxs-lookup"><span data-stu-id="ea606-165">In the drop-down of the "Operation completed" information bar, you will see that two vouchers have been posted, one per company.</span></span>
23. <span data-ttu-id="ea606-166">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea606-166">Close the page.</span></span>

## <a name="use-audit-trails-to-verify-the-intercompany-accounting-posting"></a><span data-ttu-id="ea606-167">استخدام سجلات المراجعة للتحقق من الترحيل المحاسبي بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="ea606-167">Use audit trails to verify the intercompany accounting posting</span></span> 

1.  <span data-ttu-id="ea606-168">في شركة **USMF**، انتقل إلى **دفتر الأستاذ العام > الاستعلامات والتقارير > سجل المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="ea606-168">In company **USMF**, go to **General ledger > Inquiries and reports > Audit trail**.</span></span>
2.  <span data-ttu-id="ea606-169">حدد الصف الذي يحتوي على الحركة بين الشركات الشقيقة التي سبق أن أنشأتها.</span><span class="sxs-lookup"><span data-stu-id="ea606-169">Select the row with the intercompany transaction you created earlier.</span></span>
3.  <span data-ttu-id="ea606-170">حدد **حركات الايصالات**.</span><span class="sxs-lookup"><span data-stu-id="ea606-170">Select **Voucher transactions**.</span></span> <span data-ttu-id="ea606-171">راجع الحركات بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="ea606-171">Review the intercompany transactions.</span></span>
3.  <span data-ttu-id="ea606-172">حدد **الإيصالات ذات الصلة** لعرض الحركة بين الشركات الشقيقة في الشركة الوجهة.</span><span class="sxs-lookup"><span data-stu-id="ea606-172">Select **Related vouchers** to view the intercompany in the destination company.</span></span> <span data-ttu-id="ea606-173">للوصول إلى هذه، قد تحتاج إلى تقليل حجم الخط في مستعرض الإنترنت مؤقتاً: حدد أيقونة أدوات ثم **تكبير/تصغير (50%)**.</span><span class="sxs-lookup"><span data-stu-id="ea606-173">To access this you may need to temporarily reduce the font size in the internet browser: Select the Tools icon and then **Zoom(50%)**.</span></span>
4.  <span data-ttu-id="ea606-174">قم بإغلاق الصفحة **إيصالات حركات دفتر الأستاذ ذات الصلة**.</span><span class="sxs-lookup"><span data-stu-id="ea606-174">Close the **Related ledger transaction vouchers** page.</span></span>
8.  <span data-ttu-id="ea606-175">قم بالتبديل إلى شركة **USP2**.</span><span class="sxs-lookup"><span data-stu-id="ea606-175">Switch to **USP2** company.</span></span>
9.  <span data-ttu-id="ea606-176">حدد **إلغاء** في صفحة **الاستعلام** التي يتم فتحها.</span><span class="sxs-lookup"><span data-stu-id="ea606-176">Select **Cancel** in the **Inquiry** page that opens.</span></span>
10. <span data-ttu-id="ea606-177">انتقل إلى **دفتر الأستاذ العام > الاستعلامات والتقارير > سجل المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="ea606-177">Go to **General ledger > Inquiries and reports > Audit trail**.</span></span>
10. <span data-ttu-id="ea606-178">حدد الصف الذي يحتوي على الحركة بين الشركات الشقيقة التي سبق أن أنشأتها.</span><span class="sxs-lookup"><span data-stu-id="ea606-178">Select the row with the intercompany transaction you created earlier.</span></span>
10. <span data-ttu-id="ea606-179">حدد **حركات الايصالات**.</span><span class="sxs-lookup"><span data-stu-id="ea606-179">Select **Voucher transactions**.</span></span> <span data-ttu-id="ea606-180">راجع الحركات بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="ea606-180">Review the intercompany transactions.</span></span>
11. <span data-ttu-id="ea606-181">أغلق صفحة **حركات الإيصال**.</span><span class="sxs-lookup"><span data-stu-id="ea606-181">Close the **Voucher transactions** page.</span></span>
12. <span data-ttu-id="ea606-182">قم بإغلاق صفحة **سجل المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="ea606-182">Close the **Audit trail** page.</span></span>
13. <span data-ttu-id="ea606-183">انتقل إلى **‏‫إدارة النقد والبنوك‬ > مساحات العمل > الحسابات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="ea606-183">Go to **Cash and bank management > Bank accounts > Bank accounts**.</span></span>
14. <span data-ttu-id="ea606-184">حدد **USP2 OPER**</span><span class="sxs-lookup"><span data-stu-id="ea606-184">Select **USP2 OPER**</span></span>
14. <span data-ttu-id="ea606-185">حدد **الرصيد**.</span><span class="sxs-lookup"><span data-stu-id="ea606-185">Select **Balance**.</span></span>
15. <span data-ttu-id="ea606-186">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ea606-186">Select **OK**.</span></span>
16. <span data-ttu-id="ea606-187">حدد **الحركات**.</span><span class="sxs-lookup"><span data-stu-id="ea606-187">Select **Transactions**.</span></span>
17. <span data-ttu-id="ea606-188">حدد **الإيصال**.</span><span class="sxs-lookup"><span data-stu-id="ea606-188">Select **Voucher**.</span></span>
18. <span data-ttu-id="ea606-189">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="ea606-189">Close all pages.</span></span>

## <a name="close-the-lab-environment"></a><span data-ttu-id="ea606-190">أغلق بيئة التمرين العملي</span><span class="sxs-lookup"><span data-stu-id="ea606-190">Close the lab environment</span></span> 

1. <span data-ttu-id="ea606-191">حدد الزر **التالي** في الركن الأيسر السفلي من الشريط الجانبي.</span><span class="sxs-lookup"><span data-stu-id="ea606-191">Select the **Next** button in the bottom-right corner of the side bar.</span></span>
2. <span data-ttu-id="ea606-192">حدد **مغادرة** في النافذة المنبثقة التي تظهر.</span><span class="sxs-lookup"><span data-stu-id="ea606-192">Select **Leave** in the pop-up window that appears.</span></span>
