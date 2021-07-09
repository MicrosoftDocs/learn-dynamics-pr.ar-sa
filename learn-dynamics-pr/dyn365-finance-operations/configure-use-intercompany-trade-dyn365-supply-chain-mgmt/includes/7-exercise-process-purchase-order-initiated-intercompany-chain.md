---
ms.openlocfilehash: efaa4458c970c270c14f9a78283326b24a9c831f
ms.sourcegitcommit: c30d04e437514a1b7fe1d143dc8771662953312c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/03/2021
ms.locfileid: "6073668"
---
> [!NOTE]
> <span data-ttu-id="028cb-101">قبل القيام بهذا التمرين، يجب عليك إكمال التمرين السابق **تكوين العلاقات بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-101">Before you perform this exercise, you must complete the preceding exercise **Configure intercompany relations**.</span></span>
## <a name="scenario"></a><span data-ttu-id="028cb-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="028cb-102">Scenario</span></span>
<span data-ttu-id="028cb-103">أنت مساعد الشراء في **USRT**، ويجب عليك شراء 10 وحدات من الصنف الجديد **D0001** من مصنع الإنتاج **USMF**.</span><span class="sxs-lookup"><span data-stu-id="028cb-103">You are the purchasing assistant in **USRT**, and you must purchase 10 units of the new item **D0001** from the production plant **USMF**.</span></span> <span data-ttu-id="028cb-104">تبدأ سلسلة الشركات الشقيقة بأمر شراء لكمية 10 وحدات من **D0001** من **USMF**.</span><span class="sxs-lookup"><span data-stu-id="028cb-104">You start the intercompany chain with a purchase order for a quantity of 10 units of **D0001** from **USMF**.</span></span>

<span data-ttu-id="028cb-105">في هذا التمرين، ستقوم بإجراء تحديثات في كل من USRT وشركة USMF الموردة حتى يتم تحديث فاتورة أمر الشراء بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="028cb-105">In this exercise, you will perform updates in both USRT and the vendor company USMF until the intercompany purchase order is invoice-updated.</span></span> <span data-ttu-id="028cb-106">تُعرف أيضاً سلسلة بين الشركات الشقيقة التي بدأت في أمر الشراء باسم السلسلة ذات القدمين.</span><span class="sxs-lookup"><span data-stu-id="028cb-106">The purchase order initiated intercompany chain is also known as the two-legged chain.</span></span>

### <a name="create-the-intercompany-purchase-order-in-usrt"></a><span data-ttu-id="028cb-107">إنشاء أمر الشراء بين الشركات الشقيقة في USRT</span><span class="sxs-lookup"><span data-stu-id="028cb-107">Create the intercompany purchase order in USRT</span></span>

