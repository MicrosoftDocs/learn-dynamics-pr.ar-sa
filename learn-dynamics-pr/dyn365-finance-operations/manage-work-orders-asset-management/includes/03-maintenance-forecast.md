---
ms.openlocfilehash: 101f168a1e4209f57f56f445c01728b6368026ca
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072433"
---
<span data-ttu-id="e49e0-101">عند إنشاء أمر عمل، يتم إنشاء مهام أمر العمل التي لها أصول وأنواع مهام الصيانة.</span><span class="sxs-lookup"><span data-stu-id="e49e0-101">When a work order is created, work order jobs are created that have assets and maintenance job types.</span></span> <span data-ttu-id="e49e0-102">يمكن أن يكون لنوع مهمة الصيانة أيضاً تنبؤ بمتطلبات الصيانة، وفي هذه الحالة، يتم نسخ التنبؤ تلقائياً إلى أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="e49e0-102">A maintenance job type can also have a maintenance forecast, in which case, the forecast is automatically copied to the work order.</span></span> 

<span data-ttu-id="e49e0-103">يتم تعريف التنبؤ بأنه الساعات والأصناف والمصروفات المتوقعة في أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="e49e0-103">A forecast is defined as the expected hours, items, and expenses on a work order.</span></span> <span data-ttu-id="e49e0-104">يمكن حذف بنود التنبؤ هذه من أمر العمل أو يمكنك إضافة بنود.</span><span class="sxs-lookup"><span data-stu-id="e49e0-104">Those forecast lines can be deleted from the work order or you could add lines.</span></span> <span data-ttu-id="e49e0-105">يتم تحديد ما إذا كان يجب حذف بنود التنبؤ أو إضافتها بواسطة حالة دورة الحياة ونوع المشروع وقاعدة المرحلة المرتبطة بنوع المشروع.</span><span class="sxs-lookup"><span data-stu-id="e49e0-105">Whether the forecast lines should be deleted or added is determined by the lifecycle state, the project type, and the stage rule that is related to the project type.</span></span> 

## <a name="view-maintenance-forecast-lines"></a><span data-ttu-id="e49e0-106">عرض بنود التنبؤ بمتطلبات الصيانة</span><span class="sxs-lookup"><span data-stu-id="e49e0-106">View maintenance forecast lines</span></span> 
<span data-ttu-id="e49e0-107">لعرض تنبؤ بمتطلبات الصيانة، انتقل إلى **إدارة الأصول > شائع > أوامر العمل > كافة أوامر العمل** وفي قسم **المشروع**، حدد **التنبؤ**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-107">To view a maintenance forecast, go to **Asset management > Common > Work orders > All work orders** and, in the **Project** section, select **Forecast**.</span></span> <span data-ttu-id="e49e0-108">تظهر صفحة **التنبؤ بمتطلبات صيانة أمر العمل**، حيث يمكنك الاطلاع على علامات التبويب السريعة **الساعات** و **الأصناف** و **المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-108">The **Work order maintenance forecast** page appears, where you can see the **Hours**, **Items**, and **Expense** FastTabs.</span></span> <span data-ttu-id="e49e0-109">في هذه الصفحة، يمكنك عرض التنبؤات للساعات والأصناف، حيث يستخدم كل منها خصائص البنود للأصناف القابلة للفوترة أو غير القابلة للفوترة.</span><span class="sxs-lookup"><span data-stu-id="e49e0-109">On this page, you can view the forecasts for hours and items, each using line properties of billable or non-billable items.</span></span> <span data-ttu-id="e49e0-110">بالنسبة للأصناف، سيتضمن إعداد **تلقائياً** سعر التكلفة الخاص بالصنف.</span><span class="sxs-lookup"><span data-stu-id="e49e0-110">For the items, the setup of **Automatically** will include the cost price of the item.</span></span> 

