---
ms.openlocfilehash: db32c5c6ed59d3a41d975eb7c8ef6576717afd39
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072377"
---
<span data-ttu-id="15a6d-101">تعتبر أوامر العمل هي المركبة التي تقوم فيها إدارة الأصول في Dynamics 365 Supply Chain Management بإدارة مهام الصيانة والإصلاح الخاصة بأصول المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="15a6d-101">Work orders are the vehicle in which Asset Management for Dynamics 365 Supply Chain Management manages the maintenance and repair jobs of your organization’s assets.</span></span> <span data-ttu-id="15a6d-102">يمكن إنشاء أمر عمل لأصل واحد أو لعدة أصول، وفقاً لما يجب إكماله.</span><span class="sxs-lookup"><span data-stu-id="15a6d-102">A work order can be created for one or many assets, depending on what needs to be completed.</span></span> 

<span data-ttu-id="15a6d-103">يتم إنشاء أوامر العمل في إدارة الأصول بعدة طرق:</span><span class="sxs-lookup"><span data-stu-id="15a6d-103">Work orders are created in Asset Management in several ways:</span></span>

- <span data-ttu-id="15a6d-104">يمكن إعداد خطة صيانة للأصل الذي سينشئ أمر عمل تلقائياً باستخدام ميزة جدولة خطة الصيانة.</span><span class="sxs-lookup"><span data-stu-id="15a6d-104">A maintenance plan can be set up on the asset that will automatically create a work order by using the schedule maintenance plan feature.</span></span>
- <span data-ttu-id="15a6d-105">إذا كانت لديك مهام صيانة وقائية أو طلبات صيانة، يمكن إنشاء جدول صيانة، كما يمكن إنشاء أوامر عمل من هذا النموذج.</span><span class="sxs-lookup"><span data-stu-id="15a6d-105">If you have preventive maintenance jobs or maintenance requests, a maintenance schedule can be created, and work orders can be created from that form.</span></span>
- <span data-ttu-id="15a6d-106">ويمكن إنشاء أمر العمل يدوياً.</span><span class="sxs-lookup"><span data-stu-id="15a6d-106">A work order can be created manually.</span></span>
- <span data-ttu-id="15a6d-107">من صفحة **طلب الصيانة**، حيث أنشأ شخص ما الطلب.</span><span class="sxs-lookup"><span data-stu-id="15a6d-107">From the **Maintenance request** page, where someone has created the request.</span></span>

