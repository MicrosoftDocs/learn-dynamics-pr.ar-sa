---
ms.openlocfilehash: 1aaa6de3d3359c8ebfeefe3c250777268e15be52
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070699"
---
## <a name="scenario"></a><span data-ttu-id="9227d-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="9227d-101">Scenario</span></span>

<span data-ttu-id="9227d-102">ستقوم بتكوين مكونات الحسابات الدائنة في الشركة التجريبية USMF.</span><span class="sxs-lookup"><span data-stu-id="9227d-102">You will configure the components of Accounts payable in the USMF demo company.</span></span> <span data-ttu-id="9227d-103">ستقوم بتنفيذ المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="9227d-103">You will perform the following tasks:</span></span>

- <span data-ttu-id="9227d-104">‏‫حدد رسوم دفع المورّد‬.</span><span class="sxs-lookup"><span data-stu-id="9227d-104">Define vendor payment fees.</span></span>
- <span data-ttu-id="9227d-105">قم بإعداد أكواد المصاريف للحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="9227d-105">Set up charge codes for Accounts payable.</span></span>
- <span data-ttu-id="9227d-106">قم بإنشاء مجموعات رسوم للموردين.</span><span class="sxs-lookup"><span data-stu-id="9227d-106">Create charges groups for vendors.</span></span>
- <span data-ttu-id="9227d-107">قم بإنشاء مجموعات مصاريف الأصناف.</span><span class="sxs-lookup"><span data-stu-id="9227d-107">Create item charges groups.</span></span>
- <span data-ttu-id="9227d-108">حدد الرسوم التلقائية.</span><span class="sxs-lookup"><span data-stu-id="9227d-108">Define auto charges.</span></span>

## <a name="define-vendor-payment-fees"></a><span data-ttu-id="9227d-109">‏‫تحديد رسوم دفع المورّد‬</span><span class="sxs-lookup"><span data-stu-id="9227d-109">Define vendor payment fees</span></span> 

1.  <span data-ttu-id="9227d-110">انتقل إلى **الحسابات الدائنة > إعداد الدفع > رسوم الدفع**.</span><span class="sxs-lookup"><span data-stu-id="9227d-110">Go to **Accounts payable > Payment setup > Payment fee**.</span></span>
2.  <span data-ttu-id="9227d-111">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9227d-111">Select **New**.</span></span>
3.  <span data-ttu-id="9227d-112">في الحقل **معرف الرسوم**، أدخل **EFT_Fee**.</span><span class="sxs-lookup"><span data-stu-id="9227d-112">In the **Fee ID** field, enter **EFT_Fee**.</span></span>
4.  <span data-ttu-id="9227d-113">في الحقل **الاسم**، أدخل **رسم EFT**.</span><span class="sxs-lookup"><span data-stu-id="9227d-113">In the **Name** field, enter **EFT Fee**.</span></span>
5.  <span data-ttu-id="9227d-114">في الحقل **وصف الرسوم**، ادخل وصفاً يوفر مزيداً من التفاصيل حول الرسوم مثل **رسوم النقل الإلكترونية**.</span><span class="sxs-lookup"><span data-stu-id="9227d-114">In the **Fee description** field, enter a description that provides more detail about the fee such as **Electronic Transfer Fee**.</span></span>
6.  <span data-ttu-id="9227d-115">في الحقل **التكلفة**، حدد **المورد**.</span><span class="sxs-lookup"><span data-stu-id="9227d-115">In the **Charge** field, select **Vendor**.</span></span>
    <span data-ttu-id="9227d-116">ملاحظه: يستخدم **المورد** عندما يتم تقييم الرسوم إلى المورد.</span><span class="sxs-lookup"><span data-stu-id="9227d-116">Note: **Vendor** is used when the fee will be assessed to the vendor.</span></span> <span data-ttu-id="9227d-117">يستخدم **دفتر الأستاذ** عندما يتم توسيع الرسوم إلى مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="9227d-117">**Ledger** is used when the fee will be expensed to your organization.</span></span> 
