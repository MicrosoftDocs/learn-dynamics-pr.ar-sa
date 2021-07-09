---
ms.openlocfilehash: 5e5630869deed14429ef8c34eb88ca8d84bc145b
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072270"
---
<span data-ttu-id="b6248-101">تدعم Microsoft الترقيات من Dynamics AX 2012 R2 وR3 إلى تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="b6248-101">Microsoft supports upgrades from Dynamics AX 2012 R2 and R3 to Finance and Operations apps.</span></span> <span data-ttu-id="b6248-102">تكون جميع أدوات الترقية متاحة بشكل عام.</span><span class="sxs-lookup"><span data-stu-id="b6248-102">All tools to upgrade are generally available.</span></span> <span data-ttu-id="b6248-103">تتوفر منهجية ترقية Microsoft Dynamics 365 Lifecycle Services لمساعدتك خلال العملية.</span><span class="sxs-lookup"><span data-stu-id="b6248-103">A Microsoft Dynamics 365 Lifecycle Services upgrade methodology is available to help you through the process.</span></span>

<span data-ttu-id="b6248-104">وينقسم إجراء الترقية إلى ثلاث مراحل:</span><span class="sxs-lookup"><span data-stu-id="b6248-104">The upgrade procedure is divided into three phases:</span></span>

- <span data-ttu-id="b6248-105">**التحليل** – تقدير مهام الترقية وتحليلها، وإجراء تحليل الفروق والملاءمة، وإنشاء خطة مشروع.</span><span class="sxs-lookup"><span data-stu-id="b6248-105">**Analyze** – Estimate and analyze upgrade tasks, perform a fit-gap analysis, and create a project plan.</span></span>
- <span data-ttu-id="b6248-106">**التنفيذ** – إعداد قاعدة بيانات Dynamics AX 2012 وترقية الكود وترقية البيانات.</span><span class="sxs-lookup"><span data-stu-id="b6248-106">**Execute** – Dynamics AX 2012 database preparation, code upgrade, and data upgrade.</span></span>
- <span data-ttu-id="b6248-107">**التحقق من الصحة** – التحقق من صحة الترقية واجتياز الاختبار الوظيفي والاختبار المرحلي.</span><span class="sxs-lookup"><span data-stu-id="b6248-107">**Validate** – Upgrade validation, functional test pass, and cutover testing.</span></span>
<span data-ttu-id="b6248-108">يوضح المخطط التالي عمليه الترقية الشاملة.</span><span class="sxs-lookup"><span data-stu-id="b6248-108">The following diagram shows the overall upgrade process.</span></span>

