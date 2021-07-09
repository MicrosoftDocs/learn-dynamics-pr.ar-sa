---
ms.openlocfilehash: 9c52cc0351bfc008086471a6342405db513c2e99
ms.sourcegitcommit: f699c9a05571bd0157969b1a0e0f33c3a4790958
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "6073825"
---
<span data-ttu-id="7df52-101">يعد انتقاء أمر المبيعات عملية ضرورية لأي عمل باستخدام جهاز محمول أو عميل الويب.</span><span class="sxs-lookup"><span data-stu-id="7df52-101">Sales order picking is a necessary process for any business using a mobile device or the web client.</span></span> <span data-ttu-id="7df52-102">بغض النظر عن الخيارات المختلفة المتوفرة، فإن عملية انتقاء أمر المبيعات هي نفس الشيء:</span><span class="sxs-lookup"><span data-stu-id="7df52-102">Regardless of the various options are available, the sales order picking process is the same:</span></span>

1. <span data-ttu-id="7df52-103">يتم إنشاء أمر المبيعات وإدخاله في النظام.</span><span class="sxs-lookup"><span data-stu-id="7df52-103">The sales order is created and entered into the system.</span></span>
1. <span data-ttu-id="7df52-104">تم تأكيد الأمر في النظام.</span><span class="sxs-lookup"><span data-stu-id="7df52-104">The order is confirmed in the system.</span></span>
1. <span data-ttu-id="7df52-105">في مرحلة ما، يكون الأمر جاهزاً بعد ذلك لإصداره للانتقاء.</span><span class="sxs-lookup"><span data-stu-id="7df52-105">At some point, the order is then ready to be released for picking.</span></span> <span data-ttu-id="7df52-106">يمكن أن يكون هذا في نفس اليوم أو في أي وقت.</span><span class="sxs-lookup"><span data-stu-id="7df52-106">This can be the same day or anytime.</span></span>


## <a name="staging-with-sales-order-picking"></a><span data-ttu-id="7df52-107">التجهيز لانتقاء أوامر المبيعات</span><span class="sxs-lookup"><span data-stu-id="7df52-107">Staging with sales order picking</span></span>

<span data-ttu-id="7df52-108">يمكنك تكوين قالب العمل لتخطي خطوة التجهيز باستخدام زوج انتقاء وإيداع واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="7df52-108">You can configure the work template to skip the staging step by only using one pick and put pair.</span></span>

<span data-ttu-id="7df52-109">في عمليات المستودعات الأكثر تعقيداً، يمكنك استخدام عمليات تجهيز متعددة.</span><span class="sxs-lookup"><span data-stu-id="7df52-109">In more complex warehouse operations, you can use multiple staging operations.</span></span> <span data-ttu-id="7df52-110">على سبيل المثال، يمكن أن تكون عمليات التجهيز المتعددة مفيدة بعد انتقاء الأصناف من المستودع وتتطلب عملية تعبئة معقدة لأصناف الاختتام بالفقاعات للشحن.</span><span class="sxs-lookup"><span data-stu-id="7df52-110">For example, multiple staging operations can be useful after items are picked from the warehouse and they require a complex packing operation to bubble wrap items for shipping.</span></span>

<span data-ttu-id="7df52-111">بعد اختتام الأصناف بالفقاعات، يتم تجهيزها عند باب الرصيف للتحميل.</span><span class="sxs-lookup"><span data-stu-id="7df52-111">After the items are bubble wrapped, they are staged at a dock door for loading.</span></span> <span data-ttu-id="7df52-112">باستخدام هذا المثال، يمكنك إنشاء ثلاثة أزواج انتقاء وإيداع لتتبع حركة الصنف من خلال الخطوات المختلفة:</span><span class="sxs-lookup"><span data-stu-id="7df52-112">With this example, you could create three pick and put pairs to track the movement of the item through the various steps:</span></span>

-   <span data-ttu-id="7df52-113">يقوم زوج الانتقاء والإيداع الأول بنقل الصنف خارج موقع الانتقاء وإلى موقع التعبئة.</span><span class="sxs-lookup"><span data-stu-id="7df52-113">The first pick-put pair moves the item out of the picking location and into a packing location.</span></span>

-   <span data-ttu-id="7df52-114">يقوم زوج الانتقاء والإيداع الثاني بنقل الصنف خارج موقع التعبئة وإلى موقع التحميل.</span><span class="sxs-lookup"><span data-stu-id="7df52-114">The second pick-put pair moves the item out of the packing location and into the loading location.</span></span>

-   <span data-ttu-id="7df52-115">يقوم زوج الانتقاء والإيداع الأخير بنقل الصنف من مواقع التحميل وإلى شاحنة أو خارج المستودع الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="7df52-115">The final pick-put pair moves the item out of the loading locations and onto a truck or out of your warehouse.</span></span>

