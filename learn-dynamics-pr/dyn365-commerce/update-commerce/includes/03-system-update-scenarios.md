---
ms.openlocfilehash: b82ff90fcb4b34a3611803a3e568ac9c486187c1
ms.sourcegitcommit: ca87deefdcd512d3b8e382cd49adf8a15d5995fc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/02/2021
ms.locfileid: "6070449"
---
<span data-ttu-id="63eba-101">يمكن إجراء عملية تحديث التجارة في عدة سيناريوهات.</span><span class="sxs-lookup"><span data-stu-id="63eba-101">The update process of Commerce can be performed in several scenarios.</span></span> <span data-ttu-id="63eba-102">يتم تمييز هذه السيناريوهات بناءً على نوع التحديث الذي سيتم تطبيقه.</span><span class="sxs-lookup"><span data-stu-id="63eba-102">These scenarios are differentiated depending on the type of update that will be applied.</span></span> <span data-ttu-id="63eba-103">السيناريوهات المحتملة هي:</span><span class="sxs-lookup"><span data-stu-id="63eba-103">The possible scenarios are:</span></span>

- <span data-ttu-id="63eba-104">التحديث التلقائي</span><span class="sxs-lookup"><span data-stu-id="63eba-104">Auto update</span></span>
- <span data-ttu-id="63eba-105">التحديث الذاتي</span><span class="sxs-lookup"><span data-stu-id="63eba-105">Self-update</span></span> 
- <span data-ttu-id="63eba-106">الإصدار الأول</span><span class="sxs-lookup"><span data-stu-id="63eba-106">First release</span></span>

## <a name="auto-update"></a><span data-ttu-id="63eba-107">التحديث التلقائي</span><span class="sxs-lookup"><span data-stu-id="63eba-107">Auto update</span></span>
<span data-ttu-id="63eba-108">يُعرف التحديث التلقائي أيضاً باسم **إصدار واحدة** والغرض من ذلك هو أن جميع العملاء يستخدمون نفس الإصدار عبر النظام الأساسي.</span><span class="sxs-lookup"><span data-stu-id="63eba-108">Auto update is also known as **One Version**, the purpose being that all customers are using the same version across the platform.</span></span> <span data-ttu-id="63eba-109">تصبح التحديثات عبارة عن تحديثات لا تعمل باللمس، مما يعني أن التحديثات تتم تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="63eba-109">The updates become zero touch updates, meaning that the updates are automated.</span></span> 

<span data-ttu-id="63eba-110">يتيح هذا السيناريو التحديث التلقائي لـ TEST،UAT،Sandbox والإنتاج، وهو موضح في الصورة التالية.</span><span class="sxs-lookup"><span data-stu-id="63eba-110">This scenario enables the automatic update of TEST, UAT, Sandbox, and Production, and it is illustrated in the following image.</span></span>

