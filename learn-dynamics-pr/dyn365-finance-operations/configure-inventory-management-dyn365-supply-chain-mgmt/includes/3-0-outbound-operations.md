---
ms.openlocfilehash: e158c19c50af959e97cc74c30bca8510edc78317
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073678"
---
<span data-ttu-id="f7457-101">تُستخدم أوامر المخرجات لربط سطور أوامر المبيعات وسطور أوامر النقل بعمليات الانتقاء الصادرة التي تستخدم قوائم الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="f7457-101">Output orders are used to link sales order lines and transfer order lines with the outbound picking processes that use picking lists.</span></span>

<span data-ttu-id="f7457-102">عند إنشاء قوائم الانتقاء من أوامر المبيعات أو أوامر النقل، يتم إنشاء أوامر المخرجات والشحنات تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="f7457-102">When picking lists are generated from either sales orders or transfer orders, output orders and shipments are automatically created.</span></span> <span data-ttu-id="f7457-103">توجد علاقة واحد لواحد بين قائمة الانتقاء والشحنة.</span><span class="sxs-lookup"><span data-stu-id="f7457-103">A picking list has a one-to-one relationship with a shipment.</span></span> <span data-ttu-id="f7457-104">يمكن معالجة شحنة أمر النقل أو إيصال تعبئة أمر المبيعات من الشحنة.</span><span class="sxs-lookup"><span data-stu-id="f7457-104">The transfer order shipment or the sales order packing slip can be processed from the shipment.</span></span>

<span data-ttu-id="f7457-105">يظهر الشكل التالي نظرة عامة حول العملية الخاصة بالأوامر الخارجية.</span><span class="sxs-lookup"><span data-stu-id="f7457-105">The following figure shows an overview of the process for outbound orders.</span></span>
 
![مخطط العملية الخاصة بالأوامر الخارجية.](../media/outbound-operations.png)

<span data-ttu-id="f7457-107">يمكنك إعداد قواعد صادرة لتحديد كيف ينبغي لـ Supply Chain Management معالجة العملية الصادرة.</span><span class="sxs-lookup"><span data-stu-id="f7457-107">You can set up outbound rules to define how Supply Chain Management should handle the outbound process.</span></span> <span data-ttu-id="f7457-108">يمكنك استخدام هذه القواعد للتحكم في عملية الشحن والتحكم في المرحلة أثناء العملية التي يمكن إرسال الشحنة فيها.</span><span class="sxs-lookup"><span data-stu-id="f7457-108">You can use these rules to control the shipment process and to control during which stage in the process a shipment can be sent.</span></span> 

<span data-ttu-id="f7457-109">تحدد الإعدادات التالية كيفية معالجة العمليات الصادرة.</span><span class="sxs-lookup"><span data-stu-id="f7457-109">The following settings define how the outbound processes are handled.</span></span>

## <a name="picking-route-status-for-sales-and-transfer-orders"></a><span data-ttu-id="f7457-110">حالة مسار الانتقاء لأوامر المبيعات والتحويل</span><span class="sxs-lookup"><span data-stu-id="f7457-110">Picking route status for sales and transfer orders</span></span> 

<span data-ttu-id="f7457-111">انتقل إلى **حساب المقبوضات > الإعداد > معلمات الحسابات المدينة**، ثم من علامة التبويب **التحديثات**، حدد قيمة في حقل **حالة مسار الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="f7457-111">Go to **Account receivable > Setup > Account receivable parameters** and then, on the **Updates** tab, select a value in the **Picking route status** field.</span></span> 

<span data-ttu-id="f7457-112">إذا تم تعيين حقل **حالة مسار الانتقاء** على **مكتمل**، يتم إجراء عملية الانتقاء تلقائياً كجزء من عملية إنشاء قوائم الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="f7457-112">If the **Picking route status** field is set to **Completed**, the picking process occurs automatically as part of the process of generating picking lists.</span></span> <span data-ttu-id="f7457-113">إذا تم تعيين الحقل إلى **نشط**، فيجب تحديث بنود قائمة الانتقاء يدوياً.</span><span class="sxs-lookup"><span data-stu-id="f7457-113">If the field is set to **Activated**, the picking list lines must be manually updated.</span></span>
 
