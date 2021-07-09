---
ms.openlocfilehash: a4b0f0a6c7e39d65eca6fb51ef24235d275d5931
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073059"
---

<span data-ttu-id="a4a33-101">تتيح لك Supply Chain Management جدولة بطاقات كانبان على موارد بديلة.</span><span class="sxs-lookup"><span data-stu-id="a4a33-101">Supply Chain Management allows you to schedule kanbans on alternate resources.</span></span> <span data-ttu-id="a4a33-102">تسمح هذه الوظيفة لمدير تدفق القيم باستخدام موارد بديلة لموازنة عبء العمل عبر المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="a4a33-102">This functionality allows the value stream manager to use alternate resources to balance the workload throughout the organization.</span></span> 

<span data-ttu-id="a4a33-103">لتحسين الإنتاجية في أي عملية، تحتوي لوحة **التحكم بالإنتاج > كانبان‬ > جدولة وظيفة كانبان‬** على وظيفة تسمى **‎استخدام قاعدة كانبان بديلة**.</span><span class="sxs-lookup"><span data-stu-id="a4a33-103">To optimize the throughput in any process, the **Production control > Kanban > Kanban job scheduling** board has a function called **Use alternative kanban rule**.</span></span> <span data-ttu-id="a4a33-104">تسمح هذه الوظيفة للمخطط بإعادة جدولة كانبان الذي تم إنشاؤه في الأصل لخلية عمل واحدة إلى خلية عمل بديلة.</span><span class="sxs-lookup"><span data-stu-id="a4a33-104">This function allows the planner to reschedule a kanban that was originally created for one work cell to an alternative work cell.</span></span> <span data-ttu-id="a4a33-105">قد تكون هذه الخلية عبارة عن مورد داخلي بديل أو مورد تعاقد من الباطن؛ وتكون العملية الخاصة بالمخطط هي نفسها لكليهما.</span><span class="sxs-lookup"><span data-stu-id="a4a33-105">This cell could be an alternate in-house resource or a subcontracting resource; the process for the planner is the same for both.</span></span>

<span data-ttu-id="a4a33-106">يمكن للمخطط تعيين قاعدة كانبان بديلة لوظيفة كانبان مباشرة من لوحة جدولة كانبان.</span><span class="sxs-lookup"><span data-stu-id="a4a33-106">The planner can assign an alternate kanban rule to the kanban job straight from the Kanban schedule board.</span></span> <span data-ttu-id="a4a33-107">يتم إكمال هذه المهمة بتحديد وظيفة كانبان ثم تحديد الزر **استخدام قاعدة كانبان البديلة**.</span><span class="sxs-lookup"><span data-stu-id="a4a33-107">This task is completed by selecting the kanban job and then selecting the **Use alternative kanban rule** button.</span></span>

## <a name="open-kanban"></a><span data-ttu-id="a4a33-108">فتح الكانبان</span><span class="sxs-lookup"><span data-stu-id="a4a33-108">Open kanban</span></span>

<span data-ttu-id="a4a33-109">يمكن للمخطط الانتقال إلى **التحكم في الإنتاج > كانبان > لوحة جدول كانبان** والنقر بزر الماوس الأيمن فوق كانبان، ثم تحديد **فتح الكانبان** لتغيير قاعدة كانبان.</span><span class="sxs-lookup"><span data-stu-id="a4a33-109">The planner can go to **Production control > Kanban > Kanban schedule board**, right-click the kanban, and then select **Open kanban** to change the kanban rule.</span></span>

<span data-ttu-id="a4a33-110">يمكن بعد ذلك استخدام الزر **الخطة > استخدام قاعدة كانبان البديلة** لتعيين قاعدة كانبان بديلة لوظيفة كانبان.</span><span class="sxs-lookup"><span data-stu-id="a4a33-110">The **Plan > Use alternative kanban rule** button can then be used to assign an alternate kanban rule to the kanban job.</span></span>


## <a name="alternate-kanban-functionality"></a><span data-ttu-id="a4a33-111">وظيفة كانبان البديلة</span><span class="sxs-lookup"><span data-stu-id="a4a33-111">Alternate kanban functionality</span></span>

