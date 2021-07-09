---
ms.openlocfilehash: c51b2488e397a7677b6287bca9a9a8399fb31cd6
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073027"
---
<span data-ttu-id="6e790-101">عادةً ما يكون سيناريو lean manufacturing أكثر من مجرد تراكم لقواعد كانبان أو سياسات توريد المواد غير المرتبطة.</span><span class="sxs-lookup"><span data-stu-id="6e790-101">A lean manufacturing scenario is usually more than an accumulation of unrelated kanban rules or material-supply policies.</span></span> <span data-ttu-id="6e790-102">يمكن وصف تدفق المواد والمنتجات في جميع أنحاء خلايا العمل والمواقع لسيناريو إنتاج أو توريد معين على أنه تسلسل أو شبكة صغيرة من أنشطة المعالجة أو التحويل تسمى تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="6e790-102">The flow of material and products throughout work cells and locations for a specific production or supply scenario can be described as a sequence or small network of process or transfer activities called a production flow.</span></span> 

<span data-ttu-id="6e790-103">تهدف تدفقات الإنتاج المستندة إلى النشاط في Dynamics 365 Supply Chain Management إلى إنشاء سياق الإنتاج والتكلفة لسيناريوهات كانبان المختلفة.</span><span class="sxs-lookup"><span data-stu-id="6e790-103">The activity-based production flows in Dynamics 365 Supply Chain Management are to establish a production and cost context for various kanban scenarios.</span></span> <span data-ttu-id="6e790-104">ترتبط جميع قواعد كانبان مباشرةً بهذه البنية المحددة مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="6e790-104">All kanban rules are directly connected to this pre-defined structure.</span></span>

<span data-ttu-id="6e790-105">يسمح النموذج المستند إلى النشاط للمستخدمين بإعداد مجموعة واسعة من السيناريوهات.</span><span class="sxs-lookup"><span data-stu-id="6e790-105">The activity-based model allows users to set up a wide range of scenarios.</span></span> <span data-ttu-id="6e790-106">أيضاً، يأتي النموذج المستند إلى النشاط بدون التعقيد الإضافي لعاملي ورشة العمل لأن جميع السيناريوهات تستخدم نفس واجهة المستخدم القائمة على النشاط.</span><span class="sxs-lookup"><span data-stu-id="6e790-106">Also, the activity-based model comes without the added complexity for the shop floor workers because all scenarios use the same activity-based user interface.</span></span>

## <a name="work-cell"></a><span data-ttu-id="6e790-107">خلية العمل</span><span class="sxs-lookup"><span data-stu-id="6e790-107">Work cell</span></span>

<span data-ttu-id="6e790-108">خلية العمل هي نوع من مجموعات الموارد التي يمكن استخدامها في أنشطة عملية lean manufacturing.</span><span class="sxs-lookup"><span data-stu-id="6e790-108">A work cell is a type of resource group that can be used in lean manufacturing process activities.</span></span> <span data-ttu-id="6e790-109">تحتوي خلايا العمل على مواقع الإدخال والإخراج وتعريف القدرة الإنتاجية بناءً على نموذج تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="6e790-109">Work cells have input and output locations and a capacity definition based on a production flow model.</span></span>

## <a name="semi-finished-products"></a><span data-ttu-id="6e790-110">المنتجات شبه المنتهية</span><span class="sxs-lookup"><span data-stu-id="6e790-110">Semi-finished products</span></span>

<span data-ttu-id="6e790-111">في التصنيع التقليدي ضمن Supply Chain Management، تسمح أوامر الإنتاج للمستخدمين بالإبلاغ عن الوظائف على مستوى العملية.</span><span class="sxs-lookup"><span data-stu-id="6e790-111">In traditional manufacturing within Supply Chain Management, production orders allow users to report jobs on an operation level.</span></span> <span data-ttu-id="6e790-112">مع كل عملية نهائية، يصل المنتج إلى حالة مختلفة من المنتج شبه المنتهي.</span><span class="sxs-lookup"><span data-stu-id="6e790-112">With each finished operation, the product reaches a different state of semi-finished product.</span></span> <span data-ttu-id="6e790-113">ومع ذلك، لا يتم تسجيل هذه الحالة في المخزون ما لم يتم إكمال العملية الأخيرة لأمر الإنتاج والوصول إلى مستوى قائمة مكونات الصنف التالي.</span><span class="sxs-lookup"><span data-stu-id="6e790-113">However, this status is not registered in inventory unless the last operation of a production order has been completed and the next BOM level is reached.</span></span>