## <a name="all-work-orders-list-page"></a><span data-ttu-id="15a6d-108">صفحه قائمة جميع أوامر العمل</span><span class="sxs-lookup"><span data-stu-id="15a6d-108">All work orders list page</span></span> 
<span data-ttu-id="15a6d-109">في صفحة قائمة **جميع أوامر العمل**، يمكنك عرض جميع أوامر العمل في النظام، بغض النظر عن حالتها.</span><span class="sxs-lookup"><span data-stu-id="15a6d-109">On the **All work orders** list page, you can view all work orders in the system, regardless of their state (status).</span></span> <span data-ttu-id="15a6d-110">يمكن أن يكون لأمر العمل حالات دورة حياة متعددة وفقاً لاحتياجات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="15a6d-110">A work order can have several lifecycle states depending on your organization’s needs.</span></span> <span data-ttu-id="15a6d-111">على سبيل المثال، يمكن أن يكون أمر العمل بالحالة **مُنشأ** أو **مُجدول** أو **مكتمل**.</span><span class="sxs-lookup"><span data-stu-id="15a6d-111">For example, a work order can be in the state of **Created**, **Scheduled**, or **Complete**.</span></span> <span data-ttu-id="15a6d-112">يمكنك إعداد حالات دورة الحياة وفقاً لاحتياجات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="15a6d-112">Depending on your organization’s needs, you can set up lifecycle states.</span></span> <span data-ttu-id="15a6d-113">لمعرفة كيفية إعداد حالات دورة الحياة ونماذج دورة الحياة، انتقل إلى [حالات دورة الحياة لأمر العمل](https://docs.microsoft.com/dynamics365/supply-chain/asset-management/setup-for-work-orders/work-order-lifecycle-states/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="15a6d-113">To learn how to set up your lifecycle states and lifecycle models, go to [Work order lifecycle states](https://docs.microsoft.com/dynamics365/supply-chain/asset-management/setup-for-work-orders/work-order-lifecycle-states/?azure-portal=true).</span></span>

<span data-ttu-id="15a6d-114">**إدارة الأصول > عام > أوامر العمل > جميع أوامر العمل**</span><span class="sxs-lookup"><span data-stu-id="15a6d-114">**Asset Management > Common > Work orders > All work orders**</span></span>
 
<span data-ttu-id="15a6d-115">[![لقطة شاشة لصفحة قائمة جميع أوامر العمل.](../media/all-work-orders-ss.png)](../media/all-work-orders-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="15a6d-115">[![Screenshot of the All work orders list page.](../media/all-work-orders-ss.png)](../media/all-work-orders-ss.png#lightbox)</span></span>

<span data-ttu-id="15a6d-116">بالإضافة إلى ذلك، يمكنك الاطلاع على معلومات حول كل أمر من أوامر العمل، بما في ذلك عدد البنود الموجودة في أمر العمل (بمعني آخر، عدد المهام الموجودة في أمر العمل، ويمكن أن تكون لديك مهمة واحدة أو عدة مهام في أمر العمل)، والوصف، وتفاصيل وقت البدء والانتهاء ونوع الصيانة والتجارة المطلوبة والمزيد.</span><span class="sxs-lookup"><span data-stu-id="15a6d-116">Additionally, you can see information about each work order, including how many lines are on the work order (in other words, how many jobs are on the work order, and you can have one or you can have many jobs on a work order), description, start and end time details, maintenance type, trade required, and more.</span></span> <span data-ttu-id="15a6d-117">إذا كنت بحاجة إلى الاطلاع على التفاصيل الخاصة بأي أمر عمل في هذه الصفحة، فحدد **أمر العمل** الذي تريد عرضه من صفحة القائمة.</span><span class="sxs-lookup"><span data-stu-id="15a6d-117">If you need to see the details for any work order on this page, select the **Work order** that you want to view from the list page.</span></span>  

<span data-ttu-id="15a6d-118">في صفحة **جميع أوامر العمل**، يمكنك التنقل في أوامر العمل الفردية والاطلاع على مزيد من التفاصيل حول كل أمر.</span><span class="sxs-lookup"><span data-stu-id="15a6d-118">On the **All work orders** page, you can drill into the individual work orders and see more details about each order.</span></span>

<span data-ttu-id="15a6d-119">[![لقطة شاشة لأمر عمل مع الأصل والاسم وتفاصيل البدء والانتهاء.](../media/work-orders-ssm.png)](../media/work-orders-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="15a6d-119">[![Screenshot of a Work order with asset, name, and start and end details.](../media/work-orders-ssm.png)](../media/work-orders-ssm.png#lightbox)</span></span>
 
<span data-ttu-id="15a6d-120">التفاصيل الرئيسية التي يمكنك العثور عليها في صفحة **أمر العمل**:</span><span class="sxs-lookup"><span data-stu-id="15a6d-120">The key details that you find on the **Work order** page:</span></span>

- <span data-ttu-id="15a6d-121">معرف الأصل واسمه</span><span class="sxs-lookup"><span data-stu-id="15a6d-121">Asset ID and name</span></span>
- <span data-ttu-id="15a6d-122">اسم المهمة ومتغير النوع (أسبوعياً، كما هو موضح في الصورة السابقة)، والتجارة (فني الكهرباء، في أمر العمل هذا)</span><span class="sxs-lookup"><span data-stu-id="15a6d-122">Name of the job, type variant (Weekly, as shown in the preceding image), and trade (Electrician, in this work order)</span></span>
- <span data-ttu-id="15a6d-123">البدء المجدول والنهاية المجدولة لأمر العمل</span><span class="sxs-lookup"><span data-stu-id="15a6d-123">Scheduled start and scheduled end of the work order</span></span>

<span data-ttu-id="15a6d-124">ضمن جزء الإجراءات، في صفحة **أمر العمل**، توجد القائمة الفرعية حيث يمكنك الاطلاع على أقسام مختلفة تحدد الوظائف المختلفة المرتبطة بأمر العمل، كما هو موضح في المقاطع التالية.</span><span class="sxs-lookup"><span data-stu-id="15a6d-124">Under the Action Pane, on the **Work order** page, is the submenu where you can see different sections outlining the various functions that are related to the work order, as described in the subsequent segments.</span></span>

## <a name="maintain"></a><span data-ttu-id="15a6d-125">الاحتفاظ</span><span class="sxs-lookup"><span data-stu-id="15a6d-125">Maintain</span></span>
<span data-ttu-id="15a6d-126">يحتوي قسم **الاحتفاظ** على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="15a6d-126">The **Maintain** section contains the following options:</span></span>

- <span data-ttu-id="15a6d-127">**وعاء أوامر العمل** - يمكنك إضافة أمر العمل أو إزالته من وعاء أوامر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-127">**Work order pool** – Add or remove the work order from a work order pool.</span></span>
- <span data-ttu-id="15a6d-128">**التعديل** - يمكنك إجراء تعديلات على الكيانات مثل تاريخ البدء أو الانتهاء الجديد والأولوية ومجموعة المسؤولين وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="15a6d-128">**Adjust** – Make adjustments to entities such as new start or end date, priority, responsible group, and so on.</span></span>

## <a name="new"></a><span data-ttu-id="15a6d-129">جديد</span><span class="sxs-lookup"><span data-stu-id="15a6d-129">New</span></span>
<span data-ttu-id="15a6d-130">يحتوي قسم **جديد** على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="15a6d-130">The **New** section contains the following options:</span></span>

- <span data-ttu-id="15a6d-131">**أمر العمل المرتبط** – يمكنك إنشاء أمر عمل جديد مرتبط بالأمر الحالي أو إضافة أمر العمل الجديد إلى أمر موجود.</span><span class="sxs-lookup"><span data-stu-id="15a6d-131">**Related work order** – Create a new work order that is related to the current one or add the new work order to an existing one.</span></span>
- <span data-ttu-id="15a6d-132">**نسخ أمر العمل** – يمكنك إنشاء أمر عمل جديد استناداً إلى الأمر الموجود.</span><span class="sxs-lookup"><span data-stu-id="15a6d-132">**Copy work order** – Create a new work order based on the existing one.</span></span>

## <a name="view"></a><span data-ttu-id="15a6d-133">العرض</span><span class="sxs-lookup"><span data-stu-id="15a6d-133">View</span></span>
<span data-ttu-id="15a6d-134">يحتوي قسم **العرض** على الخيار **محفوظات الأحداث**، حيث يمكنك عرض المحفوظات المرتبطة بأمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-134">The **View** section contains the **Event history** option, where you can view the history that is related to the work order.</span></span>

## <a name="lines"></a><span data-ttu-id="15a6d-135">البنود</span><span class="sxs-lookup"><span data-stu-id="15a6d-135">Lines</span></span>
<span data-ttu-id="15a6d-136">يحتوي قسم **البنود** على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="15a6d-136">The **Lines** section contains the following options:</span></span>

- <span data-ttu-id="15a6d-137">**ملاحظات مهمة صيانة أمر العمل** – يمكنك قراءة الملاحظات المرتبطة بمهمة الصيانة.</span><span class="sxs-lookup"><span data-stu-id="15a6d-137">**Work order maintenance job notes** – Read the notes that are related to the maintenance job.</span></span>
- <span data-ttu-id="15a6d-138">**الأدوات** - يمكنك عرض الأدوات المطلوبة لإكمال أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-138">**Tools** - View tools that are required to complete the work order.</span></span>
- <span data-ttu-id="15a6d-139">**قائمة فحص الصيانة** - يمكنك عرض الخطوات المطلوبة لإكمال أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-139">**Maintenance checklist** – View the steps that are required to complete the work order.</span></span>

## <a name="asset"></a><span data-ttu-id="15a6d-140">الأصل</span><span class="sxs-lookup"><span data-stu-id="15a6d-140">Asset</span></span>
<span data-ttu-id="15a6d-141">يحتوي قسم **الأصل** على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="15a6d-141">The **Asset** section contains the following options:</span></span>

- <span data-ttu-id="15a6d-142">**خطأ الأصل** - يمكنك عرض أخطاء الأصول، مثل الأعراض التي تم الكشف عنها والتي ينتج عنها أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-142">**Asset fault** - View the asset faults, such as detected symptoms that cause the work order.</span></span>
- <span data-ttu-id="15a6d-143">**وقت تعطل الصيانة** – يمكنك جدولة أي وقت تعطل مرتبط بإكمال أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-143">**Maintenance downtime** – Schedule any downtime that is associated with completing the work order.</span></span>
- <span data-ttu-id="15a6d-144">**تقييم الشرط** – يمكنك إضافة تقييم للشرط الذي تم الكشف عنه.</span><span class="sxs-lookup"><span data-stu-id="15a6d-144">**Condition assessment** – Add an assessment of the detected condition.</span></span>
- <span data-ttu-id="15a6d-145">**عدادات الأصول** – يمكنك إضافة أي عدادات مرتبطة بأمر العمل أو عرضها.</span><span class="sxs-lookup"><span data-stu-id="15a6d-145">**Asset counters** – Add or view any counters that are related to the work order.</span></span>

## <a name="project"></a><span data-ttu-id="15a6d-146">المشروع</span><span class="sxs-lookup"><span data-stu-id="15a6d-146">Project</span></span>
<span data-ttu-id="15a6d-147">يحتوي قسم **المشروع** على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="15a6d-147">The **Project** section contains the following options:</span></span>

- <span data-ttu-id="15a6d-148">**التنبؤ** - يمكنك عرض تفاصيل التنبؤ المرتبطة بأمر العمل أو إضافتها (الساعات أو الأصناف أو المصروفات).</span><span class="sxs-lookup"><span data-stu-id="15a6d-148">**Forecast** – View or add forecast details that are related to the work order (hours, items, or expense).</span></span>
- <span data-ttu-id="15a6d-149">**دفاتر اليومية** - يمكنك عرض دفاتر يومية أوامر العمل ونسخها والتحقق من صحتها وترحيلها.</span><span class="sxs-lookup"><span data-stu-id="15a6d-149">**Journals** - View, copy, validate, and post work order journals.</span></span>
- <span data-ttu-id="15a6d-150">**حركات المشروع** - يمكنك عرض جميع المشروعات التي تم ترحيلها.</span><span class="sxs-lookup"><span data-stu-id="15a6d-150">**Project transactions** – View all posted projects.</span></span> 

## <a name="lifecycle-state"></a><span data-ttu-id="15a6d-151">حالة دورة الحياة</span><span class="sxs-lookup"><span data-stu-id="15a6d-151">Lifecycle state</span></span>
<span data-ttu-id="15a6d-152">يحتوي قسم **حالة دورة الحياة** على الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="15a6d-152">The **Lifecycle state** section contains the following options:</span></span>

- <span data-ttu-id="15a6d-153">**تحديث حالة أمر العمل** – يمكنك تغيير حالة أمر العمل إلى حالة مختلفة.</span><span class="sxs-lookup"><span data-stu-id="15a6d-153">**Update work order state** – Change the work order state to a different one.</span></span>
- <span data-ttu-id="15a6d-154">**سجل حالة دورة الحياة** – يمكنك عرض سجل دورة الحياة لأمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-154">**Lifecycle state log** – View the work order lifecycle log.</span></span>

## <a name="attachments"></a><span data-ttu-id="15a6d-155">المرفقات‬</span><span class="sxs-lookup"><span data-stu-id="15a6d-155">Attachments</span></span>
<span data-ttu-id="15a6d-156">يحتوي قسم **المرفقات** على الخيار **مستندات الأصول**، حيث يمكنك عرض أي مستندات مرتبطة بأمر العمل.</span><span class="sxs-lookup"><span data-stu-id="15a6d-156">The **Attachments** section contains the **Asset documents** option, where you can view any documents that are related to the work order.</span></span> 