<span data-ttu-id="b6248-109">[ ![مخطط المراحل الثلاثة لعملية الترقية الشاملة.](../media/overview.png) ](../media/overview.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b6248-109">[ ![Diagram of the three phases of the overall upgrade process.](../media/overview.png) ](../media/overview.png#lightbox)</span></span>

<span data-ttu-id="b6248-110">وسيُعتبر تحديد منهجية الترقية من الخطوات الأولى التي تتخذها عند إعداد مشروع Lifecycle Services.</span><span class="sxs-lookup"><span data-stu-id="b6248-110">Selecting your upgrade methodology will be one of the first steps that you take when setting up your Lifecycle Services project.</span></span> <span data-ttu-id="b6248-111">في مشروع Lifecycle Services الجديد، حدّد منهجية المشروع **لترقيه AX 2012 إلى تطبيقات Dynamics 365 for Finance and Operations**، التي تم تصميمها خصيصاً لعملاء AX Dynamics 2012 الذين يقومون بالترقية.</span><span class="sxs-lookup"><span data-stu-id="b6248-111">In your new Lifecycle Services project, set the project methodology to **Upgrade AX 2012 to Dynamics 365 for Finance and Operations apps**, which is specifically designed for Dynamics AX 2012 customers who are upgrading.</span></span> <span data-ttu-id="b6248-112">وتصف المنهجية المراحل الثلاث بالتفصيل كما توفر ارتباطات للوثائق الداعمة حول العملية.</span><span class="sxs-lookup"><span data-stu-id="b6248-112">The methodology describes the three phases in detail and provides links to the supporting documentation about the process.</span></span> <span data-ttu-id="b6248-113">يمكنك إعداد مشروع Lifecycle Services قبل شراء Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b6248-113">You can set up your Lifecycle Services project before you purchase Dynamics 365.</span></span>   

<span data-ttu-id="b6248-114">اتبع الخطوات التالية لإنشاء مشروع Lifecycle Services للترقية:</span><span class="sxs-lookup"><span data-stu-id="b6248-114">Follow these steps to create a new Lifecycle Services project for upgrade:</span></span> 

1. <span data-ttu-id="b6248-115">افتح مستعرضاً وانتقل إلى [https://lcs.dynamics.com](https://lcs.dynamics.com/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="b6248-115">Open a browser and go to [https://lcs.dynamics.com](https://lcs.dynamics.com/?azure-portal=true).</span></span>
1. <span data-ttu-id="b6248-116">حدد **تسجيل الدخول** وسجّل الدخول باستخدام حسابك في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="b6248-116">Select **Sign in** and sign in with your organizational account.</span></span>  
1. <span data-ttu-id="b6248-117">بعد تسجيل الدخول، حدد علامة الزائد (+) في قسم **المشاريع** لإنشاء مشروع جديد.</span><span class="sxs-lookup"><span data-stu-id="b6248-117">After you have signed in, select the plus (+) icon in the **Projects** section to create a new project.</span></span>  
1. <span data-ttu-id="b6248-118">أدخِل **اسماً** و **وصفاً** للمشروع.</span><span class="sxs-lookup"><span data-stu-id="b6248-118">Enter the **Name** for your project and a **Description**.</span></span>  
1. <span data-ttu-id="b6248-119">حدّد **Finance and Operations** **لاسم المنتج** و **إصدار المنتج**.</span><span class="sxs-lookup"><span data-stu-id="b6248-119">Select **Finance and Operations** for the **product name** and **Product version**.</span></span>  
1. <span data-ttu-id="b6248-120">حدد صناعتك في حقل **الصناعة**.</span><span class="sxs-lookup"><span data-stu-id="b6248-120">Specify your industry in the **Industry** field.</span></span>  
1. <span data-ttu-id="b6248-121">حدّد **ترقية AX 2012إلى Dynamics 365 for Finance and Operations** في حقل **المنهجية**.</span><span class="sxs-lookup"><span data-stu-id="b6248-121">Select **Upgrade AX 2012 to Dynamics 365 for Finance and Operations** in the **Methodology** field.</span></span>  
1. <span data-ttu-id="b6248-122">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="b6248-122">Select **Create**.</span></span> <span data-ttu-id="b6248-123">ستظهر كل مرحلة من مراحل منهجية الترقية على الشاشة، بطريقة مشابهة لطريقة ظهورها في لقطه الشاشة اللاحقة.</span><span class="sxs-lookup"><span data-stu-id="b6248-123">Each phase for the upgrade methodology will be shown on the screen, similar to how they’re shown in the subsequent screenshot.</span></span>  
    <span data-ttu-id="b6248-124">[ ![لقطة شاشة لصفحة منهجية الترقية.](../media/methodology.png) ](../media/methodology.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b6248-124">[ ![ Screenshot of the Upgrade methodology page.](../media/methodology.png) ](../media/methodology.png#lightbox)</span></span>
1. <span data-ttu-id="b6248-125">يمكنك تحديد كل مرحلة من المراحل والاطلاع على المهام التي يجب إكمالها في كل مرحلة، بالإضافة إلى وصف.</span><span class="sxs-lookup"><span data-stu-id="b6248-125">You can select each of the phases and see the tasks that must be completed in each of the phases, along with a description.</span></span>  







