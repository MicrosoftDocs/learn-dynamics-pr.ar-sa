---
ms.openlocfilehash: 119c13e899e0ddf9d5fe35c294e551b56b0eab31
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073804"
---
<span data-ttu-id="ddc6d-101">يمكن استخدام أوامر العزل لحظر المخزون.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-101">Quarantine orders can be used to block inventory.</span></span> <span data-ttu-id="ddc6d-102">على سبيل المثال، قد ترغب في عزل الأصناف لأسباب تتعلق بمراقبة الجودة.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-102">For example, you might want to quarantine items for quality control reasons.</span></span> <span data-ttu-id="ddc6d-103">يتم نقل المخزون الذي تم عزله إلى مستودع عزل.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-103">Inventory that has been quarantined is transferred to a quarantine warehouse.</span></span> 

<span data-ttu-id="ddc6d-104">لاحظ أنه إذا كنت تستخدم مستودعاً تتم إدارته باستخدام وحدة إدارة المستودعات، فسيتم استخدام معالجة أوامر العزل فقط لأوامر مبيعات المرتجعات.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-104">Note that if you're using a warehouse that is managed by using the Warehouse management module, quarantine order processing is used only for return sales orders.</span></span>

## <a name="quarantine-on-hand-inventory-items"></a><span data-ttu-id="ddc6d-105">عزل أصناف المخزون المتاحة</span><span class="sxs-lookup"><span data-stu-id="ddc6d-105">Quarantine on-hand inventory items</span></span> 

<span data-ttu-id="ddc6d-106">عندما تقوم بعزل الأصناف، يمكنك إما إنشاء أوامر العزل يدوياً أو إعداد النظام لإنشاء أوامر العزل تلقائياً أثناء المعالجة الواردة.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-106">When you quarantine items, you can either create the quarantine orders manually or set up the system to create the quarantine orders automatically during inbound processing.</span></span>

<span data-ttu-id="ddc6d-107">لإنشاء أوامر العزل تلقائياً، انتقل إلى صفحة **إدارة المخزون > الإعداد > المخزون > مجموعات نماذج الأصناف**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-107">To create quarantine orders automatically, go to the  **Inventory management > Setup > Inventory > Item model groups** page.</span></span> <span data-ttu-id="ddc6d-108">حدد خيار  **إدارة العزل** في علامة التبويب  **سياسات المخزون** .</span><span class="sxs-lookup"><span data-stu-id="ddc6d-108">Select the **Quarantine management** option on the **Inventory policies** tab.</span></span>