<span data-ttu-id="7df52-116">تحتاج إلى تكوين قالب عمل باستخدام أزواج الانتقاء والإيداع الصحيحة، وإنشاء توجيهات الموقع للإشارة إلى أنه يجب وضع الأصناف في مواقع التعبئة والتحميل، على التوالي.</span><span class="sxs-lookup"><span data-stu-id="7df52-116">You need to configure a work template with the correct pick and put pairs, and create location directives to indicate that items should be placed in the packing and loading locations, respectively.</span></span> <span data-ttu-id="7df52-117">سيتم بعد ذلك ربط توجيهات الموقع هذه بقالب العمل للإشارة إلى المكان الذي يجب وضع الأصناف فيه.</span><span class="sxs-lookup"><span data-stu-id="7df52-117">These location directives would then be linked to the work template to indicate where the items should be placed.</span></span> <span data-ttu-id="7df52-118">عند تكوين أصناف القائمة لانتقاء أمر المبيعات، تتوفر بعض الخيارات الإضافية لمساعدتك في إدارة عملية التجهيز.</span><span class="sxs-lookup"><span data-stu-id="7df52-118">When you configure the menu items for sales order picking, some additional options are available to help you manage the staging process.</span></span>

<span data-ttu-id="7df52-119">*الارتساء* هو مفهوم يسمح للمستخدم بتجاوز موقع التجهيز أو التحميل؛ سيتم توجيه جميع عمليات الإيداع المفتوحة اللاحقة إلى موقع التجهيز الجديد أو موقع التحميل.</span><span class="sxs-lookup"><span data-stu-id="7df52-119">*Anchoring* is a concept that allows the user to override the staging or loading location; all subsequent open puts will be directed to the new staging or loading location.</span></span> 

<span data-ttu-id="7df52-120">يمكنك العثور على خيار **الارتساء** في صفحة **أصناف قائمة الأجهزة المحمولة‬**.</span><span class="sxs-lookup"><span data-stu-id="7df52-120">You can find the **Anchoring** option on the **MOBILE DEVICE MENU ITEMS** page.</span></span> <span data-ttu-id="7df52-121">في حالة تعيين شريط تمرير **الارتساء** إلى **نعم**، ثم يمكن للمستخدم تحديد الإرساء حسب الشحنة أو حمل العمل.</span><span class="sxs-lookup"><span data-stu-id="7df52-121">If the **Anchoring** slider is set to **Yes**, then the user can select to anchor by the shipment or the load.</span></span>
<span data-ttu-id="7df52-122">إذا كان الإرساء حسب الشحنة، فسيتم تغيير عمليات الإيداع المفتوحة اللاحقة لنفس الشحنة أو حمل العمل إلى الموقع الجديد لتلك الشحنة.</span><span class="sxs-lookup"><span data-stu-id="7df52-122">If anchoring is by shipment, then the subsequent open puts for the same shipment or load will be changed to the new location for that shipment.</span></span>
<span data-ttu-id="7df52-123">إذا كان الإرساء حسب حمل العمل، فسيتم تغيير عمليات الإيداع المفتوحة اللاحقة إلى الموقع الجديد لتلك الحمولة.</span><span class="sxs-lookup"><span data-stu-id="7df52-123">If anchoring is by load, then the subsequent open puts will be changed to the new location for that load.</span></span>