<span data-ttu-id="63eba-111">[![رسم تخطيطي لـ Dynamics 365 Commerce سيناريو التحديث التلقائي.](../media/auto-update.jpg)](../media/auto-update.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63eba-111">[![Diagram of the Dynamics 365 Commerce auto-update scenario.](../media/auto-update.jpg)](../media/auto-update.jpg#lightbox)</span></span>


## <a name="self-update"></a><span data-ttu-id="63eba-112">التحديث الذاتي</span><span class="sxs-lookup"><span data-stu-id="63eba-112">Self-update</span></span>
<span data-ttu-id="63eba-113">ينطبق نهج التحديث الذاتي على متاجر الطوب والملاط ووحدات مقياس التجارة (CSUs).</span><span class="sxs-lookup"><span data-stu-id="63eba-113">The self-update approach applies to brick and mortar stores and Commerce Scale Units (CSUs).</span></span> <span data-ttu-id="63eba-114">تبدأ التحديثات بتحديث مكون المقر الرئيسي للتجارة (HQ) ثم كل وحدات CSUs بشكل منفصل لتمكين منهجية الطرح التدريجي.</span><span class="sxs-lookup"><span data-stu-id="63eba-114">The updates start by updating the Commerce Headquarters (HQ) component and then all the CSUs separately to enable a gradual rollout methodology.</span></span> 

<span data-ttu-id="63eba-115">يتيح لك الطرح التدريجي التحقق من صحة سيناريوهات الإنتاج قبل دفع التحديث إلى الإنتاج، ويساعدك على التأكد من أن جميع المتاجر تستخدم نفس الإصدار.</span><span class="sxs-lookup"><span data-stu-id="63eba-115">The gradual rollout lets you validate production scenarios prior to pushing the update to production, and it helps you to ensure that all stores are using the same version.</span></span> 

<span data-ttu-id="63eba-116">يتمثل الاختلاف بين هذا الأسلوب والتحديث الآلي بالكامل في أنه على الرغم من تحديث كل شيء تلقائياً، تتم إدارة عملية التحديث الذاتي فيما يتعلق بجدول التحديث.</span><span class="sxs-lookup"><span data-stu-id="63eba-116">The difference between this approach and the fully automated update is that, even though everything is automatically updated, the self-update process is managed regarding the update schedule.</span></span> <span data-ttu-id="63eba-117">يمكّنك هذا النهج من إنشاء فترة تجميد مؤقتة في حالة الإجازات أو فترات العمل الحرجة التي لم يتم فيها تنفيذ عملية التحديث التلقائي.</span><span class="sxs-lookup"><span data-stu-id="63eba-117">This approach enables you to create a temporary freeze period in case of holidays or critical business operational periods where the auto update process has not been implemented.</span></span> <span data-ttu-id="63eba-118">بعد انتهاء هذه الفترة، سيتم تشغيل التحديث يدوياً أو إجراء سيناريو التحديث التلقائي.</span><span class="sxs-lookup"><span data-stu-id="63eba-118">After the end of this period, the update will be run manually or an automatic update scenario will be conducted.</span></span> 

<span data-ttu-id="63eba-119">يظهر سيناريو التحديث الذاتي في الصورة التالية.</span><span class="sxs-lookup"><span data-stu-id="63eba-119">The self-update scenario is shown in the following image.</span></span>


<span data-ttu-id="63eba-120">[![رسم تخطيطي لـ Dynamics 365 Commerce سيناريو التحديث الذاتي.](../media/self-update.jpg)](../media/self-update.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63eba-120">[![Diagram of the Dynamics 365 Commerce self-update scenario.](../media/self-update.jpg)](../media/self-update.jpg#lightbox)</span></span>
  

## <a name="first-release"></a><span data-ttu-id="63eba-121">الإصدار الأول</span><span class="sxs-lookup"><span data-stu-id="63eba-121">First release</span></span>
<span data-ttu-id="63eba-122">الإصدار الأول هو المكان الذي قمت فيه بالاشتراك للحصول على أحدث الإصدارات بشكل متكرر أكثر من نوع التوفر العام القياسي للعميل.</span><span class="sxs-lookup"><span data-stu-id="63eba-122">First release is where you have opted in to get the latest versions more frequently than your standard general availability type of customer.</span></span> <span data-ttu-id="63eba-123">من حيث التحديثات، إنه نفس نموذج التحديثات التلقائية.</span><span class="sxs-lookup"><span data-stu-id="63eba-123">In terms of updates, it's the same model as automatic updates.</span></span> <span data-ttu-id="63eba-124">الاختلاف الوحيد هو أنك في هيكل أحدث من البيئة القياسية، مع آخر التحديثات والمعلومات.</span><span class="sxs-lookup"><span data-stu-id="63eba-124">The only difference is that you are in a structure that is newer than the standard environment, with the latest updates and information.</span></span> 

<span data-ttu-id="63eba-125">يظهر سيناريو الإصدار الأول في الصورة التالية.</span><span class="sxs-lookup"><span data-stu-id="63eba-125">The First release scenario is shown in the following image.</span></span>

<span data-ttu-id="63eba-126">[![رسم تخطيطي لـ Dynamics 365 Commerce سيناريو الإصدار الأول.](../media/first-release.jpg)](../media/first-release.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63eba-126">[![Diagram of the Dynamics 365 Commerce first-release scenario.](../media/first-release.jpg)](../media/first-release.jpg#lightbox)</span></span>
 

## <a name="update-options"></a><span data-ttu-id="63eba-127">خيارات التحديث</span><span class="sxs-lookup"><span data-stu-id="63eba-127">Update options</span></span>

<span data-ttu-id="63eba-128">يتوفر نوعان من التحديثات:</span><span class="sxs-lookup"><span data-stu-id="63eba-128">Two types of updates are available:</span></span>

- <span data-ttu-id="63eba-129">**تحديث الجودة** – إصدار تراكمي يحتوي على إصلاحات للمشكلات المتعلقة بإصدار المنتج الذي تقوم بتشغيله حالياً.</span><span class="sxs-lookup"><span data-stu-id="63eba-129">**Quality update** – A cumulative, roll-up build that contains fixes for issues that are related to a product version that you are currently running.</span></span>
- <span data-ttu-id="63eba-130">**تحديث الخدمة** – الإصدار الذي يتم تطبيقه تلقائياً حالياً على البيئات استناداً إلى إعدادات التحديث في Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="63eba-130">**Service update** – The version that is currently automatically applied to environments based on the update settings in Lifecycle Services (LCS).</span></span> <span data-ttu-id="63eba-131">وهو عبارة عن إصدار تراكمي يحتوي على ميزات ووظائف جديدة وتحديثات الجودة ذات الصلة المتوفرة بشكل عام.</span><span class="sxs-lookup"><span data-stu-id="63eba-131">It is a cumulative, roll-up build that contains new features, functionality, and related quality updates that are generally available.</span></span>

<span data-ttu-id="63eba-132">لمزيد من المعلومات، راجع [قم بتنزيل التحديثات من Lifecycle Services (LCS)](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs/?azure-portal=true#segment-update-option-by-product-and-version).</span><span class="sxs-lookup"><span data-stu-id="63eba-132">For more information, see [Download updates from Lifecycle Services (LCS)](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs/?azure-portal=true#segment-update-option-by-product-and-version).</span></span>

