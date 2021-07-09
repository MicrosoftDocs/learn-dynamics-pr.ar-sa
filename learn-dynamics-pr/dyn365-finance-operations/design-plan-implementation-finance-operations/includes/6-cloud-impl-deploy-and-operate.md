---
ms.openlocfilehash: 99a1d4659d40ca336d019c6fa3c00521a7426013
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071709"
---
<span data-ttu-id="81fc2-101">تعد هذه الوحدة ملخصاً للخطوات الواردة في خطوات نشر وتشغيل تنفيذ مجموعة النظراء لتطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="81fc2-101">This unit is a summary of the steps in the deploy and operate steps of a cloud implementation of Finance and Operations apps.</span></span>

## <a name="deploy"></a><span data-ttu-id="81fc2-102">توزيع</span><span class="sxs-lookup"><span data-stu-id="81fc2-102">Deploy</span></span>

### <a name="deploy-production-environment"></a><span data-ttu-id="81fc2-103">نشر بيئة الإنتاج</span><span class="sxs-lookup"><span data-stu-id="81fc2-103">Deploy production environment</span></span>

<span data-ttu-id="81fc2-104">يمكن نشر بيئات الإنتاج من خلال Lifecycle Service‏ (LCS) عن طريق استكمال قائمه الاختيار الخاصة بالتزويد.</span><span class="sxs-lookup"><span data-stu-id="81fc2-104">Production environments can be deployed through Lifecycle Service (LCS) by completing the provisioning checklist.</span></span> <span data-ttu-id="81fc2-105">يمكنك البدء في استكمال قائمة الاختيار الخاصة بالتزويد، بعد تحديد مرشح الإصدار في الحزم القابلة للنشر للبرامج وحزم البيانات في مكتبه الأصول LCS واستيفاء جميع المتطلبات الأساسية.</span><span class="sxs-lookup"><span data-stu-id="81fc2-105">After you have the release candidate identified from your software deployable packages and data packages in the LCS Asset library and all prerequisites are met, you can start completing the provisioning checklist.</span></span> 

<span data-ttu-id="81fc2-106">يتطلب إدخال نشر الإنتاج قيام ممثل المؤسسة الذي يمتلك المشروع بتسجيل الخروج.</span><span class="sxs-lookup"><span data-stu-id="81fc2-106">Production deployment input needs sign-off from a representative of the organization who owns the project.</span></span> <span data-ttu-id="81fc2-107">ستتم إضافة هذا المستخدم كمسؤول عن تطبيقات Finance and Operations أثناء عملية التزويد.</span><span class="sxs-lookup"><span data-stu-id="81fc2-107">This user will be added as a Finance and Operations apps administrator during provisioning.</span></span> <span data-ttu-id="81fc2-108">سيراجع فريق الموثوقية بموقع Microsoft أيضاً الإدخالات ومتطلبات تسجيل الخروج، التي ستبدأ عملية النشر.</span><span class="sxs-lookup"><span data-stu-id="81fc2-108">Microsoft’s site reliability team will also review the inputs and sign-off requirements, which will initiate the deployment.</span></span>

### <a name="perform-mock-cutover"></a><span data-ttu-id="81fc2-109">تنفيذ التكوين المرحلي الوهمي</span><span class="sxs-lookup"><span data-stu-id="81fc2-109">Perform mock cutover</span></span>

<span data-ttu-id="81fc2-110">للتأكد من نجاح حزم التعليمات البرمجية والبيئة والبيانات، يجب إجراء تكوين مرحلي وهمي.</span><span class="sxs-lookup"><span data-stu-id="81fc2-110">To ensure that environment, data, and code packages are successful, a mock cutover should be performed.</span></span> <span data-ttu-id="81fc2-111">تتشابه عملية التكوين المرحلي الوهمي مع التحقق من صحة ترقية البيانات الأساسية في بيئة اختبار معزولة.</span><span class="sxs-lookup"><span data-stu-id="81fc2-111">The mock cutover process is similar to a basic data upgrade validation in a sandbox environment.</span></span> 

### <a name="monitor-system-health"></a><span data-ttu-id="81fc2-112">مراقبة سلامة النظام</span><span class="sxs-lookup"><span data-stu-id="81fc2-112">Monitor system health</span></span>

<span data-ttu-id="81fc2-113">يمكنك سلامة النظام، في أي مرحلة، باستخدام لوحة معلومات **المراقبة والتشخيص** في LCS.</span><span class="sxs-lookup"><span data-stu-id="81fc2-113">At any point, you can monitor the system health by using the **Monitoring and diagnostics** dashboard in LCS.</span></span> <span data-ttu-id="81fc2-114">يمكنك إصلاح أية مشكلات موجودة في البيئة.</span><span class="sxs-lookup"><span data-stu-id="81fc2-114">You can fix any issues found in the environment.</span></span>

### <a name="perform-go-live-health-check"></a><span data-ttu-id="81fc2-115">إجراء التحقق من سلامة العرض المباشر</span><span class="sxs-lookup"><span data-stu-id="81fc2-115">Perform Go-live health check</span></span>

<span data-ttu-id="81fc2-116">يجب على فريق المشروع بأكمله المشاركة في التحقق من سلامة العرض المباشر لضمان أن كافة أوجه النظام تعمل كما هو متوقع؛ من الناحية الوظيفية والفنية على السواء.</span><span class="sxs-lookup"><span data-stu-id="81fc2-116">The entire project team should participate in a Go-live health check to ensure that all aspects of the system are operating as expected; both functionally and technically.</span></span>

## <a name="operate"></a><span data-ttu-id="81fc2-117">التشغيل</span><span class="sxs-lookup"><span data-stu-id="81fc2-117">Operate</span></span>

### <a name="get-updates-from-microsoft"></a><span data-ttu-id="81fc2-118">الحصول على تحديثات من Microsoft</span><span class="sxs-lookup"><span data-stu-id="81fc2-118">Get updates from Microsoft</span></span>
<span data-ttu-id="81fc2-119">يمكنك تنزيل الإصلاحات الضرورية المتعلقة بأي بيئة من صفحة **البيئة**.</span><span class="sxs-lookup"><span data-stu-id="81fc2-119">At any point in the lifecycle, you can download hotfixes relevant to any environment from the **Environment** page.</span></span>

### <a name="support-tickets"></a><span data-ttu-id="81fc2-120">تذاكر الدعم</span><span class="sxs-lookup"><span data-stu-id="81fc2-120">Support tickets</span></span>

<span data-ttu-id="81fc2-121">يمكنك رفع تذكره دعم مع Microsoft باستخدام خدمة الدعم في LCS.</span><span class="sxs-lookup"><span data-stu-id="81fc2-121">You can raise a support ticket with Microsoft using the support service in LCS.</span></span>

### <a name="microsoft-site-reliability-work-orders"></a><span data-ttu-id="81fc2-122">أوامر العمل الخاصة بموثوقية موقع Microsoft</span><span class="sxs-lookup"><span data-stu-id="81fc2-122">Microsoft site reliability work orders</span></span>
<span data-ttu-id="81fc2-123">يمكنك الاتصال بدعم Microsoft للحصول على أوامر العمل الخاصة بفريق موثوقية Microsoft.</span><span class="sxs-lookup"><span data-stu-id="81fc2-123">You can contact Microsoft support for Microsoft site reliability team work orders.</span></span>
 
