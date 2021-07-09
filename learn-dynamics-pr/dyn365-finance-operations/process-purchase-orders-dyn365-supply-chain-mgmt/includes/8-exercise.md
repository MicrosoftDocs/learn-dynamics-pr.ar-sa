---
ms.openlocfilehash: f28c6040b5ab4dd05864d5cebc2dedc7700fa28d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6072965"
---

## <a name="scenario"></a><span data-ttu-id="69133-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="69133-101">Scenario</span></span>
<span data-ttu-id="69133-102">أنت منسق الحسابات الدائنة في شركة Entertainment Systems USA Contoso، ويجب عليك إنشاء رمز مصاريف جديد لتكاليف النقل التي ستتم إضافتها إلى عناصر مختلفة وتحملها المورّد.</span><span class="sxs-lookup"><span data-stu-id="69133-102">You are the Accounts payable coordinator at Contoso Entertainment Systems USA, and you must create a new charges code for transport charges that will be added to various items and charged by the vendor.</span></span>

<span data-ttu-id="69133-103">أنشئ تكلفةاً جديداً لتكاليف النقل بالمواصفات التالية:</span><span class="sxs-lookup"><span data-stu-id="69133-103">Create a new charge for transportation fees with the following specifications:</span></span>

-   <span data-ttu-id="69133-104">**الاسم**:‏ TRANSTO</span><span class="sxs-lookup"><span data-stu-id="69133-104">**Name**: TRANSTO</span></span>
-   <span data-ttu-id="69133-105">**الوصف**: تكلفة النقل إلى مواقعنا</span><span class="sxs-lookup"><span data-stu-id="69133-105">**Description**: Transportation Fee to our sites</span></span>
-   <span data-ttu-id="69133-106">**الحساب**:‏ 411400</span><span class="sxs-lookup"><span data-stu-id="69133-106">**Account**: 411400</span></span>

<span data-ttu-id="69133-107">لا تتطلب هذه التكاليف مجموعة ضريبة مبيعات صنف.</span><span class="sxs-lookup"><span data-stu-id="69133-107">This fee does not require an item sales tax group.</span></span>

## <a name="create-a-charges-code"></a><span data-ttu-id="69133-108">إنشاء رمز تكاليف</span><span class="sxs-lookup"><span data-stu-id="69133-108">Create a charges code</span></span>

1.  <span data-ttu-id="69133-109">انتقل إلى **حسابات المدفوعات > إعداد التكاليف > رمز التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="69133-109">Go to **Accounts payable> Charges setup > Charges code**.</span></span>
2.  <span data-ttu-id="69133-110">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="69133-110">Select **New**.</span></span>
3.  <span data-ttu-id="69133-111">في حقل **رمز التكاليف**، أدخل **TRANSTO**.</span><span class="sxs-lookup"><span data-stu-id="69133-111">In the **Charges code** field, enter **TRANSTO**.</span></span>
4.  <span data-ttu-id="69133-112">في حقل **الوصف**، أدخل **تكلفة النقل إلى مواقعنا**.</span><span class="sxs-lookup"><span data-stu-id="69133-112">In the **Description** field, enter **Transportation Fee to our sites**.</span></span>
5.  <span data-ttu-id="69133-113">قم بالتغيير إلى قسم **الخصم**.</span><span class="sxs-lookup"><span data-stu-id="69133-113">Change to the **Debit** section.</span></span>
6.  <span data-ttu-id="69133-114">في حقل **النوع**، حدد **حساب دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="69133-114">In the **Type** field, select **Ledger account**.</span></span>
7.  <span data-ttu-id="69133-115">في حقل **الترحيل**، حدد **تكلفة الدفع**.</span><span class="sxs-lookup"><span data-stu-id="69133-115">In the **Posting** field, select **Payment fee**.</span></span>
8.  <span data-ttu-id="69133-116">في حقل **الحساب**، حدد **411400**.</span><span class="sxs-lookup"><span data-stu-id="69133-116">In the **Account** field, select **411400**.</span></span>
9.  <span data-ttu-id="69133-117">قم بالتغيير إلى قسم **الائتمان**.</span><span class="sxs-lookup"><span data-stu-id="69133-117">Change to the **Credit** section.</span></span>
10. <span data-ttu-id="69133-118">في الحقل **نوع**، حدد **عميل/مورد**.</span><span class="sxs-lookup"><span data-stu-id="69133-118">In the **Type** field, select **Customer/Vendor**.</span></span>
11. <span data-ttu-id="69133-119">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-119">Select **Save**.</span></span>

