---
ms.openlocfilehash: ebcd55f74398fb630cea3c0df13c8c7af705e71a
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073539"
---
## <a name="scenario"></a><span data-ttu-id="21fb7-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="21fb7-101">Scenario</span></span>
<span data-ttu-id="21fb7-102">في شركة **USMF**، تحتاج إلى توسيع قاعدة حساب العمولة التي انتهت صلاحيتها في 12/31/2017.</span><span class="sxs-lookup"><span data-stu-id="21fb7-102">In the **USMF** company, you need to extend the commission calculation rule that expired on 12/31/2017.</span></span> <span data-ttu-id="21fb7-103">تحتاج إلى إعداد كافة حسابات العمولة اللازمة لضمان حساب عمولة العميل US-013 لجميع الأصناف.</span><span class="sxs-lookup"><span data-stu-id="21fb7-103">You need to have all the necessary commission calculations set up to ensure that the commission for customer US-013 for all items is being calculated.</span></span>

## <a name="create-a-commission-calculation"></a><span data-ttu-id="21fb7-104">إنشاء حساب عمولة</span><span class="sxs-lookup"><span data-stu-id="21fb7-104">Create a Commission calculation</span></span>
1. <span data-ttu-id="21fb7-105">انتقل إلى **المبيعات والتسويق > العمولات > حساب العمولة**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-105">Go to **Sales and marketing > Commissions > Commission calculation**.</span></span>
2. <span data-ttu-id="21fb7-106">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-106">Select **New**.</span></span>
3. <span data-ttu-id="21fb7-107">في حقل **كود الصنف**، حدد **الكل**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-107">In the **Item code** field select **All**.</span></span>
4. <span data-ttu-id="21fb7-108">في حقل **كود العميل**، حدد **الكل**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-108">In the **Customer code** field select **All**.</span></span>
5. <span data-ttu-id="21fb7-109">في حقل **كود مندوب المبيعات**، حدد **الكل**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-109">In the **Sales rep code** field select **All**.</span></span>
6. <span data-ttu-id="21fb7-110">في حقل **نسبة العمولة**، أدخل **4.00**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-110">In the  **Commission percentage** field enter  **4.00**.</span></span>
7. <span data-ttu-id="21fb7-111">في حقل **سارٍ من**، أدخِل **1/01/2020**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-111">In the **From** field enter **1/01/2020**.</span></span>
8. <span data-ttu-id="21fb7-112">في حقل **حتى**، أدخِل **12/31/2020**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-112">In the **To** field enter **12/31/2020**.</span></span>

## <a name="create-a-commission-customer-group"></a><span data-ttu-id="21fb7-113">إنشاء مجموعة عملاء العمولات</span><span class="sxs-lookup"><span data-stu-id="21fb7-113">Create a Commission customer group</span></span>
1. <span data-ttu-id="21fb7-114">انتقل إلى **المبيعات والتسويق > العمولات > مجموعات العملاء للعمولات**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-114">Go to **Sales and marketing > Commissions > Customer groups for Commission**.</span></span>
2. <span data-ttu-id="21fb7-115">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-115">Select **New**.</span></span>
3. <span data-ttu-id="21fb7-116">في حقل **المجموعة**، أدخل **01**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-116">In the **Group** field enter **01**.</span></span>
4. <span data-ttu-id="21fb7-117">في حقل **الاسم** أدخل **جميع مجموعات العملاء**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-117">In the **Name** field enter  **All customer group**.</span></span>

## <a name="add-commission-share-amount"></a><span data-ttu-id="21fb7-118">إضافة مبلغ مشاركة العمولة</span><span class="sxs-lookup"><span data-stu-id="21fb7-118">Add Commission share amount</span></span>
1. <span data-ttu-id="21fb7-119">انتقل إلى **المبيعات والتسويق > العمولات > مجموعات المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-119">Go to **Sales and marketing > Commissions > Sales groups."**</span></span>
2. <span data-ttu-id="21fb7-120">حدد **عام** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="21fb7-120">Select **General** in the Action Pane.</span></span>
3. <span data-ttu-id="21fb7-121">حدد **مندوب مبيعات**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-121">Select **Sales rep**.</span></span>
4. <span data-ttu-id="21fb7-122">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-122">Select **Edit**.</span></span>
5. <span data-ttu-id="21fb7-123">في حقل **مشاركة العمولة**، أدخل **4.00**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-123">Enter **4.00** in the **Commission share** field.</span></span>