<span data-ttu-id="6e790-114">عادةً ما يتم تحديد المنتجات شبه المنتهية التي لا تمثل مستوى قائمة مكونات الصنف من خلال معرف المنتج لمستوى قائمة المواد التالي وآخر عملية مكتملة.</span><span class="sxs-lookup"><span data-stu-id="6e790-114">Semi-finished products that do not represent a BOM level are usually identified by the product ID of the next BOM level and the last completed operation.</span></span>
<span data-ttu-id="6e790-115">لا يمكن أن يكون النشاط الذي يستهلك منتجات شبه منتهية هو النشاط الأول في تدفق إنتاج.</span><span class="sxs-lookup"><span data-stu-id="6e790-115">An activity that consumes semi-finished products cannot be the first activity in a production flow.</span></span>

<span data-ttu-id="6e790-116">باستخدام lean manufacturing لـ Supply Chain Management، يمكن تطبيق هذا المفهوم على الإنتاج باستخدام بطاقات كانبان التصنيع من خلال أنشطة تدفق الإنتاج الأساسية.</span><span class="sxs-lookup"><span data-stu-id="6e790-116">With lean manufacturing for Supply Chain Management, this concept can be applied to production with manufacturing kanbans through the underlying production flow activities.</span></span>

<span data-ttu-id="6e790-117">الخيارات شبه المنتهية هي:</span><span class="sxs-lookup"><span data-stu-id="6e790-117">The semi-finished options are:</span></span>

- <span data-ttu-id="6e790-118">**تحديث استلام المخزون الفعلي** - تحديد ما إذا كان النشاط ينتج منتجات نهائية (مستوى قائمة مكونات الصنف) وإيصال استلام المنتج مسجلاً في المخزون.</span><span class="sxs-lookup"><span data-stu-id="6e790-118">**Update on hand receipt** - Select if the activity outputs products that are finished products (BOM level) and the product receipt is registered in inventory.</span></span> 


    - <span data-ttu-id="6e790-119">عند استخدام المحددة **تحديث استلام المخزون الفعلي**، يتم نقل قيمة المنتج النهائي خارج تدفق الإنتاج بالتكلفة القياسية.</span><span class="sxs-lookup"><span data-stu-id="6e790-119">When you use the **Update on hand receipt** parameter, the value of the finished product is moved out of the production flow at standard cost.</span></span>


    - <span data-ttu-id="6e790-120">عند مسح خانة الاختيار، تظل قيمة المنتج المستلم في WIP لتدفق الإنتاج ذي الصلة.</span><span class="sxs-lookup"><span data-stu-id="6e790-120">When you clear the check box, the value of the received product remains in the WIP of the related production flow.</span></span> <span data-ttu-id="6e790-121">يتم نقل القيمة خارج WIP عندما يتم نقل البضائع أو استهلاكها بواسطة النشاط التالي في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="6e790-121">The value is moved out of WIP when the goods are transferred or consumed by the succeeding activity in the production flow.</span></span>



- <span data-ttu-id="6e790-122">**انتقاء** - تحديد ما إذا كان النشاط يستهلك منتجات شبه منتهية.</span><span class="sxs-lookup"><span data-stu-id="6e790-122">**Pick up** - Select if the activity consumes semi-finished products.</span></span> <span data-ttu-id="6e790-123">المنتج شبه المنتهي هو أي حالة وسيطة لمنتج يقع بين مستويين من قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="6e790-123">A semi-finished product is any intermediate state of a product that is between two BOM levels.</span></span>



- <span data-ttu-id="6e790-124">**استلام** - تحديد ما إذا كان النشاط ينتج منتجات شبه منتهية.</span><span class="sxs-lookup"><span data-stu-id="6e790-124">**Receive** - Select if the activity outputs semi-finished products.</span></span> <span data-ttu-id="6e790-125">يمكنك فقط تحديد خانة الاختيار هذه إذا لم يتم تحديد خانة الاختيار **تحديث استلام المخزون الفعلي**.</span><span class="sxs-lookup"><span data-stu-id="6e790-125">You can only select this check box if the **Update on hand receipt** check box is not selected.</span></span> 
