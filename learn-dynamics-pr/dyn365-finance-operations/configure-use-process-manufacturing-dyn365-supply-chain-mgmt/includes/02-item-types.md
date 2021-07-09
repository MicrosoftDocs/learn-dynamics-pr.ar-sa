---
ms.openlocfilehash: ca44e5cfc34ef5717d4ac448bac644fc702043b2
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073760"
---
<span data-ttu-id="dc3b8-101">يدعم Dynamics 365 Supply Chain Management أنواعاً متعددة من الأصناف، بما في ذلك المعادلة ووزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-101">Dynamics 365 Supply Chain Management supports multiple item types, including formula and catch weight.</span></span>

## <a name="formula-items"></a><span data-ttu-id="dc3b8-102">الأصناف المركبة</span><span class="sxs-lookup"><span data-stu-id="dc3b8-102">Formula items</span></span>

<span data-ttu-id="dc3b8-103">في Supply Chain Management، يطلق على الأصناف التي يتم إنتاجها (شبه منتهية أو منتهية) في تصنيع العمليات *الأصناف المركبة*:</span><span class="sxs-lookup"><span data-stu-id="dc3b8-103">In Supply Chain Management, the items that are produced (semi-finished or finished) in process manufacturing are called *formula items*:</span></span>

-   <span data-ttu-id="dc3b8-104">يتم إنتاج الأصناف المركبة من سلسلة من عمليات مختلطة، أو تفاعلات كيميائية، أو استخراجات، أو الإجراءات الأخرى التي تقوم على تحويل المواد الخام إلى منتج نهائي قابل للبيع.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-104">Formula items are produced from a series of mixing operations, chemical reactions, extraction, or other actions that transform raw materials into a final, sellable product.</span></span>

-   <span data-ttu-id="dc3b8-105">قد يتم إنتاج الصنف المركب من خلال منتجات مشتركة أو منتجات ثانوية.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-105">A formula item might be produced with coproducts and by-products.</span></span>

-   <span data-ttu-id="dc3b8-106">يتم إنتاج الصنف المركب بأحجام معينة، تسمي أحجام الدفعات، ويمكن تتبعها برقم دفعة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-106">The formula item is produced in specific sizes, called batch sizes, and can be tracked with a batch number.</span></span>

-   <span data-ttu-id="dc3b8-107">سيؤدي العائد إلى اختلاف كميات المكونات لتحقيق المخرجات المخطط لها لصنف المعادلة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-107">Yield will cause the ingredient quantities to differ to achieve the planned output of the formula item.</span></span>



## <a name="catch-weight-items"></a><span data-ttu-id="dc3b8-108">أصناف وزن التعبئة</span><span class="sxs-lookup"><span data-stu-id="dc3b8-108">Catch weight items</span></span>

<span data-ttu-id="dc3b8-109">هناك أصناف معينة، عندما تقوم بشرائها أو بيعها، يجب أن يتم وزنها، مثل البطيخ أو اللحوم أو الماس.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-109">Certain items, when you are buying or selling them, need to be weighed, such as watermelon, meat, or diamonds.</span></span> <span data-ttu-id="dc3b8-110">في هذا السيناريو، يتم تحديد السعر حسب وزن الصنف.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-110">In that scenario, the price is determined by the weight of the item.</span></span> 

<span data-ttu-id="dc3b8-111">وتعرف أنواع الأصناف هذه بأصناف وزن التعبئة، ويمكنك شراء الأصناف أو بيعها في وحدة واحدة كعلبة أو عبوة أو أكياس أو كل منها.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-111">These types of items are known as catch weight items, and you can buy or sell the items in one unit such as a bag, box, pcs., or each.</span></span>
<span data-ttu-id="dc3b8-112">ومع ذلك، ستقوم بقياس وحدتي السعر والمخزون الخاصة بالصنف من خلال وحدة تقوم بقياس الوزن مثل الكيلوجرام (الجم) أو الرطل (أرطال).</span><span class="sxs-lookup"><span data-stu-id="dc3b8-112">However, you will measure the price and inventory units of the item by a unit that measures weight such as kilograms (kg) or pounds (lbs).</span></span>

<span data-ttu-id="dc3b8-113">يتم تعريف أصناف وزن التعبئة كصنف وزن تعبئة في المستوى العام عند إنشاء المنتج.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-113">Catch weight items are defined as a catch weight item at the global level when the product is created.</span></span> <span data-ttu-id="dc3b8-114">يجب أن تقوم جميع المؤسسات التي تستخدم ذلك المنتج باستخدام وظيفة وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-114">All enterprises that use that product must use the catch weight functionality.</span></span>

<span data-ttu-id="dc3b8-115">**إدارة معلومات المنتج > المنتجات > المنتجات > جديد**.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-115">**Product information management > Products > Products > New**</span></span>

![لقطه لصفحة المنتج الجديد مع شريط تمرير وزن التعبئة المحدد.](../media/new-catch-weight.png) 


### <a name="catch-weight-related-setup"></a><span data-ttu-id="dc3b8-117">الاعداد ذي الصلة بوزن التعبئة</span><span class="sxs-lookup"><span data-stu-id="dc3b8-117">Catch weight-related setup</span></span>