1.  <span data-ttu-id="028cb-108">ابدأ في شركة **USRT** وانتقل إلى **حسابات المدفوعات > أوامر الشراء > جميع أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="028cb-108">Start in company **USRT** and go to **Accounts Payable > Purchase orders > All purchase orders**.</span></span> 
2.  <span data-ttu-id="028cb-109">حدد **جديد** في جزء الإجراء لإنشاء أمر شراء جديد.</span><span class="sxs-lookup"><span data-stu-id="028cb-109">Select **New** in the Action Pane to create a new purchase order.</span></span>
3.  <span data-ttu-id="028cb-110">حدد المورد 9009 في حقل **حساب المورد**.</span><span class="sxs-lookup"><span data-stu-id="028cb-110">Select Vendor 9009 in the **Vendor account** field.</span></span>
4.  <span data-ttu-id="028cb-111">في علامة التبويب السريعة **عام**، حدد **مركزي** في حقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="028cb-111">In the **General** FastTab, select **Central** in the **Site** field.</span></span>
5.  <span data-ttu-id="028cb-112">حدد **شيكاغو**، في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="028cb-112">Select **Chicago** in the **Warehouse** field.</span></span>
6.  <span data-ttu-id="028cb-113">تحقق من تعيين خيار **بين الشركات الشقيقة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="028cb-113">Verify that the **Intercompany** option is set to **Yes**.</span></span>
4.  <span data-ttu-id="028cb-114">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="028cb-114">Select **OK**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="028cb-115">قد تتلقى رسالة تفيد بإنشاء أمر مبيعات بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="028cb-115">You may get a message that an Intercompany sales order has been created.</span></span>
5.  <span data-ttu-id="028cb-116">سيتم إنشاء أمر الشراء وستفتح صفحة أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="028cb-116">The purchase order will be generated and the purchase order page will open.</span></span> 
7.  <span data-ttu-id="028cb-117">في علامة التبويب السريعة **بنود أوامر الشراء**، أضف رقم الصنف **T0004، اللون الفضي** في البند الأول.</span><span class="sxs-lookup"><span data-stu-id="028cb-117">In **Purchase order lines** FastTab, add item number **T0004, color of Silver** in the first line.</span></span>
6.  <span data-ttu-id="028cb-118">تحقق مما يلي في البند: **الموقع: مركزي**، **المستودع: شيكاغو**.</span><span class="sxs-lookup"><span data-stu-id="028cb-118">Verify the following on the line: **Site: Central**, **Warehouse: Chicago**.</span></span>
7.  <span data-ttu-id="028cb-119">في حقل **الكمية**، أدخِل **10**.</span><span class="sxs-lookup"><span data-stu-id="028cb-119">In the **Quantity** field, enter **10**.</span></span> 
8.  <span data-ttu-id="028cb-120">سيتم تعيين **سعر الوحدة** إلى السعر الافتراضي البالغ **160.00**.</span><span class="sxs-lookup"><span data-stu-id="028cb-120">**Unit price** will be set to the default price of **160.00**.</span></span>
7.  <span data-ttu-id="028cb-121">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="028cb-121">Select **Save** in the Action Pane.</span></span>
8.  <span data-ttu-id="028cb-122">حدد علامة التبويب **شراء** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="028cb-122">Select the **Purchase** tab on the Action Pane.</span></span>
9.  <span data-ttu-id="028cb-123">في مجموعة **الإجراءات**، حدد **تأكيد** لتأكيد أمر الشراء الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="028cb-123">In the **Actions** group, select **Confirm** to confirm the purchase order.</span></span>

    > [!NOTE]
    > <span data-ttu-id="028cb-124">إذا رأيت خطأً يفيد بأن تاريخ الشحن غير صالح، فيمكن تجاهله.</span><span class="sxs-lookup"><span data-stu-id="028cb-124">If you see an error that the ship date is invalid, it can be ignored.</span></span> <span data-ttu-id="028cb-125">تم تأكيد أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="028cb-125">The PO is confirmed.</span></span> 

9.  <span data-ttu-id="028cb-126">أغلق أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="028cb-126">Close the purchase order.</span></span>

### <a name="verify-the-intercompany-sales-order-in-usmf"></a><span data-ttu-id="028cb-127">تحقق من أمر المبيعات بين الشركات الشقيقة في USMF</span><span class="sxs-lookup"><span data-stu-id="028cb-127">Verify the intercompany sales order in USMF</span></span>

