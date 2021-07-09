---
ms.openlocfilehash: b78e3b563225454879ed65a0380b61e35ec0a3b1
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6073833"
---
<span data-ttu-id="d7e4e-101">تتيح لك ميزة توزيع البضائع المخططة نقل المخزون الوارد لأمر موجود مباشرةً إلى منطقة التوزيع أو منطقة التدريج الصادرة.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-101">The Planned cross docking feature allows you to move inbound inventory for an existing order directly to an outbound dock or staging area.</span></span> <span data-ttu-id="d7e4e-102">إذا لم يكن المخزون ضرورياً للأوامر، فسيتم توجيهه إلى موقع التخزين الصحيح من خلال عملية الإيداع العادية.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-102">If inventory is not needed for orders, it will be directed to the correct storage location through the regular put-away process.</span></span> <span data-ttu-id="d7e4e-103">تقلل هذه العملية من لمسات المخزون والوقت والمساحة في المستودع.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-103">This process minimizes inventory touches, time, and space in the warehouse.</span></span>

<span data-ttu-id="d7e4e-104">يمكن لخيار قالب **توزيع البضائع** أن يجعل عملية توزيع البضائع تلقائية.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-104">The **Cross docking** template option can make the cross docking process automatic.</span></span> <span data-ttu-id="d7e4e-105">توضح لقطة الشاشة التالية كيفية استخدام النموذج في **إدارة المستودعات > الإعداد > العمل >قوالب توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-105">The following screenshot shows how the template is used at **Warehouse management > Setup > Work > Cross docking templates**.</span></span>