7.  <span data-ttu-id="9227d-118">اترك **الحساب الرئيسي** فارغا عند توفر هذا الخيار فقط عند تحديد **دفتر الأستاذ** كخيار **التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="9227d-118">Leave **Main account** blank as this option is only available when selecting **Ledger** as the **Charge** option.</span></span>
8.  <span data-ttu-id="9227d-119">حدد **نوع دفتر اليومية** الذي يمكن استخدام هذه الرسوم عليه.</span><span class="sxs-lookup"><span data-stu-id="9227d-119">Select the **Journal type** on which this fee can be used.</span></span> <span data-ttu-id="9227d-120">نظراً لأن هذه رسوم دفع مورد، يتم تحديد **مصروفات المورد**.</span><span class="sxs-lookup"><span data-stu-id="9227d-120">Since this is a vendor payment fee select **Vendor disbursement**.</span></span>
9.  <span data-ttu-id="9227d-121">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9227d-121">Select **Save**.</span></span>
10. <span data-ttu-id="9227d-122">في جزء الإجراء، حدد **إعداد رسوم الدفع**.</span><span class="sxs-lookup"><span data-stu-id="9227d-122">On the Action Pane, select **Payment fee setup**.</span></span> 
11. <span data-ttu-id="9227d-123">في الحقل **المجموعات**، حدد **مجموعة**.</span><span class="sxs-lookup"><span data-stu-id="9227d-123">In the **Groupings** field, select **Group**.</span></span>
12. <span data-ttu-id="9227d-124">في الحقل **علاقة البنك**، حدد **BankUSA**.</span><span class="sxs-lookup"><span data-stu-id="9227d-124">In the **Bank relation** field, select **BankUSA**.</span></span>
13. <span data-ttu-id="9227d-125">حدد **طريقة الدفع** على **إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="9227d-125">Select the **Method of payment** as **Electronic**.</span></span>
14. <span data-ttu-id="9227d-126">حدد عملة الدفع **دولار أمريكي**.</span><span class="sxs-lookup"><span data-stu-id="9227d-126">Select the Payment currency **USD - US Dollar**.</span></span>
14. <span data-ttu-id="9227d-127">حدد **مواصفة الدفع** على **CCD - إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="9227d-127">Select the **Payment specification** as **CCD - Electronic**.</span></span>
15. <span data-ttu-id="9227d-128">حدد **مبلغ** لـ **النسبة المئوية/المبلغ**.</span><span class="sxs-lookup"><span data-stu-id="9227d-128">Select **Amount** for the **Percentage/Amount**.</span></span>
16. <span data-ttu-id="9227d-129">أدخل مبلغ الرسوم على أنه **2.95**.</span><span class="sxs-lookup"><span data-stu-id="9227d-129">Enter the fee amount as **2.95**.</span></span>
17. <span data-ttu-id="9227d-130">في الحقل **عملة الرسوم**، حدد **الدولار الأمريكي** كالعملة التي سيتم تقييم الرسوم بها.</span><span class="sxs-lookup"><span data-stu-id="9227d-130">In the **Fee currency** field, select **USD** as the currency in which the fee will be assessed.</span></span> 
18. <span data-ttu-id="9227d-131">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9227d-131">Select **Save**.</span></span>

## <a name="set-up-charge-codes-for-accounts-payable"></a><span data-ttu-id="9227d-132">قم بإعداد أكواد المصاريف للحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="9227d-132">Set up charge codes for Accounts payable</span></span> 

1.  <span data-ttu-id="9227d-133">انتقل إلى **الحسابات الدائنة > إعداد الرسوم > كود الرسوم**.</span><span class="sxs-lookup"><span data-stu-id="9227d-133">Go to **Accounts payable > Charges setup > Charges code**.</span></span>
2.  <span data-ttu-id="9227d-134">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="9227d-134">Select **New**.</span></span> 
3. <span data-ttu-id="9227d-135">في الحقل **كود التكاليف**، أدخل **تعجيل**.</span><span class="sxs-lookup"><span data-stu-id="9227d-135">In the **Charges code** field, enter **EXPEDITE**.</span></span>
3.  <span data-ttu-id="9227d-136">في الحقل **وصف**، أدخل **تعجيل**.</span><span class="sxs-lookup"><span data-stu-id="9227d-136">In the **Description** field, enter  **Expedite**.</span></span>
4.  <span data-ttu-id="9227d-137">في علامة التبويب السريعة **الترحيل**، ضمن القسم **المدين**، حدد **العميل/المورد** من القائمة المنسدلة **النوع**.</span><span class="sxs-lookup"><span data-stu-id="9227d-137">On the **Posting** FastTab, under the **DEBIT** section, select **Customer/Vendor** from the **Type** drop down menu.</span></span>
5.  <span data-ttu-id="9227d-138">أسفل القسم **الدائن**، حدد **حساب دفتر الأستاذ** من القائمة المنسدلة **نوع**.</span><span class="sxs-lookup"><span data-stu-id="9227d-138">Under the **CREDIT** section, select **Ledger account** from the **Type** drop down menu.</span></span>
6.  <span data-ttu-id="9227d-139">ضمن القائمة المنسدلة **ترحيل**، حدد **دفتر يومية دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="9227d-139">Under the **Posting** drop-down menu, select **Ledger journal**.</span></span>
7.  <span data-ttu-id="9227d-140">من القائمة المنسدلة **الحساب**، حدد **110110 - حساب بنكي بالدولار الأمريكي**.</span><span class="sxs-lookup"><span data-stu-id="9227d-140">From the **Account** drop down menu, select **110110 - Bank account USD**.</span></span>
8.  <span data-ttu-id="9227d-141">لتمكين مقارنة قيم المصاريف لفاتورة تحتوي على المصاريف الواردة من البنود أو الرأس الخاص بأمر الشراء المطابق، حدد **نعم** في شريط التبديل **مقارنة قيم أمر الشراء والفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="9227d-141">To enable the comparison of charges values for an invoice that contains the charges from the corresponding purchase order header or lines, select **Yes** on the **Compare purchase order and invoice values** toggle bar.</span></span>
9.  <span data-ttu-id="9227d-142">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9227d-142">Select **Save**.</span></span>

