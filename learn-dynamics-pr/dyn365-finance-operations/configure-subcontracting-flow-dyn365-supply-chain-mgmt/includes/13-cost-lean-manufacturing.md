---
ms.openlocfilehash: 39ca210e9e55d0983f7fa275660484cdea459f75
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073053"
---

<span data-ttu-id="268ed-101">تتكون تكاليف lean manufacturing من الأنواع التالية من التكاليف:</span><span class="sxs-lookup"><span data-stu-id="268ed-101">Costing for lean manufacturing consists of the following types of costs:</span></span>

-   <span data-ttu-id="268ed-102">غير محدد</span><span class="sxs-lookup"><span data-stu-id="268ed-102">Undefined</span></span> 
-   <span data-ttu-id="268ed-103">مواد مباشرة</span><span class="sxs-lookup"><span data-stu-id="268ed-103">Direct materials</span></span> 
-   <span data-ttu-id="268ed-104">تصنيع مباشر (تسمي أيضاً تكاليف العمالة)</span><span class="sxs-lookup"><span data-stu-id="268ed-104">Direct manufacturing  (also called labor costs)</span></span>
-   <span data-ttu-id="268ed-105">غير مباشر</span><span class="sxs-lookup"><span data-stu-id="268ed-105">Indirect</span></span> 
-   <span data-ttu-id="268ed-106">مصادر خارجية</span><span class="sxs-lookup"><span data-stu-id="268ed-106">Outsourcing</span></span> 

<span data-ttu-id="268ed-107">تأكد من إعداد إصدار التكاليف وفئات التكلفة ومجموعات التكلفة وورقة التكاليف قبل حساب تكلفة الصنف وتفعيلها في تكلفة قياسية، وهو أمر مطلوب لإنشاء قواعد كانبان.</span><span class="sxs-lookup"><span data-stu-id="268ed-107">Make sure that you set up a costing version, cost categories, cost groups, and the costing sheet prior to calculating the item's cost and activating that into a standard cost, which is required to create kanban rules.</span></span>

<span data-ttu-id="268ed-108">**إصدار التكاليف** هو المستودع الرئيسي للاحتفاظ بالتكاليف الخاصة بكافة الأنواع.</span><span class="sxs-lookup"><span data-stu-id="268ed-108">The **Costing version** is the main repository for maintaining costs of all types.</span></span> <span data-ttu-id="268ed-109">تعمل مجموعات التكلفة كتصنيف لعناصر التكاليف وهي الأساس لتحليل تصنيف التكلفة.</span><span class="sxs-lookup"><span data-stu-id="268ed-109">Cost groups serve as a classification of elements of costs and are the basis for cost breakdown analysis.</span></span>

<span data-ttu-id="268ed-110">كما تستخدم مجموعات التكاليف لتحديد أساس حساب التكلفة غير المباشرة.</span><span class="sxs-lookup"><span data-stu-id="268ed-110">Cost groups are also used to identify the basis for indirect cost calculation.</span></span>
<span data-ttu-id="268ed-111">يتم تحديد قواعد حساب التكاليف غير المباشرة في كشف التكاليف.</span><span class="sxs-lookup"><span data-stu-id="268ed-111">Rules for calculating indirect costs are defined in the costing sheet.</span></span>
<span data-ttu-id="268ed-112">تستخدم فئات التكلفة لتحديد التكاليف وحسابات دفتر الأستاذ للموارد كأنواع خلايا عمل.</span><span class="sxs-lookup"><span data-stu-id="268ed-112">Cost categories are used to define costs and ledger accounts for resources as work cell types.</span></span>

<span data-ttu-id="268ed-113">يتم تطبيق تكاليف **التصنيع المباشر** عندما تقوم بالإبلاغ عن كميات مكتملة من منتج باستخدام الاستخدام المخطط لتدفق الإنتاج لمورد العملية في السعر القياسي لمورد العملية (معدل فئة التكلفة).</span><span class="sxs-lookup"><span data-stu-id="268ed-113">**Direct manufacturing** costs are applied when you are reporting completed quantities of a product by using the production flow planned usage of the operation resource at the operation resource standard rate (cost category rate).</span></span>

<span data-ttu-id="268ed-114">يجب تعيين فئة التكلفة إلى فئة وقت التشغيل لخلية العمل.</span><span class="sxs-lookup"><span data-stu-id="268ed-114">A cost category must be assigned to the run time category of the work cell.</span></span> <span data-ttu-id="268ed-115">لا يتم تضمين فئات التكلفة الخاصة بالإعداد والكمية في تكاليف lean manufacturing.</span><span class="sxs-lookup"><span data-stu-id="268ed-115">The cost categories for setup and quantity are not considered in costing for lean manufacturing.</span></span> <span data-ttu-id="268ed-116">يتم تجاهل حسابات الأعمال تحت التنفيذ لكل مجموعة موارد في تحديد تكاليف الإصدار التلقائي.</span><span class="sxs-lookup"><span data-stu-id="268ed-116">The WIP accounts for each resource group are ignored in backflush costing.</span></span> <span data-ttu-id="268ed-117">بالنسبة للأنشطة المتعاقد عليها من الباطن، لا توجد فئة تكلفة مطلوبة لأنه يتم استخدام مجموعة التكلفة التي تم تعيينها إلى الخدمة النشطة بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="268ed-117">For subcontracted activities, no cost category is needed because the cost group that is assigned to the active service is used instead.</span></span>