<span data-ttu-id="a4a33-112">لاستخدام وظيفة كانبان البديلة، يجب استيفاء بعض المتطلبات الأساسية في قواعد كانبان.</span><span class="sxs-lookup"><span data-stu-id="a4a33-112">To use the alternate kanban functionality, certain prerequisites must be met in the kanban rules.</span></span>

-   <span data-ttu-id="a4a33-113">تعمل قواعد كانبان البديلة فقط مع وظائف كانبان المجدولة أو كانبان الأحداث، وليس مع كانبان الكمية الثابتة.</span><span class="sxs-lookup"><span data-stu-id="a4a33-113">Alternate kanban rules only work with scheduled or event kanbans, not with fixed quantity kanbans.</span></span>

-   <span data-ttu-id="a4a33-114">يجب أن تحتوي قواعد كانبان البديلة على وظائف مماثلة:</span><span class="sxs-lookup"><span data-stu-id="a4a33-114">Alternate kanban rules must have similar functions:</span></span>

    -   <span data-ttu-id="a4a33-115">تحديد المنتج</span><span class="sxs-lookup"><span data-stu-id="a4a33-115">Product selection</span></span>

    -   <span data-ttu-id="a4a33-116">استراتيجية التجديد (مجدول أو حدث)</span><span class="sxs-lookup"><span data-stu-id="a4a33-116">Replenishment strategy (scheduled or event)</span></span>

    -   <span data-ttu-id="a4a33-117">الموقع المجهز (الموقع، المستودع، الموقع)</span><span class="sxs-lookup"><span data-stu-id="a4a33-117">Supplied location (site, warehouse, location)</span></span>

    -   <span data-ttu-id="a4a33-118">نوع الحدث (المبيعات، قائمة مكونات الصنف، كانبان، الحد الأدنى للمخزون)</span><span class="sxs-lookup"><span data-stu-id="a4a33-118">Type of event (sales, BOM, kanban, minimum stock)</span></span>

-   <span data-ttu-id="a4a33-119">يمكن تغيير قاعدة كانبان في كانبان إلى قاعدة كانبان بديلة في المواقف التالية:</span><span class="sxs-lookup"><span data-stu-id="a4a33-119">The kanban rule of a kanban can be changed to an alternative kanban rule in the following situations:</span></span>

    -   <span data-ttu-id="a4a33-120">تشتمل كانبان على حالة وحدة معالجة المواد غير معينة</span><span class="sxs-lookup"><span data-stu-id="a4a33-120">The kanban has a handling unit status of Not assigned</span></span>

    -   <span data-ttu-id="a4a33-121">لا يتم تخطيط وظائف كانبان</span><span class="sxs-lookup"><span data-stu-id="a4a33-121">The kanban jobs are not planned</span></span>

    -   <span data-ttu-id="a4a33-122">تكون حالة تزويد كانبان "مجدول" أو "حدث"</span><span class="sxs-lookup"><span data-stu-id="a4a33-122">The kanban has a replenishment status of Scheduled or Event</span></span>

-   <span data-ttu-id="a4a33-123">عند تغيير قاعدة كانبان، سيقوم التحويل بإجراء المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="a4a33-123">When you change a kanban rule, the conversion will perform the following tasks:</span></span>

    -   <span data-ttu-id="a4a33-124">حذف وظائف كانبان القديمة ووظائف كانبان</span><span class="sxs-lookup"><span data-stu-id="a4a33-124">Delete old kanban jobs and kanbans</span></span>

    -   <span data-ttu-id="a4a33-125">إنشاء وظائف كانبان جديدة ووظائف كانبان</span><span class="sxs-lookup"><span data-stu-id="a4a33-125">Create new kanban jobs and kanbans</span></span>

    -   <span data-ttu-id="a4a33-126">الحفاظ على كمية كانبان وتاريخ الاستحقاق</span><span class="sxs-lookup"><span data-stu-id="a4a33-126">Preserve the kanban quantity and due date</span></span>

    -   <span data-ttu-id="a4a33-127">تحويل تثبيت سعر الحدث إلى كانبان الجديد للأحداث</span><span class="sxs-lookup"><span data-stu-id="a4a33-127">Transfer the event pegging to the new kanban for events</span></span>