<span data-ttu-id="dc3b8-118">عند تمكين خانة الاختيار **منتج CW** في المستوى العام وإصداره إلى الشركات الفردية، يتعين عليك إجراء إعداد وزن التعبئة للصنف، بما في ذلك المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="dc3b8-118">When you enable the **CW product** check box at the global level and release it to individual companies, you must perform catch weight setup on the item, including the following tasks:</span></span>

-   <span data-ttu-id="dc3b8-119">قم بإنشاء بيانات تحويل الوحدات بين الوحدة الاساسية ووحدة وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-119">Create the unit conversion data between the base unit and the catch weight unit.</span></span>

-   <span data-ttu-id="dc3b8-120">قم بتعيين وحدة وزن التعبئة لقياس الصنف.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-120">Assign the catch weight unit of measure to the item.</span></span>

-   <span data-ttu-id="dc3b8-121">أدخل حقلي **الحد الأدنى للكمية** و **الحد الأقصى للكمية** في مجموعة حقول **وزن التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-121">Enter the **Minimum quantity** and **Maximum quantity** fields in the **Catch weight** field group.</span></span>

-   <span data-ttu-id="dc3b8-122">قم بتعيين **مجموعة أبعاد التعقب**.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-122">Set the **Tracking Dimension Group**.</span></span>

-   <span data-ttu-id="dc3b8-123">حدد مجموعة أبعاد التعقب مع اختيار **الدفعة النشطة** إذا كنت ترغب في تعقب رقم دفعة أو فترة الصلاحية.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-123">Select a tracking dimension group with the selection of **Batch active** if you want to track a batch number or a shelf life.</span></span>

### <a name="full-or-partial-visibility"></a><span data-ttu-id="dc3b8-124">الرؤية الكاملة أو الجزئية</span><span class="sxs-lookup"><span data-stu-id="dc3b8-124">Full or partial visibility</span></span>

<span data-ttu-id="dc3b8-125">يعمل تكوين البعد والوزن اللذين قمت بإعدادهما لمنتج وزن التعبئة على تحديد ما إذا كان الصنف يستخدم رؤية كاملة أو جزئية.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-125">The dimension configuration and weight that you set up for a catch weight product determines whether the item uses full or partial visibility.</span></span>

-   <span data-ttu-id="dc3b8-126">**أصناف وزن التعبئة التي تستخدم الرؤية الكاملة** - تتطلب أن تكون كمية المخزون معروفة لكل وحدة من وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-126">**Catch weight items that use full visibility** - Require that the inventory quantity be known for each catch weight unit.</span></span> <span data-ttu-id="dc3b8-127">على سبيل المثال، لنفرض أنه تم بيع الجمبري في صناديق وطلب العميل أن يكون لكل صندوق معرف فريد ووزن معروف.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-127">For example, assume that shrimp is sold in boxes and the customer requires that each box has a unique identification and a known weight.</span></span> <span data-ttu-id="dc3b8-128">في هذا المثال، يجب إنشاء رقم الصنف لصناديق الجمبري كصنف وزن التقاط يستخدم امكانيه الرؤية الكاملة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-128">In this example, the item number for the boxes of shrimp should be created as a catch weight item that uses full visibility.</span></span> <span data-ttu-id="dc3b8-129">يمكنك إنشاء أصناف وزن التعبئة الت تستخدم الرؤية الكاملة إذا قمت بتعيين رقم تسلسلي فريد لكل وحدة وزن تعبئة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-129">You can create catch weight items that use full visibility if you assign a unique serial number to each catch weight unit.</span></span>

-   <span data-ttu-id="dc3b8-130">**أصناف وزن التعبئة التي تستخدم الرؤية الجزئية** - تتطلب أن تكون كمية المخزون معروفة لأجزاء الأصناف التي تستخدم وحدة وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-130">**Catch weight items that use partial visibility** - Require that the inventory quantity be known for batches of items that use a catch weight unit.</span></span> <span data-ttu-id="dc3b8-131">على سبيل المثال، افترض أن الشركة تتلقى دفعة من 100 صندوق من الجمبري بوزن معين يبلغ 10 كيلو جرامات.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-131">For example, assume that a company receives a batch of 100 boxes of shrimp with a nominal weight of 10 kilograms.</span></span> <span data-ttu-id="dc3b8-132">ونظراً لأن كل الصناديق تنتمي لنفس الدفعة، فكل منها يستخدم رقم الدفعة ذاته.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-132">Because all the boxes belong to the same batch, they all use the same batch number.</span></span> <span data-ttu-id="dc3b8-133">قد يختلف وزن كل صندوق، لذا يتم وزن دفعة الصناديق بالكامل.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-133">Each box can vary in weight; therefore, the whole batch of boxes is weighed.</span></span> <span data-ttu-id="dc3b8-134">يمكن تسجيل عدد الصناديق ووزنها الإجمالي في حركة واحدة.</span><span class="sxs-lookup"><span data-stu-id="dc3b8-134">The number of boxes and their total weight can be registered in a single transaction.</span></span>
