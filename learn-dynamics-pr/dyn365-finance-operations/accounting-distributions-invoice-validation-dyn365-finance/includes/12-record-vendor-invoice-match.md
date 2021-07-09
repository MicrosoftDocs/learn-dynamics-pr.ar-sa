---
ms.openlocfilehash: f52bd0a123d4824fb0eeba6b580d8fadbccf7dc1
ms.sourcegitcommit: c30d04e437514a1b7fe1d143dc8771662953312c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/03/2021
ms.locfileid: "6071024"
---
## <a name="scenario"></a><span data-ttu-id="0ba63-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="0ba63-101">Scenario</span></span>
<span data-ttu-id="0ba63-102">عند استلام فاتورة من مورد بضائع أو خدمات في أمر شراء، قد تتطلب العمليات التجارية استلام البضائع أو الخدمات قبل اعتماد الفاتورة للدفع.</span><span class="sxs-lookup"><span data-stu-id="0ba63-102">When you receive an invoice from a vendor for goods or services on a purchase order, the business processes might require that the goods or services be received before the invoice can be approved for payment.</span></span>
 
## <a name="before-you-begin"></a><span data-ttu-id="0ba63-103">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="0ba63-103">Before you begin</span></span> 

<span data-ttu-id="0ba63-104">في الصفحة **الحسابات الدائنة > إعداد >معلمات حسابات الدائنة**، حدد الخيار **التحقق من صحة الفاتورة** وتأكد من تحديد الخيار **تمكين التحقق من صحة مطابقة الفاتورة**، وتعيين الحقل **ترحيل فاتورة مع اختلافات** على **المطالبة بالاعتماد**، وتعيين حقل **سياسة مطابقه البند** إلى **مطابقة ثلاثية**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-104">On the **Accounts payable > Setup > Accounts payable parameters** page, select **Invoice validation** and ensure the **Enable invoice matching validation** option is selected, the **Post invoice with discrepancies** field is set to **Require approval**, and the **Line matching policy** field is set to **Three-way matching**.</span></span>

## <a name="create-a-purchase-order"></a><span data-ttu-id="0ba63-105">إنشاء أمر شراء</span><span class="sxs-lookup"><span data-stu-id="0ba63-105">Create a purchase order</span></span> 