## <a name="create-charges-groups-for-vendors"></a><span data-ttu-id="9227d-143">قم بإنشاء مجموعات رسوم للموردين.</span><span class="sxs-lookup"><span data-stu-id="9227d-143">Create charges groups for vendors.</span></span> 

1.  <span data-ttu-id="9227d-144">انتقل إلى **الحسابات الدائنة > إعداد الرسوم > مجموعة رسوم المورد**.</span><span class="sxs-lookup"><span data-stu-id="9227d-144">Go to **Accounts payable > Charges setup > Vendor charges group**.</span></span>
2.  <span data-ttu-id="9227d-145">حدد **جديد**</span><span class="sxs-lookup"><span data-stu-id="9227d-145">Select **New**</span></span>
3. <span data-ttu-id="9227d-146">في حقل **مجموعة التكاليف**، أدخل **02**.</span><span class="sxs-lookup"><span data-stu-id="9227d-146">In the **Charges group** field, enter **02**.</span></span> <span data-ttu-id="9227d-147">يمكن أن يحتوي الكود على كل من الحروف والأرقام.</span><span class="sxs-lookup"><span data-stu-id="9227d-147">The code can contain both letters and numbers.</span></span>
3.  <span data-ttu-id="9227d-148">في الحقل **الوصف**، أدخل وصفاً لمجموعة المصاريف مثل **مجموعة مصاريف المورد رقم 2**.</span><span class="sxs-lookup"><span data-stu-id="9227d-148">In the **Description** field, enter a description of the charges group such as **Vendor charge group No. 2**.</span></span>
4.  <span data-ttu-id="9227d-149">حدد **حفظ** وأغلق الصفحة لحفظ التغييرات التي قمت بها.</span><span class="sxs-lookup"><span data-stu-id="9227d-149">Select **Save** and close the page to save your changes.</span></span>

## <a name="create-item-charges-groups"></a><span data-ttu-id="9227d-150">إنشاء مجموعات رسوم الأصناف</span><span class="sxs-lookup"><span data-stu-id="9227d-150">Create item charges groups</span></span> 

1.  <span data-ttu-id="9227d-151">انتقل إلى **الحسابات الدائنة > إعداد الرسوم > مجموعة رسوم الصنف**.</span><span class="sxs-lookup"><span data-stu-id="9227d-151">Go to **Accounts payable > Charges setup > Item charge groups**.</span></span>
2.  <span data-ttu-id="9227d-152">حدد **جديد** لإنشاء مجموعة رسوم للصنف.</span><span class="sxs-lookup"><span data-stu-id="9227d-152">Select **New** to create an item charges group.</span></span>
3.  <span data-ttu-id="9227d-153">في الحقل **مجموعة الرسوم**، أدخِل كوداً للمجموعة.</span><span class="sxs-lookup"><span data-stu-id="9227d-153">In the **Charges group** field, enter a code for the group.</span></span> <span data-ttu-id="9227d-154">أدخِل **02**.</span><span class="sxs-lookup"><span data-stu-id="9227d-154">Enter **02**.</span></span>
4.  <span data-ttu-id="9227d-155">في حقل **الوصف**، أدخل  **مجموعة رسوم الصنف رقم 2**.</span><span class="sxs-lookup"><span data-stu-id="9227d-155">In the **Description** field, enter **Item charges group No. 2**.</span></span>
5.  <span data-ttu-id="9227d-156">أغلق الصفحة لحفظ التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="9227d-156">Close the page to save your changes.</span></span>