<span data-ttu-id="7df52-124">[![لقطة شاشة لإعدادات الارتساء في Finance and Operations.](../media/anchoring-1.png)](../media/anchoring-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7df52-124">[![Screenshot of the Finance and Operations Anchoring settings.](../media/anchoring-1.png)](../media/anchoring-1.png#lightbox)</span></span>

## <a name="pick-sales-orders-with-the-mobile-device"></a><span data-ttu-id="7df52-125">انتقاء أوامر المبيعات باستخدام الجهاز المحمول</span><span class="sxs-lookup"><span data-stu-id="7df52-125">Pick sales orders with the mobile device</span></span>

<span data-ttu-id="7df52-126">يمكن إجراء انتقاء أمر المبيعات باستخدام الجهاز المحمول بعد إصدار الأمر إلى المستودع وإنشاء العمل.</span><span class="sxs-lookup"><span data-stu-id="7df52-126">Sales order picking with the mobile device can be done after the order is released to the warehouse and the work is created.</span></span> <span data-ttu-id="7df52-127">سيُمكّن هذا أي مستخدم لديه الأذونات المناسبة من استخدام القائمة في الجهاز للوصول إلى خيارات الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="7df52-127">This will enable any user with the proper permissions to use the menu in the device to access the picking options.</span></span>

<span data-ttu-id="7df52-128">ضع في اعتبارك الخطوات التالية لعملية الانتقاء:</span><span class="sxs-lookup"><span data-stu-id="7df52-128">Consider the following steps for the picking process:</span></span>

1.  <span data-ttu-id="7df52-129">إنشاء أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="7df52-129">Create the sales order.</span></span>

2.  <span data-ttu-id="7df52-130">تأكيد أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="7df52-130">Confirm the sales order.</span></span>

3.  <span data-ttu-id="7df52-131">الإصدار لمستودع وإنشاء العمل.</span><span class="sxs-lookup"><span data-stu-id="7df52-131">Release to warehouse and create the work.</span></span>

4.  <span data-ttu-id="7df52-132">انتقاء أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="7df52-132">Pick the sales order.</span></span>

## <a name="work-pick-line-overview"></a><span data-ttu-id="7df52-133">نظرة عامة على بند انتقاء العمل</span><span class="sxs-lookup"><span data-stu-id="7df52-133">Work pick line overview</span></span>
<span data-ttu-id="7df52-134">تعمل ميزة **نظرة عامة على بند الانتقاء** الاختيارية على تمكين عمال المستودعات من عرض والاختيار من قائمة بجميع بنود العمل المتعلقة بمهمتهم الحالية.</span><span class="sxs-lookup"><span data-stu-id="7df52-134">The optional **Pick line overview** feature enables warehouse workers to view and select from a list of all the work lines related to their current task.</span></span> <span data-ttu-id="7df52-135">تساعد هذه القدرة العمال على تحسين تسلسل الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="7df52-135">This capability helps workers to optimize their picking sequence.</span></span> 

<span data-ttu-id="7df52-136">توفر الميزة خيارات تحل محل الزر **تخطي** القياسي يتيح للعمال التنقل عبر الخطوط واحداً تلو الآخر، بترتيب ثابت.</span><span class="sxs-lookup"><span data-stu-id="7df52-136">The feature provides options that replace the standard **Skip** button that lets workers cycle through the lines one at a time, in a fixed order.</span></span> <span data-ttu-id="7df52-137">لتمكين هذه الميزة وتكوينها، راجع [إعداد عنصر قائمة جهاز محمول لتوفير نظرة عامة على بند انتقاء](https://docs.microsoft.com/dynamics365/supply-chain/warehousing/pick-line-overview/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="7df52-137">To enable and configure this feature, see [Set up a mobile device menu item to provide a pick line overview](https://docs.microsoft.com/dynamics365/supply-chain/warehousing/pick-line-overview/?azure-portal=true).</span></span>


## <a name="shipment-consolidation-policies"></a><span data-ttu-id="7df52-138">سياسات دمج الشحنات</span><span class="sxs-lookup"><span data-stu-id="7df52-138">Shipment consolidation policies</span></span>

<span data-ttu-id="7df52-139">تسمح ميزة سياسة دمج الشحنات بالتكوين المرن للدمج الآلي للشحنة في وقت إصدار الدُفعة لأوامر المبيعات أو التحويل.</span><span class="sxs-lookup"><span data-stu-id="7df52-139">The consolidate shipment policy feature allows for flexible configuration of automated consolidation of a shipment at the time of batch releasing sales or transfer orders.</span></span> <span data-ttu-id="7df52-140">يمكن تحديد السياسات في صفحة **إدارة المستودعات > الإعداد > إصدار إلى المستودع > سياسات دمج الشحنات**.</span><span class="sxs-lookup"><span data-stu-id="7df52-140">Policies can be defined on the **Warehouse management > Setup > Release to warehouse > Shipment consolidation policies** page.</span></span> <span data-ttu-id="7df52-141">تحتوي السياسات على استعلامات لتحديد مدى قابليتها للتطبيق ومجموعة قابلة للتعديل من الحقول التي تقود قرار تجميع خطوط التحميل على مستوى الشحن تلقائياً عند الإصدار إلى المستودع.</span><span class="sxs-lookup"><span data-stu-id="7df52-141">The policies have queries to define their applicability and a modifiable set of fields driving the decision for grouping load lines on shipment level automatically at release to warehouse.</span></span> <span data-ttu-id="7df52-142">عند إعداد سياسة جديدة، يمكنك تشغيل تبديل **الدمج مع الشحنات المفتوحة** للسماح بدمج الشحنات الجديدة مع الشحنة المفتوحة الموجودة بالفعل.</span><span class="sxs-lookup"><span data-stu-id="7df52-142">Upon setting up a new policy, you can toggle **Consolidate with open shipments** on to allow new shipments to be consolidated with already existing open shipment.</span></span> <span data-ttu-id="7df52-143">بالإضافة إلى ذلك، خيار إنشاء الإعداد الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="7df52-143">In addition, a Create default setup option.</span></span>

![لقطة شاشة لسياسات دمج شحنة Finance and Operations.](../media/shipment-consolidation-policies-ssm.png)

<span data-ttu-id="7df52-145">يمكن العثور على خيار تحديد الشحنة المدمجة حسب نوع سياسة أوامر المبيعات أو أوامر التحويل، أو العميل والموقع، على **إدارة المستودعات > الإعداد > إصدار إلى المستودع > قوالب دمج الشحنات**.</span><span class="sxs-lookup"><span data-stu-id="7df52-145">The option to further define the consolidated shipment by policy type of sales orders or transfer orders, customer and location, can be found at **Warehouse management > Setup > Release to warehouse > Shipment consolidation templates**.</span></span>


![لقطة شاشة لقالب دمج شحنات Finance and Operations.](../media/shipment-consolidation-template-ss.png)

<span data-ttu-id="7df52-147">عند إصدار أوامر المبيعات والتحويل إلى المستودع، يتم إصدارها وتصبح متاحة للدمج.</span><span class="sxs-lookup"><span data-stu-id="7df52-147">When sales and transfer orders are released to the warehouse, they are released and become available to consolidate.</span></span> <span data-ttu-id="7df52-148">في **إدارة المستودعات > الشحنات > جميع الشحنات** هناك خيار لدمج الشحنات عن طريق تحديد دمج الشحنات.</span><span class="sxs-lookup"><span data-stu-id="7df52-148">In **Warehouse management > Shipments > All shipments** there is an option to consolidate shipments, by selecting consolidate shipments.</span></span>

![لقطه شاشة لصفحة جميع شحنات Finance and Operations مع تمييز دمج الشحنات.](../media/shipment-consolidation-ss.png)

<span data-ttu-id="7df52-150">يمكن أيضاً إدارة الشحنات يدوياً في **إدارة المستودعات > إصدار إلى المستودع > منضدة عمل دمج الشحنات‬**.</span><span class="sxs-lookup"><span data-stu-id="7df52-150">Shipments can also be manually managed in **Warehouse Management > Release to warehouse > Shipment consolidation workbench**.</span></span> <span data-ttu-id="7df52-151">حدد القالب الذي تم إعداده مسبقاً، ثم حدد **دمج الشحنات**.</span><span class="sxs-lookup"><span data-stu-id="7df52-151">Select the template that was previously set up, and select **Consolidate shipments**.</span></span>

![لقطة شاشة لمنضدة عمل دمج شحنات Finance and Operations.](../media/shipment-consolidation-workbench-ssm.png)

## <a name="outbound-workload-visualization"></a><span data-ttu-id="7df52-153">مرئيات أحمال العمل الصادرة</span><span class="sxs-lookup"><span data-stu-id="7df52-153">Outbound workload visualization</span></span>

<span data-ttu-id="7df52-154">توفر ميزة **مرئيات حمل العمل الصادر‬** الاختيارية عرضاً مرئياً قابلاً للتخصيص لأحمال العمل الصادرة في المستودع، بحيث يمكن مراقبة التقدم في عمل الانتقاء وعرضه على شاشات أداء المستودع.</span><span class="sxs-lookup"><span data-stu-id="7df52-154">The optional **Outbound workload visualization** feature provides a customizable, visual display of outbound workloads in the warehouse, so the progress of picking work can be monitored and displayed on warehouse performance screens.</span></span>

<span data-ttu-id="7df52-155">يمكنك بسهولة إنشاء مخططات مخصصة لأحمال العمل تراقب تقدم العمل الحالي والعمل المتبقي.</span><span class="sxs-lookup"><span data-stu-id="7df52-155">You can easily create custom workload charts that monitor the progress of current work and what work remains.</span></span> <span data-ttu-id="7df52-156">يمكنك إنشاء عروض متعددة، وتصفية البيانات للتركيز على العناصر الأكثر أهميةً، وإعداد التحديث التلقائي حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="7df52-156">You can create multiple views, filter the data to focus on the most critical elements, and set up auto-refresh as needed.</span></span> 

<span data-ttu-id="7df52-157">لمعرفة المزيد حول التكوين وإعداد مرئيات أحمال العمل الصادرة، راجع [مرئيات أحمال العمل الصادرة](https://docs.microsoft.com/dynamics365/supply-chain/warehousing/outbound-workload-visualization/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="7df52-157">To learn more about configuration and the setup of Outbound workload visualization, see [Outbound workload visualization](https://docs.microsoft.com/dynamics365/supply-chain/warehousing/outbound-workload-visualization/?azure-portal=true).</span></span>

