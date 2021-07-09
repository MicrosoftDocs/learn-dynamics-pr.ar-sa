---
ms.openlocfilehash: 8aa63c5ecde1c7f159fdf81eca5adf5293bf2461
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070616"
---
<span data-ttu-id="66ce0-101">تحتاج إلى مساعدة المحاسب في شركة USMF، حول كيفية تكوين واستخدام أنظمة الاستحقاق في تطبيقات Finance.</span><span class="sxs-lookup"><span data-stu-id="66ce0-101">You need to assist the accountant in USMF, on how to configure and use accrual schemes in Finance.</span></span> <span data-ttu-id="66ce0-102">يرغب في استئجار سيارة من مورد مقابل 81،720 دولاراً أمريكياً وتسجيل المستحقات ضمن شروط الإيجار لمدة 24 شهراً.</span><span class="sxs-lookup"><span data-stu-id="66ce0-102">They want to lease a vehicle from a vendor for 81,720 USD and record accruals within the terms of lease of 24 months.</span></span> <span data-ttu-id="66ce0-103">كما يرغب في فهم الخيارات **شهري** و **عدد الأيام** الموجودة في أنظمة الاستحقاق.</span><span class="sxs-lookup"><span data-stu-id="66ce0-103">They want to understand the **Monthly** and **Number of days** options in the accrual schemes.</span></span> 

## <a name="before-you-begin"></a><span data-ttu-id="66ce0-104">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="66ce0-104">Before you begin</span></span> 

<span data-ttu-id="66ce0-105">للحصول على أقصى استفادة من هذا التدريب وغيره من التدريبات الأخرى في هذه الوحدة النمطية، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Finance والتي يتم تثبيتها باستخدام Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="66ce0-105">To get the most out of this exercise and the other exercises that are included with this module, we recommend that you have the standard sample data available in Dynamics 365 Finance that is installed using Lifecycle Services (LCS).</span></span> 

## <a name="create-accrual-schemes"></a><span data-ttu-id="66ce0-106">إنشاء أنظمة استحقاق</span><span class="sxs-lookup"><span data-stu-id="66ce0-106">Create accrual schemes</span></span> 

1.  <span data-ttu-id="66ce0-107">انتقل إلى **دفتر الأستاذ العام > إعداد دفتر اليومية > أنظمة الاستحقاق**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-107">Go to **General ledger > Journal setup > Accrual schemes**.</span></span>
2.  <span data-ttu-id="66ce0-108">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-108">Select **New**.</span></span>
3.  <span data-ttu-id="66ce0-109">في حقل **تعريف الاستحقاق**، أدخل **‎24M**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-109">In the **Accrual identification** field, enter **24M**.</span></span>
4.  <span data-ttu-id="66ce0-110">في حقل **وصف نظام الاستحقاق**، أدخل **عقد الإيجار لمدة 2 سنتين**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-110">In the **Description of accrual scheme** field, enter **2 Year Lease**.</span></span>
5.  <span data-ttu-id="66ce0-111">في حقل **مدين**، حدد القيم **420100**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-111">In the **Debit** field, specify the values **420100**.</span></span>
6.  <span data-ttu-id="66ce0-112">في حقل **دائن**، حدد القيم **420200**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-112">In the **Credit** field, specify the values **420200**.</span></span>
7.  <span data-ttu-id="66ce0-113">في حقل **الايصال**، حدد **إيصالاً جديداً لكل حركة**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-113">In the **Voucher** field, select **New voucher for each transaction**.</span></span>
8.  <span data-ttu-id="66ce0-114">في حقل **رمز التسلسل الرقمي**، أدخل أو حدد قيمةً.</span><span class="sxs-lookup"><span data-stu-id="66ce0-114">In the **Number sequence code** field, enter or select a value.</span></span>
9.  <span data-ttu-id="66ce0-115">في حقل **تكرار الفترة**، حدد **شهري**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-115">In the **Period frequency** field, select **Monthly**.</span></span>
10. <span data-ttu-id="66ce0-116">في حقل **عدد مرات التكرار حسب الفترة**، أدخل **24**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-116">In the **Number of occurrences by period** field, enter **24**.</span></span>
11. <span data-ttu-id="66ce0-117">في حقل **ترحيل الحركات**، حدد **شهر**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-117">In the **Post transactions** field, select **Month**.</span></span>
12. <span data-ttu-id="66ce0-118">في حقل **الترحيل في الأسبوع**، **أو الشهر أو ربع السنة**، حدد **منتصف**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-118">In the **Post in week**, **month or quarter** field, select **Middle**.</span></span>
13. <span data-ttu-id="66ce0-119">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="66ce0-119">Close the page.</span></span>