## <a name="create-a-vendor-charges-group"></a><span data-ttu-id="69133-120">أنشئ مجموعة تكاليف مورد.</span><span class="sxs-lookup"><span data-stu-id="69133-120">Create a vendor charges group</span></span>

<span data-ttu-id="69133-121">لدى المورد Fabrikam حسابان للمورد تشتري منهما الأصناف.</span><span class="sxs-lookup"><span data-stu-id="69133-121">Vendor Fabrikam has two vendor accounts that you purchase items from.</span></span>
<span data-ttu-id="69133-122">لقد قرروا إدخال تكاليف شحن إضافية بنسبة 15 بالمائة لجميع أوامر الشراء.</span><span class="sxs-lookup"><span data-stu-id="69133-122">They have decided to enter an additional 15 percent freight charges for all purchase orders.</span></span>

<span data-ttu-id="69133-123">بصفتك مسؤول حسابات المدفوعات، أنت بحاجة إلى إعداد مجموعة جديدة لتكاليف الموردين وتعيين الرمز إلى البائعين US-101 وUS-104.</span><span class="sxs-lookup"><span data-stu-id="69133-123">As the Accounts payable administrator, you need to set up a new vendor charges group and assign the code to vendors US-101 and US-104.</span></span>
<span data-ttu-id="69133-124">اسم مجموعه التكاليف الجديدة هي **06** والوصف هو **شحن 15%**.</span><span class="sxs-lookup"><span data-stu-id="69133-124">The name of the new charges group is **06** and the description is **Freight 15%**.</span></span>


1.  <span data-ttu-id="69133-125">انتقل إلى **حسابات المدفوعات > إعداد التكاليف > مجموعة تكاليف المورد**.</span><span class="sxs-lookup"><span data-stu-id="69133-125">Go to **Accounts payable > Charges setup > Vendor charges group**.</span></span>
2.  <span data-ttu-id="69133-126">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="69133-126">Select **New**.</span></span>
3.  <span data-ttu-id="69133-127">في حقل **مجموعة التكاليف**، أدخل **06**.</span><span class="sxs-lookup"><span data-stu-id="69133-127">In the **Charges group** field, enter **06**.</span></span>
4.  <span data-ttu-id="69133-128">في الحقل **وصف**، أدخل **شحن 15%**.</span><span class="sxs-lookup"><span data-stu-id="69133-128">In the **Description** field, enter **Freight 15%**.</span></span>
5.  <span data-ttu-id="69133-129">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-129">Select **Save**.</span></span>
 
## <a name="update-vendors-to-use-the-new-vendor-charges-group"></a><span data-ttu-id="69133-130">تحديث الموردين لاستخدام مجموعة تكاليف المورد الجديدة</span><span class="sxs-lookup"><span data-stu-id="69133-130">Update vendors to use the new vendor charges group</span></span>