1.  <span data-ttu-id="0ba63-106">في الشركة، **USMF** انتقل إلى **الحسابات الدائنة > أوامر الشراء > كافة أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-106">In the company **USMF** go to **Accounts payable > Purchase orders > All purchase orders**.</span></span>
2.  <span data-ttu-id="0ba63-107">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-107">Select **New**.</span></span>
3.  <span data-ttu-id="0ba63-108">في حقل **حساب المورد**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="0ba63-108">In the **Vendor account** field, select the drop-down button to open the lookup.</span></span>
4.  <span data-ttu-id="0ba63-109">في حقل **حساب المورد**، حدد **Rain Projectors US-103**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-109">In the **Vendor account** field, select **US-103 Rain Projectors**.</span></span>
5.  <span data-ttu-id="0ba63-110">تحت علامة التبويب السريعة **عام**، في حقل **المستودع** حدد 11</span><span class="sxs-lookup"><span data-stu-id="0ba63-110">Under the **General** FastTab, in the **Warehouse** field select 11</span></span>
6.  <span data-ttu-id="0ba63-111">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-111">Select **OK**.</span></span>
7.  <span data-ttu-id="0ba63-112">دون ملاحظة عن **رقم أمر الشراء**، ستحتاج إلى ذلك لتمرين التالي.</span><span class="sxs-lookup"><span data-stu-id="0ba63-112">Make a note of the **purchase order number**, you will need this for the next exercise.</span></span> <span data-ttu-id="0ba63-113">يتم عرض رقم أمر الشراء في أعلى يسار الصفحة، كما هو موضح أدناه.</span><span class="sxs-lookup"><span data-stu-id="0ba63-113">The purchase order number will be shown on the upper left of the page, as shown below.</span></span>
    <span data-ttu-id="0ba63-114">    [![لقطة شاشة لكافة صفحات أوامر الشراء التي تظهر رقم أمر الشراء.](../media/po-number.png)](../media/po-number.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0ba63-114">    [ ![Screenshot of All purchase orders page showing the purchase order number.](../media/po-number.png) ](../media/po-number.png#lightbox)</span></span>



8.  <span data-ttu-id="0ba63-115">ضمن **بنود أمر الشراء**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-115">Under the **Purchase order lines**, select **Add line**.</span></span>
9.  <span data-ttu-id="0ba63-116">في الحقل **رقم الصنف**، حدد A0001.</span><span class="sxs-lookup"><span data-stu-id="0ba63-116">In the **Item number** field, select A0001.</span></span>
10. <span data-ttu-id="0ba63-117">في حقل **الكمية**، أدخِل 60.</span><span class="sxs-lookup"><span data-stu-id="0ba63-117">In the **Quantity** field type 60.</span></span>
11. <span data-ttu-id="0ba63-118">في جزء الإجراء، حدد علامة التبويب **شراء**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-118">On the Action Pane, select the **Purchase** tab.</span></span>
12. <span data-ttu-id="0ba63-119">حدد **تأكيد**، موجود ضمن القائمة الفرعية **الإجراءات**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-119">Select **Confirm**, found under the **Actions** submenu.</span></span>


## <a name="post-a-product-receipt"></a><span data-ttu-id="0ba63-120">ترحيل إيصال استلام</span><span class="sxs-lookup"><span data-stu-id="0ba63-120">Post a product receipt</span></span> 

1.  <span data-ttu-id="0ba63-121">في جزء الإجراء، حدد **استلام**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-121">On the Action Pane, select **Receive**.</span></span>
2.  <span data-ttu-id="0ba63-122">حدد **إيصال استلام المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-122">Select **Product receipt**.</span></span>
3.  <span data-ttu-id="0ba63-123">في الحقل **إيصال استلام المنتجات**، اكتب **RainPR1**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-123">In the **Product receipt** field, type **RainPR1**.</span></span>
4.  <span data-ttu-id="0ba63-124">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-124">Select **OK**.</span></span>


## <a name="record-and-match-a-vendor-invoice-to-a-product-receipt"></a><span data-ttu-id="0ba63-125">تسجيل فاتورة مورد ومطابقتها بإيصال استلام منتجات</span><span class="sxs-lookup"><span data-stu-id="0ba63-125">Record and match a vendor invoice to a product receipt</span></span> 

1.  <span data-ttu-id="0ba63-126">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-126">On the Action Pane, select **Invoice**.</span></span>
2.  <span data-ttu-id="0ba63-127">حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-127">Select **Invoice**.</span></span>
3.  <span data-ttu-id="0ba63-128">ضمن **رأس فاتورة المورد**، في الحقل **الرقم**، اكتب **RainInv1**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-128">Under the **Vendor invoice header**, in the **Number** field, type **RainInv1**.</span></span>
4.  <span data-ttu-id="0ba63-129">في جزء الإجراء، حدد **الافتراضي من: كمية إيصال استلام المنتجات** لفتح القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="0ba63-129">In the Action Pane, select **Default from: Product receipt quantity** to open the drop-down menu.</span></span>
     <span data-ttu-id="0ba63-130">![لقطة شاشة للأسفل تحت القائمة الافتراضية من: كمية إيصال استلام المنتجات.](../media/default-from-dialog-box.png)</span><span class="sxs-lookup"><span data-stu-id="0ba63-130">![Screenshot of the the drop-down menu under Default from: Product receipt quantity.](../media/default-from-dialog-box.png)</span></span>

5.  <span data-ttu-id="0ba63-131">في الحقل **الكمية الافتراضية للبنود**، قم بتحديد **كمية إيصال استلام المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-131">In the **Default quantity for lines** field, select **Product receipt quantity**.</span></span>
6.  <span data-ttu-id="0ba63-132">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-132">Select **OK**.</span></span>
7.  <span data-ttu-id="0ba63-133">في الرسالة حول تغيير الإعداد، حدد **نعم**، في حالة تلقي الرسالة.</span><span class="sxs-lookup"><span data-stu-id="0ba63-133">In the message about changing the setting, select **Yes**, if message received.</span></span>
8.  <span data-ttu-id="0ba63-134">في جزء الإجراء، حدد **مطابقة إيصالات استلام المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-134">In the Action Pane, select **Match product receipts**.</span></span>
9.  <span data-ttu-id="0ba63-135">التحقق من حالة **مطابقة إيصالات استلام المنتجات بالفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-135">Verify the status of **Match product receipts to invoice**.</span></span>
    <span data-ttu-id="0ba63-136">[ ![لقطة شاشة لصفحة مطابقة إيصالات استلام المنتجات بالفاتورة.](../media/match-product-receipts-to-invoice-2.png) ](../media/match-product-receipts-to-invoice-2.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0ba63-136">[ ![Screenshot of the Match product receipts to invoice page.](../media/match-product-receipts-to-invoice-2.png) ](../media/match-product-receipts-to-invoice-2.png#lightbox)</span></span>

10. <span data-ttu-id="0ba63-137">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-137">Select **OK**.</span></span>
11. <span data-ttu-id="0ba63-138">في جزء الإجراء، حدد **مراجعة** ملاحظة: قد تحتاج إلى تحديد موقع علامة التبويب مراجعة عن طريق تحديد علامة التبويب أكثر (...) إلى اليمين.</span><span class="sxs-lookup"><span data-stu-id="0ba63-138">On the Action Pane, select **Review** Note: You may need to locate the Review tab by selecting the More (...) tab at the right.</span></span>
    <span data-ttu-id="0ba63-139">[![لقطة شاشة لجزء الإجراءات، وتظهر علامة التبويب "أكبر" على اليمين. ](../media/more.png)](../media/more.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0ba63-139">[ ![Screenshot of the Action Pane, showing the More tab at the right.](../media/more.png) ](../media/more.png#lightbox)</span></span>

12. <span data-ttu-id="0ba63-140">حدد **تفاصيل المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="0ba63-140">Select **Matching details**.</span></span>
13. <span data-ttu-id="0ba63-141">تحقق من النتائج.</span><span class="sxs-lookup"><span data-stu-id="0ba63-141">Verify results.</span></span>
14. <span data-ttu-id="0ba63-142">**عدم** ترحيل الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="0ba63-142">Do **NOT** post the invoice.</span></span>
15. <span data-ttu-id="0ba63-143">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="0ba63-143">Close all pages.</span></span>