![لقطة شاشة لحقل حالة مسار الانتقاء في علامة التبويب "تحديثات".](../media/picking-route-status.png)

<span data-ttu-id="f7457-115">يتم تطبيق نفس الإعداد على أوامر التحويل.</span><span class="sxs-lookup"><span data-stu-id="f7457-115">The same setup applies to transfer orders.</span></span> <span data-ttu-id="f7457-116">انتقل إلى **إدارة المخزون > الإعداد > معلمات Warehouse Management والمخزون**، ثم في علامة التبويب **أوامر التحويل**، حدد قيمة في حقل **حالة مسار الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="f7457-116">Go to **Inventory management > Setup > Inventory and warehouse management parameters** and then, on the **Transfer orders** tab, select a value in the **Picking route status** field.</span></span>
 
![لقطة شاشة لحقل حالة مسار الانتقاء في علامة التبويب أوامر التحويل.](../media/picking-route-status-2.png)
 
## <a name="end-output-inventory-order"></a><span data-ttu-id="f7457-118">إنهاء أمر مخزني للمخرجات</span><span class="sxs-lookup"><span data-stu-id="f7457-118">End output inventory order</span></span> 

<span data-ttu-id="f7457-119">انتقل إلى **إدارة المخزون > إعداد > معلمات Warehouse Management والمخزون**، ثم في علامة التبويب **عام**، قم بتعيين خيار **إنهاء أمر مخزني للمخرجات** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="f7457-119">Go to **Inventory management > Setup > Inventory and warehouse management parameters** and then, on the **General** tab, set the **End output inventory order** option to **Yes**.</span></span>
 
![لقطة شاشة لإنهاء أمر مخزني للمخرجات معين إلى نعم.](../media/end-output-inventory-order.png)

<span data-ttu-id="f7457-121">عندما يقوم عامل المستودع بتقليل كميات قائمة الانتقاء، ستتم إزالة كميات أمر المخزون المقابلة من الشحنة.</span><span class="sxs-lookup"><span data-stu-id="f7457-121">When the warehouse worker reduces the picking list quantities, then the corresponding inventory order quantities will be removed from the shipment.</span></span> 
 
<span data-ttu-id="f7457-122">عند تحديث قائمة الانتقاء في نقطة زمنية ما، يتم إرسال تقرير بالكميات المتبقية إلى الأمر في حالة تعيين خيار **إنهاء أمر مخزني للمخرجات** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="f7457-122">When the picking list is updated at a point in time, the remaining quantities are reported back to the order if the **End output inventory order** option is set to **Yes**.</span></span> 
 
<span data-ttu-id="f7457-123">في حالة تعيين خيار **إنهاء أمر مخزني للمخرجات** إلى **لا**، يتم الاحتفاظ بالكميات المتبقية ككمية أمر مخرجات مفتوحة ويجب إضافتها إلى قائمة انتقاء جديدة كجزء من وظيفة **أوامر المخرجات المفتوحة**.</span><span class="sxs-lookup"><span data-stu-id="f7457-123">If the **End output inventory order** option is set to **No**, the remaining quantities are kept as an open output order quantity and must be added to a new picking list as part of the **Open output orders** functionality.</span></span>

![لقطة شاشة لأوامر المخرجات المفتوحة في قائمة الوظائف المنسدلة.](../media/open-output-orders.png)

## <a name="reduce-quantity"></a><span data-ttu-id="f7457-125">خفض الكمية</span><span class="sxs-lookup"><span data-stu-id="f7457-125">Reduce quantity</span></span> 

