---
ms.openlocfilehash: 52934b14a98bae8825733f83af8ebe42f750f911
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072632"
---
<span data-ttu-id="a51b2-101">توفر أوامر التغيير الهندسي عملية منظمة لإجراء تغييرات على المنتجات الهندسية.</span><span class="sxs-lookup"><span data-stu-id="a51b2-101">Engineering change orders provide a structured process for making changes to engineering products.</span></span><span data-ttu-id="a51b2-102"> يمكن إنشاء أوامر التغيير من خلال طلبات أوامر التغيير أو من البداية.</span><span class="sxs-lookup"><span data-stu-id="a51b2-102"> Change orders can be created by change order requests or from scratch.</span></span>

<span data-ttu-id="a51b2-103">يمكنك تضمين منتجات متعددة في أمر التغيير الهندسي باتباع أي من الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="a51b2-103">You can include multiple products on the engineering change order by following any of these steps:</span></span>

-   <span data-ttu-id="a51b2-104">تحديد المنتجات يدوياً</span><span class="sxs-lookup"><span data-stu-id="a51b2-104">Manually select products</span></span>

-   <span data-ttu-id="a51b2-105">استخدام قائمة مكونات الصنف لتضمين الأصناف الفرعية</span><span class="sxs-lookup"><span data-stu-id="a51b2-105">Use the BOM to include child items</span></span>

-   <span data-ttu-id="a51b2-106">استخدم البحث الذي تم استخدامه لتضمين الصنف الأصل لبند قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="a51b2-106">Use a where used search to include the parent item for a BOM line.</span></span>

<span data-ttu-id="a51b2-107">بعد اكتمال التغييرات المقترحة على الصفحة، يمكن تنفيذ عملية المراجعة والموافقة تلقائياً باستخدام مهام سير العمل، كما تمت مناقشتها.</span><span class="sxs-lookup"><span data-stu-id="a51b2-107">After the proposed changes have been completed on the page, the review and approval process can be automated using the workflows, as discussed.</span></span> <span data-ttu-id="a51b2-108">سواء اختارت شركتك معالجة أوامر التغيير الهندسي مباشرة بعد الموافقة عليها، كجزء من سير العمل، أو كخطوة يدوية، عند معالجة أمر التغيير، يتم تحديث البيانات الهندسية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="a51b2-108">Whether your company chooses to process engineering change orders directly after it's approved, as part of a workflow, or as a manual step, when the change order is processed, the product's engineering data is updated.</span></span>

## <a name="engineering-change-orders-in-engineering-or-operational-companies"></a><span data-ttu-id="a51b2-109">أوامر التغيير الهندسي في الشركات الهندسية أو التشغيلية</span><span class="sxs-lookup"><span data-stu-id="a51b2-109">Engineering change orders in engineering or operational companies</span></span>

<span data-ttu-id="a51b2-110">بناءً على نوع الكيان القانوني الذي تقوم بإنشاء أمر التغيير فيه، سواء كانت شركة هندسية أو تشغيلية، تختلف بيانات المنتج التي يمكن تغييرها.</span><span class="sxs-lookup"><span data-stu-id="a51b2-110">Depending on the type of legal entity that you are creating the change order in, whether an Engineering or Operational company, the product data that can be changed varies.</span></span>

<span data-ttu-id="a51b2-111">وإليك بعض الأمثلة:</span><span class="sxs-lookup"><span data-stu-id="a51b2-111">Here are some examples:</span></span>

