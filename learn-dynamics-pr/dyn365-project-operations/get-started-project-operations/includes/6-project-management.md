---
ms.openlocfilehash: aabb04d82cd08b904ccba7b83ae2fe763e4a9d1e
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072894"
---
<span data-ttu-id="ca0b1-101">تساعدك أدوات إدارة المشاريع في Project Operations في تشغيل المشاريع.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-101">The project management tools in Project Operations help you to run projects.</span></span> <span data-ttu-id="ca0b1-102">تساعد أدوات الجدولة مديري المشروعات والفرق في الحفاظ على إنتاجيتهم.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-102">The scheduling tools help project managers and teams stay productive.</span></span> <span data-ttu-id="ca0b1-103">تتضمن بعض المهام التي تساعد فيها الأدوات ما يلي:</span><span class="sxs-lookup"><span data-stu-id="ca0b1-103">Some of the tasks that the tools help with include:</span></span>

- <span data-ttu-id="ca0b1-104">تخطيط المشروعات باستخدام جدول العمل والتقديرات.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-104">Plan projects by using a work schedule and estimates.</span></span>
- <span data-ttu-id="ca0b1-105">تقدير تكاليف المشروع والإيرادات وتعقبها.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-105">Estimate and track project costs and revenue.</span></span>
- <span data-ttu-id="ca0b1-106">استخدم تقديرات المشروع أثناء عملية المبيعات.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-106">Use project estimates during the sales process.</span></span>
- <span data-ttu-id="ca0b1-107">التنبؤ بمتطلبات الموارد للمشاريع الموجودة في البنية الأساسية لبرنامج ربط العمليات التجارية.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-107">Forecast resource requirements for projects that are in the pipeline.</span></span>
- <span data-ttu-id="ca0b1-108">تسليم المشاريع بنجاح من خلال تعقب التقدم المحرز واستهلاك التكلفة.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-108">Deliver projects successfully by tracking progress and cost consumption.</span></span>

## <a name="project-stages"></a><span data-ttu-id="ca0b1-109">مراحل المشروع</span><span class="sxs-lookup"><span data-stu-id="ca0b1-109">Project stages</span></span>

<span data-ttu-id="ca0b1-110">يتم تصميم مراحل المشروع لتعكس حالة المشروع أثناء تقدمه.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-110">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="ca0b1-111">يمكن استخدام التخصيصات لتحديث المراحل تلقائياً من خلال تدفقات عمليات الأعمال أو Microsoft Power Automate أو ملحقات المكونات الإضافية.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-111">Customizations can be used to automatically update the stages with business process flows, Microsoft Power Automate, or plug-in extensions.</span></span>

![رسم تخطيطي لسير إجراءات العمل الافتراضي.](../media/project-stages-c.png)

<span data-ttu-id="ca0b1-113">يتم تحديد المراحل التالية في سير إجراءات العمل الافتراضي:</span><span class="sxs-lookup"><span data-stu-id="ca0b1-113">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="ca0b1-114">**جديد** - عند إنشاء مشروع، يتم تعيين مرحلة المشروع على **جديد**.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-114">**New** – When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="ca0b1-115">إذا تم إنشاء المشروع من قالب، فقد يتضمن جدول زمني وتقدير وبيانات الفريق.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="ca0b1-116">وإلا، فسيكون مخطط تفصيلي للمشروع، ويتعين عليك إدخال المكونات المتبقية.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-116">Otherwise, it is an outline of the project, and the remaining components must be entered.</span></span>

- <span data-ttu-id="ca0b1-117">**عرض الأسعار** – عند إقران مشروع بعرض أسعار أو عند إنشاء مشروع من عرض أسعار، يتم تعيين مرحلة المشروع على **عرض الأسعار**، ويتم تحديث تاريخي البدء والانتهاء المقدرين.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-117">**Quote** – When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote** and the estimated start and end dates are updated.</span></span> <span data-ttu-id="ca0b1-118">أثناء وجود المشروع في مرحلة **عرض الأسعار**، ستعرض علامة التبويب **المبيعات** في الصفحة **كيان المشروع** تفاصيل عرض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-118">While the project is in the **Quote** stage, the **Sales** tab on the **Project entity** page shows details of the quote.</span></span>