<span data-ttu-id="f7457-126">المعلمة الثالثة التي يمكنك استخدامها كجزء من عملية إنشاء قوائم الانتقاء هي معلمة **تقليل الكمية**.</span><span class="sxs-lookup"><span data-stu-id="f7457-126">The third parameter that you can use as part of the process of generating picking lists is the **Reduce quantity** parameter.</span></span> <span data-ttu-id="f7457-127">يعمل إعداد هذه المعلمة مع إعداد **الحجز** الذي يشغل عملية الحجز كجزء من الإصدار إلى المستودع.</span><span class="sxs-lookup"><span data-stu-id="f7457-127">The setting of this parameter works together with the **Reservation** setting that triggers a reservation process as part of the release to the warehouse.</span></span>
 
![لقطة الشاشة لمعلمة الكمية المخفضة.](../media/reduced-quantity.png)
 
## <a name="example-of-an-outbound-process-for-a-sales-order"></a><span data-ttu-id="f7457-129">مثال على عملية صادرة لأمر المبيعات</span><span class="sxs-lookup"><span data-stu-id="f7457-129">Example of an outbound process for a sales order</span></span> 

<span data-ttu-id="f7457-130">في هذا المثال، يوجد أمر مبيعات لصنفين.</span><span class="sxs-lookup"><span data-stu-id="f7457-130">For this example, there is a sales order for two items.</span></span> <span data-ttu-id="f7457-131">أثناء إنشاء قائمة الانتقاء، حدد **معلمة تقليل الكمية**.</span><span class="sxs-lookup"><span data-stu-id="f7457-131">During picking list generation, you select the **Reduce quantity** parameter.</span></span>
 
<span data-ttu-id="f7457-132">بالتالي، يمكنك تحرير بنود الانتقاء وإنشائها فقط للمخزون الفعلي المتاح.</span><span class="sxs-lookup"><span data-stu-id="f7457-132">Therefore, you release and create picking lines only for available on-hand inventory.</span></span> <span data-ttu-id="f7457-133">يجب الإبلاغ عن الانتقاء بواسطة عملية تسجيل لقوائم الانتقاء (حالة **مسار الانتقاء** = **منشَّطة**).</span><span class="sxs-lookup"><span data-stu-id="f7457-133">The picking must be reported by means of a registration process for picking lists (**Picking route** status = **Activated**).</span></span>

![لقطة شاشة تُظهر تسجيل قائمة الانتقاء.](../media/updates-1.png)

<span data-ttu-id="f7457-135">يتم حجز المخزون الذي لم يتم حجزه بالفعل أثناء إنشاء قائمة الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="f7457-135">The inventory that hasn't already been reserved is reserved during picking list generation.</span></span> <span data-ttu-id="f7457-136">ويمكن إزالة المخزون غير المتاح من أمر المبيعات أو إصداره إلى المستودع للمعالجة الصادرة لاحقاً، عندما يكون المخزون متاحاً للانتقاء.</span><span class="sxs-lookup"><span data-stu-id="f7457-136">The unavailable inventory can be either removed from the sales order or released to the warehouse for outbound processing later, when inventory is available for picking.</span></span>

<span data-ttu-id="f7457-137">وبمجرد انتقاء كافة بنود الانتقاء في صفحة **تسجيل قائمة الانتقاء**، يتم إكمال الشحنة المرتبطة.</span><span class="sxs-lookup"><span data-stu-id="f7457-137">As soon as all the picking lines have been picked on the **Picking list registration** page, the associated shipment is completed.</span></span> <span data-ttu-id="f7457-138">يمكن بعد ذلك تهيئة عملية إيصالات التعبئة لأمر المبيعات استناداً إلى المخزون الذي تم انتقاؤه.</span><span class="sxs-lookup"><span data-stu-id="f7457-138">The process for sales order packing slips can then be initialized based on the picked inventory.</span></span>
 
<span data-ttu-id="f7457-139">[![لقطة شاشة لصفحة الشحنات تعرض شحنة مكتملة.](../media/shipment-1.png)](../media/shipment-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f7457-139">[![Screenshot of the Shipments page showing a completed shipment.](../media/shipment-1.png)](../media/shipment-1.png#lightbox)</span></span>
