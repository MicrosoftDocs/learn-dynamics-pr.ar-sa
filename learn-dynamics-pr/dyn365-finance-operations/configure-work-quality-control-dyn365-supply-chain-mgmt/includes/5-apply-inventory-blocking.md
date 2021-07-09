---
ms.openlocfilehash: ec3aa35874de38eb2e90a38eefcf08746ccf4337
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073772"
---
<span data-ttu-id="a59bc-101">تساعد عملية حظر المخزون في منع معالجة الأصناف أو استهلاكها.</span><span class="sxs-lookup"><span data-stu-id="a59bc-101">Inventory blocking helps prevent items from being processed or consumed.</span></span> <span data-ttu-id="a59bc-102">يمكنك حظر أصناف المخزون بالطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="a59bc-102">You can block inventory items in the following ways:</span></span>

-   <span data-ttu-id="a59bc-103">يدوياً</span><span class="sxs-lookup"><span data-stu-id="a59bc-103">Manually</span></span>
-   <span data-ttu-id="a59bc-104">عن طريق إنشاء أمر جودة</span><span class="sxs-lookup"><span data-stu-id="a59bc-104">By creating a quality order</span></span>
-   <span data-ttu-id="a59bc-105">عن طريق استخدام عملية تُنشئ أمر جودة</span><span class="sxs-lookup"><span data-stu-id="a59bc-105">By using a process that generates a quality order</span></span>
-   <span data-ttu-id="a59bc-106">عن طريق استخدام معلمة **حظر المخزون**</span><span class="sxs-lookup"><span data-stu-id="a59bc-106">By using the **Inventory blocking** parameter</span></span>

## <a name="blocking-items-manually"></a><span data-ttu-id="a59bc-107">حظر الأصناف يدوياً</span><span class="sxs-lookup"><span data-stu-id="a59bc-107">Blocking items manually</span></span> 

<span data-ttu-id="a59bc-108">يمكنك حظر كمية من أحد الأصناف عن طريق إنشاء حركة في صفحة **حظر المخزون**.</span><span class="sxs-lookup"><span data-stu-id="a59bc-108">You can block a quantity of an item by creating a transaction on the **Inventory blocking** page.</span></span> <span data-ttu-id="a59bc-109">تجدر الإشارة إلى أنه يمكن إجراء حظر يدوي للأصناف المتوفّرة في المخزون الفعلي فقط.</span><span class="sxs-lookup"><span data-stu-id="a59bc-109">Only items that are available as on-hand inventory can be blocked manually.</span></span>

<span data-ttu-id="a59bc-110">وبالنسبة إلى الكميات التي يتم حظرها يدوياً، عليك تحديد ما إذا كان يجب أن تتضمن أنشطة التخطيط عمليات الاستلام المتوقعة ككمية فعلية متوقعة.</span><span class="sxs-lookup"><span data-stu-id="a59bc-110">For manually-blocked quantities, you need to decide whether planning activities should include expected receipts as an expected on-hand quantity.</span></span>
<span data-ttu-id="a59bc-111">عمليات الاستلام المتوقعة هي أصناف محظورة تتوقع توفّرها كمخزون فعلي بعد اكتمال الفحص.</span><span class="sxs-lookup"><span data-stu-id="a59bc-111">Expected receipts are blocked items that you expect to be available as on-hand inventory after inspection is completed.</span></span> <span data-ttu-id="a59bc-112">ويمكنك الاحتفاظ بالتاريخ المتوقع.</span><span class="sxs-lookup"><span data-stu-id="a59bc-112">You can maintain the expected date.</span></span>

<span data-ttu-id="a59bc-113">يكون خيار **عمليات الاستلام المتوقعة** محدداً بشكل افتراضي للأصناف المحظورة من خلال أمر جودة.</span><span class="sxs-lookup"><span data-stu-id="a59bc-113">By default, the **Expected receipts** option is selected for items that are blocked through a quality order.</span></span> <span data-ttu-id="a59bc-114">يمكنك إلغاء الحظر اليدوي لكمية معيّنة عن طريق حذف الحركة في صفحة **إدارة المخزون > مهام دورية > حظر المخزون**.</span><span class="sxs-lookup"><span data-stu-id="a59bc-114">You can cancel a manual block on a quantity by deleting the transaction on the **Inventory management > Periodic tasks > Inventory blocking** page.</span></span>