<span data-ttu-id="d7e4e-106">[ ![لقطة شاشة لنموذج توزيع البضائع مع تمييز الميزات.](../media/cross-docking-template-ssm.png) ](../media/cross-docking-template-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d7e4e-106">[ ![Screenshot of cross docking template with features highlighted.](../media/cross-docking-template-ssm.png) ](../media/cross-docking-template-ssm.png#lightbox)</span></span>

1.  <span data-ttu-id="d7e4e-107">يشير **رقم التسلسل** إلى الترتيب الذي سيحدد به النظام البيانات من النموذج.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-107">The **Sequence number** indicates the order in which the system will select data from the template.</span></span> <span data-ttu-id="d7e4e-108">إذا كانت البيانات لا تفي بالمعايير المحددة، فسينتقل النظام إلى التسلسل التالي، وهكذا دواليك، حتى يتم استيفاء المعايير (إن وجدت).</span><span class="sxs-lookup"><span data-stu-id="d7e4e-108">If the data doesn’t meet the criteria specified, the system will move on to the next sequence, and so forth, until the criteria is met (if at all).</span></span>
2.  <span data-ttu-id="d7e4e-109">ستكون **سياسة إصدار الطلب** التي ستحددها إما **قبل استلام التوريد** أو **عند استلام التوريد**.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-109">The **Demand release policy** that you would select will be either **Before supply receipt** or **At supply receipt**.</span></span> <span data-ttu-id="d7e4e-110">بمعنى آخر، يعتمد التحديد على ما إذا كان سيتم التخطيط له قبل استلامه أم أنه سيتم التخطيط له فقط في وقت استلامه.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-110">In other words, the selection depends on whether it will be planned before it is received or if it will be planned only at the time it is received.</span></span> 
3.  <span data-ttu-id="d7e4e-111">تحتوي علامة التبويب السريعة **التخطيط** على عدة خيارات:</span><span class="sxs-lookup"><span data-stu-id="d7e4e-111">The **Planning** FastTab contains several options:</span></span>

    - <span data-ttu-id="d7e4e-112">**متطلبات الطلب** – حدد **محدد** إذا كان الطلب مطلوباً لربطه بالتوريد قبل الإصدار، أو حدد **حجز الطلب** إذا كان الطلب مطلوب مقابل العرض قبل الإصدار.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-112">**Demand requirements** – Select **Marked** if the demand is required to be linked to the supply before the release, or select **Order reservation** if the demand is required against the supply prior to release.</span></span>

    - <span data-ttu-id="d7e4e-113">**إنشاء العمل** – يحدد كيفية العثور على مواقع الوضع، والتي تستند إلى توجيهات الموقع أو الموروثة من المواقع الموجودة على الشحنة.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-113">**Work creation** – Determines how to find the put locations, which are based on location directives or inherited from the locations on the shipment.</span></span>
 
    - <span data-ttu-id="d7e4e-114">**قالب العمل** – حدد هذا الخيار إذا كنت بحاجة إلى إعداد أي قوالب عمل توزيع البضائع.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-114">**Work template** – Select this option if you need to set up any cross-docking work templates.</span></span>

    - <span data-ttu-id="d7e4e-115">**إعادة التحقق عند استلام التوريد** – يشير هذا الخيار إلى ما إذا كان يجب إعادة التحقق من التوريد أثناء الاستلام أم لا.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-115">**Revalidate on supply receipt** – This option indicates whether the supply should be revalidated during receipt or not.</span></span> <span data-ttu-id="d7e4e-116">إذا تم تعيين الخيار على **نعم**، فسيتم تحديد أقصى فترة زمنية ونطاق أيام انتهاء الصلاحية لتلك الأطر الزمنية.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-116">If the option is set to **Yes**, the maximum window and expiration days range will be selected for those time frames.</span></span>

    - <span data-ttu-id="d7e4e-117">**تحقق من نافذة الوقت** – يشير إلى ما إذا كان يجب تقييم أقصى نافذة زمنية عند تحديد مصدر الإمداد.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-117">**Validate time window** – Indicates if the maximum time window should be evaluated when you are selecting a supply source.</span></span>

    - <span data-ttu-id="d7e4e-118">**أقصى نافذة زمنية** – أقصى فترة زمنية مسموح بها بين وصول العرض ومغادرة الطلب.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-118">**Maximum time window** – The maximum time period allowed between the supply arrival and demand departure.</span></span>  

    - <span data-ttu-id="d7e4e-119">**أقصى نافذة زمنية للوحدة** – تشير إلى نافذة زمنية بحد أقصى أيام أو ساعات.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-119">**Maximum time window unit** – Indicates a maximum time window of days or hours.</span></span>

    - <span data-ttu-id="d7e4e-120">**الحد الأدنى للنافذة** – الحد الأدنى للفترة الزمنية المسموح بها بين وصول العرض ومغادرة الطلب.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-120">**Minimum time window** – The minimum time period allowed between the supply arrival and demand departure.</span></span> 

    - <span data-ttu-id="d7e4e-121">**الحد الأدنى من وحدة النافذة الزمنية** – يشير إلى الحد الأدنى من النافذة الزمنية للأيام أو الساعات.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-121">**Minimum time window unit** – Indicates a minimum time window of days or hours.</span></span>

    - <span data-ttu-id="d7e4e-122">**نطاق أيام انتهاء الصلاحية** – الحد الأقصى للأيام بين تاريخ انتهاء صلاحية الدُفعة الأولى المنتهية الصلاحية والدُفعة التي يتم استلامها.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-122">**Expiration days range** – The maximum days between the expiration date of the first expiring batch and the batch that is being received.</span></span>

4. <span data-ttu-id="d7e4e-123">في منطقة **مصادر التوريد** يمكنك تنفيذ الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="d7e4e-123">In the **Supply sources** area, you can perform the following actions:</span></span> 

    - <span data-ttu-id="d7e4e-124">حدد بين **أمر الشراء**، **أمر الإنتاج**، و **إيصال أمر التحويل**.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-124">Select between **Purchase order**, **Production order**, and **Transfer order receipt**.</span></span> 

    - <span data-ttu-id="d7e4e-125">استخدم الخيار **تحرير الاستعلام** لتحديد مورد معين في أمر الشراء أو حقل آخر في مصدر التوريد المحدد (على سبيل المثال).</span><span class="sxs-lookup"><span data-stu-id="d7e4e-125">Use the **Edit query** option to select a specific vendor on a purchase order or another field in the selected supply source (for example).</span></span> 

    ![لقطة شاشة لصفحة توزيع البضائع أوامر الشراء.](../media/cd-query-ssm.png)

5. <span data-ttu-id="d7e4e-127">في الجزء العلوي من الصفحة يوجد خيار **تحرير الاستعلام** آخر.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-127">At the top of the page is another **Edit query** option.</span></span> <span data-ttu-id="d7e4e-128">ومع ذلك، فإن الحقل الوحيد المراد تحديده هو **رقم الصنف**، والذي سيشير إلى العنصر (العناصر) التي سيتم إرساءها بشكل عرضي.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-128">However, the only field that it is intended to select is **Item number**, which will indicate the item(s) that will be cross docked.</span></span> 

    ![لقطة شاشة لصفحة توزيع البضائع مع تمييز المعايير.](../media/cdt-query-ssm.png) 

## <a name="auto-release-shipment-for-cross-docking"></a><span data-ttu-id="d7e4e-130">الإصدار التلقائي للشحنة لتوزيع البضاعة</span><span class="sxs-lookup"><span data-stu-id="d7e4e-130">Auto-release shipment for cross docking</span></span>

<span data-ttu-id="d7e4e-131">تتيح لك ميزة **الإصدار التلقائي للشحنة لتوزيع البضائع** إمكانية إصدار أمر إلى المستودع تلقائياً عندما يتم الإبلاغ عن أمر الإنتاج الذي يوفر المنتج كمنتهي.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-131">The **Auto-release shipment for cross-docking** feature lets you automatically release an order to the warehouse when the production order that supplies the product is reported as finished.</span></span> <span data-ttu-id="d7e4e-132">يتم نقل الكمية المطلوبة لأمر المبيعات أو أمر التحويل مباشرةً من موقع إخراج الإنتاج إلى موقع الصادر.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-132">The quantity that is needed for the sales order or transfer order is moved directly from the production output location to the outbound location.</span></span> 

- <span data-ttu-id="d7e4e-133">على عكس المناقشة السابقة حول توزيع البضائع، تدعم هذه الميزة أوامر الإنتاج فقط كعرض وأوامر المبيعات وأوامر التحويل فقط كطلب.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-133">As opposed to the earlier discussion of cross docking, this feature only supports production orders as supply and only sales orders and transfer orders as demand.</span></span> 

- <span data-ttu-id="d7e4e-134">يمكن بدء توزيع البضائع حتى إذا لم يتم تحرير أمر الطلب (المبيعات أو النقل) إلى المستودع قبل الإبلاغ عن أمر الإنتاج كمنتهي.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-134">Cross docking can be started even if the demand order (sales or transfer) wasn't released to the warehouse before the production order was reported as finished.</span></span> 

### <a name="example---cross-docking-flow-for-auto-release-shipment"></a><span data-ttu-id="d7e4e-135">مثال - تدفق توزيع البضائع للإصدار التلقائي للشحنة</span><span class="sxs-lookup"><span data-stu-id="d7e4e-135">Example - Cross docking flow for auto-release shipment</span></span>

<span data-ttu-id="d7e4e-136">يوضح الرسم التخطيطي التالي مثالاً على تدفق توزيع البضائع للإصدار التلقائي للشحنة.</span><span class="sxs-lookup"><span data-stu-id="d7e4e-136">The following diagram shows an example of a cross-docking flow for an auto-release shipment.</span></span>

<span data-ttu-id="d7e4e-137">[ ![يوضح الرسم التخطيطي التالي مثالاً على تدفق توزيع البضائع للإصدار التلقائي للشحنة.](../media/example-flow-c.png) ](../media/example-flow-c.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d7e4e-137">[ ![Diagram example of a cross docking flow for an auto release shipment.](../media/example-flow-c.png) ](../media/example-flow-c.png#lightbox)</span></span>