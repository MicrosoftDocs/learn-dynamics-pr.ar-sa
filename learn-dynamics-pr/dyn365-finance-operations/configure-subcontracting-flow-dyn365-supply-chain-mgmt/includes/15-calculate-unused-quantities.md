---
ms.openlocfilehash: 1f6e938b0fdff78e96afd71dee664720b0007d08
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073808"
---

<span data-ttu-id="cd8db-101">تحسب تكاليف الإصدار التلقائي الكميات غير المستخدمة من المواد التي لا تزال ضمن تدفق الإنتاج في تاريخ انتهاء الفترة.</span><span class="sxs-lookup"><span data-stu-id="cd8db-101">Backflush costing calculates the unused quantities of materials that are still in the production flow at the period end date.</span></span> <span data-ttu-id="cd8db-102">ولإنجاز هذه المهمة، يتم حساب كميات مكافئة من المواد للمنتجات غير المكتملة التي لا تزال قيد المعالجة.</span><span class="sxs-lookup"><span data-stu-id="cd8db-102">To accomplish this task, equivalent quantities of materials for non-completed products that are still in process are calculated.</span></span>

<span data-ttu-id="cd8db-103">**إدارة التكاليف > محاسبة التصنيع**</span><span class="sxs-lookup"><span data-stu-id="cd8db-103">**Cost management > manufacturing accounting**</span></span>

<span data-ttu-id="cd8db-104">يتم التعبير عن استخدام المواد المحسوبة وفقاً لتدفق الإنتاج الساري المفعول في ذلك الوقت وما إذا كان المخزون الفعلي يتم الاحتفاظ به أم لا.</span><span class="sxs-lookup"><span data-stu-id="cd8db-104">The calculated material usage is expressed in accordance with the production flow that is effective at the time and whether on-hand inventory is maintained or not.</span></span> <span data-ttu-id="cd8db-105">يتم تحويل الكميات الفرعية والمنتجات شبه النهائية التي يتم إنتاجها في تدفق الإنتاج والتي يخضع تدفقها المادي للأنشطة التي لا يتم التحكم في مخزونها بكميات مكافئة من مكوناتها.</span><span class="sxs-lookup"><span data-stu-id="cd8db-105">Subassemblies and semi-finished products that are produced in the production flow and whose physical flow is governed by activities that are not inventory controlled are converted in equivalent quantities of their components.</span></span>