## <a name="create-sales-order"></a><span data-ttu-id="21fb7-124">إنشاء أمر مبيعات</span><span class="sxs-lookup"><span data-stu-id="21fb7-124">Create Sales order</span></span>
1.  <span data-ttu-id="21fb7-125">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-125">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>
1.  <span data-ttu-id="21fb7-126">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-126">Select **New**.</span></span>
1.  <span data-ttu-id="21fb7-127">في حقل **حساب العميل**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="21fb7-127">In the **Customer account** field, select the drop-down button to open the lookup.</span></span>
1.  <span data-ttu-id="21fb7-128">في القائمة، ابحث عن **US-013** وحدده.</span><span class="sxs-lookup"><span data-stu-id="21fb7-128">In the list, find and select **US-013**.</span></span>
1. <span data-ttu-id="21fb7-129">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-129">Select **OK**.</span></span>
1. <span data-ttu-id="21fb7-130">في الركن الأيسر العلوي من الصفحة، حدد عرض **رأسي**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-130">On the upper right of the page, select **Header** view.</span></span>
1. <span data-ttu-id="21fb7-131">قم بتوسيع قسم **الإعداد**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-131">Expand the **Setup** section.</span></span>

    <span data-ttu-id="21fb7-132">تمثل القيمة الموجودة في الحقل **مجموعة المبيعات** مجموعة تحتوي على مندوب مبيعات واحد أو أكثر يتم تعيينه لها.</span><span class="sxs-lookup"><span data-stu-id="21fb7-132">The value in the **Sales group** field represents a group with one or more sales representatives that are assigned to it.</span></span> <span data-ttu-id="21fb7-133">الأشخاص في المجموعة هم أولئك الذين سيحصلون على عمولات عند فوترة الطلب، وفقاً للأسعار والتوزيع المحدد مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="21fb7-133">The people in the group are those who will receive commissions when the order is invoiced, according to the predefined rates and distribution.</span></span> <span data-ttu-id="21fb7-134">يتم نسخ القيمة من بطاقة **العميل**، ولكن يمكنك تغييرها إذا أردت.</span><span class="sxs-lookup"><span data-stu-id="21fb7-134">The value is copied from the **Customer** card, but you can change it if you want.</span></span> <span data-ttu-id="21fb7-135">يتم أيضاً نسخ مجموعة المبيعات إلى بند أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="21fb7-135">The Sales group is also copied to the sales order line.</span></span> <span data-ttu-id="21fb7-136">يمكنك تغيير المجموعة بحيث يمكن أن تختلف عن تلك الموجودة في الرأس و/أو بين الأسطر.</span><span class="sxs-lookup"><span data-stu-id="21fb7-136">You can change the group so that it can differ from the one in the header and/or between lines.</span></span>

    <span data-ttu-id="21fb7-137">تمثل القيمة الموجودة في الحقل **مجموعة العمولة** إحدى المجموعات التي قمت بإنشائها لعميل واحد أو أكثر بغرض تعقب العمولات.</span><span class="sxs-lookup"><span data-stu-id="21fb7-137">The value in the **Commission group** field represents a group that you have created for one or more customers with the purpose of tracking commissions.</span></span> <span data-ttu-id="21fb7-138">يتم نسخ القيمة من بطاقة العميل، ولكن يمكنك تغييرها إذا أردت.</span><span class="sxs-lookup"><span data-stu-id="21fb7-138">The value is copied from the Customer card, but you can change it if you want.</span></span>

