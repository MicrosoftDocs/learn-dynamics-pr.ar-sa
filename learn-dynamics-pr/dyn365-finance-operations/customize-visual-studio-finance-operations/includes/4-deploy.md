---
ms.openlocfilehash: b3bee359f9714f5eb40438d2a31cdf56c32b32e3
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071412"
---
<span data-ttu-id="c9f13-101">لتطبيق تغييرات التعليمات البرمجية الخاصة بك على بيئة غير تطويرية، قم بإنشاء حزمة برامج قابلة للنشر (SDP) وقمّ بتحميلها إلى Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="c9f13-101">To apply your code changes to a non-development environment, build a Software Deployable Package (SDP) and upload it to Lifecycle Services (LCS).</span></span> <span data-ttu-id="c9f13-102">يتيح ذلك عملية تطبيق التعليمات البرمجية الموثوقة والقابلة للتكرار مع اقتراب التعليمات البرمجية الخاصة بك من الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="c9f13-102">This allows for a reliable and repeatable code application process as your code gets closer to production.</span></span> 

<span data-ttu-id="c9f13-103">لإنشاء حزمة برامج قابلة للنشر من Visual Studio، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="c9f13-103">To build an SDP from Visual Studio, follow these steps.</span></span>

1.  <span data-ttu-id="c9f13-104">انتقل إلى **عمليات الإنشاء** في مستكشف الفريق.</span><span class="sxs-lookup"><span data-stu-id="c9f13-104">Go to **Builds** in Team Explorer.</span></span>
2.  <span data-ttu-id="c9f13-105">انقر بزر الماوس الأيمن فوق تعريف الإنشاء المطلوب.</span><span class="sxs-lookup"><span data-stu-id="c9f13-105">Right-click the desired build definition.</span></span>
3.  <span data-ttu-id="c9f13-106">حدد **وضع قائمة انتظار لإنشاء جديد**.</span><span class="sxs-lookup"><span data-stu-id="c9f13-106">Select **Queue New Build**.</span></span>
4.  <span data-ttu-id="c9f13-107">في نافذة المستعرض التي تفتح، قُم بتسجيل الدخول إلى Azure DevOps (ما لم يتم تسجيل دخولك تلقائياً).</span><span class="sxs-lookup"><span data-stu-id="c9f13-107">In the browser window that opens, sign in to Azure DevOps (unless you are automatically signed in).</span></span>
5.  <span data-ttu-id="c9f13-108">استخدم زر **قائمة الانتظار** لفتح مربع الحوار قائمة انتظار الإنشاء.</span><span class="sxs-lookup"><span data-stu-id="c9f13-108">Use the **Queue** button to open the build queue dialog box.</span></span>
6.  <span data-ttu-id="c9f13-109">أدخل أي محددات تحتاج إليها في مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="c9f13-109">Enter any parameters that you need to in the dialog box.</span></span>
7.  <span data-ttu-id="c9f13-110">حدد **تأكيد** لوضع قائمة انتظار للإنشاء.</span><span class="sxs-lookup"><span data-stu-id="c9f13-110">Select **Confirm** to queue the build.</span></span>

<span data-ttu-id="c9f13-111">عند اكتمال الإنشاء، تتوفر السجلات والتعليمات البرمجية التي تم إنشاؤها للتنزيل.</span><span class="sxs-lookup"><span data-stu-id="c9f13-111">When the build completes, the logs and the built code are available to download.</span></span> <span data-ttu-id="c9f13-112">التعليمات البرمجية متوفرة فقط في النماذج التي تتضمنها أو ما تطلق عليه Azure DevOps وقت تشغيل AX القابل للنشر.</span><span class="sxs-lookup"><span data-stu-id="c9f13-112">The code is available as just the models that it includes, or as what Azure DevOps calls an AX Deployable Runtime.</span></span> <span data-ttu-id="c9f13-113">يعد وقت تشغيل AX القابل للنشر هو حزمة برامج قابلة للنشر.</span><span class="sxs-lookup"><span data-stu-id="c9f13-113">The AX Deployable Runtime is an SDP.</span></span> <span data-ttu-id="c9f13-114">يمكن الوصول إلى كافة هذه التحميلات باستخدام زر **البيانات الاصطناعية‬** في صفحة حالة الإنشاء المكتمل.</span><span class="sxs-lookup"><span data-stu-id="c9f13-114">All these downloads are accessible by using the **Artifacts** button on a completed build's status page.</span></span>

<span data-ttu-id="c9f13-115">يمكنك استخدام Visual Studio لمراقبة وتعقب عمليات إنشاء Azure DevOps الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="c9f13-115">You can use Visual Studio to monitor and track your Azure DevOps builds.</span></span>
<span data-ttu-id="c9f13-116">من شاشة **عمليات الإنشاء** لمستكشف الفريق، تكون عمليات الإنشاء النشطة مرئية في القسم **عمليات الإنشاء الخاصة بي**.</span><span class="sxs-lookup"><span data-stu-id="c9f13-116">From the **Builds** screen of Team Explorer, your active builds are visible in the **My Builds** section.</span></span> <span data-ttu-id="c9f13-117">يقوم كل إدخال بملاحظة وقت تغيير الحالة الأخير، مثل "بدأ منذ 20 دقيقة" أو "تم منذ 6 ثوانِ".</span><span class="sxs-lookup"><span data-stu-id="c9f13-117">Each entry notes the time of the last status change, such as "started 20 minutes ago" or "completed 6 seconds ago."</span></span> <span data-ttu-id="c9f13-118">عند اكتمال الإنشاء، يمكنك تنزيل وقت تشغيل AX القابل للنشر الناتج من موقع مشروع Azure DevOps المتصل به وتحميله إلى مكتبة أصول LCS.</span><span class="sxs-lookup"><span data-stu-id="c9f13-118">When the build completes, you can download the resulting AX Deployable Runtime from the connected Azure DevOps project site and upload it to the LCS Asset Library.</span></span>

<span data-ttu-id="c9f13-119">شاهد الفيديو التالي للتعرّف على كيفية إنشاء حزمة قابلة للنشر.</span><span class="sxs-lookup"><span data-stu-id="c9f13-119">Watch the following video to learn about creating a deployable package.</span></span> 

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4byCh]

