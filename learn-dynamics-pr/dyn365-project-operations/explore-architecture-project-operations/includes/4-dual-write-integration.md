---
ms.openlocfilehash: 03e485513a32c953ff59cc1747e668568413b2e3
ms.sourcegitcommit: 0a6b3a31165f421c2f7d3afb98b75c9100325f57
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2021
ms.locfileid: "6083804"
---
<span data-ttu-id="633e2-101">تعد الكتابة المزدوجة هي بنيه أساسية جاهزة توفر تفاعلاً قريباً من الوقت الحقيقي بين تطبيقات Customer Engagement وتطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="633e2-101">Dual-write is an out-of-the-box infrastructure that provides near real-time interaction between customer engagement apps and Finance and Operations apps.</span></span> <span data-ttu-id="633e2-102">عندما تتدفق البيانات حول العملاء والمنتجات والأفراد والعمليات خارج حدود التطبيق، يتم تمكين جميع الأقسام في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="633e2-102">When data about customers, products, people, and operations flows beyond application boundaries, all departments in an organization are empowered.</span></span>

<span data-ttu-id="633e2-103">توفر الكتابة المزدوجة تكاملاً مقترناً بشكل وثيق ثنائي الاتجاه بين تطبيقات Finance and Operations وDataverse.</span><span class="sxs-lookup"><span data-stu-id="633e2-103">Dual-write provides tightly coupled, bidirectional integration between Finance and Operations apps and Dataverse.</span></span> <span data-ttu-id="633e2-104">تؤدي تغييرات البيانات في تطبيقات Finance and Operations إلى الكتابة إلى Dataverse، وتؤدي تغييرات البيانات في Dataverse إلى الكتابة إلى تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="633e2-104">Data changes in Finance and Operations apps cause writes to Dataverse, and data changes in Dataverse cause writes to Finance and Operations apps.</span></span> <span data-ttu-id="633e2-105">يوفر تدفق البيانات الآلي هذا تجربة مستخدم متكاملة عبر التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="633e2-105">This automated data flow provides an integrated user experience across the apps.</span></span>

<span data-ttu-id="633e2-106">تتضمن الكتابة المزدوجة جانبين: **البنية الأساسية** و **التطبيق**.</span><span class="sxs-lookup"><span data-stu-id="633e2-106">Dual-write has two aspects: **infrastructure** and **application**.</span></span>

## <a name="infrastructure-aspect"></a><span data-ttu-id="633e2-107">جانب البنية الأساسية</span><span class="sxs-lookup"><span data-stu-id="633e2-107">Infrastructure aspect</span></span>

<span data-ttu-id="633e2-108">تعد البنية الأساسية للكتابة المزدوجة قابلة للتوسعة ويمكن الاعتماد عليها وتتضمن الميزات الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="633e2-108">Dual-write infrastructure is extensible and reliable and includes the following key features:</span></span>

-   <span data-ttu-id="633e2-109">تدفق البيانات المتزامن وثنائي الاتجاه بين التطبيقات</span><span class="sxs-lookup"><span data-stu-id="633e2-109">Synchronous and bidirectional data flow between applications</span></span>

-   <span data-ttu-id="633e2-110">المزامنة، جنباً إلى جنب مع أوضاع التشغيل والإيقاف المؤقت والالتقاط لدعم النظام أثناء أوضاع الاتصال بالإنترنت وعدم الاتصال/غير المتزامن</span><span class="sxs-lookup"><span data-stu-id="633e2-110">Synchronization, together with play, pause, and catch-up modes to support the system during online and offline/asynchronous modes</span></span>

-   <span data-ttu-id="633e2-111">القدرة على مزامنة البيانات الأولية بين التطبيقات</span><span class="sxs-lookup"><span data-stu-id="633e2-111">Ability to sync initial data between the applications</span></span>

-   <span data-ttu-id="633e2-112">طريقة عرض مدمجة لسجلات النشاط والأخطاء لمسؤولي البيانات</span><span class="sxs-lookup"><span data-stu-id="633e2-112">Combined view of activity and error logs for data admins</span></span>

-   <span data-ttu-id="633e2-113">القدرة على تكوين التنبيهات والحدود المخصصة، وللاشتراك في الإخطارات</span><span class="sxs-lookup"><span data-stu-id="633e2-113">Ability to configure custom alerts and thresholds and to subscribe to notifications</span></span>

-   <span data-ttu-id="633e2-114">واجهة مستخدم بديهية (UI) للتصفية والتحويلات</span><span class="sxs-lookup"><span data-stu-id="633e2-114">Intuitive user interface (UI) for filtering and transformations</span></span>

-   <span data-ttu-id="633e2-115">القدرة على تعيين تبعيات الكيانات والعلاقات وعرضها</span><span class="sxs-lookup"><span data-stu-id="633e2-115">Ability to set and view entity dependencies and relationships</span></span>