13.  <span data-ttu-id="21fb7-139">في الركن الأيسر العلوي من الصفحة، حدد عرض **البنود**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-139">On the upper right of the page select **Lines** view.</span></span>
14. <span data-ttu-id="21fb7-140">في الحقل **رقم الصنف**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="21fb7-140">In the **Item number** field, select the drop-down button to open the lookup.</span></span>
19. <span data-ttu-id="21fb7-141">في القائمة، حدد **D0001**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-141">In the list, select **D0001**.</span></span>
20. <span data-ttu-id="21fb7-142">في حقل **الكمية**، أدخِل **2**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-142">In the **Quantity** field, enter **2**.</span></span>
21. <span data-ttu-id="21fb7-143">لاحظ **المبلغ الصافي** للبند.</span><span class="sxs-lookup"><span data-stu-id="21fb7-143">Note the line's **Net amount**.</span></span> <span data-ttu-id="21fb7-144">وهو يمثل إيرادات المبيعات، والتي في هذا المثال هي أساس حساب العمولة.</span><span class="sxs-lookup"><span data-stu-id="21fb7-144">It represents the sales revenue, which in this example is the basis for commission calculation.</span></span>
22. <span data-ttu-id="21fb7-145">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-145">Select **Save**.</span></span>
23. <span data-ttu-id="21fb7-146">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-146">On the Action Pane, select **Invoice**.</span></span>
24. <span data-ttu-id="21fb7-147">ضمن مجموعة الحقل **إنشاء**، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-147">Under the **Generate** field group, select **Invoice**.</span></span>
25. <span data-ttu-id="21fb7-148">قم بتوسيع القسم **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-148">Expand the **Parameters** section.</span></span>
26. <span data-ttu-id="21fb7-149">في الحقل **الكمية**، حدد **الكل**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-149">In the **Quantity** field, select **All**.</span></span>
27. <span data-ttu-id="21fb7-150">حدد **نعم** في الحقل **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-150">Select **Yes** in the **Posting** field.</span></span>
28. <span data-ttu-id="21fb7-151">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-151">Select **OK**.</span></span>
29. <span data-ttu-id="21fb7-152">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-152">Select **OK**.</span></span> <span data-ttu-id="21fb7-153">السماح للمعالجة بإكمال الصفحة وعدم إغلاقها.</span><span class="sxs-lookup"><span data-stu-id="21fb7-153">Allow the processing to complete and don't close the page.</span></span>

## <a name="review-the-registered-sales-commissions"></a><span data-ttu-id="21fb7-154">مراجعة عمولة المبيعات المسجلة</span><span class="sxs-lookup"><span data-stu-id="21fb7-154">Review the registered sales commissions</span></span>

1.  <span data-ttu-id="21fb7-155">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-155">On the Action Pane, select **Invoice**.</span></span>
2.  <span data-ttu-id="21fb7-156">ضمن مجموعة الحقل **إنشاء**، حدد **‏‫دفاتر اليومية‬**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-156">Under the **Journals** field group, select **Invoice**.</span></span>
3.  <span data-ttu-id="21fb7-157">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-157">On the Action Pane, select **Invoice**.</span></span>
4.  <span data-ttu-id="21fb7-158">حدد **حركات العمولة**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-158">Select **Commission transactions**.</span></span>
5.  <span data-ttu-id="21fb7-159">تعرض علامة التبويب **نظرة عامة** البنود التي تمثل مبالغ العمولة المستحقة على ممثلي المبيعات والمرتبطة بأمر المبيعات المفوتر.</span><span class="sxs-lookup"><span data-stu-id="21fb7-159">The **Overview** tab displays lines that represent the commission amounts that are payable to sales representatives who are associated with the invoiced sales order.</span></span>
6.  <span data-ttu-id="21fb7-160">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="21fb7-160">Close the page.</span></span>
7.  <span data-ttu-id="21fb7-161">حدد **الإيصال**.</span><span class="sxs-lookup"><span data-stu-id="21fb7-161">Select **Voucher**.</span></span> <span data-ttu-id="21fb7-162">يمكنك مراجعة حركات الإيصال الخاصة بمبالغ العمولة التي تم ترحيلها إلى حساب مصروفات العمولة المعرفة مسبقاً وحسابات العمولات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="21fb7-162">You can review the voucher transactions for the commission amounts that have been posted to the predefined commission expense and commission payable accounts.</span></span>
8.  <span data-ttu-id="21fb7-163">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="21fb7-163">Close all pages.</span></span>