<span data-ttu-id="ddc6d-109">![لقطة شاشة لصفحة مجموعات نماذج الأصناف.(../media/item-model-group.png)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-109">![Screenshot of the Item model groups page.(../media/item-model-group.png)</span></span>

<span data-ttu-id="ddc6d-110">يجب عليك أيضاً تحديد مستودع عزل افتراضي في حقل  **مستودع العزل** لمستودعات الاستلام في صفحة **إدارة المخزون > الإعداد > تصنيف المخزون > المستودعات**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-110">You must also specify a default quarantine warehouse in the  **Quarantine warehouse** field for the receiving warehouses on the **Inventory management > Setup > Inventory breakdown > Warehouses** page.</span></span>

![لقطة شاشة لصفحة المستودعات مع تمييز حقل مستودع العزل.](../media/warehouse-1.png)

<span data-ttu-id="ddc6d-112">عندما يتم تسجيل المخزون المتاح فعلياً في أمر شراء أو أمر إنتاج، يتم نقل الأصناف المعزولة تلقائياً إلى مستودع عزل في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-112">When the physically on-hand inventory is recorded in a purchase order or production order, quarantined items are automatically moved to a quarantine warehouse in Supply Chain Management.</span></span>

<span data-ttu-id="ddc6d-113">تحدث هذه الحركة بسبب تغيير حالة أمر العزل إلى  **تم البدء**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-113">This movement occurs because the status of the quarantine order is changed to **Started**.</span></span> <span data-ttu-id="ddc6d-114">عند إنشاء أوامر العزل يدوياً، لا يلزم إعداد الصنف لإدارة وحدة العزل في مجموعة نماذج الأصناف المرتبطة.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-114">When you manually create quarantine orders, the item doesn't have to be set up for quarantine management in the associated item model group.</span></span>

<span data-ttu-id="ddc6d-115">بالنسبة لهذه العملية، يجب عليك تحديد المخزون المتاح الذي يجب عزله ومستودع العزل الذي يجب استخدامه.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-115">For this process, you must specify the on-hand inventory that should be quarantined and the quarantine warehouse that should be used.</span></span> <span data-ttu-id="ddc6d-116">يمكنك استخدام حالات أمر العزل للمساعدة في تخطيط العملية.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-116">You can use the quarantine order statuses to help plan the process.</span></span>

## <a name="quarantine-order-statuses"></a><span data-ttu-id="ddc6d-117">حالات أوامر العزل</span><span class="sxs-lookup"><span data-stu-id="ddc6d-117">Quarantine order statuses</span></span> 

<span data-ttu-id="ddc6d-118">يمكن أن يكون لأوامر العزل الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="ddc6d-118">Quarantine orders can have the following statuses:</span></span>

-   <span data-ttu-id="ddc6d-119">تم الإنشاء</span><span class="sxs-lookup"><span data-stu-id="ddc6d-119">Created</span></span>
-   <span data-ttu-id="ddc6d-120">تم البدء</span><span class="sxs-lookup"><span data-stu-id="ddc6d-120">Started</span></span>
-   <span data-ttu-id="ddc6d-121">تم الإبلاغ عنه كمنته</span><span class="sxs-lookup"><span data-stu-id="ddc6d-121">Reported as finished</span></span>
-   <span data-ttu-id="ddc6d-122">تم الإنهاء</span><span class="sxs-lookup"><span data-stu-id="ddc6d-122">Ended</span></span>

### <a name="created"></a><span data-ttu-id="ddc6d-123">تم الإنشاء</span><span class="sxs-lookup"><span data-stu-id="ddc6d-123">Created</span></span>

<span data-ttu-id="ddc6d-124">عندما يتم إنشاء أمر العزل يدوياً، ولكن الصنف ليس في مستودع العزل بعد، يكون لأمر العزل حالة  **تم الإنشاء** في صفحة **إدارة المخزون > المهام الدورية > إدارة الجودة > أوامر العزل**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-124">When a quarantine order has been created manually, but the item isn't yet in the quarantine warehouse, the quarantine order has a status of  **Created** on the **Inventory management > Periodic tasks > Quality management > Quarantine orders** page.</span></span>

<span data-ttu-id="ddc6d-125">[ ![لقطة شاش لصفحة أوامر العزل.](../media/created-1.png) ](../media/created-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-125">[ ![Screenshot of the Quarantine orders page.](../media/created-1.png) ](../media/created-1.png#lightbox)</span></span> 

<span data-ttu-id="ddc6d-126">حركتا مخزون، تم عرضهما في جزء الإجراء، حدد **المخزون** ثم حدد **الحركات**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-126">Two inventory transactions, viewed on the Action Pane, select **Inventory** and then select **Transactions**.</span></span>  <span data-ttu-id="ddc6d-127">تم الإنشاء: الأولى هي حركة إصدار يمكن أن تكون بحالة  **قيد الأمر** أو  **محجوز فعلي** أو  **منتقى**، والأخرى هي حركة إيصال يمكن أن تكون بحالة  **تم إصدار الأمر** أو  **مسجل** في مستودع العزل.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-127">are generated: One is an issue transaction that can have a status of **On order**, **Reserved physical**, or **Picked**, and the other is a receipt transaction that can have a status of **Ordered** or **Registered** at the quarantine warehouse.</span></span> <span data-ttu-id="ddc6d-128">يمكنك حجز التحديثات وانتقاؤها وتسجيلها في المخزون باستخدام العمليات المعتادة.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-128">You can reserve, pick, and register updates to the inventory by using the usual processes.</span></span>
 
<span data-ttu-id="ddc6d-129">[ ![لقطة شاشة لصفحة حركات المخزون.](../media/transactions-1.png) ](../media/transactions-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-129">[ ![Screenshot of the Inventory transactions page.](../media/transactions-1.png) ](../media/transactions-1.png#lightbox)</span></span>

### <a name="started"></a><span data-ttu-id="ddc6d-130">تم البدء</span><span class="sxs-lookup"><span data-stu-id="ddc6d-130">Started</span></span>

<span data-ttu-id="ddc6d-131">عندما يكون أمر عزل بحالة  **تم البدء**، يتم نقل المخزون من المستودع العادي إلى مستودع العزل، ويتم إنشاء عمليتي مخزون: واحدة بحالة **تم الخصم**، والأخرى بحالة **تم الاستلام**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-131">When a quarantine order has a status of  **Started**, the inventory is transferred from the regular warehouse to the quarantine warehouse, and two inventory transactions are generated: One that has a status of **Deducted**, and the other that has a status of **Received**.</span></span>
 
<span data-ttu-id="ddc6d-132">[![لقطة شاشة لصفحة أوامر العزل بالحالة "تم البدء". ](../media/started-1.png)](../media/started-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-132">[ ![Screenshot of the Quarantine orders page with the status Started.](../media/started-1.png) ](../media/started-1.png#lightbox)</span></span>

<span data-ttu-id="ddc6d-133">في الوقت نفسه، يتم إنشاء حركتي مخزون للتعامل مع تحويل المرتجعات.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-133">At the same time, two inventory transactions are created to handle the return transfer.</span></span>
<span data-ttu-id="ddc6d-134">هذه الحركات غير مؤرخة.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-134">These transactions aren't dated.</span></span> <span data-ttu-id="ddc6d-135">توجد حركة مخزون واحدة بحالة  **محجوز فعلي**، والأخرى بحالة  **تم إصدار الأمر**.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-135">One inventory transaction has a status of **Reserved physical**, and the other has a status of **Ordered**.</span></span>

 
<span data-ttu-id="ddc6d-136">[![لقطة شاشة لصفحة حركات المخزون بالحالة "تم البدء". ](../media/transactions-started-status.png)](../media/transactions-started-status.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-136">[ ![Screenshot of the inventory transactions page with the status Started.](../media/transactions-started-status.png) ](../media/transactions-started-status.png#lightbox)</span></span>

### <a name="reported-as-finished"></a><span data-ttu-id="ddc6d-137">تم الإبلاغ عنه كمنته</span><span class="sxs-lookup"><span data-stu-id="ddc6d-137">Reported as finished</span></span>

<span data-ttu-id="ddc6d-138">من خلال تحديد  **الإبلاغ عنه كمنتهٍ**، يمكنك الإبلاغ عن أمر العزل الذي تم بدء تشغيله باعتباره منتهياً.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-138">By selecting **Report as finished**, you can report a started quarantine order as finished.</span></span> <span data-ttu-id="ddc6d-139">تم إصدار الصنف من وحدة العزل ولكن لم يتم إرجاعه بعد إلى المستودع العادي.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-139">The item is released from quarantine but isn't yet moved back to the regular warehouse.</span></span>
 
<span data-ttu-id="ddc6d-140">[![لقطة شاشة لصفحة أوامر العزل بالحالة "تم بالإبلاغ عنه كمنتهٍ". ](../media/report-as-finished.png)](../media/report-as-finished.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-140">[ ![Screenshot of the Quarantine orders page with the status Reported as finished.](../media/report-as-finished.png) ](../media/report-as-finished.png#lightbox)</span></span>

<span data-ttu-id="ddc6d-141">يمكن معالجة النقل مرة أخرى إلى المستودع العادي من خلال دفتر يومية وصول صنف يمكن تهيئته أثناء عملية الإبلاغ عنه كمنتهٍ.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-141">The movement back to the regular warehouse can be processed through an Item arrival journal that can be initialized during the Report as finished process.</span></span>


<span data-ttu-id="ddc6d-142">[![لقطة شاشة لصفحة حركات المخزون بالحالة "تم بالإبلاغ عنه كمنتهٍ".](../media/transactions-report-as-finished-status.png)](../media/transactions-report-as-finished-status.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-142">[ ![Screenshot of the inventory transactions page with the status Reported as finished.](../media/transactions-report-as-finished-status.png) ](../media/transactions-report-as-finished-status.png#lightbox)</span></span>
### <a name="ended"></a><span data-ttu-id="ddc6d-143">تم الإنهاء</span><span class="sxs-lookup"><span data-stu-id="ddc6d-143">Ended</span></span>

<span data-ttu-id="ddc6d-144">عند إنهاء أمر العزل، يتم نقل الصنف من مستودع العزل إلى المستودع العادي.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-144">When a quarantine order is ended, the item is moved from the quarantine warehouse back to the regular warehouse.</span></span>
 
<span data-ttu-id="ddc6d-145">[![لقطة شاشة لصفحة أوامر العزل بالحالة "تم الإنهاء".](../media/ended-1.png)](../media/ended-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-145">[ ![Screenshot of the Quarantine orders page with the status Ended.](../media/ended-1.png) ](../media/ended-1.png#lightbox)</span></span>

<span data-ttu-id="ddc6d-146">تم تعيين حالة حركة الصنف إلى  **مباع** في مستودع العزل و **مشتراة** في المستودع العادي.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-146">The status of the item transaction is set to **Sold** at the quarantine warehouse and **Purchased** at the regular warehouse.</span></span>
 
<span data-ttu-id="ddc6d-147">[![لقطة شاشة لصفحة حركات المخزون بالحالة "تم الإنهاء".](../media/transactions-ended-status.png)](../media/transactions-ended-status.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ddc6d-147">[ ![Screenshot of the inventory transactions page with the status Ended.](../media/transactions-ended-status.png) ](../media/transactions-ended-status.png#lightbox)</span></span>

## <a name="quarantine-order-scrap"></a><span data-ttu-id="ddc6d-148">التخلص من أمر العزل</span><span class="sxs-lookup"><span data-stu-id="ddc6d-148">Quarantine order scrap</span></span> 

<span data-ttu-id="ddc6d-149">كجزء من عملية أمر العزل، يمكنك إلغاء المخزون.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-149">As part of the quarantine order process, you can scrap inventory.</span></span> <span data-ttu-id="ddc6d-150">عند معالجة التخلص، سيتم تعيين حالة المخزون إلى  **مباع** بحركة إصدار من مستودع العزل.</span><span class="sxs-lookup"><span data-stu-id="ddc6d-150">When you process scrap, the status of the inventory will be set to **Sold** by an issue transaction from the quarantine warehouse.</span></span>
