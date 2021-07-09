---
ms.openlocfilehash: 2552f7a4a26313b7df597020da730e1813d26e98
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073777"
---

## <a name="set-up-action-policies"></a><span data-ttu-id="9f2ed-101">إعداد سياسات الإجراءات</span><span class="sxs-lookup"><span data-stu-id="9f2ed-101">Set up action policies</span></span>
 
<span data-ttu-id="9f2ed-102">تعمل أنت لصالح شركة **USMF** والآن تحتاج **USRT** إلى القدرة على شراء المنتجات من خلال علاقة بين الشركات الشقيقة من **USMF**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-102">You work for the company **USMF**, and now **USRT** needs the ability to buy products through an intercompany relationship from **USMF**.</span></span> 

<span data-ttu-id="9f2ed-103">لتسهيل علاقة الشراء/البيع هذه، يجب عليك إنشاء علاقة تجارية بين الشركات الشقيقة بين العميل **US-002** في **USMF** والمورد **9009** في **USRT**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-103">To facilitate this buy/sell relationship, you must create an intercompany trading relationship between customer **US-002** in **USMF** and vendor **9009** in **USRT**.</span></span>

<span data-ttu-id="9f2ed-104">ستشمل هذه العلاقة التجارية بين الشركات الشقيقة سياسات الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-104">This intercompany trading relationship will include action policies.</span></span> <span data-ttu-id="9f2ed-105">استخدم المعلومات التالية لإعداد سياسات الإجراءات المناسبة:</span><span class="sxs-lookup"><span data-stu-id="9f2ed-105">Use the following information to set up the appropriate action policies:</span></span>

<span data-ttu-id="9f2ed-106">**سياسات أوارمر الشراء:**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-106">**Purchase order policies:**</span></span>

-   <span data-ttu-id="9f2ed-107">**أمر المبيعات الأصلي (تسليم مباشر)**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-107">**Original sales order (direct delivery)**</span></span>
    -   <span data-ttu-id="9f2ed-108">ترحيل الفاتورة بشكل تلقائي</span><span class="sxs-lookup"><span data-stu-id="9f2ed-108">Post invoice automatically</span></span>
    -   <span data-ttu-id="9f2ed-109">طباعة الفاتورة بشكل تلقائي</span><span class="sxs-lookup"><span data-stu-id="9f2ed-109">Print invoice automatically</span></span>
-   <span data-ttu-id="9f2ed-110">**أسعار أمر شراء مشترك بين الشركات الشقيقة**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-110">**Intercompany purchase order prices**</span></span>
    -   <span data-ttu-id="9f2ed-111">السماح بتحرير السعر</span><span class="sxs-lookup"><span data-stu-id="9f2ed-111">Allow price edit</span></span>
    -   <span data-ttu-id="9f2ed-112">السماح بتحرير الخصم</span><span class="sxs-lookup"><span data-stu-id="9f2ed-112">Allow discount edit</span></span>
-   <span data-ttu-id="9f2ed-113">**أمر الشراء بين الشركات الشقيقة أمر المبيعات بين الشركات الشقيقة**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-113">**Intercompany purchase order intercompany sales order**</span></span>
    -   <span data-ttu-id="9f2ed-114">مزامنة معلومات العميل في العنوان **سياسات أوامر المبيعات:**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-114">Sync customer information on the header **Sales order policies:**</span></span>
-   <span data-ttu-id="9f2ed-115">**إنشاء أمر مبيعات مشترك بين الشركات الشقيقة**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-115">**Intercompany sales order creation**</span></span>
    -   <span data-ttu-id="9f2ed-116">استخدم **الشركة + الرقم الأصلي** لترقيم أوامر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-116">Use **Company + original number** for the sales order numbering.</span></span>
    -   <span data-ttu-id="9f2ed-117">اسمح بتحديث تلخيص المستندات للعميل الأصلي.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-117">Allow summary update of documents for original customer.</span></span>
    -   <span data-ttu-id="9f2ed-118">اطبع قائمة الانتقاء بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-118">Print picking list automatically.</span></span>
-   <span data-ttu-id="9f2ed-119">**الدفع**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-119">**Payment**</span></span>
    -   <span data-ttu-id="9f2ed-120">استخدم دفتر يومية دفع **CustPay**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-120">Use the **CustPay** payment journal.</span></span>
    -   <span data-ttu-id="9f2ed-121">قم بترحيل دفتر اليومية تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-121">Post the journal automatically.</span></span>
