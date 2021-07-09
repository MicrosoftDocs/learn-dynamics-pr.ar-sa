---
ms.openlocfilehash: b00298f11d825fa023ee59a099cdcd316de8fbe5
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074834"
---
<span data-ttu-id="44b35-101">والآن بعد قيام قسم الهندسة بتصميم المنتج، تكون جاهزاً لإصدار المنتج إلى الشركات التشغيلية التي تخطط لاستخدامه.</span><span class="sxs-lookup"><span data-stu-id="44b35-101">Now that the Engineering department has designed the product, you are ready to release the product to the operational companies that plan to use it.</span></span> <span data-ttu-id="44b35-102">عند إصدار المنتج الهندسي، تقوم أيضاً بإصدار قائمة BOM والأصناف التي تكون قائمة BOM والمسار.</span><span class="sxs-lookup"><span data-stu-id="44b35-102">When you release the engineering product, you are also releasing the BOM and the items that make up the BOM and the route.</span></span>

<span data-ttu-id="44b35-103">إذا كنت تستخدم خيار **مالك المنتج**، فيمكن لمالك ذلك المنتج فقط إصدار المنتج.</span><span class="sxs-lookup"><span data-stu-id="44b35-103">If you are using the **Product owner** option, only the owner of that product can release the product.</span></span> <span data-ttu-id="44b35-104">ومع ذلك، عندما يكون منتج جزءاً من قائمة BOM، لا يفحص النظام جميع المنتجات الموجودة في قائمة BOM، الأصل فقط.</span><span class="sxs-lookup"><span data-stu-id="44b35-104">However, when a product is part of a BOM, the system doesn't check all products in the BOM, only the parent.</span></span> <span data-ttu-id="44b35-105">إذا كان لسطر قائمة BOM مالك منتج مختلف، فإنه يمكن إصدارها بواسطة مالك الصنف الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="44b35-105">If a BOM line has a different product owner, then it can be released by the parent item owner.</span></span>

<span data-ttu-id="44b35-106">يعرف مالكو المنتج كيفية استخدام المنتجات وتغييرها.</span><span class="sxs-lookup"><span data-stu-id="44b35-106">Product owners know how the products should be used and changed.</span></span> <span data-ttu-id="44b35-107">عندما تستخدم عمليات سير عمل المنتج الهندسي لإصدار المنتجات أو طلبات تغيير المنتج، نوصي باستخدام خيار **مالك المنتج** في عملية الاعتماد.</span><span class="sxs-lookup"><span data-stu-id="44b35-107">When you are using engineering product workflows to release products or product change requests, we recommend that you use the **Product owner** option in the approval process.</span></span>

<span data-ttu-id="44b35-108">لإصدار المنتج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="44b35-108">To release the product, follow these steps:</span></span>

1.  <span data-ttu-id="44b35-109">انتقل إلى  **إدارة معلومات المنتجات > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="44b35-109">Go to **Product information management > Products > Released products**.</span></span>

1.  <span data-ttu-id="44b35-110">في جزء الإجراءات، ضمن علامة التبويب  **المنتج** ، في مجموعة  **الصيانة** ، حدد  **بنية إصدار المنتج**  لفتح معالج  **إصدار المنتجات** .</span><span class="sxs-lookup"><span data-stu-id="44b35-110">On the Action Pane, on the **Product** tab, in the **Maintain** group, select **Release product structure** to open the **Release products** wizard.</span></span>

1.  <span data-ttu-id="44b35-111">في صفحة **تحديد المنتجات الهندسية للإصدار** ، حدد خانة الاختيار **تحديد** .</span><span class="sxs-lookup"><span data-stu-id="44b35-111">On the **Select engineering products to release** page, select the **Select** check box.</span></span>
1.  <span data-ttu-id="44b35-112">حدد **تفاصيل الإصدار**.</span><span class="sxs-lookup"><span data-stu-id="44b35-112">Select **Release details**.</span></span>

1.  <span data-ttu-id="44b35-113">تظهر صفحة **تفاصيل إصدار المنتج** ، حيث يمكنك مراجعة تفاصيل المنتج الذي تم إصداره وبنيته.</span><span class="sxs-lookup"><span data-stu-id="44b35-113">The **Product release details** page appears, where you can review the details of the released product and its structure.</span></span> <span data-ttu-id="44b35-114">يمكنك تحديد أي عنصر فرعي في الجزء الأيمن لمراجعة التفاصيل الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="44b35-114">You can select any child item in the left pane to review its details.</span></span> <span data-ttu-id="44b35-115">إذا كان لأي صنف فرعي قائمة BOM، فيمكنك أيضاً تحديد إصدار قائمة BOM لهذا الفرع.</span><span class="sxs-lookup"><span data-stu-id="44b35-115">If any child item has a BOM, you can also select to release that child's BOM.</span></span>

1.  <span data-ttu-id="44b35-116">أغلق الصفحة للعودة إلى معالج معالج **‏‫إصدار المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="44b35-116">Close the page to return to the **Release products** wizard.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="44b35-117">[![لقطة شاشة لمعالج إصدار المنتجات مع تمييز الارتباطات الخاصة بتفاصيل الإصدار وتفاصيل المنتج.](../media/release-details.png)](../media/release-details.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44b35-117">[![Screenshot of the Release products wizard with the links to Release details and Product details highlighted.](../media/release-details.png)](../media/release-details.png#lightbox)</span></span>
    
    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="44b35-118">[![لقطة شاشة لصفحة تفاصيل إصدار المنتج التي تفتح عند تحديد ارتباط تفاصيل الإصدار.](../media/product-release-details.png)](../media/product-release-details.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44b35-118">[![Screenshot of the Product release detail page that opens when selecting the Release details link.](../media/product-release-details.png)](../media/product-release-details.png#lightbox)</span></span>

1.  <span data-ttu-id="44b35-119">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="44b35-119">Select **Next**.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="44b35-120">[![لقطة شاشة لمعالج إصدار المنتجات مع علامة اختيار في المربع "تحديد". وجميع الحقول الأخرى الموضحة في لقطة الشاشة السابقة للمنتج الأصلي معروضة.](../media/release-product-wizard.png)](../media/release-product-wizard.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44b35-120">[![Screenshot for the Release products wizard with a check mark in the Select box. All other fields that are described in the previous screenshot for the Parent product displayed.](../media/release-product-wizard.png)](../media/release-product-wizard.png#lightbox)</span></span>

1.  <span data-ttu-id="44b35-121">في الصفحة **تحديد الشركات**، حدد **موقع الشركة** و **الاستلام**.</span><span class="sxs-lookup"><span data-stu-id="44b35-121">On the **Select companies** page, select the **Company** and **Receiving site**.</span></span>

1.  <span data-ttu-id="44b35-122">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="44b35-122">Select **Next**.</span></span>

1.  <span data-ttu-id="44b35-123">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="44b35-123">Select **Finish**.</span></span>