1. <span data-ttu-id="028cb-128">في **USMF**، انتقل إلى **المبيعات والتسويق > أوامر المبيعات > الأوامر بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-128">In **USMF**, go to **Sales and marketing > Sales  orders > Intercompany orders**.</span></span>
2. <span data-ttu-id="028cb-129">تحقق من إنشاء أمر المبيعات بين الشركات الشقيقة الجديد.</span><span class="sxs-lookup"><span data-stu-id="028cb-129">Verify that the new intercompany sales order was created.</span></span> <span data-ttu-id="028cb-130">بادئة رقم أمر المبيعات هي **usrt**.</span><span class="sxs-lookup"><span data-stu-id="028cb-130">The prefix of the sales order number is **usrt**.</span></span>
3. <span data-ttu-id="028cb-131">انقر نقراً مزدوجاً فوق أمر المبيعات بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="028cb-131">Double-click the intercompany sales order.</span></span>
4. <span data-ttu-id="028cb-132">تحقق من الموقع والمستودع الذي تتداول منه.</span><span class="sxs-lookup"><span data-stu-id="028cb-132">Verify the site and warehouse that you are trading from.</span></span>
5. <span data-ttu-id="028cb-133">قد يعكس **سعر الوحدة** سعر البيع العادي للصنف.</span><span class="sxs-lookup"><span data-stu-id="028cb-133">The **Unit price** may reflect the normal sales price for the item.</span></span> <span data-ttu-id="028cb-134">قم بتغييره إلى **160.00**.</span><span class="sxs-lookup"><span data-stu-id="028cb-134">Change it to **160.00**.</span></span>

## <a name="remove-credit-blocking--prerequisite-step"></a><span data-ttu-id="028cb-135">إزالة حظر الائتمان - خطوة مطلوبة مسبقاً</span><span class="sxs-lookup"><span data-stu-id="028cb-135">Remove credit blocking – prerequisite step</span></span>

1. <span data-ttu-id="028cb-136">انتقل إلى **الائتمان والتحصيلات > الإعداد > معلمات الائتمان والتحصيل**.</span><span class="sxs-lookup"><span data-stu-id="028cb-136">Go to **Credit and collections > Setup > Credit and collection parameters**.</span></span>
2. <span data-ttu-id="028cb-137">حدد علامة التبويب **ائتمان**، ثم علامة التبويب السريعة **نقطة فحص إدارة الائتمان**.</span><span class="sxs-lookup"><span data-stu-id="028cb-137">Select the **Credit** tab, and then the **Credit management checkpoint** FastTab.</span></span> 
3. <span data-ttu-id="028cb-138">قم بإزالة علامة الاختيار الموجودة على **التأكيد وقائمة الانتقاء وإيصال التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-138">Remove the check mark on **Confirmation, Picking list, and Packing slip**.</span></span>
4. <span data-ttu-id="028cb-139">إغلاق النموذج.</span><span class="sxs-lookup"><span data-stu-id="028cb-139">Close the form.</span></span> 


## <a name="generate-picking-lists-packing-slips-and-product-receipts"></a><span data-ttu-id="028cb-140">إنشاء قوائم الانتقاء وإيصالات التعبئة وإيصالات المنتجات</span><span class="sxs-lookup"><span data-stu-id="028cb-140">Generate picking lists, packing slips, and product receipts</span></span>
 

<span data-ttu-id="028cb-141">أنت مساعد الشراء في **USRT**، واشتريت 10 وحدات من الصنف **T0004، فضي** من مصنع الإنتاج (**USMF**).</span><span class="sxs-lookup"><span data-stu-id="028cb-141">You are the purchasing assistant in **USRT**, and you have purchased 10 units of item **T0004, Silver** from the production plant (**USMF**).</span></span>

<span data-ttu-id="028cb-142">لقد بدأت سلسلة الشركات الشقيقة بأمر شراء لكمية 10 وحدات من **T0004، فضي** من **USMF**.</span><span class="sxs-lookup"><span data-stu-id="028cb-142">You have started the intercompany chain with a purchase order for a quantity of 10 units of **T0004, Silver** from **USMF**.</span></span>

### <a name="generate-the-packing-slip-and-product-receipt-that-are-associated-with-this-purchase-order"></a><span data-ttu-id="028cb-143">إنشاء إيصال التعبئة وإيصال المنتج المرتبطين بأمر الشراء هذا</span><span class="sxs-lookup"><span data-stu-id="028cb-143">Generate the packing slip and product receipt that are associated with this purchase order</span></span>