-   <span data-ttu-id="9f2ed-122">**أسعار أمر مبيعات مشترك بين الشركات الشقيقة**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-122">**Intercompany sales order prices**</span></span>
    -   <span data-ttu-id="9f2ed-123">البحث بالسعر والخصم</span><span class="sxs-lookup"><span data-stu-id="9f2ed-123">Price and discount search</span></span>
    -   <span data-ttu-id="9f2ed-124">السماح بتحرير السعر</span><span class="sxs-lookup"><span data-stu-id="9f2ed-124">Allow price edit</span></span>
    -   <span data-ttu-id="9f2ed-125">السماح بتحرير الخصم</span><span class="sxs-lookup"><span data-stu-id="9f2ed-125">Allow discount edit</span></span>
-   <span data-ttu-id="9f2ed-126">**أمر المبيعات بين الشركات الشقيقة أمر الشراء بين الشركات الشقيقة**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-126">**Intercompany sales order intercompany purchase order**</span></span>
    -   <span data-ttu-id="9f2ed-127">مزامنة معلومات العميل في العنوان</span><span class="sxs-lookup"><span data-stu-id="9f2ed-127">Sync customer information on the header</span></span>

### <a name="create-a-trading-relationship-with-usmf-vendor-9009"></a><span data-ttu-id="9f2ed-128">إنشاء علاقة تجارية مع مورد USMF 9009</span><span class="sxs-lookup"><span data-stu-id="9f2ed-128">Create a trading relationship with USMF vendor 9009</span></span> 

> [!NOTE] 
> <span data-ttu-id="9f2ed-129">إذا كنت تستخدم بيانات العرض التوضيحي، فهناك علاقة تجارية بين الشركات الشقيقة موجودة بالفعل بين USMF وDEMF.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-129">If you are using demo data, an intercompany trade relation already exists between USMF and DEMF.</span></span> 

1.  <span data-ttu-id="9f2ed-130">في شركة **USRT**، انتقل إلى وحدة **الحسابات الدائنة** أو وحدة **التدبير والتوريد**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-130">In company **USRT**, go to the **Accounts payable** module or the **Procurement and sourcing** module.</span></span>
2.  <span data-ttu-id="9f2ed-131">انتقل إلى **الموردين**، ثم إلى **جميع الموردين**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-131">Go to **Vendors** and then **All vendors**.</span></span>
3.  <span data-ttu-id="9f2ed-132">حدد **جديد** في جزء الإجراء لإنشاء مورد جديد.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-132">Select **New** in the Action Pane to create a new vendor.</span></span>
4.  <span data-ttu-id="9f2ed-133">في الحقل **حساب المورد**، أدخل **9009**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-133">In the **Vendor account** field, enter **9009**.</span></span>
5.  <span data-ttu-id="9f2ed-134">في حقل **الاسم**، أدخل **Contoso ‏Entertainment System USA**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-134">In the **Name** field, enter **Contoso Entertainment System USA**.</span></span>
6.  <span data-ttu-id="9f2ed-135">في حقل **المجموعة**، حدد مجموعة الموارد **90، الموردين بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-135">In the **Group** field, select Vendor group **90, Intercompany vendors**.</span></span>
7.  <span data-ttu-id="9f2ed-136">في علامة التبويب **عام** في جزء الإجراء في الجزء العلوي، في مجموعة **الإعداد**، حدد **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-136">On the **General** tab of the Action Pane at the top, in the **Set up** group, select **Intercompany**.</span></span>
8.  <span data-ttu-id="9f2ed-137">حدد علامة التبويب **العلاقة التجارية**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-137">Select the **Trading relationship** tab.</span></span>
9.  <span data-ttu-id="9f2ed-138">ضمن **تنشيط**، حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-138">Under **ACTIVATION**, select **Yes**.</span></span>
10. <span data-ttu-id="9f2ed-139">ضمن قسم **علاقة الشراء**، ستتم تعبئة حقل **شركتي** تلقائياً بـ **USRT**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-139">Under the **PURCHASE RELATION** section, the **My Company** field will auto-populate with **USRT**.</span></span> <span data-ttu-id="9f2ed-140">ستتم تعبئة حقل **حساب المورد** تلقائياً بـ **9009**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-140">The **Vendor account** field will auto-populate with **9009**.</span></span>
11. <span data-ttu-id="9f2ed-141">في قسم **علاقة المبيعات**، حقل **شركة العميل**، حدد **USMF**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-141">In the **SALES RELATION** section, **Customer company** field, select **USMF**.</span></span> <span data-ttu-id="9f2ed-142">في حقل **حسابي**، حدد **US-002**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-142">In the **My account** field, select **US-002**.</span></span>
12. <span data-ttu-id="9f2ed-143">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-143">Select **Save** in the Action Pane.</span></span>