-   <span data-ttu-id="633e2-116">القابلية للتوسعة للكيانات والمخططات القياسية والمخصصة</span><span class="sxs-lookup"><span data-stu-id="633e2-116">Extensibility for standard and custom entities and maps</span></span>

-   <span data-ttu-id="633e2-117">إدارة دورة حياة التطبيق الموثوقة (ALM)</span><span class="sxs-lookup"><span data-stu-id="633e2-117">Reliable application lifecycle management (ALM)</span></span>

-   <span data-ttu-id="633e2-118">تجربة إعداد جاهزة للعملاء الجدد</span><span class="sxs-lookup"><span data-stu-id="633e2-118">Out-of-the-box setup experience for new customers</span></span>

## <a name="application-aspect"></a><span data-ttu-id="633e2-119">جانب التطبيق</span><span class="sxs-lookup"><span data-stu-id="633e2-119">Application aspect</span></span>

<span data-ttu-id="633e2-120">تعمل الكتابة المزدوجة على إنشاء تعيين بين المفاهيم في تطبيقات Finance and Operations والمفاهيم في تطبيقات Customer Engagement.</span><span class="sxs-lookup"><span data-stu-id="633e2-120">Dual-write creates mapping between concepts in Finance and Operations apps and concepts in customer engagement apps.</span></span> <span data-ttu-id="633e2-121">يدعم هذا التكامل السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="633e2-121">This integration supports the following scenarios:</span></span>

-   <span data-ttu-id="633e2-122">أصل العميل المتكامل</span><span class="sxs-lookup"><span data-stu-id="633e2-122">Integrated customer master</span></span>

-   <span data-ttu-id="633e2-123">الوصول إلى بطاقات ولاء العملاء ونقاط المكافآت</span><span class="sxs-lookup"><span data-stu-id="633e2-123">Access to customer loyalty cards and reward points</span></span>

-   <span data-ttu-id="633e2-124">تجربه إدارة المنتج الموحدة</span><span class="sxs-lookup"><span data-stu-id="633e2-124">Unified product mastering experience</span></span>

-   <span data-ttu-id="633e2-125">توعية التدرج الهرمي للمؤسسات</span><span class="sxs-lookup"><span data-stu-id="633e2-125">Awareness of organization hierarchy</span></span>

-   <span data-ttu-id="633e2-126">أصل المورّد المتكامل</span><span class="sxs-lookup"><span data-stu-id="633e2-126">Integrated vendor master</span></span>

-   <span data-ttu-id="633e2-127">الوصول إلى البيانات المالية وبيانات مرجع الضريبة</span><span class="sxs-lookup"><span data-stu-id="633e2-127">Access to finance and tax reference data</span></span>

-   <span data-ttu-id="633e2-128">تجربة محرك أسعار حسب الطلب</span><span class="sxs-lookup"><span data-stu-id="633e2-128">On-demand price engine experience</span></span>

-   <span data-ttu-id="633e2-129">تجربة متكاملة من العميل المتوقع إلى النقدي</span><span class="sxs-lookup"><span data-stu-id="633e2-129">Integrated prospect-to-cash experience</span></span>

-   <span data-ttu-id="633e2-130">القدرة على خدمة الأصول الداخلية وأصول العملاء من خلال وكلاء ميدانيين</span><span class="sxs-lookup"><span data-stu-id="633e2-130">Ability to serve in-house assets and customer assets through field agents</span></span>

-   <span data-ttu-id="633e2-131">تجربة الشراء إلى الدفع المتكاملة</span><span class="sxs-lookup"><span data-stu-id="633e2-131">Integrated procure-to-pay experience</span></span>

-   <span data-ttu-id="633e2-132">أنشطة وملاحظات متكاملة لبيانات العملاء ومستنداتهم</span><span class="sxs-lookup"><span data-stu-id="633e2-132">Integrated activities and notes for customer data and documents</span></span>

-   <span data-ttu-id="633e2-133">القدرة على البحث عن توافر المخزون الفعلي والتفاصيل</span><span class="sxs-lookup"><span data-stu-id="633e2-133">Ability to look up on-hand inventory availability and details</span></span>

-   <span data-ttu-id="633e2-134">تجربة المشروع إلى النقد</span><span class="sxs-lookup"><span data-stu-id="633e2-134">Project-to-cash experience</span></span>

-   <span data-ttu-id="633e2-135">القدرة على معالجة العديد من العناوين والأدوار من خلال مفهوم الطرف</span><span class="sxs-lookup"><span data-stu-id="633e2-135">Ability to handle multiple addresses and roles through the party concept</span></span>

-   <span data-ttu-id="633e2-136">إدارة مصدر واحد للمستخدمين</span><span class="sxs-lookup"><span data-stu-id="633e2-136">Single source management for users</span></span>