<span data-ttu-id="cd8db-106">[![لقطة شاشة لصفحة حساب تكاليف الإصدار التلقائي.](../media/backflush-costing.png)](../media/backflush-costing.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="cd8db-106">[![Screenshot of the Backflush costing calculation page.](../media/backflush-costing.png)](../media/backflush-costing.png#lightbox)</span></span>


<span data-ttu-id="cd8db-107">على سبيل المثال، إذا تم إنتاج المنتج L0002 في تدفق إنتاج، ولكن الأنشطة التي تحكم تدفقه المادي لا يتم التحكم فيها من قِبل المخزون، ثم كان هناك حاجة إلى 20 وحدة من L0002 ويتم تحويلها في وحدات مكافئة من مكوناته.</span><span class="sxs-lookup"><span data-stu-id="cd8db-107">For instance, if product L0002 is produced in a production flow, but activities that govern its physical flow are not inventory controlled, then 20 units of L0002 are needed and are converted in equivalent units of its components.</span></span> <span data-ttu-id="cd8db-108">و هذا النهج هو توفير قائمة بوحدات مكافئة من المنتجات التي يمكن أن تتطابق مع مساهمات كمية المنتج المسجلة في عمل تدفق الإنتاج الجاري ومقارنتها.</span><span class="sxs-lookup"><span data-stu-id="cd8db-108">This approach is to provide a list of equivalent units of products that can match and compare with the product quantity contributions that are recorded in the production flow work in progress.</span></span>

### <a name="released-to-production"></a><span data-ttu-id="cd8db-109">الإصدار إلى الإنتاج</span><span class="sxs-lookup"><span data-stu-id="cd8db-109">Released to production</span></span>

<span data-ttu-id="cd8db-110">بشكل أساسي، تتم معاملة الأصناف غير المتحكم فيها بالمخزون على أنها أصناف وهمية.</span><span class="sxs-lookup"><span data-stu-id="cd8db-110">Essentially, the non-inventory-controlled items are treated as phantoms.</span></span>
<span data-ttu-id="cd8db-111">ويتم تصحيح الكميات المكافئة المحتسبة من المواد وفقاً لما إذا كان قد تم إصدار كميات المكونات إلى الإنتاج أم لا.</span><span class="sxs-lookup"><span data-stu-id="cd8db-111">The calculated equivalent quantities of materials are corrected according to whether the quantities of components have been released to production.</span></span>

<span data-ttu-id="cd8db-112">على سبيل المثال، إذا لم يتم تحرير مكون من المخزون إلى تدفق الإنتاج بشكل فعال، فلا ينبغي اعتبار مكوناته كميات غير مستخدمة متبقية (لأنها لا تزال قيد الجرد وليست في الأعمال تحت التنفيذ الخاصة بتدفق الإنتاج).</span><span class="sxs-lookup"><span data-stu-id="cd8db-112">For example, if a component has not yet been effectively released from inventory to the production flow, then its components should not be considered as remaining unused quantities (because they're still in inventory and not in the production flow's WIP).</span></span>

<span data-ttu-id="cd8db-113">يؤدي التحديث المالي لحركات المخزون للكميات المكتملة إلى عكس ترحيلات دفتر الأستاذ الفعلي وإعادة ترحيلها على أنها محدثة مالياً.</span><span class="sxs-lookup"><span data-stu-id="cd8db-113">The financial updating of inventory transactions for completed quantities reverses the physical ledger postings and reposts them as financially updated.</span></span>
<span data-ttu-id="cd8db-114">يتم تحديث حالة استلام حركات المخزون إلى **‏‫تم الشراء‬**.</span><span class="sxs-lookup"><span data-stu-id="cd8db-114">The inventory transactions' receipt status is updated to **Purchased**.</span></span>

<span data-ttu-id="cd8db-115">يعكس التحديث المالي لحركات المخزون للمنتجات المستهلكة ترحيلات دفتر الأستاذ الفعلية وإعادة ترحيلها على أنها محدثة مالياً، ثم يتم تحديث حالة استلام حركات المخزون إلى **مُباع**.</span><span class="sxs-lookup"><span data-stu-id="cd8db-115">The financial updating of inventory transactions for consumed products reverses the physical ledger postings and reposts them as financially updated, and then the inventory transactions' receipt status is updated to **Sold**.</span></span>

<span data-ttu-id="cd8db-116">يؤدي إلغاء الأعمال تحت التنفيذ لتكاليف تحويل التصنيع المباشرة لتدفق الإنتاج إلى عكس ترحيلات دفتر الأستاذ الفعلية وإعادة ترحيلها على أنها محدثة مالياً.</span><span class="sxs-lookup"><span data-stu-id="cd8db-116">Clearing WIP for the production flow's direct manufacturing conversion costs reverses the physical ledger postings and reposts them as financially updated.</span></span> <span data-ttu-id="cd8db-117">يتم تحديث حركة تكلفة التحويل إلى **تكلفة محسوبة**.</span><span class="sxs-lookup"><span data-stu-id="cd8db-117">The conversion cost transaction is updated to **Cost accounted**.</span></span>

<span data-ttu-id="cd8db-118">يتم إلغاء تكاليف التصنيع غير المباشرة، والتي يتم تكديسها عبر الفترة من الأعمال تحت التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="cd8db-118">The indirect manufacturing costs, which are accumulated over the period, are all cleared from WIP.</span></span> <span data-ttu-id="cd8db-119">وسيتعين إعادة التكلفة غير المباشرة للمواد غير المستخدمة.</span><span class="sxs-lookup"><span data-stu-id="cd8db-119">The indirect cost for unused materials will need to be reinstated.</span></span>

<span data-ttu-id="cd8db-120">لإعادة تعيين تكاليف التصنيع غير المباشرة للكميات غير المستخدمة التي لا تزال قيد التنفيذ في أعمال تدفق الإنتاج التي تم مسحها من الأعمال تحت التنفيذ:</span><span class="sxs-lookup"><span data-stu-id="cd8db-120">To reset the indirect manufacturing costs for the unused quantities that are still in production flow work in progress that had been cleared from WIP:</span></span>

-   <span data-ttu-id="cd8db-121">حساب التكلفة غير المباشرة للكميات غير المستخدمة المُبلغ عنها في تدفق الإنتاج في نهاية الفترة استناداً إلى إعداد كشف التكاليف.</span><span class="sxs-lookup"><span data-stu-id="cd8db-121">Compute the indirect cost for reported unused quantities in the production flow at the period end based on the cost sheet setup.</span></span>

-   <span data-ttu-id="cd8db-122">إدراج حركة تكلفة تحويل جديدة (من نوع التكلفة غير المباشرة) في المرحلة المحدثة فعلياً للتكلفة غير المباشرة المحسوبة.</span><span class="sxs-lookup"><span data-stu-id="cd8db-122">Insert a new conversion cost transaction (of type indirect cost) in the physically updated stage for the calculated indirect cost.</span></span>

-   <span data-ttu-id="cd8db-123">إدراج حركة تكلفة تحويل سالبة جديدة (من نوع التكلفة غير المباشرة) للتكلفة غير المباشرة المحسوبة في المرحلة المحدثة مالياً.</span><span class="sxs-lookup"><span data-stu-id="cd8db-123">Insert a new negative conversion cost transaction (of type indirect cost) for the calculated indirect cost in the financially updated stage.</span></span>
