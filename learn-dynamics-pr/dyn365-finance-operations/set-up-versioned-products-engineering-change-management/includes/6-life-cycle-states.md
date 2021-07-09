---
ms.openlocfilehash: 98b20533bd842e3338b3b28c3d301e1eaf9feee8
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6075012"
---
<span data-ttu-id="c4cb4-101">سيكون لجميع المنتجات دورة حياة، بداية من تاريخ بدئها وإلي استخدامها النشط وحتى نهايتها.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-101">All products will have a life cycle, from their start, to their active usage, and to their end.</span></span> <span data-ttu-id="c4cb4-102">عند إعداد هذه الحالات، ستحدد الحركات وأوامر المبيعات وأوامر الشراء وأوامر الإنتاج وما إلى ذلك، التي تم تمكينها وحظرها.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-102">When setting up these states, you will determine which transactions, sales orders, purchase orders, production orders, and so on, are enabled and which ones are blocked.</span></span>

<span data-ttu-id="c4cb4-103">ترتبط المنتجات الهندسية وتغييرات دورة الحياة بالإصدار الهندسي للمنتج.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-103">Engineering products and life cycle changes are tied to the product's engineering version.</span></span> <span data-ttu-id="c4cb4-104">ضع في اعتبارك سيناريو تستخدم فيه بُعد منتج مع إصدار.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-104">Consider a scenario where you're using a product dimension with a version.</span></span> <span data-ttu-id="c4cb4-105">في هذه الحالة، يمكنك استخدام حالة دورة الحياة للإشارة إلى الحركات المسموح بها لكل إصدار.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-105">In that case, you can use the life cycle state to indicate which transactions are allowed for each version.</span></span>

## <a name="set-up-product-life-cycle-states"></a><span data-ttu-id="c4cb4-106">إعداد حالات دورة حياة المنتج</span><span class="sxs-lookup"><span data-stu-id="c4cb4-106">Set up product life cycle states</span></span>

<span data-ttu-id="c4cb4-107">لاستخدام حالات دورة الحياة، انتقل إلى **إدارة التغيير الهندسي > إعداد > حالة دورة حياة المنتج**.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-107">To use life cycle states, go to **Engineering change management > Setup > Product lifecycle state**.</span></span> <span data-ttu-id="c4cb4-108">حدد **جديد** لإنشاء دورة حياة جديدة أو **تحرير** لتعديل الإعدادات في إحدى الحالات الحالية.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-108">Select **New** to create a new life cycle or **Edit** to modify the settings on one of the current states.</span></span>

### <a name="header"></a><span data-ttu-id="c4cb4-109">الرأس </span><span class="sxs-lookup"><span data-stu-id="c4cb4-109">Header</span></span>

<span data-ttu-id="c4cb4-110">في الرأس، ستُنشئ اسماً ووصفاً لحالة دورة حياة المنتج.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-110">In the header, you'll create a name and a description for the product life cycle state.</span></span>

### <a name="general-fasttab"></a><span data-ttu-id="c4cb4-111">علامة التبويب السريعة عام</span><span class="sxs-lookup"><span data-stu-id="c4cb4-111">General FastTab</span></span>

<span data-ttu-id="c4cb4-112">تحتوي علامة التبويب السريعة **عام** على خيارين:</span><span class="sxs-lookup"><span data-stu-id="c4cb4-112">The **General** FastTab contains two options:</span></span>

- <span data-ttu-id="c4cb4-113">**القيمة الافتراضية عند الإصدار إلى الكيان القانوني** - بالنسبة للمنتجات العادية، يمكنك تحديد **نعم** إذا كنت تريد تطبيق حالة دورة الحياة على المنتجات عند إصدارها للكيانات القانونية.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-113">**Default when released to legal entity** - For regular products, you would select **Yes** if you wanted the life cycle state to apply to products when they're released to legal entities.</span></span> <span data-ttu-id="c4cb4-114">يمكنك تحديد **لا** إذا تم تطبيق دورة الحياة يدوياً لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-114">You would select **No** if the life cycle is manually applied later.</span></span>

    <span data-ttu-id="c4cb4-115">لن يتم تطبيق هذا الخيار على المنتجات الهندسية لأنه يتم إنشاء دورة الحياة عند تعيينها لفئة تغيير هندسي.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-115">This option wouldn't apply to engineering products because the life cycle is established when it's assigned to an engineering change category.</span></span>