-   <span data-ttu-id="633e2-137">قنوات متكاملة للبيع بالتجزئة والتسويق</span><span class="sxs-lookup"><span data-stu-id="633e2-137">Integrated channels for retailing and marketing</span></span>

-   <span data-ttu-id="633e2-138">الرؤية في العروض الترويجية والخصومات</span><span class="sxs-lookup"><span data-stu-id="633e2-138">Visibility into promotions and discounts</span></span>

-   <span data-ttu-id="633e2-139">وظائف طلب الخدمة</span><span class="sxs-lookup"><span data-stu-id="633e2-139">Request-for-service functions</span></span>

-   <span data-ttu-id="633e2-140">عمليات الخدمة المبسطة</span><span class="sxs-lookup"><span data-stu-id="633e2-140">Streamlined service operations</span></span>

<span data-ttu-id="633e2-141">توفر الكتابة المزدوجة تكامل البيانات عبر تطبيقات Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="633e2-141">Dual-write provides data integration across Microsoft Dynamics 365 applications.</span></span> <span data-ttu-id="633e2-142">يربط إطار العمل القوي هذا البيئات ويمكّن تطبيقات الأعمال المختلفة من العمل معاً.</span><span class="sxs-lookup"><span data-stu-id="633e2-142">This robust framework links environments and enables different business applications to work together.</span></span>

<span data-ttu-id="633e2-143">فيما يلي أسباب استخدام إطار عمل الكتابة المزدوجة:</span><span class="sxs-lookup"><span data-stu-id="633e2-143">Reasons for using the dual-write framework include:</span></span>

-   <span data-ttu-id="633e2-144">يوفر تكاملاً مقترناً بشكل وثيق ثنائي الاتجاه وقريب من الوقت الحقيقي بين تطبيقات Finance and Operations والتطبيقات المستندة إلى النموذج في Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="633e2-144">It provides tightly coupled, near real-time, and bidirectional integration between Finance and Operations apps and model-driven apps in Dynamics 365.</span></span> <span data-ttu-id="633e2-145">ويجعل هذا التكامل تطبيقات Microsoft Dynamics 365 مكاناً واحداً للانتقال إلى كافة حلول الأعمال الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="633e2-145">This integration makes Microsoft Dynamics 365 the one place to go for all your business solutions.</span></span> <span data-ttu-id="633e2-146">ينتقل العملاء الذين يستخدمون Dynamics 365 Finance وDynamics 365 Supply Chain Management، ولكن لا يستخدمون حلولاً غير تابعة لـ Microsoft لإدارة علاقة العملاء (CRM)، إلى Dynamics 365 لدعم الكتابة المزدوجة.</span><span class="sxs-lookup"><span data-stu-id="633e2-146">Customers who use Dynamics 365 Finance and Dynamics 365 Supply Chain Management, but who use non-Microsoft solutions for customer relationship management (CRM), are moving toward Dynamics 365 for its dual-write support.</span></span>

-   <span data-ttu-id="633e2-147">البيانات الواردة من العملاء والمنتجات والعمليات والمشاريع وإنترنت الأشياء (IoT) تتدفق تلقائياً إلى Dataverse خلال الكتابة المزدوجة.</span><span class="sxs-lookup"><span data-stu-id="633e2-147">Data from customers, products, operations, projects, and the Internet of Things (IoT) automatically flows to Dataverse through dual-write.</span></span> <span data-ttu-id="633e2-148">يُعد هذا الاتصال مفيداً للأعمال المهتمة بتوسعات Power Platform.</span><span class="sxs-lookup"><span data-stu-id="633e2-148">This connection is useful for businesses that are interested in Power Platform expansions.</span></span>

-   <span data-ttu-id="633e2-149">تتبع البنية الأساسية مبدأ بدون تعليمات برمجية/تعليمات برمجية منخفضة.</span><span class="sxs-lookup"><span data-stu-id="633e2-149">The infrastructure follows the no-code/low-code principle.</span></span> <span data-ttu-id="633e2-150">الحد الأدنى من الجهد الهندسي مطلوب لتوسيع الخرائط القياسية من جدول إلى جدول ولتضمين خرائط مخصصة.</span><span class="sxs-lookup"><span data-stu-id="633e2-150">Minimal engineering effort is required to extend the standard table-to-table maps and to include custom maps.</span></span>

-   <span data-ttu-id="633e2-151">يدعم كلاً من الوضع عبر الإنترنت والوضع دون اتصال.</span><span class="sxs-lookup"><span data-stu-id="633e2-151">It supports online mode and offline mode.</span></span> <span data-ttu-id="633e2-152">شركه Microsoft هي الشركة الوحيدة التي تقدم الدعم للوضع المتصل ودون اتصال.</span><span class="sxs-lookup"><span data-stu-id="633e2-152">Microsoft is the only company that offers support for online and offline modes.</span></span>
