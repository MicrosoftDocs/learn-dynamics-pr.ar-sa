---
ms.openlocfilehash: ef752d8d19587a163757524b8328893bcfcb71fb
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073389"
---

## <a name="scenario"></a><span data-ttu-id="ec5c4-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="ec5c4-101">Scenario</span></span>

<span data-ttu-id="ec5c4-102">في هذا التمرين العملي، ستقوم بإعداد شحن الإصدار التلقائي.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-102">In this lab you will set up auto-release shipment.</span></span> <span data-ttu-id="ec5c4-103">يجب عليك استخدام شركة USMF، وإتمام التمرين العملي السابق **إعداد توزيع البضائع المخطط له**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-103">You must use the USMF company, and have completed the previous lab **Set up planned cross-docking**.</span></span>

## <a name="cross-docking-template"></a><span data-ttu-id="ec5c4-104">قالب توزيع البضائع</span><span class="sxs-lookup"><span data-stu-id="ec5c4-104">Cross-docking template</span></span>

1. <span data-ttu-id="ec5c4-105">انتقل إلى **إدارة المستودعات > الإعداد > العمل > قوالب توزيع البضائع**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-105">Go to **Warehouse management > Setup > Work > Cross docking templates**</span></span>
1. <span data-ttu-id="ec5c4-106">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-106">Select **New**.</span></span>
1. <span data-ttu-id="ec5c4-107">في **حقل الرقم التسلسلي**، أدخل **1**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-107">In the **Sequence number field**, enter **1**</span></span>
1. <span data-ttu-id="ec5c4-108">في الحقل **معرف قالب توزيع البضائع**، أدخل اسماً، مثل **XDock_RAF**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-108">In the **Cross docking template ID** field, enter a name, such as **XDock_RAF**</span></span>
1. <span data-ttu-id="ec5c4-109">في الحقل **سياسة إصدار الطلب**، حدد **الاستلام عند التوريد**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-109">In the **Demand release policy** field, select **At supply receipt**.</span></span>
1. <span data-ttu-id="ec5c4-110">في الحقل **المستودع**، أدخل رقم المستودع الذي ترغب في إعداد عملية توزيع البضائع فيه.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-110">In the **Warehouse** field, enter the number of the warehouse where you want to set up the cross-docking process.</span></span> <span data-ttu-id="ec5c4-111">بالنسبة لهذا المثال، حدد **51**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-111">For this example, select **51**</span></span>


## <a name="cross-dock-finished-goods-to-the-outbound-location"></a><span data-ttu-id="ec5c4-112">توزيع البضائع النهائية إلى الموقع الخارجي</span><span class="sxs-lookup"><span data-stu-id="ec5c4-112">Cross-dock finished goods to the outbound location</span></span>


1. <span data-ttu-id="ec5c4-113">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-113">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>
1. <span data-ttu-id="ec5c4-114">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-114">Select **New**.</span></span>
1. <span data-ttu-id="ec5c4-115">بالنسبة لرأس أمر المبيعات، حدد حساب العميل **US-001** و **المستودع** **51**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-115">For the sales order header, select customer account **US-001** and **Warehouse** **51**</span></span>
1. <span data-ttu-id="ec5c4-116">أضف سطراً لصنفيّ **D0003**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-116">Add a line for 2 items of **D0003**</span></span>
1. <span data-ttu-id="ec5c4-117">في القسم **سطور أمر المبيعات**، حدد **المنتج والتوريد > أمر الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-117">In the **Sales order lines** section, select **Product and supply > Production order**.</span></span>
1. <span data-ttu-id="ec5c4-118">في مربع الحوار **إنشاء أمر إنتاج**، راجع القيم الافتراضية، ثم حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-118">In the **Create production order** dialog box, review the default values, and then select **Create**.</span></span> <span data-ttu-id="ec5c4-119">يتم إنشاء أمر إنتاج جديد وربطه بأمر المبيعات (أي أنه محجوز ومحدد).</span><span class="sxs-lookup"><span data-stu-id="ec5c4-119">A new production order is created and linked to the sales order (that is, it's reserved and marked).</span></span>
8. <span data-ttu-id="ec5c4-120">في الصفحة **أمر الإنتاج**، في جزء الإجراء، ضمن **علامة التبويب أمر الإنتاج**، في مجموعة العملية، حدد **تقدير**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-120">On the **Production order** page, on the Action Pane, on the **Production order tab**, in the Process group, select **Estimate**, and then select **OK**.</span></span> <span data-ttu-id="ec5c4-121">يتم تقدير الأمر، ويتم حجز كمية المادة الخام للإنتاج.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-121">The order is estimated, and the raw material quantity is reserved for the production.</span></span>
9. <span data-ttu-id="ec5c4-122">في جزء الإجراء، ضمن علامة التبويب **أمر الإنتاج**، في مجموعة **العملية**، حدد **إصدار**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-122">On the Action Pane, on the **Production order** tab, in the **Process** group, select **Release**, and then select **OK**.</span></span> <span data-ttu-id="ec5c4-123">يتم إنشاء عمل انتقاء في المستودع للمواد الخام.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-123">Warehouse pick work is created for the raw materials.</span></span>
10. <span data-ttu-id="ec5c4-124">افتح العمل وقم بمراجعته.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-124">Open and review the work.</span></span> <span data-ttu-id="ec5c4-125">في جزء الإجراء، في علامة التبويب **المستودع**، في المجموعة **عام**، حدد **تفاصيل العمل**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-125">On the Action Pane, on the **Warehouse** tab, in the **General** group, select **Work details**.</span></span> <span data-ttu-id="ec5c4-126">سجِّل معرف العمل.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-126">Make a note of the work ID.</span></span>
11. <span data-ttu-id="ec5c4-127">افتح Dynamics 365 for Finance and Operations وسجل الدخول إليه – تطبيق الأجهزة المحمولة</span><span class="sxs-lookup"><span data-stu-id="ec5c4-127">Open and sign in to Dynamics 365 for Finance and Operations – Mobile App</span></span> 
12. <span data-ttu-id="ec5c4-128">انتقل إلى **الإنتاج > انتقاء الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-128">Go to **Production > Production pick**.</span></span>
13. <span data-ttu-id="ec5c4-129">أدخل معرف العمل لبدء انتقاء المادة الخام وإكماله.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-129">Enter the work ID to start and complete the raw material picking.</span></span> 
    > [!NOTE]
    >  <span data-ttu-id="ec5c4-130">بعد الإبلاغ عن انتهاء العمل، تكون كمية المواد الخام متاحة في موقع إدخال الإنتاج (**005** في بيانات العرض التوضيحي لـ USMF)، ويمكن بدء تنفيذ أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-130">After the work is reported as finished, the quantity of raw materials is available in the production input location (**005** in USMF demo data), and execution of the production order can start.</span></span>

