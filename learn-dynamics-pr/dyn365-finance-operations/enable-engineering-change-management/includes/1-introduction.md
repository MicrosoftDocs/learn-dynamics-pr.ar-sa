---
ms.openlocfilehash: 345b5c8d3f8b22fadf6b73fbb8c922ad64a61df5
ms.sourcegitcommit: 9b600794e2cc61eeb0409f924725f765f528e8b1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6072655"
---
<span data-ttu-id="9c3ae-101">قبل استخدام الوظيفة الإضافية لإدارة التغيير الهندسي، يجب تمكين الميزة ومفتاح التكوين.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-101">Before using the Engineering Change Management Add-in, you must enable the feature and configuration key.</span></span>

<span data-ttu-id="9c3ae-102">لتمكين ميزة **إدارة التغيير الهندسي**، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9c3ae-102">To enable the **Engineering Change Management** feature, follow these steps:</span></span>

1. <span data-ttu-id="9c3ae-103">انتقل إلى **إدارة النظام > مساحات العمل > إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-103">Go to **System administration > Workspaces > Feature management**.</span></span>

1. <span data-ttu-id="9c3ae-104">حدد علامة التبويب **الكل**.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-104">Select the **All** tab.</span></span>

1. <span data-ttu-id="9c3ae-105">ابحث عن "**إدارة التغيير الهندسي‬**."</span><span class="sxs-lookup"><span data-stu-id="9c3ae-105">Search for '**Engineering change management**.'</span></span>

1. <span data-ttu-id="9c3ae-106">حدد الزر **تمكين** في أسفل يمين الشاشة.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-106">Select the **Enable** button in the lower right of the screen.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="9c3ae-107">[![لقطة شاشة لصفحة إدارة الميزات مع *الهندسة* في مربع البحث وميزة إدارة التغيير الهندسي مع وجود مربع أحمر حولها.](../media/engineering-feature-management.png)](../media/engineering-feature-management.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9c3ae-107">[![Screenshot of the Feature management page with *engineering* in the search box and Engineering change management feature with a red box around it.](../media/engineering-feature-management.png)](../media/engineering-feature-management.png#lightbox)</span></span>

<span data-ttu-id="9c3ae-108">إذا كنت ترغب في تمكين إدارة التغيير الهندسي بالمنتجات الموجودة في النظام.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-108">If you want to enable engineering change management on existing products in the system.</span></span> <span data-ttu-id="9c3ae-109">في هذه الحالة، يجب عليك أيضاً تمكين ميزة "**تمكين إدارة التغيير بالمنتجات الحالية‬**".</span><span class="sxs-lookup"><span data-stu-id="9c3ae-109">In that case, you must also enable the '**Enable change management on existing products**' feature.</span></span>

<span data-ttu-id="9c3ae-110">عندما تقوم بتمكين إدارة التغيير لمنتج موجود، يمكنك إنشاء إصدارات من هذا المنتج وتتبع التغييرات التي تم إجراؤها عليه طوال حياته.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-110">When you enable change management for an existing product, you can create versions of that product and trace changes made to it throughout its life.</span></span> <span data-ttu-id="9c3ae-111">لتمكين إدارة التغيير، يجب عليك تحويل المنتجات ذات الصلة إلى  *أصناف هندسية* (يشار إليها أيضاً باسم المنتجات الهندسية).</span><span class="sxs-lookup"><span data-stu-id="9c3ae-111">To enable change management, you must convert the relevant products to *engineering items* (also referred to as engineering products).</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="9c3ae-112">[![لقطة شاشة لصفحة إدارة الميزات مع "تمكين إدارة التغيير بالمنتجات الحالية" في التصفية ومربع أحمر حول الميزة.](../media/existing-products-feature.png)](../media/existing-products-feature.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9c3ae-112">[![Screenshot of the Feature management page with 'Enable change management on existing products' in the filter and a red box around the feature.](../media/existing-products-feature.png)](../media/existing-products-feature.png#lightbox)</span></span>

<span data-ttu-id="9c3ae-113">بعد ذلك، يجب عليك تشغيل مفتاح التكوين لإدارة التغيير الهندسي باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9c3ae-113">Next, you must turn on the configuration key for Engineering change management by following these steps:</span></span>

1. <span data-ttu-id="9c3ae-114">ضع نظامك في وضع الصيانة، راجع [وضع الصيانة](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/maintenance-mode/?azure-portal=true) لمعرفة كيفية القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-114">Put your system in maintenance mode, see [Maintenance mode](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/maintenance-mode/?azure-portal=true) to learn how to do that.</span></span>

1. <span data-ttu-id="9c3ae-115">انتقل إلى  **إدارة النظام** > **الإعداد** > **تكوين الترخيص**.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-115">Go to  **System administration** > **Setup** > **License configuration**.</span></span>

1. <span data-ttu-id="9c3ae-116">قم بتوسيع عقدة  **التجارة** .</span><span class="sxs-lookup"><span data-stu-id="9c3ae-116">Expand the **Trade** node.</span></span>

1. <span data-ttu-id="9c3ae-117">حدد خانة الاختيار  **إدارة التغيير الهندسي** .</span><span class="sxs-lookup"><span data-stu-id="9c3ae-117">Select the **Engineering Change Management** check box.</span></span>

1. <span data-ttu-id="9c3ae-118">قم بإيقاف تشغيل وضع الصيانة.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-118">Turn off maintenance mode.</span></span>

> [!NOTE]
> <span data-ttu-id="9c3ae-119">يجب تشغيل مفتاح تكوين إضافي للعمل مع إصدارات المنتج.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-119">An additional configuration key must be turned on to work with product versions.</span></span> <span data-ttu-id="9c3ae-120">راجع [إنشاء مجموعات أبعاد المنتجات باستخدام بُعد الإصدار](https://docs.microsoft.com/learn/modules/set-up-versioned-products-engineering-change-management/5-dimension-groups/?azure-portal=true) لمعرفة المزيد.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-120">See [Create product dimension groups using the version dimension](https://docs.microsoft.com/learn/modules/set-up-versioned-products-engineering-change-management/5-dimension-groups/?azure-portal=true) to learn more.</span></span>

<span data-ttu-id="9c3ae-121">الآن بعد أن قمت بتمكين الميزات المطلوبة لاستخدام وظيفة إدارة التغيير الهندسي، أنت جاهز لإعداد الوظائف التي سيستخدمها عملك.</span><span class="sxs-lookup"><span data-stu-id="9c3ae-121">Now that you've enabled the features required to use the engineering change management functionality, you're ready to set up the functions that your business will use.</span></span>