<span data-ttu-id="e49e0-111">[![لقطه شاشة لصفحة التنبؤ بمتطلبات صيانة أمر العمل مع تفاصيل الأصناف.](../media/work-order-maintenance-forecast-detail-ss.png)](../media/work-order-maintenance-forecast-detail-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="e49e0-111">[![Screenshot of the Work order maintenance forecast page with items details.](../media/work-order-maintenance-forecast-detail-ss.png)](../media/work-order-maintenance-forecast-detail-ss.png#lightbox)</span></span>
 
<span data-ttu-id="e49e0-112">تعرض علامة التبويب السريعة **المصروفات** كلاً من **سعر التكلفة** و **سعر المبيعات**، وهو ما يتيح لك تحديد **قابل للفوترة** أو **غير قابل للفوترة**، كما هو موضح في الصورة التالية.</span><span class="sxs-lookup"><span data-stu-id="e49e0-112">The **Expense** FastTab displays the **Cost price** and **Sales price**, which allow you to select **Billable** or **NonBill**, as shown in the following image.</span></span>

![لقطة شاشة لتفاصيل علامة التبويب السريعة المصروفات.](../media/expense-fasttab-ss.png)
 
<span data-ttu-id="e49e0-114">يتم توفير ملخص لإجماليات التنبؤ في علامة التبويب السريعة **إجماليات التنبؤ بمتطلبات الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-114">A summary of the forecast totals is provided on the **Maintenance forecast totals** FastTab.</span></span>

<span data-ttu-id="e49e0-115">[![لقطة شاشة لعلامة التبويب السريعة إجماليات التنبؤ بمتطلبات الصيانة.](../media/maintenance-forecast-totals-fasttab-ss.png)](../media/maintenance-forecast-totals-fasttab-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="e49e0-115">[![Screenshot of the Maintenance forecast totals FastTab.](../media/maintenance-forecast-totals-fasttab-ss.png)](../media/maintenance-forecast-totals-fasttab-ss.png#lightbox)</span></span>
 
<span data-ttu-id="e49e0-116">شاهد الفيديو التالي للتعرف على كيفية إضافة بنود التنبؤ إلى أمر عمل.</span><span class="sxs-lookup"><span data-stu-id="e49e0-116">Watch the following video to learn how to add forecast lines to a work order.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4pmuD]
 
## <a name="integration-with-project-management-and-accounting"></a><span data-ttu-id="e49e0-117">التكامل مع إدارة المشاريع ومحاسبتها</span><span class="sxs-lookup"><span data-stu-id="e49e0-117">Integration with Project management and accounting</span></span>
<span data-ttu-id="e49e0-118">يمكن إعداد أوامر العمل لتتكامل مع مشروع في Dynamics 365 Supply Chain Management، في صفحة **معلمات إدارة الأصول**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-118">Work orders can be set up to be integrated with a project in Dynamics 365 Supply Chain Management, on the **Asset management parameters** page.</span></span> <span data-ttu-id="e49e0-119">توضح الصورة التالية أنه تم إدخال مشروع في الحقل **مشروع التنبؤ بمتطلبات الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-119">The following image shows that a project has been entered in the **Maintenance forecast project** field.</span></span> <span data-ttu-id="e49e0-120">سيتم تحديث هذا المشروع تلقائياً ببيانات أمر العمل، وسيتم ملء أي معاملات تم إنشاؤها في المشروع في أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="e49e0-120">This project will automatically be updated with work order data, and any transactions that are created on the project will be populated on the work order.</span></span> 

<span data-ttu-id="e49e0-121">**إدارة الأصول > الإعداد > معلومات إدارة الأصول**</span><span class="sxs-lookup"><span data-stu-id="e49e0-121">**Asset management > Setup > Asset management parameters**</span></span>

![لقطة شاشة لصفحة معلمات إدارة الأصول مع تمييز التنبؤ.](../media/asset-management-parameters-ssm.png)
 
<span data-ttu-id="e49e0-123">لتحديث التنبؤ بناءً على الإدخالات في الوحدات النمطية الأخرى، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="e49e0-123">To update a forecast based on entries in other modules, follow these steps:</span></span>

1.  <span data-ttu-id="e49e0-124">حدد **إدارة الأصول > دوري > التنبؤ > تحديث التنبؤ بأمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-124">Select **Asset management > Periodic > Forecast > Update work order forecast**.</span></span>
2.  <span data-ttu-id="e49e0-125">في مربع الحوار **تحديث التنبؤ بأمر العمل** في علامة التبويب السريعة **السجلات المطلوب تضمينها**، أضف أوامر عمل معينة أو مهام صيانة أوامر العمل، حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="e49e0-125">In the **Update work order forecast** dialog box, on the **Records to include** FastTab, add specific work orders or work order maintenance jobs, as needed.</span></span> <span data-ttu-id="e49e0-126">حدد **عامل تصفية** للقيام بالتحديدات ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="e49e0-126">Select **Filter** to make the relevant selections.</span></span>
3.  <span data-ttu-id="e49e0-127">في علامة التبويب السريعة **تشغيل في الخلفية**، قم بإعداد التحديث التلقائي كوظيفة دفعية، على النحو الذي تطلبه.‬</span><span class="sxs-lookup"><span data-stu-id="e49e0-127">On the **Run in the background** FastTab, set up the automatic update as a batch job, as you require.</span></span>
4.  <span data-ttu-id="e49e0-128">حدد **موافق** لبدء تحديث التنبؤ.</span><span class="sxs-lookup"><span data-stu-id="e49e0-128">Select **OK** to start the forecast update.</span></span>

<span data-ttu-id="e49e0-129">توضح الصورة التالية أن التنبؤ الذي تم إدخاله في أمر العمل موجود الآن في صفحة **المشروع**.</span><span class="sxs-lookup"><span data-stu-id="e49e0-129">The following image shows that the forecast that was entered on the work order now resides on the **Project** page.</span></span>

<span data-ttu-id="e49e0-130">**إدارة المشاريع والمحاسبة > المشاريع > كافة المشاريع**</span><span class="sxs-lookup"><span data-stu-id="e49e0-130">**Project management and accounting > Projects > All projects**</span></span>

<span data-ttu-id="e49e0-131">[![لقطة شاشة لطريقة العرض "كافة المشاريع" مع عرض التفاصيل.](../media/project-page-details-ss.png)](../media/project-page-details-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="e49e0-131">[![Screenshot of the All projects view with details displayed.](../media/project-page-details-ss.png)](../media/project-page-details-ss.png#lightbox)</span></span>

<span data-ttu-id="e49e0-132">وعلى العكس من ذلك، ستقوم أي بيانات تنبؤ تم إدخالها من المشروع بتحديث التنبؤ بأمر العمل.</span><span class="sxs-lookup"><span data-stu-id="e49e0-132">Conversely, any forecast data that was entered from the project will update the work order forecast.</span></span>

<span data-ttu-id="e49e0-133">**إدارة الأصول > شائع > أوامر العمل > كافة أوامر العمل** > تحديد بند أمر عمل > **علامة التبويب السريعة** المشروع > **التنبؤ > التنبؤ بالساعات**</span><span class="sxs-lookup"><span data-stu-id="e49e0-133">**Asset management > Common > Work orders > All work orders** > select a work order line > **Project** FastTab > **Forecast > Hour forecasts**</span></span>

<span data-ttu-id="e49e0-134">[![لقطة شاشة لتفاصيل مشروع التنبؤ بالساعات.](../media/work-order-forecast-project-details-ssm.png)](../media/work-order-forecast-project-details-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="e49e0-134">[![Screenshot of the Hour forecast project details.](../media/work-order-forecast-project-details-ssm.png)](../media/work-order-forecast-project-details-ssm.png#lightbox)</span></span>
 
<span data-ttu-id="e49e0-135">تم تحديث التنبؤ بأمر العمل في صفحة **التنبؤ بمتطلبات صيانة أمر العمل** كما هو موضح في الصورة التالية.</span><span class="sxs-lookup"><span data-stu-id="e49e0-135">The work order forecast has been updated on the **Work order maintenance forecast** page, as shown in the following image.</span></span>

![لقطة شاشة لصفحة التنبؤ بمتطلبات صيانة أمر العمل.](../media/work-order-maintenance-forecast-hours-detail-ssm.png)