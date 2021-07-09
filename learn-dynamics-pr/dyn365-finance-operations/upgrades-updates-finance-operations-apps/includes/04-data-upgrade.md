---
ms.openlocfilehash: bc26da1e2a9b47e52832162f95591813477e4fff
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071306"
---
<span data-ttu-id="f058c-101">لإجراء ترقية لبيانات بيئة الاختبار المعزولة، اتبع هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="f058c-101">To perform a sandbox data upgrade, follow these steps.</span></span>

1.  <span data-ttu-id="f058c-102">**اختيار ترقية البيانات** - في LCS، انتقل إلى قائمة **تفاصيل البيئة > احتفاظ > ترقية**.</span><span class="sxs-lookup"><span data-stu-id="f058c-102">**Choose data upgrade** - In LCS, go to **Environment details > Maintain > Upgrade** menu.</span></span> <span data-ttu-id="f058c-103">حدد التطبيق الجديد وإصدارات النظام الأساسي.</span><span class="sxs-lookup"><span data-stu-id="f058c-103">Select your new application and platform versions.</span></span> 
2.  <span data-ttu-id="f058c-104">**الإعداد** - خلال هذا الوقت، يتم توفير بنية أساسية جديدة نيابةً عنك.</span><span class="sxs-lookup"><span data-stu-id="f058c-104">**Prepare** - During this time, new infrastructure is being provisioned on your behalf.</span></span> <span data-ttu-id="f058c-105">لا يحدث وقت تعطل في بيئة الاختبار المعزولة الحالية لديك.</span><span class="sxs-lookup"><span data-stu-id="f058c-105">No downtime occurs on your current sandbox environment.</span></span> 
3.  <span data-ttu-id="f058c-106">**تطبيق الحزم** - تطبيق حزم البرامج القابلة للتوزيع المنشأة حديثاً على بيئة الترقية.</span><span class="sxs-lookup"><span data-stu-id="f058c-106">**Apply packages** - Apply newly created software deployable packages on your upgrade environment.</span></span> <span data-ttu-id="f058c-107">يجب أن تكون هذه الحزمة قد تم تجميعها بالفعل واختبارها في بيئة مطور، ويجب أن تكون الحزمة قد تم إنتاجها من بيئة إنشاء جديدة.</span><span class="sxs-lookup"><span data-stu-id="f058c-107">This package should already have been compiled and tested on a developer environment, and the package should have been produced from a new build environment.</span></span> <span data-ttu-id="f058c-108">لا يحدث وقت تعطل في بيئة الاختبار المعزولة الحالية لديك.</span><span class="sxs-lookup"><span data-stu-id="f058c-108">No downtime occurs on your current sandbox environment.</span></span> 

 
    ![رسم تخطيطي يوضح الخطوة الأولى لترقية البيانات](../media/data-upgrade-1.png)

4.  <span data-ttu-id="f058c-110">**ترقية البيانات** - ستتبدل هذه الخطوة في بيئة الترقية الخاصة بك، وستقوم بإلغاء توزيع بيئة الاختبار المعزولة السابقة لديك.</span><span class="sxs-lookup"><span data-stu-id="f058c-110">**Upgrade data** - This step will swap in your upgrade environment and will deallocate your prior sandbox environment.</span></span> <span data-ttu-id="f058c-111">سيتم تطبيق حزمة ترقية البيانات المناسبة لك بناءً على إصدار التطبيق الأصلي والهدف.</span><span class="sxs-lookup"><span data-stu-id="f058c-111">The appropriate data upgrade package will be applied for you based on your original application version and the target.</span></span> 

 
    ![رسم تخطيطي يوضح الخطوة الثانية لترقية البيانات](../media/data-upgrade-2.png)

5.  <span data-ttu-id="f058c-113">**التحقق من الصحة وتسجيل الخروج** - سجِّل الدخول إلى البيئة، وتأكد من أن البيانات والكود يعملان بالشكل المتوقع.</span><span class="sxs-lookup"><span data-stu-id="f058c-113">**Validate and sign off** – Sign in to the environment and ensure that the data and code are working as expected.</span></span> <span data-ttu-id="f058c-114">سجِّل الخروج عند الترقية، وبعد ذلك يمكن إجراء نفس الخطوات في بيئة التشغيل باستخدام الحزم نفسها.</span><span class="sxs-lookup"><span data-stu-id="f058c-114">Sign off on the upgrade, and then the same can be performed in the production environment by using the exact same packages.</span></span> 


<span data-ttu-id="f058c-115">ترقية بيانات بيئة الاختبار هي خدمة ذاتية تماماً؛ ويمكنك جدولتها في وقتك الخاص.</span><span class="sxs-lookup"><span data-stu-id="f058c-115">The sandbox data upgrade is completely self-service; you can schedule it on your own time.</span></span> <span data-ttu-id="f058c-116">يمكنك الحصول على مثيل موازٍ للمساعدة في تقليل وقت التعطل.</span><span class="sxs-lookup"><span data-stu-id="f058c-116">You can have a parallel instance provided to help minimize downtime.</span></span> <span data-ttu-id="f058c-117">في حالة حدوث أي مشاكل، يتم دعم العودة إلى الحالة السابقة لبيئة الاختبار المعزولة.</span><span class="sxs-lookup"><span data-stu-id="f058c-117">In case any issues occur, rollback is supported for the sandbox.</span></span> 

<span data-ttu-id="f058c-118">عادةً ما تحتوي بيئة الاختبار المعزولة على أحدث بيانات الإنتاج، مما يعني أن كود الإنتاج سيكون مطابقاً لبيئة الاختبار المعزولة.</span><span class="sxs-lookup"><span data-stu-id="f058c-118">Typically, the sandbox environment has the latest production data, meaning that the production code will be identical to the sandbox.</span></span> 

<span data-ttu-id="f058c-119">وبعد الترقية، لن تتم مطالبتك بتشغيل مزيد من الترقيات، فقط التحديثات المستمرة.</span><span class="sxs-lookup"><span data-stu-id="f058c-119">After upgrading, you will not be required to run more upgrades, only continuous updates.</span></span> 