<span data-ttu-id="a59bc-115">[ ![لقطة شاشة لصفحة "حظر المخزون".](../media/inventory-blocking.png) ](../media/inventory-blocking.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="a59bc-115">[ ![Screenshot of the Inventory blocking page.](../media/inventory-blocking.png) ](../media/inventory-blocking.png#lightbox)</span></span> 

## <a name="blocking-items-by-creating-a-quality-order"></a><span data-ttu-id="a59bc-116">حظر الأصناف عن طريق إنشاء أمر جودة</span><span class="sxs-lookup"><span data-stu-id="a59bc-116">Blocking items by creating a quality order</span></span>

<span data-ttu-id="a59bc-117">يمكنك تحديد أصناف يجب فحصها عن طريق إنشاء أمر جودة في صفحة **أوامر الجودة**.</span><span class="sxs-lookup"><span data-stu-id="a59bc-117">You can specify items that must be inspected by creating a quality order on the **Quality orders** page.</span></span> <span data-ttu-id="a59bc-118">عند إنشاء أمر جودة، يتم حظر الكمية التي تحددها لأحد الأصناف.</span><span class="sxs-lookup"><span data-stu-id="a59bc-118">When you create a quality order, the quantity that you specify for an item is blocked.</span></span> <span data-ttu-id="a59bc-119">وتتحكم خطة أخذ العينات المقترنة بعناصر التحكم في أمر الجودة في كمية الأصناف التي يجب فحصها فقط، وليس في الكمية التي يتم حظرها.</span><span class="sxs-lookup"><span data-stu-id="a59bc-119">The sampling plan that is associated with a quality order controls only the quantity of items that must be inspected, not the quantity that is blocked.</span></span>

<span data-ttu-id="a59bc-120">ويُذكر أن الكمية التي يتم إدخالها في أمر الجودة هي الكمية المحظورة، بصرف النظر عن الكمية التي تحدد خطة أخذ العينات ضرورة إرسالها للفحص.</span><span class="sxs-lookup"><span data-stu-id="a59bc-120">The quantity that is entered on the quality order is the quantity that is blocked, regardless of the quantity that the sampling plan specifies should be sent for inspection.</span></span>

## <a name="blocking-items-by-using-a-process-that-generates-a-quality-order"></a><span data-ttu-id="a59bc-121">حظر الأصناف عن طريق استخدام عملية تُنشئ أمر جودة</span><span class="sxs-lookup"><span data-stu-id="a59bc-121">Blocking items by using a process that generates a quality order</span></span> 

<span data-ttu-id="a59bc-122">إذا حددت عملية جودة ضرورة فحص أحد الأصناف، يتم حظر كمية من هذا الصنف تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="a59bc-122">If a quality process specifies that an item must be inspected, a quantity of the item is blocked automatically.</span></span> <span data-ttu-id="a59bc-123">وبالتالي، عند إنشاء أمر جودة تلقائياً، تتحكم خطة أخذ عينات الصنف المقترنة بأمر الجودة في كمية الأصناف المحظورة والكمية التي يجب فحصها.</span><span class="sxs-lookup"><span data-stu-id="a59bc-123">Therefore, when a quality order is generated automatically, the item sampling plan that is associated with the quality order controls the quantity of items that is blocked and the quantity that must be inspected.</span></span>

<span data-ttu-id="a59bc-124">في حالة تحديد الخيار **حظر كامل** في صفحة **إدارة المخزون > الإعداد > التحكم في الجودة > أخذ عينات للصنف**، يتم على سبيل المثال حظر الكمية الكاملة لبند أمر الشراء خلال عملية الفحص، بصرف النظر عن كمية أخذ عينات الصنف.</span><span class="sxs-lookup"><span data-stu-id="a59bc-124">If the **Full blocking** option on the **Inventory management > Setup > Quality control > Item sampling** page is selected, the full quantity of a purchase order line, for example, is blocked during inspection, regardless of the item sampling quantity.</span></span>
 
<span data-ttu-id="a59bc-125">[ ![لقطة شاشة للخيار "حظر كامل" على صفحة أخذ عينات الصنف.](../media/full-blocking.png) ](../media/full-blocking.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="a59bc-125">[ ![Screenshot of Full blocking on the item samplings page.](../media/full-blocking.png) ](../media/full-blocking.png#lightbox)</span></span>


<span data-ttu-id="a59bc-126">**مثال**</span><span class="sxs-lookup"><span data-stu-id="a59bc-126">**Example**</span></span>

<span data-ttu-id="a59bc-127">يحدد اقتران للجودة ضرورة إنشاء أمر جودة عند ترحيل إيصال تعبئة أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="a59bc-127">A quality association specifies that a quality order must be generated when a purchase order packing slip is posted.</span></span>

<span data-ttu-id="a59bc-128">ويحدد إعداد أخذ عينات الصنف لأمر الجودة ضرورة فحص 10 بالمائة من الكمية الموجودة في بند أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="a59bc-128">The item sampling setup of the quality order specifies that 10 percent of the quantity on the purchase order line must be inspected.</span></span>

<span data-ttu-id="a59bc-129">ولأن الخيار **حظر كامل** محدد في إعداد أخذ عينات الصنف، يجب حظر الكمية الكاملة لبند أمر الشراء خلال عملية الفحص، بصرف النظر عن الكمية التي يتم إرسالها للفحص.</span><span class="sxs-lookup"><span data-stu-id="a59bc-129">Because the **Full blocking** option is selected in the item sampling setup, the full quantity of the purchase order line must be blocked during inspection, regardless of the quantity that is sent for inspection.</span></span>

<span data-ttu-id="a59bc-130">عند ترحيل إيصال التعبئة، يتم إنشاء أمر جودة.</span><span class="sxs-lookup"><span data-stu-id="a59bc-130">When the packing slip is posted, a quality order is generated.</span></span> <span data-ttu-id="a59bc-131">يتم إرسال عشرة بالمائة من كمية أمر الشراء للصنف إلى الفحص.</span><span class="sxs-lookup"><span data-stu-id="a59bc-131">Ten percent of the purchase order quantity for the item is sent to inspection.</span></span> <span data-ttu-id="a59bc-132">ويتم حظر الكمية الكاملة لبند أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="a59bc-132">The full quantity of the purchase order line is blocked.</span></span>

## <a name="blocking-items-by-using-the-inventory-blocking-parameter"></a><span data-ttu-id="a59bc-133">حظر الأصناف عن طريق استخدام معلمة حظر المخزون</span><span class="sxs-lookup"><span data-stu-id="a59bc-133">Blocking items by using the Inventory blocking parameter</span></span> 

<span data-ttu-id="a59bc-134">يمكنك تحديد حالات المخزون التي تكون حالات حظر باستخدام معلمة **حظر المخزون** في صفحة **إدارة المستودعات > الإعداد > المخزون > حالات المخزون**.</span><span class="sxs-lookup"><span data-stu-id="a59bc-134">You can specify which inventory statuses are blocking statuses by using the **Inventory blocking** parameter on the **Warehouse management > Setup > Inventory > Inventory statuses** page.</span></span>

![لقطة شاشة لصفحة حالات المخزون.](../media/inventory-status.png)

<span data-ttu-id="a59bc-136">لا يمكنك استخدام حالات المخزون كحالات حظر لأوامر الإنتاج أو أوامر المبيعات أو أوامر النقل أو حركات الصادر أو تكامل المشاريع.</span><span class="sxs-lookup"><span data-stu-id="a59bc-136">You can't use inventory statuses as blocking statuses for production orders, sales orders, transfer orders, outbound transactions, or project integrations.</span></span> <span data-ttu-id="a59bc-137">وبالنسبة إلى العمل الصادر، استخدم الأصناف بحالة المخزون "متوفر".</span><span class="sxs-lookup"><span data-stu-id="a59bc-137">For outbound work, use items that have an Available inventory status.</span></span>

<span data-ttu-id="a59bc-138">على سبيل المثال، إذا كانت الأصناف بالحالة **حظر**، ويتم تشغيل التخطيط الرئيسي على هذه الأصناف، تعتبر هذه الأصناف غير موجودة ويتم تزويد المخزون تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="a59bc-138">For example, if items have a status of **Blocking**, and master planning is run on those items, the items are considered missing and inventory is automatically replenished.</span></span>