1.  <span data-ttu-id="028cb-144">في **USMF**، انتقل إلى **المبيعات والتسويق > أوامر المبيعات > الأوامر بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-144">In **USMF**, go to **Sales and marketing > Sales orders >     Intercompany orders**.</span></span>
2.  <span data-ttu-id="028cb-145">حدد وقم بالوصول إلى أمر المبيعات بين الشركات الشقيقة لإنشاء إيصال التعبئة.</span><span class="sxs-lookup"><span data-stu-id="028cb-145">Select and access the intercompany sales order to generate the packing slip.</span></span>
3.  <span data-ttu-id="028cb-146">في قائمة **الانتقاء والتعبئة** في الجزء العلوي من جزء الإجراء، أسفل مجموعة **إنشاء**، حدد **إنشاء قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="028cb-146">On the **PICK AND PACK** menu at the top in the Action Pane, under the **GENERATE** group, select **Generate picking list**.</span></span>
4.  <span data-ttu-id="028cb-147">في صفحة **ترحيل قائمة الانتقاء** ضمن **المعلمة**، تحقق من تحديد **الكل** في حقل **الكمية**.</span><span class="sxs-lookup"><span data-stu-id="028cb-147">On the **Posting picking list** page, under **PARAMETER**, verify that **All** is selected in the **Quantity** field.</span></span>
5.  <span data-ttu-id="028cb-148">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="028cb-148">Select **OK**.</span></span>
6.  <span data-ttu-id="028cb-149">حدد **موافق** عند المطالبة بترحيل المستند دون طباعته.</span><span class="sxs-lookup"><span data-stu-id="028cb-149">Select **OK** when prompted to post the document without printing it.</span></span>
7.  <span data-ttu-id="028cb-150">حدد من قائمة **الانتقاء والتعبئة**، **تسجيل قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="028cb-150">Select from the **PICK AND PACK** menu, **Picking list registration**.</span></span>
8.  <span data-ttu-id="028cb-151">في جزء الاجراءات، حدد **التحديثات > تحديث الكل**.</span><span class="sxs-lookup"><span data-stu-id="028cb-151">On the Action Pane, select **Updates, Update all**.</span></span>
6.  <span data-ttu-id="028cb-152">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="028cb-152">Close the page.</span></span>
6.  <span data-ttu-id="028cb-153">في صفحة **أمر المبيعات**، في علامة التبويب **الانتقاء والتعبئة** في جزء الإجراء، ضمن مجموعة **إنشاء**، حدد **نشر إيصال التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-153">On the **Sales order** page, on the **PICK AND PACK** tab of the Action Pane, under the **GENERATE** group, select **Post packing slip**.</span></span>
7.  <span data-ttu-id="028cb-154">في صفحة **نشر إيصال التعبئة** ضمن **المعلمة**، تحقق من تحديد **الكل** في حقل **الكمية**.</span><span class="sxs-lookup"><span data-stu-id="028cb-154">On the **Packing slip posting** page under **PARAMETER**, verify that **All** is selected in the **Quantity** field.</span></span>
8.  <span data-ttu-id="028cb-155">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="028cb-155">Select **OK**.</span></span> 
9.  <span data-ttu-id="028cb-156">حدد **موافق** في حالة المطالبة بترحيل المستند دون طباعته.</span><span class="sxs-lookup"><span data-stu-id="028cb-156">Select **OK** if prompted to post the document without printing it.</span></span>
9.  <span data-ttu-id="028cb-157">في صفحة **الأوامر بين الشركات الشقيقة**، تحقق من تحديث حالة أمر المبيعات إلى **تم التسليم**.</span><span class="sxs-lookup"><span data-stu-id="028cb-157">On the **INTERCOMPANY ORDERS** page, verify that the sales order status is updated to **Delivered**.</span></span>

### <a name="generate-a-product-receipt"></a><span data-ttu-id="028cb-158">إنشاء إيصال استلام المنتج</span><span class="sxs-lookup"><span data-stu-id="028cb-158">Generate a product receipt</span></span>