13. <span data-ttu-id="ec5c4-131">في الصفحة **أمر الإنتاج**، في جزء الإجراء، ضمن علامة التبويب **أمر الإنتاج**، في مجموعة **العملية**، حدد **بدء**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-131">On the **Production order** page, on the Action Pane, on the **Production order** tab, in the **Process** group, select **Start**, and then select **OK**.</span></span>
14. <span data-ttu-id="ec5c4-132">في التطبيق، انتقل إلى **الإنتاج > RAF والإبعاد**.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-132">In the app, go to **Production > RAF and put away**.</span></span>
15. <span data-ttu-id="ec5c4-133">في الحقل **معرف المنتج**، أدخل رقم أمر الإنتاج والتفاصيل الإلزامية الأخرى، ثم حدد **موافق**</span><span class="sxs-lookup"><span data-stu-id="ec5c4-133">In the **Prod ID** field, enter the production order number and other mandatory details, and then select **OK**</span></span>


<span data-ttu-id="ec5c4-134">سيؤدي ذلك إلى:</span><span class="sxs-lookup"><span data-stu-id="ec5c4-134">This will result in:</span></span>

- <span data-ttu-id="ec5c4-135">يتم تشغيل الإصدار إلى مستودع لأمر المبيعات المرتبط.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-135">The release to a warehouse is triggered for the linked sales order.</span></span>
- <span data-ttu-id="ec5c4-136">وبناءً على الإصدار، فانه يتم إنشاء الشحن وعمل توزيع البضائع.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-136">Based on the release, shipment and cross-docking work is created.</span></span> <span data-ttu-id="ec5c4-137">يرشد هذا العمل عامل المستودع لانتقاء الكميات المطلوبة لتنفيذ سطر أمر المبيعات ووضعها في الموقع الخارجي الذي تم تحديده في توجيه موقع توزيع البضائع.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-137">This work instructs the warehouse operator to pick the quantities that are required to fulfill the sales order line and put them in the outbound location that specified in the cross-docking location directive.</span></span>
- <span data-ttu-id="ec5c4-138">إذا كانت كمية أمر الإنتاج أكبر من الكمية المطلوبة لأمر المبيعات، فسيتم إنشاء عمل إبعاد عادي.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-138">If the production order quantity is more than the quantity that is required by the sales order, regular put-away work is created.</span></span> <span data-ttu-id="ec5c4-139">يرشد هذا العمل عامل المستودع لانتقاء كمية البضائع النهائية التي تبقى بعد توزيع البضائع ونقلها إلى التخزين العادي، وذلك وفقاً لتوجيه الموقع.</span><span class="sxs-lookup"><span data-stu-id="ec5c4-139">This work instructs the warehouse operator to pick the quantity of finished goods that remains after cross-docking and move it to regular storage, according to the location directive.</span></span>