## <a name="create-general-journal-to-use-accrual-schemes"></a><span data-ttu-id="66ce0-120">أنشئ دفتر يومية عام لاستخدام أنظمة الاستحقاق</span><span class="sxs-lookup"><span data-stu-id="66ce0-120">Create general journal to use accrual schemes</span></span> 

1.  <span data-ttu-id="66ce0-121">انتقل إلى **دفتر الأستاذ العام > إدخالات دفتر اليومية > دفاتر اليومية العامة**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-121">Go to **General ledger > Journal entries > General journals**.</span></span>
2.  <span data-ttu-id="66ce0-122">حدد **دفتر يومية جديد**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-122">Select **New journal**.</span></span>
3.  <span data-ttu-id="66ce0-123">في حقل **الاسم**، أدخل أو حدد **GenJrn‎**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-123">In the **Name** field, enter or select **GenJrn**.</span></span> 
4.  <span data-ttu-id="66ce0-124">في حقل **الوصف**، أدخل **دفتر اليومية العام اليومي - العرض التوضيحي للاستحقاقات**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-124">In the **Description** field, enter **General Daily Journal - Accruals Demo**.</span></span>
5.  <span data-ttu-id="66ce0-125">حدد **البنود**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-125">Select **Lines**.</span></span>
6.  <span data-ttu-id="66ce0-126">في حقل **نوع الحساب**، حدد **مورّد**</span><span class="sxs-lookup"><span data-stu-id="66ce0-126">In the **Account type** field, select **Vendor**.</span></span>
7.  <span data-ttu-id="66ce0-127">في حقل **الحساب**، حدد حساب المورّد الذي تختاره.</span><span class="sxs-lookup"><span data-stu-id="66ce0-127">In the **Account** field, specify a vendor account of your choice.</span></span>
8.  <span data-ttu-id="66ce0-128">قم بتعيين **مدين** إلى **81720**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-128">Set **Debit** to **81720**.</span></span>
9.  <span data-ttu-id="66ce0-129">في حقل **الحساب المقابل**، حدد القيم **-009-025-601512**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-129">In the **Offset account** field, specify the values **601512-025-009-**.</span></span>
10. <span data-ttu-id="66ce0-130">في حقل النص **الحركة المقابلة**، أدخل **العرض التوضيحي للاستحقاقات**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-130">In the **Offset transaction** text field, enter **Accruals Demo**.</span></span>
11. <span data-ttu-id="66ce0-131">حدد **الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-131">Select **Functions**.</span></span>
12. <span data-ttu-id="66ce0-132">حدد **استحقاقات دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-132">Select **Ledger accruals**.</span></span>
13. <span data-ttu-id="66ce0-133">في حقل **تعريف الاستحقاق**، أدخل أو حدد **‎24M**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-133">In the **Accrual identification** field, enter or select **24M**.</span></span>
14. <span data-ttu-id="66ce0-134">حدد **الحركات**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-134">Select **Transactions**.</span></span>
15. <span data-ttu-id="66ce0-135">راجع القيم.</span><span class="sxs-lookup"><span data-stu-id="66ce0-135">Review the values.</span></span> <span data-ttu-id="66ce0-136">يتم توزيع المبلغ الإجمالي بالتساوي.</span><span class="sxs-lookup"><span data-stu-id="66ce0-136">The total amount is distributed evenly.</span></span>
16. <span data-ttu-id="66ce0-137">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="66ce0-137">Close the page.</span></span>
17. <span data-ttu-id="66ce0-138">انقر لاتباع الارتباط في حقل **تعريف الاستحقاق**، أو انقر بزر الماوس الأيمن وقمّ بعرض التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="66ce0-138">Click to follow the link in the **Accrual identification** field, or right-click and view details.</span></span>
18. <span data-ttu-id="66ce0-139">في حقل **نشر قيم الشهر وربع السنة**، حدد **عدد الأيام**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-139">In the **Spread month and quarter values** field, select **Number of days**.</span></span>
19. <span data-ttu-id="66ce0-140">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="66ce0-140">Close the page.</span></span>
20. <span data-ttu-id="66ce0-141">حدد **إلغاء**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-141">Select **Cancel**.</span></span>
21. <span data-ttu-id="66ce0-142">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-142">Select **Yes**.</span></span>
22. <span data-ttu-id="66ce0-143">حدد **الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-143">Select **Functions**.</span></span>
23. <span data-ttu-id="66ce0-144">حدد **استحقاقات دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-144">Select **Ledger accruals**.</span></span>
24. <span data-ttu-id="66ce0-145">في حقل **تعريف الاستحقاق**، أدخل **‎24M** أو حدده، ثم اضغط على المفتاح "Tab".</span><span class="sxs-lookup"><span data-stu-id="66ce0-145">In the **Accrual identification** field, enter or select **24M**, and then press the Tab key.</span></span>
25. <span data-ttu-id="66ce0-146">حدد **الحركات**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-146">Select **Transactions**.</span></span> <span data-ttu-id="66ce0-147">لاحظ أنه تم تقسيم المبالغ بالتناسب لعدد الأيام المحدد.</span><span class="sxs-lookup"><span data-stu-id="66ce0-147">Note that amounts have been prorated for the specified number of days.</span></span>
26. <span data-ttu-id="66ce0-148">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="66ce0-148">Close the page.</span></span>
27. <span data-ttu-id="66ce0-149">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-149">Select **OK**.</span></span>
28. <span data-ttu-id="66ce0-150">حدد **التحقق من الصحة > التحقق من الصحة**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-150">Select **Validate > Validate**.</span></span>
29. <span data-ttu-id="66ce0-151">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-151">Select **Post**.</span></span>
30. <span data-ttu-id="66ce0-152">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="66ce0-152">Close all pages.</span></span>
31. <span data-ttu-id="66ce0-153">انتقل إلى **دفتر الأستاذ العام > الاستعلامات والتقارير > سجل المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-153">Go to **General ledger > Inquiries and reports > Audit trail**.</span></span>
32. <span data-ttu-id="66ce0-154">ابحث عن دفتر اليومية الذي قمت بترحيله للتو، والذي يجب أن نكون آخر سجل أو يمكنك استخدام خيار عامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="66ce0-154">Find the journal that you just posted, which should be the last record or you can use the filter  option.</span></span>
33. <span data-ttu-id="66ce0-155">حدد **حركات الايصالات**.</span><span class="sxs-lookup"><span data-stu-id="66ce0-155">Select **Voucher transactions**.</span></span> <span data-ttu-id="66ce0-156">مراجعة الحركات المرحلة وتحليلها.</span><span class="sxs-lookup"><span data-stu-id="66ce0-156">Review and analyze posted transactions.</span></span> <span data-ttu-id="66ce0-157">لاحظ أنه تم عكس الحركات الأصلية وتم ترحيل المستحقات خلال 24 شهراً.</span><span class="sxs-lookup"><span data-stu-id="66ce0-157">Note that the original transactions have been reversed and accruals have been posted through 24 months.</span></span>
35. <span data-ttu-id="66ce0-158">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="66ce0-158">Close all pages.</span></span>