1.  <span data-ttu-id="028cb-159">في **USRT**، انتقل إلى **التدبير والتوريد > أوامر الشراء > جميع أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="028cb-159">In **USRT**, go to **Procurement and sourcing > Purchase orders > All purchase orders**.</span></span>
2.  <span data-ttu-id="028cb-160">حدد أمر الشراء بين الشركات الشقيقة لإنشاء إيصال استلام المنتجات.</span><span class="sxs-lookup"><span data-stu-id="028cb-160">Select the intercompany purchase order to generate the product receipt.</span></span>
3.  <span data-ttu-id="028cb-161">في علامة التبويب **استلام** في جزء الإجراء، ضمن مجموعة **إنشاء**، حدد **إيصال استلام المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="028cb-161">On the **RECEIVE** tab of the Action Pane, under the **GENERATE** group, select **Product receipt**.</span></span>
4.  <span data-ttu-id="028cb-162">في صفحة **نشر إيصال استلام المنتجات**، ضمن **المعلمات**، تحقق من تحديد **الكمية المطلوبة** في حقل **الكمية**.</span><span class="sxs-lookup"><span data-stu-id="028cb-162">On the **Posting product receipt** page, under **PARAMETERS**, verify that **Ordered quantity** is selected in the **Quantity** field.</span></span>
5.  <span data-ttu-id="028cb-163">حدد **موافق** أسفل الصفحة.</span><span class="sxs-lookup"><span data-stu-id="028cb-163">Select **OK** at the bottom of the page.</span></span>
6.  <span data-ttu-id="028cb-164">في صفحة **أمر الشراء**، تحقق من تحديث حالة أمر الشراء إلى **تم الاستلام**.</span><span class="sxs-lookup"><span data-stu-id="028cb-164">On the **Purchase order** page, verify that the purchase order status is updated to **Received**.</span></span>

## <a name="generate-invoices"></a><span data-ttu-id="028cb-165">إنشاء الفواتير</span><span class="sxs-lookup"><span data-stu-id="028cb-165">Generate invoices</span></span>
 

<span data-ttu-id="028cb-166">أنت الآن بحاجة إلى إنشاء فاتورة أمر المبيعات في **USMF** ثم ترحيل فاتورة أمر الشراء في **USRT** المرتبط بأمر المبيعات بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="028cb-166">Now you need to generate the sales order invoice in **USMF** and then post the purchase order invoice in **USRT** that is associated with this intercompany sales order.</span></span>

### <a name="generate-the-sales-order-invoice-in-usmf"></a><span data-ttu-id="028cb-167">إنشاء فاتورة أمر المبيعات في USMF</span><span class="sxs-lookup"><span data-stu-id="028cb-167">Generate the sales order invoice in USMF</span></span>

1.  <span data-ttu-id="028cb-168">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > الأوامر بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-168">Go to **Sales and marketing > Sales orders > Intercompany orders**.</span></span>
2.  <span data-ttu-id="028cb-169">حدد أمر المبيعات بين الشركات الشقيقة لإنشاء الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="028cb-169">Select the intercompany sales order to generate the invoice.</span></span>
3.  <span data-ttu-id="028cb-170">في صفحة **الأوامر بين الشركات الشقيقة**، حدد علامة التبويب **الفاتورة**. ضمن مجموعة **إنشاء**، حدد **الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-170">On the **INTERCOMPANY ORDERS** page, select the **INVOICE** tab. Under the **GENERATE** group, select **Invoice**.</span></span>
4.  <span data-ttu-id="028cb-171">في صفحة **ترحيل الفاتورة**، ضمن **المعلمة**، تحقق من تحديد **إيصال التعبئة** في حقل **الكمية**.</span><span class="sxs-lookup"><span data-stu-id="028cb-171">On the **Posting invoice** page, under **PARAMETER**, verify that **Packing slip** is selected in the **Quantity** field.</span></span>
5.  <span data-ttu-id="028cb-172">تحقق من المعلومات الموجودة في علامة التبويب السريعة **البنود**، ثم حدد الزر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="028cb-172">Verify the information in the **Lines** FastTab and then select the **OK** button.</span></span>
6.  <span data-ttu-id="028cb-173">حدد **موافق** عند المطالبة بترحيل المستند دون طباعته.</span><span class="sxs-lookup"><span data-stu-id="028cb-173">Select **OK** when prompted to post the document without printing it.</span></span>
7.  <span data-ttu-id="028cb-174">في صفحة **الأوامر بين الشركات الشقيقة**، تحقق من تحديث حالة أمر المبيعات إلى **تمت الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-174">On the **INTERCOMPANY ORDERS** page, verify that the sales order status has been updated to **Invoiced**.</span></span>

