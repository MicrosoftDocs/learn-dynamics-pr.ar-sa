---
ms.openlocfilehash: 1ec0767705106696d38140734ad28a02d2e4a312
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073673"
---
<span data-ttu-id="f2664-101">المواقع هي أبعاد تخزين المخزون ويمكن ربطها بإطار عمل الأبعاد المالية لتكامل دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="f2664-101">Sites are inventory storage dimensions and can be linked to the financial dimensions framework for general ledger integration.</span></span> <span data-ttu-id="f2664-102">يجب إنشاء موقع واحد على الأقل لكل كيان قانوني في Supply Chain Management، ويجب أن تشير جميع الحركات إلى موقع.</span><span class="sxs-lookup"><span data-stu-id="f2664-102">At least one site must be created for each legal entity in Supply Chain Management, and all transactions must refer to a site.</span></span> <span data-ttu-id="f2664-103">لا يمكن مشاركة موقع واحد بواسطة كيانات قانونية متعددة.</span><span class="sxs-lookup"><span data-stu-id="f2664-103">A single site cannot be shared by multiple legal entities.</span></span> <span data-ttu-id="f2664-104">يمكن للشركة إنشاء عمليات لوجستية في مواقع متعددة لأسباب عديدة.</span><span class="sxs-lookup"><span data-stu-id="f2664-104">A company can establish logistic operations at multiple sites for many reasons.</span></span>

<span data-ttu-id="f2664-105">على الرغم من أن المواقع هي الإعداد الوحيد المطلوب، إلا أننا نوصي بإعداد أبعاد المخزون الأخرى بناءً على متطلبات العمل.</span><span class="sxs-lookup"><span data-stu-id="f2664-105">Although sites are the only required setup, we recommend that you set up the other inventory dimensions based on business requirements.</span></span> 

<span data-ttu-id="f2664-106">يوفر كل إعداد لأبعاد المخزون المادي مستوى آخر من التفاصيل لتخزين وإصدار المخزون في نظامك.</span><span class="sxs-lookup"><span data-stu-id="f2664-106">Each physical inventory dimension setup provides another level of detail for storing and issuing inventory in your system.</span></span> <span data-ttu-id="f2664-107">يساعد هذا في توفير تقارير مفصلة بشكل أفضل وكميات متاحة تكون أكثر تحديداً للموقع الفعلي للعناصر.</span><span class="sxs-lookup"><span data-stu-id="f2664-107">This helps provide better detailed reporting and on-hand quantities that are more specific to the physical location of the items.</span></span>

<span data-ttu-id="f2664-108">قد تتضمن إعدادات أبعاد المخزون المادي هذه إنشاء مراكز توزيع تخدم أسواقاً جغرافية مختلفة أو إنشاء مرافق إنتاج في موقع ما بسبب انخفاض التكاليف العامة أو القرب من المواد الخام أو النقل المريح.</span><span class="sxs-lookup"><span data-stu-id="f2664-108">These physical inventory dimension setups might include setting up distribution centers that serve different geographic markets or setting up production facilities at a location because of reduced overhead costs, closeness to raw materials, or convenient transportation.</span></span>

<span data-ttu-id="f2664-109">على سبيل المثال، يمكنك تكوين مواقع متعددة لتعكس نموذج عملك الفريد ودعم العمليات وعمليات سير مهام العمليات.</span><span class="sxs-lookup"><span data-stu-id="f2664-109">For example, you can configure multiple sites to reflect your unique business model and support operations and process flows.</span></span> <span data-ttu-id="f2664-110">تتضمن أمثلة بيئات العمل حيث يمكنك إنشاء مواقع متعددة ما يلي:</span><span class="sxs-lookup"><span data-stu-id="f2664-110">Examples of business environments where you could set up multiple sites include the following:</span></span>

- <span data-ttu-id="f2664-111">موقع إنتاج واحد يستخدم مستودعاً واحداً</span><span class="sxs-lookup"><span data-stu-id="f2664-111">A single production site that uses a single warehouse</span></span>
- <span data-ttu-id="f2664-112">موقع إنتاج واحد يستخدم مستودعات متعددة</span><span class="sxs-lookup"><span data-stu-id="f2664-112">A single production site that uses multiple warehouses</span></span>
- <span data-ttu-id="f2664-113">مواقع إنتاج متعددة تستخدم مركز توزيع مشتركاً</span><span class="sxs-lookup"><span data-stu-id="f2664-113">Multiple production sites that use a shared distribution center</span></span>
- <span data-ttu-id="f2664-114">مواقع إنتاج محلية متعددة تستخدم موقع إنتاج مشتركاً</span><span class="sxs-lookup"><span data-stu-id="f2664-114">Multiple local production sites that use a shared production site</span></span>

<span data-ttu-id="f2664-115">لإنشاء موقع جديد، انتقل إلى **إدارة المخزون > الإعداد > تقسيم المخزون > المواقع**.</span><span class="sxs-lookup"><span data-stu-id="f2664-115">To create a new site, go to **Inventory management > Setup > Inventory breakdown > Sites**.</span></span>
 
![لقطة شاشة لعلامة التبويب السريعة التدرج الهرمي في صفحة المواقع.](../media/sites-1.png)

<span data-ttu-id="f2664-117">عند إنشاء موقع، يمكنك حذفه فقط إذا:</span><span class="sxs-lookup"><span data-stu-id="f2664-117">When you have created a site, you can only delete it if:</span></span>

- <span data-ttu-id="f2664-118">لم تتم الإشارة إلى الموقع من المستودعات أو موارد الإنتاج أو البيانات الرئيسية الأخرى.</span><span class="sxs-lookup"><span data-stu-id="f2664-118">The site is not referenced from warehouses, production resources, or other master data.</span></span>
- <span data-ttu-id="f2664-119">كان لا يوجد مخزون متاح مفتوح مرتبط بالموقع.</span><span class="sxs-lookup"><span data-stu-id="f2664-119">There is no open on-hand inventory that is associated with the site.</span></span>

<span data-ttu-id="f2664-120">إذا لم تتحقق أي من هذه الشروط، تعرض Supply Chain Management رسالة خطأ، ولا يمكنك حذف الموقع.</span><span class="sxs-lookup"><span data-stu-id="f2664-120">If either of these conditions are not true, Supply Chain Management displays an error message, and you cannot delete the site.</span></span>
