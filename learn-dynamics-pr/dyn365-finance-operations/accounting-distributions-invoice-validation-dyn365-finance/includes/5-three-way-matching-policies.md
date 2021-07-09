---
ms.openlocfilehash: f235a99c73e3f3e3b5ec9333dbcb8736a0428480
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070892"
---
<span data-ttu-id="4a536-101">عند استلام فاتورة من مورد بضائع أو خدمات في أمر شراء، قد تتطلب العمليات التجارية استلام البضائع أو الخدمات قبل اعتماد الفاتورة للدفع.</span><span class="sxs-lookup"><span data-stu-id="4a536-101">When you receive an invoice from a vendor for goods or services on a purchase order, the business processes might require that the goods or services be received before the invoice can be approved for payment.</span></span> <span data-ttu-id="4a536-102">قبل البدء، تأكد من تحديد مفتاح تكوين **مطابقة الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="4a536-102">Before you begin, make sure that the **Invoice matching** configuration key is selected.</span></span>

<span data-ttu-id="4a536-103">في صفحة **الحسابات الدائنة**، تأكد من تحديد الخيار **تمكين التحقق من صحة مطابقة الفاتورة**، وتعيين الحقل **ترحيل الفاتورة التي بها اختلافات** على **طلب موافقة**، وتعيين حقل **سياسة مطابقة السطر** إلى **سياسة المطابقة الثلاثية**.</span><span class="sxs-lookup"><span data-stu-id="4a536-103">On the **Accounts payable** parameters page, ensure the **Enable invoice matching validation** option is selected, the **Post invoice with discrepancies** field is set to **Require approval**, and the **Line matching policy** field is set to **Three-way matching**.</span></span>
<span data-ttu-id="4a536-104">يستخدم هذا الإجراء شركة **USMF** للعروض التوضيحية.</span><span class="sxs-lookup"><span data-stu-id="4a536-104">This procedure uses the **USMF** demo company.</span></span> <span data-ttu-id="4a536-105">سينفذ دور مدير الحسابات الدائنة أو مدير الحسابات هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="4a536-105">The accounts payable manager or accounting manager role would perform these steps.</span></span>

## <a name="create-a-purchase-order"></a><span data-ttu-id="4a536-106">إنشاء أمر شراء</span><span class="sxs-lookup"><span data-stu-id="4a536-106">Create a purchase order</span></span> 

1.  <span data-ttu-id="4a536-107">انتقل إلى **كافة أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="4a536-107">Go to **All purchase orders**.</span></span>
2.  <span data-ttu-id="4a536-108">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="4a536-108">Select **New**.</span></span>
3.  <span data-ttu-id="4a536-109">في الحقل **حساب المورد**، اكتب قيمة.</span><span class="sxs-lookup"><span data-stu-id="4a536-109">In the **Vendor account** field, type a value.</span></span>
4.  <span data-ttu-id="4a536-110">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="4a536-110">Select **OK**.</span></span>
5.  <span data-ttu-id="4a536-111">حدد **إضافة سطر**.</span><span class="sxs-lookup"><span data-stu-id="4a536-111">Select **Add line**.</span></span>
6.  <span data-ttu-id="4a536-112">في الحقل **رقم الصنف**، اكتب قيمةً.</span><span class="sxs-lookup"><span data-stu-id="4a536-112">In the **Item number** field, type a value.</span></span>
7.  <span data-ttu-id="4a536-113">في جزء الإجراء، حدد **شراء**.</span><span class="sxs-lookup"><span data-stu-id="4a536-113">On the Action Pane, select **Purchase**.</span></span>
8.  <span data-ttu-id="4a536-114">حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="4a536-114">Select **Confirm**.</span></span>


## <a name="post-a-product-receipt"></a><span data-ttu-id="4a536-115">ترحيل إيصال استلام</span><span class="sxs-lookup"><span data-stu-id="4a536-115">Post a product receipt</span></span> 

1.  <span data-ttu-id="4a536-116">في جزء الإجراء، حدد **استلام**.</span><span class="sxs-lookup"><span data-stu-id="4a536-116">On the Action Pane, select **Receive**.</span></span>
2.  <span data-ttu-id="4a536-117">حدد **إيصال استلام المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="4a536-117">Select **Product receipt**.</span></span>
3.  <span data-ttu-id="4a536-118">في الحقل **إيصال استلام المنتجات**، اكتب قيمة.</span><span class="sxs-lookup"><span data-stu-id="4a536-118">In the **Product receipt** field, type a value.</span></span>
4.  <span data-ttu-id="4a536-119">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="4a536-119">Select **OK**.</span></span>


## <a name="record-and-match-a-vendor-invoice-to-a-product-receipt"></a><span data-ttu-id="4a536-120">تسجيل فاتورة مورد ومطابقتها بإيصال استلام منتجات</span><span class="sxs-lookup"><span data-stu-id="4a536-120">Record and match a vendor invoice to a product receipt</span></span> 

1.  <span data-ttu-id="4a536-121">في جزء الإجراء، حدد **الفاتورة > الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="4a536-121">On the Action Pane, select **Invoice > Invoice**.</span></span>
2.  <span data-ttu-id="4a536-122">وفي الحقل **الرقم**، اكتب قيمةً.</span><span class="sxs-lookup"><span data-stu-id="4a536-122">In the **Number** field, type a value.</span></span>
3.  <span data-ttu-id="4a536-123">تحديد **افتراضي من: الكمية المطلوبة** لفتح القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="4a536-123">Select **Default from: Ordered quantity** to open the drop-down menu.</span></span>
4.  <span data-ttu-id="4a536-124">في الحقل **الكمية الافتراضية للسطور**، حدد خياراً.</span><span class="sxs-lookup"><span data-stu-id="4a536-124">In the **Default quantity for lines** field, select an option.</span></span>
5.  <span data-ttu-id="4a536-125">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="4a536-125">Select **OK**.</span></span>
6.  <span data-ttu-id="4a536-126">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="4a536-126">Select **Yes**.</span></span>
7.  <span data-ttu-id="4a536-127">حدد **مطابقة إيصالات استلام المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="4a536-127">Select **Match product receipts**.</span></span>
8.  <span data-ttu-id="4a536-128">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="4a536-128">Select **OK**.</span></span>
9.  <span data-ttu-id="4a536-129">في جزء الإجراء، حدد **مراجعة**.</span><span class="sxs-lookup"><span data-stu-id="4a536-129">On the Action Pane, select **Review**.</span></span>
10. <span data-ttu-id="4a536-130">حدد **تفاصيل المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="4a536-130">Select **Matching details**.</span></span>