### <a name="post-the-purchase-order-invoice-in-usrt"></a><span data-ttu-id="028cb-175">ترحيل فاتورة أمر الشراء في USRT</span><span class="sxs-lookup"><span data-stu-id="028cb-175">Post the purchase order invoice in USRT</span></span>

1.  <span data-ttu-id="028cb-176">انتقل إلى **التدبير والتوريد > أوامر الشراء > جميع أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="028cb-176">Go to **Procurement and sourcing > Purchase orders > All    purchase orders**.</span></span>
2.  <span data-ttu-id="028cb-177">حدد أمر الشراء بين الشركات الشقيقة لإنشاء الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="028cb-177">Select the intercompany purchase order to generate the invoice.</span></span>
3.  <span data-ttu-id="028cb-178">في علامة التبويب **الفاتورة** في جزء الإجراء، ضمن مجموعة **إنشاء**، حدد **الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-178">On the **INVOICE** tab of the Action Pane, under the **GENERATE**    group, select **Invoice**.</span></span>
5.  <span data-ttu-id="028cb-179">من جزء الإجراء، حدد الزر **مطابقة إيصالات استلام المنتجات** لمطابقة إيصالات استلام المنتجات بالفاتورة.</span><span class="sxs-lookup"><span data-stu-id="028cb-179">From the Action Pane, select the **Match product receipts** button to    match the product receipts to the invoice.</span></span>
6.  <span data-ttu-id="028cb-180">في صفحة **مطابقة إيصالات استلام المنتجات بالفاتورة‬‏‫**، حدد الزر **موافق** أسفل الشاشة.</span><span class="sxs-lookup"><span data-stu-id="028cb-180">On the **Match product receipts to invoice** page, select the **OK**    button at the bottom of the screen.</span></span>
6.  <span data-ttu-id="028cb-181">في جزء الإجراء، حدد **تحديث حالة المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-181">In the Action Pane, select **Update match status**</span></span>
7.  <span data-ttu-id="028cb-182">للإنهاء، حدد **ترحيل** من جزء الإجراء، وسيتم ترحيل الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="028cb-182">To finish, select **Post** on the Action Pane, and the invoice will post.</span></span>

    > [!NOTE]
    > <span data-ttu-id="028cb-183">قد تتلقى خطأً يفيد بأن مبلغ الفاتورة يجب أن يكون مبلغاً آخر (بسبب ضريبة المبيعات)، وإذا كان الأمر كذلك، فقم بتدوين المبلغ، والعودة إلى الفاتورة وتغيير المبلغ.</span><span class="sxs-lookup"><span data-stu-id="028cb-183">You may receive an error that the invoice amount should be another amount (due to Sales tax), and if so, make a note of the amount, go back into the invoice and change the amount.</span></span>
    
8.  <span data-ttu-id="028cb-184">في صفحة **جميع أوامر الشراء**، تحقق من تحديث حالة أمر الشراء إلى **تمت الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="028cb-184">On the **ALL PURCHASE ORDERS** page, verify that the purchase order status is    updated to **Invoiced**.</span></span> 