## <a name="define-auto-charges"></a><span data-ttu-id="9227d-157">تحديد الرسوم التلقائية</span><span class="sxs-lookup"><span data-stu-id="9227d-157">Define auto charges</span></span> 

1. <span data-ttu-id="9227d-158">انتقل إلى **الحسابات الدائنة > إعداد التكلفة > الرسوم التلقائية**.</span><span class="sxs-lookup"><span data-stu-id="9227d-158">Go to **Accounts payable > Charges setup> Automatic charges**.</span></span>
2. <span data-ttu-id="9227d-159">حدد **جديد** لتحديد رسوم تلقائية جديدة.</span><span class="sxs-lookup"><span data-stu-id="9227d-159">Select **New** to define a new auto charge.</span></span>
3. <span data-ttu-id="9227d-160">في حقل **المستوى**، حدد **الرأس** الذي تريد تطبيق الرسم التلقائي على رأس الأمر.</span><span class="sxs-lookup"><span data-stu-id="9227d-160">In the **Level** field, select **Header** to apply the auto charge to the order header.</span></span> 
4. <span data-ttu-id="9227d-161">من القائمة المنسدلة **كود الحساب**، حدد **جدول** لتعيين المصاريف لمورد معين.</span><span class="sxs-lookup"><span data-stu-id="9227d-161">From the **Account code** drop-down menu, select **Table** to assign charges to a specific vendor.</span></span>
5. <span data-ttu-id="9227d-162">من القائمة المنسدلة **علاقة المورد**، حدد **ACME Office Supplies - 1001**.</span><span class="sxs-lookup"><span data-stu-id="9227d-162">From the **Vendor relation** drop-down menu, select **1001 - ACME Office Supplies**.</span></span>
6. <span data-ttu-id="9227d-163">يكون الإعداد الافتراضي للحقل **كود الصنف** هو **الكل** لأننا نقوم بتطبيق المصاريف التلقائية على المورد.</span><span class="sxs-lookup"><span data-stu-id="9227d-163">The **Item code** field defaults to **All** since we are applying the automatic charges to the vendor.</span></span> 
7. <span data-ttu-id="9227d-164">يتم ترك حقل **علاقة الصنف** فارغاً.</span><span class="sxs-lookup"><span data-stu-id="9227d-164">The **Item relation** field is left blank.</span></span>
8. <span data-ttu-id="9227d-165">قم بتوسيع علامة التبويب السريعة **البنود** لتحديد الرسوم ومعدلات الرسوم المطلوب استخدامها عند تطبيق الرسوم التلقائية الحالية.</span><span class="sxs-lookup"><span data-stu-id="9227d-165">Expand the **Lines** Fast Tab to define the charges and the charges rates to use when the current auto charge is applied.</span></span>
9. <span data-ttu-id="9227d-166">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9227d-166">Select **Save**.</span></span> 
10. <span data-ttu-id="9227d-167">في القائمة المنسدلة **العملة**، حدد **الدولار الأمريكي** كعملة لاستخدامها في حساب المصاريف.</span><span class="sxs-lookup"><span data-stu-id="9227d-167">In the **Currency** drop-down menu, select **USD** as the currency to use to calculate the charge.</span></span>
11. <span data-ttu-id="9227d-168">من القائمة المنسدلة **كود التكاليف**، حدد **المعالجة** ككود للتكاليف.</span><span class="sxs-lookup"><span data-stu-id="9227d-168">From the **Charges code** drop-down menu, select **Handling** as the code for the charge.</span></span>
12. <span data-ttu-id="9227d-169">من القائمة المنسدلة **الفئة**، حدد **النسبة المئوية** لتحديد كيفية حساب التكاليف.</span><span class="sxs-lookup"><span data-stu-id="9227d-169">From the **Category** drop-down menu, select **Percent** to specify how to calculate the charge.</span></span>
13. <span data-ttu-id="9227d-170">أدخل **5.00** في حقل **قيمة التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="9227d-170">Enter **5.00** in the **Charges value** field.</span></span>
14. <span data-ttu-id="9227d-171">حدد **حفظ** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="9227d-171">Select **Save** in the Action Pane.</span></span>
15. <span data-ttu-id="9227d-172">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9227d-172">Close the page.</span></span>