-   <span data-ttu-id="a51b2-112">بالنسبة لأوامر التغيير الهندسي في  **شركة هندسية**، يمكنك إجراء تغييرات أساسية على البيانات الهندسية.</span><span class="sxs-lookup"><span data-stu-id="a51b2-112">For engineering change orders in an **engineering company**, you can make basic changes to the engineering data.</span></span> <span data-ttu-id="a51b2-113">على سبيل المثال، يمكنك إنشاء إصدارات جديدة من أحد المنتجات، وتغيير هيكل المنتج عبر قائمة مكونات الصنف، وتغيير قيم السمات الهندسية.</span><span class="sxs-lookup"><span data-stu-id="a51b2-113">For example, you can create new versions of a product, change a product's structure via the BOM, and change engineering attribute values.</span></span> <span data-ttu-id="a51b2-114">بالنسبة لكل منتج متأثر، حدد إحدى القيم التالية في حقل  **التأثير** :</span><span class="sxs-lookup"><span data-stu-id="a51b2-114">For each affected product, select one of the following values in the **Impact** field:</span></span>

    -   <span data-ttu-id="a51b2-115">**بلا** - تحديث إصدار المنتج الموجود (التحديث داخل الإصدار).</span><span class="sxs-lookup"><span data-stu-id="a51b2-115">**None** - Update the existing product version (in-version update).</span></span>

    -   <span data-ttu-id="a51b2-116">**إصدار جديد** - إنشاء إصدار جديد يستند إلى إصدار المنتج المحدد.</span><span class="sxs-lookup"><span data-stu-id="a51b2-116">**New version** - Create a new version that is based on the selected product version.</span></span>

    -   <span data-ttu-id="a51b2-117">**منتج جديد** - إنشاء منتج جديد يستند إلى إصدار المنتج المحدد.</span><span class="sxs-lookup"><span data-stu-id="a51b2-117">**New product** - Create a new product based on the selected product version.</span></span>

    -   <span data-ttu-id="a51b2-118">**متغير جديد** - إنشاء متغير جديد للصنف بناءً على إصدار المنتج المحدد.</span><span class="sxs-lookup"><span data-stu-id="a51b2-118">**New variant** - Create a new variant of the item based on the selected product version.</span></span> <span data-ttu-id="a51b2-119">سيتم نسخ قائمة مكونات الصنف ومعلومات المسار.</span><span class="sxs-lookup"><span data-stu-id="a51b2-119">The BOM and route information will be copied.</span></span>

-   <span data-ttu-id="a51b2-120">بالنسبة لأوامر التغيير الهندسي في  **شركة تشغيلية**، يمكنك تغيير البيانات اللوجستية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="a51b2-120">For engineering change orders in an **operational company**, you can change the logistical data of the product.</span></span> <span data-ttu-id="a51b2-121">على سبيل المثال، يمكنك إثراء قائمة مكونات الصنف الحالية بإعدادات تحديد المصادر، وإضافة مسارات محلية أو قائمة مكونات الصنف المحلية، وحتى إثراء قائمة مكونات الصنف عن طريق إضافة سطور قائمة مكونات الصنف جديدة لمواد التعبئة المحلية، أو سوائل التشحيم، أو الإرشادات باللغة المحلية.</span><span class="sxs-lookup"><span data-stu-id="a51b2-121">For example, you can enrich the existing BOM with settings for sourcing, add local routes or local BOMs, and even enrich a BOM by adding new BOM lines for local packaging materials, lubrication fluids, or instructions in the local language.</span></span>

<span data-ttu-id="a51b2-122">عند إجراء تغييرات في الشركة الهندسية، يجب بعد ذلك طرح المنتجات للشركات العاملة.</span><span class="sxs-lookup"><span data-stu-id="a51b2-122">When changes are made in the engineering company, the products should then be released to the operational companies.</span></span>

## <a name="create-an-engineering-change-order"></a><span data-ttu-id="a51b2-123">إنشاء أمر تغيير هندسي</span><span class="sxs-lookup"><span data-stu-id="a51b2-123">Create an engineering change order</span></span>

<span data-ttu-id="a51b2-124">لإنشاء أمر تغيير هندسي، إما من خلال طلب أو من البداية، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="a51b2-124">To create an engineering change order, either from a request or scratch, follow these steps:</span></span>

1.  <span data-ttu-id="a51b2-125">انتقل إلى **إدارة التغيير الهندسي> عام > إدارة التغيير الهندسي > أوامر التغيير الهندسي.**</span><span class="sxs-lookup"><span data-stu-id="a51b2-125">Go to **Engineering change management > Common > Engineering change management > Engineer change orders.**</span></span>

1.  <span data-ttu-id="a51b2-126">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a51b2-126">Select **New**.</span></span>

1.  <span data-ttu-id="a51b2-127">في حقل **العنوان**، أدخل النص الذي يصف التغييرات في الطلب بإيجاز أو يحددها.</span><span class="sxs-lookup"><span data-stu-id="a51b2-127">In the **Title** field, enter the text that briefly describes or identifies the changes in the request.</span></span>

1.  <span data-ttu-id="a51b2-128">في حقل **الأولوية**، حدد قيمة للإشارة إلى مدى أولوية التغيير.</span><span class="sxs-lookup"><span data-stu-id="a51b2-128">In the **Priority** field, select a value to indicate how high the priority of the change is.</span></span> 