- <span data-ttu-id="c4cb4-116">**نشط للتخطيط** - يعني تحديد **نعم** لهذا الخيار أنه سيشمل المنتجات الموجودة في حالة دورة الحياة هذه في العمليات الحسابية للتخطيط الرئيسي ومستويات قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-116">**Is active for planning** - Selecting **Yes** for this option means that it will include products that are in this life cycle state in calculations for master planning and BOM levels.</span></span> <span data-ttu-id="c4cb4-117">إذا قمت بتحديد **لا**، فسيتم استبعاد المنتجات في هذه الحالة من الحسابات.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-117">If you select **No**, products are excluded in this state from the calculations</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="c4cb4-118">[![صفحة حالة دورة حياة المنتج للحالة التشغيلية. يتم تعيين الخيار الافتراضي عند الإصدار إلى كيان قانوني على "نعم".](../media/product-life-cycle-state.png)](../media/product-life-cycle-state.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c4cb4-118">[![Product life cycle state page for the Operational state. The Default when releasing to legal entity option is set to No. The Is active for planning option is set to Yes.](../media/product-life-cycle-state.png)](../media/product-life-cycle-state.png#lightbox)</span></span>


### <a name="enabled-business-processes-fasttab"></a><span data-ttu-id="c4cb4-119">علامة التبويب السريعة لعمليات الأعمال الممكّنة</span><span class="sxs-lookup"><span data-stu-id="c4cb4-119">Enabled business processes FastTab</span></span>

<span data-ttu-id="c4cb4-120">في علامة التبويب السريعة **عمليات الأعمال الممكّنة**، يعتبر عمود **العملية** قائمة ثابتة تضم عمليات الأعمال الممكنة.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-120">In the **Enabled business processes** FastTab, the **Process** column is a fixed list of the possible business processes.</span></span> <span data-ttu-id="c4cb4-121">يحتوي عمود **منطقة العملية** على قيمة افتراضية يمكن تغييرها، على الرغم من أن التغيير لن يكون له أي تأثير.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-121">The **Process area** column has a default value, which can be changed, though the change won't have any effect.</span></span> 

<span data-ttu-id="c4cb4-122">يحتوي عمود **السياسة** على ثلاثة خيارات يمكنك التحديد من بينها:</span><span class="sxs-lookup"><span data-stu-id="c4cb4-122">The **Policy** column has three options that you can select from:</span></span>

- <span data-ttu-id="c4cb4-123">**الممكّنة** - يتم السماح بعملية الأعمال.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-123">**Enabled** - The business process is allowed.</span></span>

- <span data-ttu-id="c4cb4-124">**المحظورة** - غير مسموح بعملية الأعمال، وفي حاله المحاولة، سيقوم النظام بحظرها وعرض الخطأ.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-124">**Blocked** - The business process isn't allowed, and if attempted, the system will block it and display an error.</span></span> <span data-ttu-id="c4cb4-125">على سبيل المثال، لا يسمح بأمر شراء بصنف قديم.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-125">For example, a purchase order wouldn't be allowed on an obsolete item.</span></span>
 
- <span data-ttu-id="c4cb4-126">**تم التمكين مع تحذير** - سيعرض النظام تنبيهاً لحالة معينة.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-126">**Enabled with warning** - The system will show an alert for a specific situation.</span></span> <span data-ttu-id="c4cb4-127">يعتبر أمر إنتاج الذي يستخدم منتجاً لا يزال قيد التصميم واحدً من الأمثلة.</span><span class="sxs-lookup"><span data-stu-id="c4cb4-127">An example might be a production order that is using a product that is still in design.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="c4cb4-128">[![لقطة شاشة لصفحة عمليات الأعمال الممكّنة تعرض جدولاً يضم أعمدة العملية ومنطقة العملية والسياسة.](../media/enable-business-processes.png)](../media/enable-business-processes.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c4cb4-128">[![Screenshot of the Enabled business processes page showing a table with Process, Process area, and Policy columns.](../media/enable-business-processes.png)](../media/enable-business-processes.png#lightbox)</span></span>