### <a name="configure-the-purchase-order-action-policies"></a><span data-ttu-id="9f2ed-144">تكوين سياسات إجراءات أوامر الشراء</span><span class="sxs-lookup"><span data-stu-id="9f2ed-144">Configure the purchase order action policies</span></span>

1. <span data-ttu-id="9f2ed-145">حدد **سياسات أوامر الشراء** في منطقة التنقل اليسرى في صفحة **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-145">Select **Purchase order policies** in the left navigation area of the **Intercompany** page.</span></span>
2. <span data-ttu-id="9f2ed-146">حدد المربعات للحصول على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="9f2ed-146">Check the boxes for the following options:</span></span>
    - <span data-ttu-id="9f2ed-147">ترحيل الفاتورة بشكل تلقائي</span><span class="sxs-lookup"><span data-stu-id="9f2ed-147">Post invoice automatically</span></span>
    - <span data-ttu-id="9f2ed-148">طباعة الفاتورة بشكل تلقائي</span><span class="sxs-lookup"><span data-stu-id="9f2ed-148">Print invoice automatically</span></span>
    - <span data-ttu-id="9f2ed-149">السماح بتحرير السعر</span><span class="sxs-lookup"><span data-stu-id="9f2ed-149">Allow price edit</span></span>
    - <span data-ttu-id="9f2ed-150">السماح بتحرير الخصم</span><span class="sxs-lookup"><span data-stu-id="9f2ed-150">Allow discount edit</span></span>
    - <span data-ttu-id="9f2ed-151">معلومات العميل في العنوان في مجموعة **أمر المبيعات الأصلي > أمر الشراء بين الشركات الشقيقة**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-151">Customer information on the header in the **Original Sales Order > Intercompany Purchase Order** group</span></span>
1. <span data-ttu-id="9f2ed-152">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-152">Select **Save** in the Action Pane.</span></span> 

### <a name="configure-the-sales-order-action-policies"></a><span data-ttu-id="9f2ed-153">تكوين سياسات إجراءات أوامر المبيعات</span><span class="sxs-lookup"><span data-stu-id="9f2ed-153">Configure the sales order action policies</span></span>