1.  <span data-ttu-id="69133-131">انتقل إلى **حسابات المدفوعات > الموردين > جميع الموردين**.</span><span class="sxs-lookup"><span data-stu-id="69133-131">Go to **Accounts payable > Vendors > All vendors**.</span></span>
2.  <span data-ttu-id="69133-132">افتح سجل المورد الخاص بالمورد **US-101** ‏(Fabrikam للإلكترونيات).</span><span class="sxs-lookup"><span data-stu-id="69133-132">Open the vendor record for vendor **US-101** (Fabrikam Electronics).</span></span>
3.  <span data-ttu-id="69133-133">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="69133-133">Select **Edit**.</span></span>
4.  <span data-ttu-id="69133-134">افتح علامة التبويب السريعة **القيم الافتراضية لأمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="69133-134">Open the **Purchase order defaults** FastTab.</span></span>
5.  <span data-ttu-id="69133-135">في حقل **مجموعة التكاليف**، حدد **06** (شحن 15%).</span><span class="sxs-lookup"><span data-stu-id="69133-135">In the **Charges group** field, select **06** (Freight 15%).</span></span>
6.  <span data-ttu-id="69133-136">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-136">Select **Save**.</span></span>
7.  <span data-ttu-id="69133-137">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="69133-137">Close all the pages.</span></span>
7.  <span data-ttu-id="69133-138">انتقل إلى **حسابات المدفوعات > الموردين > جميع الموردين**.</span><span class="sxs-lookup"><span data-stu-id="69133-138">Go to **Accounts payable > Vendors > All Vendors**.</span></span>
8.  <span data-ttu-id="69133-139">افتح سجل المورد الخاص بالمورد **US-104** ‏(مورد Fabrikam).</span><span class="sxs-lookup"><span data-stu-id="69133-139">Open the vendor record for vendor **US-104** (Fabrikam Supplier).</span></span>
9.  <span data-ttu-id="69133-140">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="69133-140">Select **Edit**.</span></span>
10. <span data-ttu-id="69133-141">افتح علامة التبويب السريعة **القيم الافتراضية لأمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="69133-141">Open the **Purchase order defaults** FastTab.</span></span>
11. <span data-ttu-id="69133-142">في حقل **مجموعة التكاليف**، حدد **06** (شحن 15%).</span><span class="sxs-lookup"><span data-stu-id="69133-142">In the **Charges group** field, select **06** (Freight 15%).</span></span>
12. <span data-ttu-id="69133-143">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-143">Select **Save**.</span></span>
13. <span data-ttu-id="69133-144">أغلق سجل المورد.</span><span class="sxs-lookup"><span data-stu-id="69133-144">Close the vendor record.</span></span>

## <a name="create-an-item-charges-group"></a><span data-ttu-id="69133-145">إنشاء مجموعة تكاليف الصنف</span><span class="sxs-lookup"><span data-stu-id="69133-145">Create an item charges group</span></span> 

<span data-ttu-id="69133-146">نظراً للكمية الكبيرة والوزن الكبير للأصناف المشتراة، تطبق Datum Receivers ‏(US-105) تكاليف شحن بنسبة 15 بالمائة لجميع الأوامر.</span><span class="sxs-lookup"><span data-stu-id="69133-146">Because of the large quantity and weight of items bought, Datum Receivers (US-105) apply a 15 percent freight charge for all orders.</span></span>

1.  <span data-ttu-id="69133-147">انتقل إلى **حسابات المدفوعات > إعداد التكاليف > مجموعة تكاليف الصنف**.</span><span class="sxs-lookup"><span data-stu-id="69133-147">Go to **Accounts payable > Charges setup > Item charge groups**.</span></span>
2.  <span data-ttu-id="69133-148">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="69133-148">Select **New**.</span></span>
3.  <span data-ttu-id="69133-149">في حقل **مجموعة التكاليف**، أدخل **123**.</span><span class="sxs-lookup"><span data-stu-id="69133-149">In the **Charges group** field, enter **123**.</span></span>
4.  <span data-ttu-id="69133-150">في الحقل **وصف**، أدخل **تكلفة شحن 15%**.</span><span class="sxs-lookup"><span data-stu-id="69133-150">In the **Description** field, enter **15% Freight Charge**.</span></span>
5.  <span data-ttu-id="69133-151">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-151">Select **Save**.</span></span>