- <span data-ttu-id="ca0b1-119">**التخطيط** – عندما تفوز بعرض أسعار مقترن بمشروع، سينتقل المشروع إلى مرحلة **العقد**، وسيتم تحديث مرحلة المشروع إلى **التخطيط**.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-119">**Plan** – When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="ca0b1-120">أثناء وجود المشروع في مرحلة **تخطيط**، ستعرض الصفحة **‎كيان المشروع** تفاصيل العقد.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-120">While the project is in the **Plan** stage, the **Project entity** page shows details of the contract.</span></span>

- <span data-ttu-id="ca0b1-121">**تسليم** – عند اكتمال خطة المشروع، وأنت جاهز لبدء المشروع، فيجب على مدير المشروع تحديث مرحلة المشروع إلى **تسليم** لإظهار أن المشروع قد بدأ.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-121">**Deliver** – When the project plan is completed, and you are ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

- <span data-ttu-id="ca0b1-122">**اكتمال** – عند اكتمال العمل في المشروع، يمكن لمدير المشروع تحديث المرحلة إلى **اكتمال**.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-122">**Complete** – When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="ca0b1-123">من خلال تحديث مرحلة المشروع إلى **اكتمال**، يشير مدير المشروع إلى أن العمل قد اكتمل بنسبة 100 في المائة ولكن يظل المشروع مفتوحاً بحيث يمكن تسجيل أي إدخالات للوقت أو المصروفات المعلقة.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-123">By updating the project stage to **Complete**, the project manager indicates that the work is 100 percent completed but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

- <span data-ttu-id="ca0b1-124">**إغلاق** – عند تسجيل كافة الحركات الخاصة بالمشروع، يمكن لمدير المشروع تحديث المرحلة إلى **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-124">**Close** – When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="ca0b1-125">في هذه المرحلة، لا يمكن تسجيل أي حركات، ويتم تعيين المشروع للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-125">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>

> [!NOTE]
> <span data-ttu-id="ca0b1-126">لا يقوم سير إجراءات العمل الافتراضي في Project Operations بإجراء انتقالات تلقائية للحالة.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-126">The default business process flow in Project Operations does not perform automatic state transitions.</span></span>

## <a name="navigate-the-user-interface"></a><span data-ttu-id="ca0b1-127">التنقل في واجهة المستخدم</span><span class="sxs-lookup"><span data-stu-id="ca0b1-127">Navigate the user interface</span></span>

<span data-ttu-id="ca0b1-128">يتم فصل صفحة **المشروع** إلى عدة علامات تبويب.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-128">The **Project** page is separated into several tabs.</span></span> <span data-ttu-id="ca0b1-129">تمثل كل علامة تبويب مستوً مختلفاً من التفاصيل داخل المشروع.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-129">Each tab represents a different level of detail within the project.</span></span>