1. <span data-ttu-id="9f2ed-154">حدد **سياسات أوامر المبيعات** في منطقة التنقل اليسرى في صفحة **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-154">Select **Sales order policies** in the left navigation area of the **Intercompany** page.</span></span>
2. <span data-ttu-id="9f2ed-155">في القائمة المنسدلة **ترقيم أوامر المبيعات** ضمن قسم **إنشاء أوامر المبيعات بين الشركات الشقيقة**، حدد **الشركة + الرقم الأصلي**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-155">In the **Sales order numbering** drop-down list under the **INTERCOMPANY SALES ORDER CREATION** section, select **Company + original number**.</span></span> 
3. <span data-ttu-id="9f2ed-156">حدد خانة الاختيار **السماح بتحديث تلخيص المستندات للعميل الأصلي‬** في قسم **إنشاء أوامر المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-156">Select the **Allow summary update of documents for original  customer** check box in the **INTERCOMPANY SALES ORDER CREATION** section.</span></span>
4. <span data-ttu-id="9f2ed-157">حدد خانة الاختيار **طباعة قائمة الانتقاء بشكل تلقائي** في قسم **إنشاء أوامر المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-157">Select the **Print picking list automatically** check box in the  **INTERCOMPANY SALES ORDER CREATION** section.</span></span>
5. <span data-ttu-id="9f2ed-158">حدد **CustPay** في القائمة المنسدلة **دفتر يومية الدفع** في قسم **الدفع**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-158">Select **CustPay** in the **Payment journal** drop-down list in the  **PAYMENT** section.</span></span>
6. <span data-ttu-id="9f2ed-159">حدد خانة الاختيار **ترحيل دفتر اليومية تلقائياً** في قسم **الدفع**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-159">Select the **Post journal automatically** check box in the  **PAYMENT** section.</span></span>
7. <span data-ttu-id="9f2ed-160">حدد خانة الاختيار **البحث بالسعر والخصم‬** في قسم **أسعار أوامر المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-160">Select the **Price and discount search** check box in the  **INTERCOMPANY SALES ORDER PRICES** section.</span></span>
8. <span data-ttu-id="9f2ed-161">حدد خانة الاختيار **السماح بتحرير السعر‬‬** في قسم **أسعار أوامر المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-161">Select the **Allow price edit** check box in the **INTERCOMPANY SALES  ORDER PRICES** section.</span></span>
9. <span data-ttu-id="9f2ed-162">حدد خانة الاختيار **السماح بتحرير الخصم‬** في قسم **أسعار أوامر المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-162">Select the **Allow discount edit** check box in the **INTERCOMPANY  SALES ORDER PRICES** section.</span></span>
10. <span data-ttu-id="9f2ed-163">حدد خانة الاختيار **معلومات العميل في العنوان** في قسم **أمر المبيعات بين الشركات الشقيقة > أمر الشراء بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-163">Select the **Customer information on the header** check box in the **INTERCOMPANY SALES ORDER > INTERCOMPANY PURCHASE ORDER** section.</span></span>
11. <span data-ttu-id="9f2ed-164">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-164">Select  **Save** on the Action Pane.</span></span>
12.  <span data-ttu-id="9f2ed-165">حدد **موافق** على أي رسائل تحذير تتلقاها.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-165">Select **OK** on any warning messages you receive.</span></span> 


## <a name="manage-order-agreement-action-policies"></a><span data-ttu-id="9f2ed-166">إدارة سياسات إجراءات اتفاقيات الأوامر</span><span class="sxs-lookup"><span data-stu-id="9f2ed-166">Manage order agreement action policies</span></span>
 

<span data-ttu-id="9f2ed-167">لتسهيل علاقة الشراء/البيع، تم إنشاء علاقة تجارية بين الشركات الشقيقة بين العميل **US-002** في **USMF** والمورد **9009** في **USRT**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-167">To facilitate the buy/sell relationship, an intercompany trading relationship has been created between customer **US-002** in **USMF** and vendor **9009** in **USRT**.</span></span>

<span data-ttu-id="9f2ed-168">ستتضمن العلاقة التجارية بين الشركات الشقيقة سياسات اتفاقيات الشراء والمبيعات.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-168">The intercompany trading relationship will include purchase and sales agreement policies.</span></span>

### <a name="allow-all-options-for-the-purchase-and-sales-agreement-policies"></a><span data-ttu-id="9f2ed-169">السماح بجميع الخيارات لسياسات اتفاقيات الشراء والمبيعات</span><span class="sxs-lookup"><span data-stu-id="9f2ed-169">Allow all options for the purchase and sales agreement policies</span></span>

1.  <span data-ttu-id="9f2ed-170">في الزاوية العلوية اليمنى من الصفحة، قم بتغيير الشركة من **USRT** إلى **USMF**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-170">In the top-right corner of the page, change the company from **USRT** to **USMF**.</span></span>
2.  <span data-ttu-id="9f2ed-171">انتقل إلى **الحسابات المدينة > العملاء > جميع العملاء**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-171">Navigate to **Accounts receivable > Customers > All customers**</span></span>
4.  <span data-ttu-id="9f2ed-172">حدد **الحساب US-002**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-172">Select **Account US-002**.</span></span>
5.  <span data-ttu-id="9f2ed-173">في علامة التبويب **عام** في جزء الإجراء، في مجموعة **الإعداد**، حدد **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-173">On the **General** tab of the Action Pane, in the **Set up**    group, select **Intercompany**.</span></span>

### <a name="configure-the-purchase-agreement-policies"></a><span data-ttu-id="9f2ed-174">تكوين سياسات اتفاقيات الشراء</span><span class="sxs-lookup"><span data-stu-id="9f2ed-174">Configure the purchase agreement policies</span></span>

