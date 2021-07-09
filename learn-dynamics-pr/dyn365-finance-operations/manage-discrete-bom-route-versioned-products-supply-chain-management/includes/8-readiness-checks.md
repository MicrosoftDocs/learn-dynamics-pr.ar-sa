---
ms.openlocfilehash: 619fa73411e5fe0fb744819dd65109bd8fec9011
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074858"
---
<span data-ttu-id="6afcb-101">عند إنشاء منتج هندسي جديد، سيحدد النظام ما إذا كان قد تم تكوين فحص الجاهزية لـ **فئة المنتج الهندسي**، كما هو موضح في [إعداد المنتجات ذات الإصدارات في الوحدة النمطية Dynamics 365 Supply Chain Management](/learn/modules/set-up-versioned-products-engineering-change-management/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="6afcb-101">When you create a new engineering product, the system will determine whether a readiness check has been configured for the **Engineering Product Category**, as described in the [Set up versioned products in Dynamics 365 Supply Chain Management](/learn/modules/set-up-versioned-products-engineering-change-management/?azure-portal=true) module.</span></span>

<span data-ttu-id="6afcb-102">يمكن تكوين فحوصات الجاهزية ليتم تطبيقها على مستوى المنتج الصادر ومستوى الإصدار الهندسي.</span><span class="sxs-lookup"><span data-stu-id="6afcb-102">Readiness checks can be configured to be applied on the released product level and engineering version level.</span></span> <span data-ttu-id="6afcb-103">إذا تم إعداد سياسة لهذه المستويات، فسوف تحدث الأحداث التالية:</span><span class="sxs-lookup"><span data-stu-id="6afcb-103">If a policy is set up for these levels, the following events will occur:</span></span>

-   <span data-ttu-id="6afcb-104">سيتم إنشاء فحوصات الجاهزية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="6afcb-104">Readiness checks will be created for the product.</span></span>

-   <span data-ttu-id="6afcb-105">سيتم تعيين الإصدار الهندسي على **‏‫غير نشط** لحظر استخدام المنتج.</span><span class="sxs-lookup"><span data-stu-id="6afcb-105">The engineering version will be set to **Inactive** to block the product from being used.</span></span>

## <a name="product"></a><span data-ttu-id="6afcb-106">المنتج</span><span class="sxs-lookup"><span data-stu-id="6afcb-106">Product</span></span>

<span data-ttu-id="6afcb-107">للعثور على فحوصات الجاهزية لأحد المنتجات، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="6afcb-107">To find the readiness checks for a product, follow these steps:</span></span>

1.  <span data-ttu-id="6afcb-108">الانتقال إلى **إدارة التغيير الهندسي > عام > تفاصيل المنتج الصادر**، ثم حدد المنتج.</span><span class="sxs-lookup"><span data-stu-id="6afcb-108">Go to **Engineering change management > Common > Released product details**, and then select the product.</span></span> <span data-ttu-id="6afcb-109">بدلاً من ذلك، انتقل إلى **إدارة معلومات المنتجات > المنتجات > تفاصيل المنتج الصادر** لتحديد المنتج.</span><span class="sxs-lookup"><span data-stu-id="6afcb-109">Alternatively, go to **Product information management > Products > Released product details** to select the product.</span></span>

1.  <span data-ttu-id="6afcb-110">في جزء الإجراءات، في علامة التبويب  **المنتج** ، في مجموعة  **فحوصات الجاهزية** ، حدد  **فحوصات الجاهزية**.</span><span class="sxs-lookup"><span data-stu-id="6afcb-110">On the Action Pane, on the **Product** tab, in the **Readiness checks** group, select **Readiness checks**.</span></span>

## <a name="product-version"></a><span data-ttu-id="6afcb-111">إصدار المنتج</span><span class="sxs-lookup"><span data-stu-id="6afcb-111">Product version</span></span>

<span data-ttu-id="6afcb-112">للبحث عن فحوصات الجاهزية لأحد المنتجات، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="6afcb-112">To find the open readiness checks for a product version, follow these steps:</span></span>

1.  <span data-ttu-id="6afcb-113">الانتقال إلى **تفاصيل المنتج الصادر > الإصدارات الهندسية** لمنتج تم إصداره ثم حدد إصداراً.</span><span class="sxs-lookup"><span data-stu-id="6afcb-113">Go to **Released product details > Engineering versions** for a released product and then select a version.</span></span>

1.  <span data-ttu-id="6afcb-114">في جزء الإجراءات، في علامة التبويب  **المنتج** ، في مجموعة  **فحوصات** ، حدد  **فحوصات الجاهزية**.</span><span class="sxs-lookup"><span data-stu-id="6afcb-114">On the Action Pane, on the **Product** tab, in the **Checklist** group, select **Readiness checks**.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="6afcb-115">[![لقطة شاشة لصفحة "إدارة التغيير الهندسي > عام > المنتجات الصادرة، وفي جزء الإجراءات، في علامة التبويب المنتج، في مجموعة فحوصات الجاهزية، يتم تمييز خيار فحوصات الجاهزية.](../media/perform-readiness-check.png)](../media/perform-readiness-check.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6afcb-115">[![Screenshot of Engineering change management > Common > Released products page, and in the Action Pane, on the Product tab, in the Readiness checks group, the Readiness checks option is highlighted.](../media/perform-readiness-check.png)](../media/perform-readiness-check.png#lightbox)</span></span>

## <a name="process-open-readiness-checks"></a><span data-ttu-id="6afcb-116">معالجة فحوصات الجاهزية المفتوحة</span><span class="sxs-lookup"><span data-stu-id="6afcb-116">Process open readiness checks</span></span>

<span data-ttu-id="6afcb-117">عند فتح صفحة **فحوصات الجاهزية**، يمكنك عرض فحوصات الجاهزية المفتوحة للمنتج أو لإصدار المنتج.</span><span class="sxs-lookup"><span data-stu-id="6afcb-117">When the **Readiness checks** page opens, you can view the readiness checks that are open for the product/product version.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="6afcb-118">[![لقطة شاشة لصفحة تحتوي على قائمة بالفحوصات التي تم إعدادها لهذا المنتج.](../media/readiness-checks.png)](../media/readiness-checks.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="6afcb-118">[![Screenshot of the page with a list of checks that are set up for this product.](../media/readiness-checks.png)](../media/readiness-checks.png#lightbox)</span></span>

<span data-ttu-id="6afcb-119">تكون  **حالة**  فحوصات الجاهزية المفتوحة  **معلقة**، مما يشير إلى أنه لا يزال يتعين معالجة فحص الجاهزية.</span><span class="sxs-lookup"><span data-stu-id="6afcb-119">Open readiness checks have a **Status** of **Pending**, indicating that the readiness check must still be processed.</span></span> <span data-ttu-id="6afcb-120">لعرض تفاصيل حول البند الذي حددته، حدد **عرض المعلومات ذات الصلة** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="6afcb-120">To view details about the line that you selected, select **View related information** in the Action Pane.</span></span> <span data-ttu-id="6afcb-121">وفقا لنوع فحص النظام، سيتم فتح صفحات مختلفة لإرشادك خلال عملية الفحص القابلة للتطبيق الذي يجب إجراؤها.</span><span class="sxs-lookup"><span data-stu-id="6afcb-121">Depending on the system check type, different pages will open to guide you through the applicable check that needs to be performed.</span></span>

<span data-ttu-id="6afcb-122">لمعالجة فحص الجاهزية، بعد تنفيذ أي إجراءات مطلوبة، اتبع إحدى الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="6afcb-122">To process a readiness check, after performing any required actions, follow one of these steps:</span></span>

- <span data-ttu-id="6afcb-123">في جزء الإجراء، حدد  **فحص/إكمال**  لمراجعة فحص الجاهزية وإكماله.</span><span class="sxs-lookup"><span data-stu-id="6afcb-123">On the Action Pane, select **Check/complete** to review and complete the readiness check.</span></span> <span data-ttu-id="6afcb-124">عند الانتهاء، سيتم تحديث حقل  **الحالة**  إلى  **‏‫تم الاجتياز**.</span><span class="sxs-lookup"><span data-stu-id="6afcb-124">When you've finished, the **Status** field will be updated to **Passed**.</span></span>

- <span data-ttu-id="6afcb-125">حدد  **تخطي**  إذا كنت تريد تخطي فحص الجاهزية غير الإلزامي في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="6afcb-125">Select **Skip** if you want to skip a readiness check that isn't mandatory on the Action Pane.</span></span> <span data-ttu-id="6afcb-126">في هذه الحالة، سيتم تحديث حقل  **الحالة**  إلى  **تم التخطي**.</span><span class="sxs-lookup"><span data-stu-id="6afcb-126">In this case, the **Status** field will be updated to **Skipped**.</span></span>

- <span data-ttu-id="6afcb-127">وفقاً لتكوين سياسة الجاهزية، عند تحديث حقل  **الحالة**  لفحص الجاهزية إلى  **تم الاجتياز**، قد تكون هناك حاجة إلى خطوة إضافية للموافقة على فحص الجاهزية.</span><span class="sxs-lookup"><span data-stu-id="6afcb-127">Depending on the readiness policy's configuration, when the **Status** field for a readiness check is updated to **Passed**, an extra step might be required to approve the readiness check.</span></span> <span data-ttu-id="6afcb-128">في هذه الحالة، حدد  **موافقة**  لإكمال فحص الجاهزية.</span><span class="sxs-lookup"><span data-stu-id="6afcb-128">In this case, select **Approval** to complete the readiness check.</span></span>

<span data-ttu-id="6afcb-129">عند معالجة جميع عمليات فحوصات الجاهزية المفتوحة لمنتج أو متغير أو إصدار جديد، يصبح المنتج نشطاً تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="6afcb-129">When all open readiness checks for a new product, variant, or version have been processed, the product becomes active automatically.</span></span>

<span data-ttu-id="6afcb-130">شاهد الفيديو التالي للحصول على عرض توضيحي لكيفية صيانة فحوصات الجاهزية.</span><span class="sxs-lookup"><span data-stu-id="6afcb-130">Watch the following video for a demonstration of how to maintain the readiness checks.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWD1qH]
