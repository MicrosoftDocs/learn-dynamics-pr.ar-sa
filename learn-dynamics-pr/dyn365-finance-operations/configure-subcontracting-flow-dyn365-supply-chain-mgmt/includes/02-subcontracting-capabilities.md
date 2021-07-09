---
ms.openlocfilehash: 00cd9e2d56a3ce80994349163315632470c51bc3
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073214"
---
<span data-ttu-id="0581d-101">يفصل التعاقد من الباطن من أجل lean manufacturing في Supply Chain Management تدفق المواد عن عملية شراء الخدمات.</span><span class="sxs-lookup"><span data-stu-id="0581d-101">Subcontracting for lean manufacturing in Supply Chain Management separates the material flow from the purchase process of the services.</span></span> <span data-ttu-id="0581d-102">يتم إنشاء أمر الشراء تلقائياً عند تحديث حالة كانبان إلى **مخطط‬**.</span><span class="sxs-lookup"><span data-stu-id="0581d-102">The purchase order is created automatically when the kanban status is updated to at least **Planned**.</span></span>

<span data-ttu-id="0581d-103">تُستخدم أصناف الخدمة هذه في أوامر الشراء لتمثيل النشاط الذي سيقوم به المورد كجزء من العملية الخارجية.</span><span class="sxs-lookup"><span data-stu-id="0581d-103">These service items are used on purchase orders to represent the activity that the vendor will conduct as part of the outside process.</span></span> <span data-ttu-id="0581d-104">يحتوي أمر الشراء على التكلفة والنتائج في فاتورة الحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="0581d-104">The purchase order contains the cost and results in an accounts payable billing.</span></span> <span data-ttu-id="0581d-105">عندما يبلغ المورد عن اكتمال العمل، يتم ترحيل إيصال أمر الشراء للخدمات.</span><span class="sxs-lookup"><span data-stu-id="0581d-105">When the vendor reports that the work is complete, the purchase order receipt is posted for the services.</span></span> <span data-ttu-id="0581d-106">عند استلام المنتجات ذات الصلة، يتم تحديث حالة كانبان إلى **مكتمل** ويتم استلام الصنف المنتهي في المخزون.</span><span class="sxs-lookup"><span data-stu-id="0581d-106">When the related products are received, the kanban state is updated to **Completed** and the finished item is received into inventory.</span></span>

<span data-ttu-id="0581d-107">نوصي بتنفيذ الإجراءات التالية عند التفاوض على التعاقد من الباطن لنشاط مع أحد الموردين:</span><span class="sxs-lookup"><span data-stu-id="0581d-107">We recommend that you perform the following actions when subcontracting for an activity has been negotiated with a vendor:</span></span>

-   <span data-ttu-id="0581d-108">إنشاء صنف الخدمة الذي يعد أحد أنواع المنتجات.</span><span class="sxs-lookup"><span data-stu-id="0581d-108">Create the service item that is a type of product.</span></span>

-   <span data-ttu-id="0581d-109">إنشاء اتفاقية الشراء وبند الاتفاقية للمورد باستخدام صنف الخدمة.</span><span class="sxs-lookup"><span data-stu-id="0581d-109">Create the purchase agreement and agreement line for the vendor by using the service item.</span></span>

-   <span data-ttu-id="0581d-110">إنشاء مجموعة موارد بدور خلية عمل خاصة بالمقاول من الباطن التي توفر الخدمة.</span><span class="sxs-lookup"><span data-stu-id="0581d-110">Create a resource group with the role of a work cell for the subcontractor that provides the service.</span></span>

-   <span data-ttu-id="0581d-111">إنشاء إصدار جديد من تدفق الإنتاج (أو تدفق إنتاج جديد).</span><span class="sxs-lookup"><span data-stu-id="0581d-111">Create a new version of a production flow (or a new production flow).</span></span>