1.  <span data-ttu-id="9f2ed-175">حدد علامة التبويب **سياسات اتفاقيات الشراء** في الجزء الأيسر.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-175">Select **Purchase agreement policies** tab in the left pane.</span></span>
2.  <span data-ttu-id="9f2ed-176">حدد خانة الاختيار **السماح بتفعيل/تعليق الإعداد** في قسم **اتفاقية الشراء بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-176">Select the **Allow setting on hold/effective** check box in the **INTERCOMPANY PURCHASE AGREEMENT** section.</span></span>
3.  <span data-ttu-id="9f2ed-177">حدد خانة الاختيار **السماح بتحرير فترة الصلاحية** في قسم **اتفاقية الشراء بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-177">Select the **Allow edit of validity period** check box in the **INTERCOMPANY PURCHASE AGREEMENT** section.</span></span>
4.  <span data-ttu-id="9f2ed-178">حدد خانة الاختيار **السماح بتحرير السعر‬‬** في قسم **أسعار اتفاقيات الشراء بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-178">Select the **Allow price edit** check box in the **INTERCOMPANY PURCHASE AGREEMENT PRICES** section.</span></span>
5. <span data-ttu-id="9f2ed-179">حدد خانة الاختيار **السماح بتحرير الخصم** في قسم **أسعار اتفاقيات الشراء بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-179">Select the **Allow discount edit** check box in the **INTERCOMPANY  PURCHASE AGREEMENT PRICES** section.</span></span>

### <a name="configure-the-sales-agreement-policies"></a><span data-ttu-id="9f2ed-180">تكوين سياسات اتفاقيات المبيعات</span><span class="sxs-lookup"><span data-stu-id="9f2ed-180">Configure the sales agreement policies</span></span>

1. <span data-ttu-id="9f2ed-181">حدد علامة التبويب **سياسات اتفاقيات المبيعات** في الجزء الأيسر.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-181">Select **Sales agreement policies** tab in the left pane.</span></span>
2. <span data-ttu-id="9f2ed-182">حدد خانة الاختيار **السماح بتفعيل/تعليق الإعداد** في قسم **اتفاقية المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-182">Select the **Allow setting on hold/effective** check box in the  **INTERCOMPANY SALES AGREEMENT** section.</span></span>
3. <span data-ttu-id="9f2ed-183">حدد خانة الاختيار **السماح بتحرير فترة الصلاحية** في قسم **اتفاقية المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-183">Select the **Allow edit of validity period** check box in the  **INTERCOMPANY SALES AGREEMENT** section.</span></span>
4. <span data-ttu-id="9f2ed-184">حدد خانة الاختيار **السماح بتحرير السعر‬‬** في قسم **أسعار اتفاقيات المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-184">Select the **Allow price edit** check box in the **INTERCOMPANY SALES  AGREEMENT PRICES** section.</span></span>
5. <span data-ttu-id="9f2ed-185">حدد خانة الاختيار **السماح بتحرير الخصم‬‬** في قسم **أسعار اتفاقيات المبيعات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-185">Select the **Allow discount edit** check box in the **INTERCOMPANY  SALES AGREEMENT PRICES** section.</span></span>
6. <span data-ttu-id="9f2ed-186">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-186">Select **Save** in the Action Pane.</span></span>

## <a name="configure-value-mapping"></a><span data-ttu-id="9f2ed-187">تكوين تعيين القيمة</span><span class="sxs-lookup"><span data-stu-id="9f2ed-187">Configure value-mapping</span></span>


<span data-ttu-id="9f2ed-188">الآن يجب عليك تحديد تعيين القيمة لهذه العلاقة.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-188">Now you must define the value-mapping for this relationship.</span></span> <span data-ttu-id="9f2ed-189">قم بتكوين تعيين قيمة الشراء والمبيعات للعلاقة التجارية بين الشركات الشقيقة بين **USRT** و **USMF**، المورد **9009**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-189">Configure the purchase and sales value-mapping for the intercompany trading relationship between **USRT** and **USMF**, vendor **9009**.</span></span>