1.  <span data-ttu-id="a51b2-129">في حقل **الفئة**، حدد قيمة لوصف نوع التغيير الذي تطلبه.</span><span class="sxs-lookup"><span data-stu-id="a51b2-129">In the **Category** field, select a value to describe the type of change that you are requesting.</span></span>

1.  <span data-ttu-id="a51b2-130">في حقل **درجة الخطورة**، حدد قيمة للإشارة إلى خطورة المشكلة التي يجب إصلاحها من خلال تنفيذ الطلب.</span><span class="sxs-lookup"><span data-stu-id="a51b2-130">In the **Severity** field, select a value to indicate the severity of the issue that should be fixed by implementing the request.</span></span><span data-ttu-id="a51b2-131">  يمكن حساب الخطورة تلقائياً بتحديد **حساب** في مجموعة **الخطورة** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="a51b2-131">  The severity can be automatically calculated by selecting **Calculate** in the **Severity** group in the Action Pane.</span></span>

1.  <span data-ttu-id="a51b2-132">سيتم ملء قسم حالة **العملية** عند معالجة التغيير.</span><span class="sxs-lookup"><span data-stu-id="a51b2-132">The **Process** status section will be populated when the change is processed.</span></span> <span data-ttu-id="a51b2-133">على سبيل المثال، يشبه أمر التغيير ملفاً تتم فيه صياغة التغييرات أو تصميمها.</span><span class="sxs-lookup"><span data-stu-id="a51b2-133">For example, the change order is like a file where the changes are being drafted, or designed.</span></span> <span data-ttu-id="a51b2-134">عند تحديد تبديل **العملية**، تحدث هذه التغييرات، وبالتالي يتم **إصدار** أو **تعديل** المنتج في الشركة الهندسية مع التغييرات التي تنعكس في أمر التغيير</span><span class="sxs-lookup"><span data-stu-id="a51b2-134">When you select the **Process** toggle, those changes take place, so the product is then **released** or **modified** in the engineering company with the changes that are reflected in the change order</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="a51b2-135">[![لقطة شاشة لصفحة أمر التغيير الهندسي التي تفتح عند إجراء التحديد السابق. الحقول الاختيارية المراد ملؤها هي العنوان والفئة والأولوية والخطورة. وبمجرد معالجة أمر التغيير، سيتم ملء الحقول تمت المعالجة بواسطة وتمت المعالجة في.](../media/change-order-identification.png)](../media/change-order-identification.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="a51b2-135">[![Screenshot of the Engineering change order page that opens when the previous selection is made. Fields that are optional to fill out are Title, Category, Priority, and Severity. Once the Change order is processed, the Processed by and Processed at fields will populate.](../media/change-order-identification.png)](../media/change-order-identification.png#lightbox)</span></span>

1.  <span data-ttu-id="a51b2-136">في علامة التبويب السريعة **المنتجات المتأثرة**، حدد **جديد** لإضافة المنتجات إلى أمر التغيير.</span><span class="sxs-lookup"><span data-stu-id="a51b2-136">In the **Impacted products** FastTab, select **New** to add products to the change order.</span></span>

1.  <span data-ttu-id="a51b2-137">مثل طلب التغيير، يمكنك البحث عن المنتجات وإضافتها بطرق مختلفة، ومعرفة تأثير الأعمال، وفتح الحركات، والمزيد، من علامة التبويب السريعة **المنتجات المتأثرة**.</span><span class="sxs-lookup"><span data-stu-id="a51b2-137">Like the change request, you can search and add products in various ways, see the business impact, open transactions, and more, from the **Impacted products** FastTab.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="a51b2-138">[![لقطة شاشة لعلامة التبويب السريعة المنتجات المتأثرة مع خيارات مثل حقول طلب التغيير.](../media/impacted-products.png)](../media/impacted-products.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="a51b2-138">[![Screenshot of the Impacted products FastTab with options like the change request fields.](../media/impacted-products.png)](../media/impacted-products.png#lightbox)</span></span>

1. <span data-ttu-id="a51b2-139">عندما يحدد مالك المنتج **الموافقة** في جزء إجراءات **أمر التغيير**، في قسم  **حالة التغيير**، تتم الموافقة على التغيير في النظام.</span><span class="sxs-lookup"><span data-stu-id="a51b2-139">When the product owner selects **Approve** in the **Change order** Action Pane, **Change status** section, the change is approved in the system.</span></span>
