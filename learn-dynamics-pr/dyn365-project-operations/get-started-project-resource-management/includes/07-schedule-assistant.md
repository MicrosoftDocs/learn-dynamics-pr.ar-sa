---
ms.openlocfilehash: 97afe8bed7cb3bf7bdfb6fa63ff217b96cd513d2
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072900"
---
<span data-ttu-id="4cc06-101">يمكنك استخدام مساعد الجدولة لحجز الموارد استناداً إلى المتطلبات التي حددها مدير المشروع.</span><span class="sxs-lookup"><span data-stu-id="4cc06-101">You can use the Schedule assistant to book resources based on requirements that are defined by the project manager.</span></span> <span data-ttu-id="4cc06-102">يعتمد مساعد الجدولة على المعلمات التي يتم توفيرها في متطلبات المَورد للعثور على المَورد.</span><span class="sxs-lookup"><span data-stu-id="4cc06-102">The Schedule assistant relies on the parameters that are provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="4cc06-103">إضافة إلى ذلك، يوصي مساعد الجدولة بالموارد التي تطابق المتطلبات ذات الصلة، مثل الإطارات الزمنية أو المهارات المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="4cc06-103">Additionally, the Schedule assistant recommends resources that match relevant requirements, such as time windows or needed skills.</span></span> <span data-ttu-id="4cc06-104">بعد تحديد الموارد المناسبة، يمكن لمدير المشروع أو المَوارد حجز المَورد للعمل.</span><span class="sxs-lookup"><span data-stu-id="4cc06-104">After suitable resources are identified, the resource or project manager can book the resource for the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cc06-105">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="4cc06-105">Prerequisites</span></span>
<span data-ttu-id="4cc06-106">يعد مساعد الجدولة جزءاً من الحل Universal Resource Scheduling.</span><span class="sxs-lookup"><span data-stu-id="4cc06-106">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="4cc06-107">يتم تضمين هذا الحل وتثبيته مع Project Operations وField Service وDynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="4cc06-107">This solution is included and installed with Project Operations, Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="match-requirements-and-resources"></a><span data-ttu-id="4cc06-108">مطابقة المتطلبات والموارد</span><span class="sxs-lookup"><span data-stu-id="4cc06-108">Match requirements and resources</span></span>
<span data-ttu-id="4cc06-109">يعتمد متطلب الموارد الذي تم إنشاؤه على تفاصيل مثل:</span><span class="sxs-lookup"><span data-stu-id="4cc06-109">A generated resource requirement is based on details such as:</span></span>

- <span data-ttu-id="4cc06-110">الخصائص</span><span class="sxs-lookup"><span data-stu-id="4cc06-110">Characteristics</span></span>
- <span data-ttu-id="4cc06-111">الأدوار</span><span class="sxs-lookup"><span data-stu-id="4cc06-111">Roles</span></span>
- <span data-ttu-id="4cc06-112">وحدات العمل</span><span class="sxs-lookup"><span data-stu-id="4cc06-112">Business units</span></span>
- <span data-ttu-id="4cc06-113">تفضيلات الموارد</span><span class="sxs-lookup"><span data-stu-id="4cc06-113">Resource preferences</span></span>
- <span data-ttu-id="4cc06-114">مخططات الجهد</span><span class="sxs-lookup"><span data-stu-id="4cc06-114">Effort contours</span></span>
- <span data-ttu-id="4cc06-115">المنطقة الزمنية</span><span class="sxs-lookup"><span data-stu-id="4cc06-115">Time zone</span></span>

<span data-ttu-id="4cc06-116">يستخدم مساعد الجدولة هذه التفاصيل لتصفية الموارد.</span><span class="sxs-lookup"><span data-stu-id="4cc06-116">The schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="4cc06-117">بدء تشغيل Schedule assistant</span><span class="sxs-lookup"><span data-stu-id="4cc06-117">Launch the Schedule assistant</span></span>

<span data-ttu-id="4cc06-118">توجد طريقتان لبدء تشغيل مساعد الجدولة وهما:</span><span class="sxs-lookup"><span data-stu-id="4cc06-118">Two ways to launch the Schedule assistant are:</span></span> 

- <span data-ttu-id="4cc06-119">إذا كنت تستخدم وضع "مختلط"، في شبكة أعضاء الفريق، يمكنك تحديد أي عضو فريق بمتطلب موارد غير مكتمل، ثم تحديد **حجز**.</span><span class="sxs-lookup"><span data-stu-id="4cc06-119">If you're using Hybrid mode, in the team member grid, you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> 

- <span data-ttu-id="4cc06-120">إذا كنت تستخدم وضع "مركزي"، فسيعثر مدير الموارد على المورد ويحدده.</span><span class="sxs-lookup"><span data-stu-id="4cc06-120">If you're using Central mode, the resource manager will find and select the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="4cc06-121">عوامل تصفية Schedule assistant</span><span class="sxs-lookup"><span data-stu-id="4cc06-121">Schedule assistant filters</span></span>
<span data-ttu-id="4cc06-122">بعد تشغيل Schedule assistant، يتم عرض تفاصيل من متطلب الموارد كقيم مصفاة في الجزء الأيسر.</span><span class="sxs-lookup"><span data-stu-id="4cc06-122">After the Schedule assistant runs, details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="4cc06-123">يمكن لمدير الموارد أو مدير المشروع ضبط النتائج بشكلٍ دقيق عن طريق ضبط عوامل التصفية لتلبية احتياجات الجدولة.</span><span class="sxs-lookup"><span data-stu-id="4cc06-123">The resource manager or the project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="4cc06-124">جزء **التصفية** يوضح الخيارات المتعلقة بالعمل، بما في ذلك:</span><span class="sxs-lookup"><span data-stu-id="4cc06-124">The **Filter** pane shows work-related options, including:</span></span>

- <span data-ttu-id="4cc06-125">بداية العمل وانتهائه</span><span class="sxs-lookup"><span data-stu-id="4cc06-125">Work start and end</span></span>
- <span data-ttu-id="4cc06-126">الخصائص</span><span class="sxs-lookup"><span data-stu-id="4cc06-126">Characteristics</span></span>
- <span data-ttu-id="4cc06-127">الأدوار</span><span class="sxs-lookup"><span data-stu-id="4cc06-127">Roles</span></span>
- <span data-ttu-id="4cc06-128">الوحدات التنظيمية</span><span class="sxs-lookup"><span data-stu-id="4cc06-128">Organizational units</span></span>
- <span data-ttu-id="4cc06-129">شركة التوريد</span><span class="sxs-lookup"><span data-stu-id="4cc06-129">Resourcing company</span></span>
- <span data-ttu-id="4cc06-130">أنواع الموارد</span><span class="sxs-lookup"><span data-stu-id="4cc06-130">Resource types</span></span>
- <span data-ttu-id="4cc06-131">الموارد المفضلة</span><span class="sxs-lookup"><span data-stu-id="4cc06-131">Preferred resources</span></span>