### <a name="set-up-purchase-value-mapping"></a><span data-ttu-id="9f2ed-190">إعداد تعيين قيمة الشراء</span><span class="sxs-lookup"><span data-stu-id="9f2ed-190">Set up Purchase value mapping</span></span>

1.  <span data-ttu-id="9f2ed-191">قم بالرجوع إلى شركة **USRT**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-191">Switch back to the **USRT** company.</span></span>  
1.  <span data-ttu-id="9f2ed-192">انتقل إلى **الحسابات الدائنة > الموردين > جميع الموردين**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-192">Navigate to **Accounts payable > Vendors > All vendors**</span></span>
3.  <span data-ttu-id="9f2ed-193">حدد **Contoso ‏Entertainment System USA** (المورد 9009).</span><span class="sxs-lookup"><span data-stu-id="9f2ed-193">Select **Contoso Entertainment System USA** (vendor 9009).</span></span>
4.  <span data-ttu-id="9f2ed-194">في علامة التبويب **عام** في جزء الإجراء، في قسم **الإعداد**، حدد **بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-194">On the **General** tab of the Action Pane, in the **Set Up** section, select **Intercompany**.</span></span>
5. <span data-ttu-id="9f2ed-195">قم بتكوين تعيين قيمة الشراء من خلال تحديد **تعيين قيمة الشراء** في الجزء الأيسر.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-195">Configure the Purchase value-mapping by selecting **Purchase value-mapping** in the left pane.</span></span>
8. <span data-ttu-id="9f2ed-196">حدد **خاص بنا** في القائمة المنسدلة للحصول على:</span><span class="sxs-lookup"><span data-stu-id="9f2ed-196">Select **Our** in the drop-down lists for:</span></span>

    -   <span data-ttu-id="9f2ed-197">**كود وضع التسليم**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-197">**Mode of delivery code**</span></span>
    -   <span data-ttu-id="9f2ed-198">**أكواد شروط التسليم**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-198">**Delivery terms codes**</span></span>
    -   <span data-ttu-id="9f2ed-199">**كود التكاليف**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-199">**Charges code**</span></span>
    -   <span data-ttu-id="9f2ed-200">**كود سبب الإرجاع**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-200">**Return reason code**</span></span>
    -   <span data-ttu-id="9f2ed-201">**كود الترتيب**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-201">**Disposition code**</span></span>
    -   <span data-ttu-id="9f2ed-202">**تصنيف**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-202">**Classification**</span></span>
9. <span data-ttu-id="9f2ed-203">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-203">Select **Save** in the Action Pane.</span></span>


### <a name="configure-the-sales-value-mapping"></a><span data-ttu-id="9f2ed-204">تكوين تعيين قيمة المبيعات</span><span class="sxs-lookup"><span data-stu-id="9f2ed-204">Configure the Sales value-mapping</span></span>

1. <span data-ttu-id="9f2ed-205">حدد **تعيين قيمة المبيعات** في الجزء الأيسر من الصفحة بين الشركات الشقيقة للمورد 9009.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-205">Select **Sales value-mapping** in the left pane of the Intercompany page for Vendor 9009.</span></span>
4. <span data-ttu-id="9f2ed-206">حدد **خاص بنا** في القائمة المنسدلة للحصول على:</span><span class="sxs-lookup"><span data-stu-id="9f2ed-206">Select **Our** in the drop-down lists for:</span></span>
 
    -   <span data-ttu-id="9f2ed-207">**كود وضع التسليم**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-207">**Mode of delivery code**</span></span>
    -   <span data-ttu-id="9f2ed-208">**أكواد شروط التسليم**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-208">**Delivery terms codes**</span></span>
    -   <span data-ttu-id="9f2ed-209">**كود التكاليف**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-209">**Charges code**</span></span>
    -   <span data-ttu-id="9f2ed-210">**كود سبب الإرجاع**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-210">**Return reason code**</span></span>
    -   <span data-ttu-id="9f2ed-211">**كود الترتيب**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-211">**Disposition code**</span></span>
    -   <span data-ttu-id="9f2ed-212">**تصنيف**</span><span class="sxs-lookup"><span data-stu-id="9f2ed-212">**Classification**</span></span>
5. <span data-ttu-id="9f2ed-213">حدد **حفظ** وأغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9f2ed-213">Select **Save** and close the page.</span></span>
 