- <span data-ttu-id="ca0b1-130">**ملخص** – يقدم وصفاً للمشروع ويجمع أداء المشروع المخطط والفعلي.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-130">**Summary** – Provides a description of the project and aggregates the planned and actual project performance.</span></span>

    <span data-ttu-id="ca0b1-131">[![لقطة شاشة لعلامة تبويب مخلص مشروع "تجديد المتجر وتغيير صورته".](../media/summary-ss.png)](../media/summary-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-131">[![Screenshot of the Store Rebrand and Refurbish project Summary tab.](../media/summary-ss.png)](../media/summary-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-132">**المهام** – يوفر تفاصيل حول هيكل تنظيم العمل الذي يمثله طريقة عرض الشبكة وعرض اللوحة وعرض المخطط الزمني، أو يُعرف أيضاً باسم مخطط Gantt.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-132">**Tasks** – Provides the details about the work breakdown structure represented by a grid view, board view, and a timeline view, or also known as a Gantt chart.</span></span>

    <span data-ttu-id="ca0b1-133">[![لقطة شاشة لعلامة تبويب مهام مشروع "تجديد المتجر وتغيير صورته".](../media/tasks-ss.png)](../media/tasks-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-133">[![Screenshot of the Store Rebrand and Refurbish project Tasks tab.](../media/tasks-ss.png)](../media/tasks-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-134">**الفريق** – يوفر تفاصيل حول المشاركين في المشروع.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-134">**Team** – Provides details about the project participants.</span></span> <span data-ttu-id="ca0b1-135">يتم أيضاً تلخيص الجهد المخصص لكل عضو في الفريق في طريقة العرض هذه.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-135">The assigned effort of each team member is also summarized in this view.</span></span>

    <span data-ttu-id="ca0b1-136">[![لقطة شاشة لعلامة تبويب فريق مشروع "تجديد المتجر وتغيير صورته".](../media/team-ss.png)](../media/team-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-136">[![Screenshot of the Store Rebrand and Refurbish project Team tab.](../media/team-ss.png)](../media/team-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-137">**تعيينات الموارد** – توفر طريقة عرض زمنية للجهد المبذول لكل مورد في المشروع.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-137">**Resource Assignments** – Provides a time-phased view of the effort for each resource on a project.</span></span>

    <span data-ttu-id="ca0b1-138">[![لقطة شاشة لعلامة تبويب مهام الموارد.](../media/resource-assignments-ss.png)](../media/resource-assignments-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-138">[![Screenshot of the Resource Assignments tab.](../media/resource-assignments-ss.png)](../media/resource-assignments-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-139">**تسوية الموارد** – توفر طريقة عرض على مراحل زمنية للاختلافات بين مهام كل مورد مسمى وعمليات الحجز الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-139">**Resource Reconciliation** – Provides a time-phased view of the differences between the assignments of each named resource and their bookings.</span></span>

    <span data-ttu-id="ca0b1-140">[![لقطة شاشة لعلامة تبويب تسوية مورد مشروع "تجديد المتجر وتغيير صورته".](../media/resource-reconciliation-ss.png)](../media/resource-reconciliation-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-140">[![Screenshot of the Store Rebrand and Refurbish project Resource Reconciliation tab.](../media/resource-reconciliation-ss.png)](../media/resource-reconciliation-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-141">**التقديرات** – توفر طريقة عرض على مراحل زمنية لتقديرات تكلفة ومبيعات مشروع ما.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-141">**Estimates** – Provides a time-phased view of the cost and sales estimates of a project.</span></span>

    <span data-ttu-id="ca0b1-142">[![لقطة شاشة لعلامة تبويب تقديرات مشروع "تجديد المتجر وتغيير صورته".](../media/estimates-ss.png)](../media/estimates-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-142">[![Screenshot of the Store Rebrand and Refurbish project Estimates tab.](../media/estimates-ss.png)](../media/estimates-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-143">**التعقب** – يوفر طريقة عرض تُظهر تقدم المهام في هيكل تنظيم العمل للجهد والتكلفة والمبيعات.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-143">**Tracking** – Provides a view that shows the progress of tasks in the work breakdown structure for effort, cost, and sales.</span></span>

    <span data-ttu-id="ca0b1-144">[![لقطة شاشة لعلامة تبويب تعقب مشروع "تجديد المتجر وتغيير صورته".](../media/tracking-ss.png)](../media/tracking-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-144">[![Screenshot of the Store Rebrand and Refurbish project Tracking tab.](../media/tracking-ss.png)](../media/tracking-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-145">**المبيعات** – توفر ارتباطات عميقة لعروض الأسعار والعقود المرتبطة بالمشروع.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-145">**Sales** – Provides deep links to quotes and contracts that are associated with the project.</span></span>

    <span data-ttu-id="ca0b1-146">[![لقطة شاشة لعلامة تبويب مبيعات مشروع "تجديد المتجر وتغيير صورته".](../media/sales-ss.png)](../media/sales-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-146">[![Screenshot of the Store Rebrand and Refurbish project Sales tab.](../media/sales-ss.png)](../media/sales-ss.png#lightbox)</span></span>

- <span data-ttu-id="ca0b1-147">**تقديرات المصروفات** – توفر شبكة تحدد مصروفات المشروع بناءً على فئات النفقات التنظيمية.</span><span class="sxs-lookup"><span data-stu-id="ca0b1-147">**Expense Estimates** – Provides a grid that defines project expenses based on organizational expense categories.</span></span>

    <span data-ttu-id="ca0b1-148">[![لقطة شاشة لعلامة تبويب مصروفات مشروع "تجديد المتجر وتغيير صورته".](../media/expense-estimates-ss.png)](../media/expense-estimates-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ca0b1-148">[![Screenshot of the Store Rebrand and Refurbish project Expense Estimates tab.](../media/expense-estimates-ss.png)](../media/expense-estimates-ss.png#lightbox)</span></span>
    
 
<span data-ttu-id="ca0b1-149">معرفة المزيد حول إدارة المشروع في الوحدة النمطية [البدء في العمل باستخدام إدارة المشروع في Dynamics 365 Project Operations](https://docs.microsoft.com/learn/modules/get-started-project-management//?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="ca0b1-149">Learn more about project management in the [Get started with project management in Dynamics 365 Project Operations](https://docs.microsoft.com/learn/modules/get-started-project-management//?azure-portal=true) module.</span></span>