## <a name="create-an-automatic-charge"></a><span data-ttu-id="69133-152">إنشاء تكلفة تلقائية</span><span class="sxs-lookup"><span data-stu-id="69133-152">Create an automatic charge</span></span> 

<span data-ttu-id="69133-153">لديك مجموعة معينة من التكاليف التي تنطبق على جميع المشتريات من موردين معينين.</span><span class="sxs-lookup"><span data-stu-id="69133-153">You have a certain set of charges that apply on all purchases from certain vendors.</span></span>

<span data-ttu-id="69133-154">قم بإعداد تكلفة تلقائية يتم تطبيقها على جميع المشتريات، حيث سيتم فرض رسوم تسليم بنسبة 15 بالمائة على جميع الأوامر على مستوى البند وتنطبق فقط على مجموعة تكاليف مورد معينة (06) ومجموعة تكاليف صنف معينة (123).</span><span class="sxs-lookup"><span data-stu-id="69133-154">Set up an automatic charge that will apply to all purchases, where it will charge a 15 percent delivery charge to all orders at the line level and applies for only a certain vendor charges group (06) and a certain item charges group (123).</span></span>

1.  <span data-ttu-id="69133-155">انتقل إلى **حسابات المدفوعات > إعداد التكلفة > الرسوم التلقائية**.</span><span class="sxs-lookup"><span data-stu-id="69133-155">Go to **Accounts payable > Charges setup > Automatic charges**.</span></span>
2.  <span data-ttu-id="69133-156">في حقل **المستوى**، حدد **البند**</span><span class="sxs-lookup"><span data-stu-id="69133-156">In the **Level** field, select **Line**</span></span> 
2.  <span data-ttu-id="69133-157">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="69133-157">Select **New**.</span></span>
4.  <span data-ttu-id="69133-158">في الحقل **كود الحساب**، حدد **مجموعة**</span><span class="sxs-lookup"><span data-stu-id="69133-158">In the **Account code** field, select **Group**.</span></span>
5.  <span data-ttu-id="69133-159">في حقل **علاقة المورد**، حدد **06** (شحن 15%).</span><span class="sxs-lookup"><span data-stu-id="69133-159">In the **Vendor relation** field, select **06** (Freight 15%).</span></span>
6.  <span data-ttu-id="69133-160">في حقل **كود الصنف**، حدد **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="69133-160">In the **Item code** field, select **Group**.</span></span>
7.  <span data-ttu-id="69133-161">في حقل **علاقة الصنف**، حدد **123**.</span><span class="sxs-lookup"><span data-stu-id="69133-161">In the **Item Relation** field, select **123**.</span></span>
8.  <span data-ttu-id="69133-162">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-162">Select **Save**.</span></span>
9.  <span data-ttu-id="69133-163">حدد **إضافة** في علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="69133-163">Select **Add** in the **Lines** FastTab.</span></span>
10. <span data-ttu-id="69133-164">في حقل **رمز التكاليف**، حدد **TRANSTO** (رسم النقل).</span><span class="sxs-lookup"><span data-stu-id="69133-164">In the **Charges code** field, select **TRANSTO** (Transportation Fee).</span></span>
11. <span data-ttu-id="69133-165">في حقل **الفئة**، حدد **نسبة مئوية**.</span><span class="sxs-lookup"><span data-stu-id="69133-165">In the **Category** field, select **Percent**.</span></span>
12. <span data-ttu-id="69133-166">في حقل **قيمة التكاليف**، أدخل **15.00**.</span><span class="sxs-lookup"><span data-stu-id="69133-166">In the **Charges value** field, enter **15.00**.</span></span>
13. <span data-ttu-id="69133-167">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="69133-167">Select **Save**.</span></span>
14. <span data-ttu-id="69133-168">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="69133-168">Close all the pages.</span></span>