<span data-ttu-id="268ed-118">يتم تطبيق تكاليف **التصنيع غير المباشر** على الخصم أو الائتمان الخاص بالأعمال تحت التنفيذ وفقاً لتعريف كشف التكاليف.</span><span class="sxs-lookup"><span data-stu-id="268ed-118">**Indirect manufacturing** costs are applied upon the debiting or crediting of WIP according to the costing sheet definition.</span></span>


<span data-ttu-id="268ed-119">تعكس نسب فرق الإنتاج في تكاليف التصنيع المباشر وتكاليف التصنيع غير المباشر الفرق بين تكاليف التحويل المطبقة لتدفق الإنتاج وتكلفة تحويل التكلفة القياسية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="268ed-119">Production variances on direct manufacturing and indirect manufacturing costs capture the difference between the applied conversion costs for the production flow and the product's standard cost conversion cost.</span></span>


## <a name="applied-conversion-costs-on-lean-manufacturing"></a><span data-ttu-id="268ed-120">تم تطبيق تكاليف التحويل على lean manufacturing</span><span class="sxs-lookup"><span data-stu-id="268ed-120">Applied conversion costs on lean manufacturing</span></span>

<span data-ttu-id="268ed-121">في lean manufacturing، لا يتم تطبيق تكاليف التحويل وفقاً لتكلفة تحويل التكلفة القياسية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="268ed-121">In lean manufacturing, conversion costs are not applied according to the product's standard cost conversion cost.</span></span> <span data-ttu-id="268ed-122">وبدلاً من ذلك، يتم حساب تكاليف التحويل وتطبيقها وفقاً لاستخدام موارد العملية المخططة لتدفق الإنتاج الفعلي للمنتج بالمعدل القياسي لموارد التشغيل.</span><span class="sxs-lookup"><span data-stu-id="268ed-122">Instead, conversion costs are calculated and applied according to the effective production flow's planned operation resource usage for the product at the standard rate for operating resources.</span></span>

<span data-ttu-id="268ed-123">يمكن أن يؤدي هذا الحساب إلى نسب الفرق إلى التكلفة القياسية على تكلفة التحويل عند عدم مراجعة التكلفة القياسية للمنتجات وفقاً للتغييرات في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="268ed-123">This calculation can result in variances to standard cost on conversion cost when the standard cost of products is not revised according to the changes to production flow.</span></span>


## <a name="flattening-of-bom-during-cost-calculation-for-lean-items"></a><span data-ttu-id="268ed-124">دمج قائمة مكونات الصنف أثناء حساب التكلفة للأصناف المحدودة الفاقد</span><span class="sxs-lookup"><span data-stu-id="268ed-124">Flattening of BOM during cost calculation for lean items</span></span>

<span data-ttu-id="268ed-125">مسح **التحديث الفعلي** الذي تم تحديده لنشاط تدفق الإنتاج، والذي يحدد الأصناف التي يتم إنتاجها في تدفق إنتاج على أنه لا يتحكم في المخزون.</span><span class="sxs-lookup"><span data-stu-id="268ed-125">Clearing the **Update on hand inventory** selection, which has been defined for the production flow activity, designates items that are produced in a production flow as non-inventory controlled.</span></span> <span data-ttu-id="268ed-126">ونتيجة لذلك، تتم معاملة هذه الأصناف على أنها مماثلة لمكون الصنف الوهمي عند تضمينها داخل قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="268ed-126">As a result, these items are treated similar to a phantom component when they are included within a BOM.</span></span>

<span data-ttu-id="268ed-127">عندما تتم مواجهة أحد هذه المكونات في قائمة مكونات الصنف، يقوم النظام بالتجزئة عبر قائمة مكونات الصنف الخاصة بالصنف ويرفع المكونات مستوى واحداً لأعلى في قائمة مكونات الصنف كما لو كانت مكونات الأصل بدلاً من مكونات الصنف المكون.</span><span class="sxs-lookup"><span data-stu-id="268ed-127">When one of these components is encountered in a BOM calculation, the system explodes through the item's BOM and lifts the components one level up in the BOM as though they were components of the parent instead of components of the composed item.</span></span>

<span data-ttu-id="268ed-128">يمكن لإعداد **تحديث المخزون الفعلي** تغيير الترحيلات المالية بشكل كبير.</span><span class="sxs-lookup"><span data-stu-id="268ed-128">The setting for **Update on hand inventory** can significantly change the financial postings.</span></span> <span data-ttu-id="268ed-129">عند إلغاء تحديد هذه العلامة، يتم اعتبار الأصناف غير قابلة للتحكم في المخزون.</span><span class="sxs-lookup"><span data-stu-id="268ed-129">When this flag is cleared, the items are considered as not inventory controlled.</span></span> 