-   <span data-ttu-id="0581d-112">إنشاء نشاط تدفق إنتاج جديد وربط الاتفاقية بالنشاط.</span><span class="sxs-lookup"><span data-stu-id="0581d-112">Create a new production flow activity and relate the agreement to the activity.</span></span>

-   <span data-ttu-id="0581d-113">توصيل النشاط المتعاقد عليه من الباطن بالأنشطة الأخرى لتدفق الإنتاج إن أمكن.</span><span class="sxs-lookup"><span data-stu-id="0581d-113">Connect the subcontracted activity to the other activities of the production flow if applicable.</span></span>

-   <span data-ttu-id="0581d-114">التحقق من صحة التدفق وتنشيطه.</span><span class="sxs-lookup"><span data-stu-id="0581d-114">Validate and activate the flow.</span></span>

<span data-ttu-id="0581d-115">شاهد الفيديو التالي لمعرفة كيفية الاستعداد للتعاقد من الباطن المستند إلى النشاط في Supply Chain Management:</span><span class="sxs-lookup"><span data-stu-id="0581d-115">Watch the following video to see how to prepare for activity-based subcontracting in Supply Chain Management:</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE487o7]


## <a name="production-flow-with-subcontracting-activities"></a><span data-ttu-id="0581d-116">تدفق الإنتاج مع الأنشطة الخاصة بالتعاقد من الباطن</span><span class="sxs-lookup"><span data-stu-id="0581d-116">Production flow with subcontracting activities</span></span>

<span data-ttu-id="0581d-117">لا يتغير المبدأ الأساسي لتدفق الإنتاج عندما يتم التعاقد من الباطن على الأنشطة.</span><span class="sxs-lookup"><span data-stu-id="0581d-117">The basic principle of a production flow does not change when activities are subcontracted.</span></span> <span data-ttu-id="0581d-118">لا تزال المواد تتدفق بين المواقع، وتقوم أنشطة العملية بتحويل المواد إلى منتجات، وتنقل أنشطة النقل المواد أو المنتجات من موقع إلى آخر.</span><span class="sxs-lookup"><span data-stu-id="0581d-118">Material still flows between locations, process activities convert material to products, and transfer activities move material or products from one location to another.</span></span> <span data-ttu-id="0581d-119">يمكن تكوين أنشطة النقل والعملية كأنشطة تعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="0581d-119">Both process and transfer activities can be configured as subcontracting activities.</span></span>

<span data-ttu-id="0581d-120">وكما هو الحال في أي نشاط آخر في تدفق الإنتاج، يمكن للأنشطة المتعاقد عليها من الباطن أن تستهلك وتورد مواد ومنتجات مخزنة وغير مخزنة (WIP) وشبه منتهية.</span><span class="sxs-lookup"><span data-stu-id="0581d-120">As any other activity in a production flow, subcontracted activities can consume and supply inventoried, non-inventoried (WIP), and semi-finished material and products.</span></span> <span data-ttu-id="0581d-121">عمليات جدولة الأنشطة المتعاقد عليها من الباطن وتنفيذها هي نفسها في جميع الحالات وهي مماثلة للعمليات التي تم إكمالها للعمل الداخلي.</span><span class="sxs-lookup"><span data-stu-id="0581d-121">The processes to schedule and implement subcontracted activities are the same in all cases and are identical to the processes that are completed for internal work.</span></span>

<span data-ttu-id="0581d-122">تحدد Supply Chain Management خلية عمل أو مستودعاً كنوع المورد عندما تقوم بإنشاء أنشطة ضمن تدفقات الإنتاج؛ بالإضافة إلى ذلك، يقوم تلقائياً بتعبئة هذه المعلومات في معالج النشاط.</span><span class="sxs-lookup"><span data-stu-id="0581d-122">Supply Chain Management identifies a work cell or warehouse as a vendor type when you create activities within production flows; additionally, it automatically populates this information into the activity wizard.</span></span>
