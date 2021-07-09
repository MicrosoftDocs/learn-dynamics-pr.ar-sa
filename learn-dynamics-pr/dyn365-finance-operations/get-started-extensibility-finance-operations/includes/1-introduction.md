---
ms.openlocfilehash: d72454ee372d4b4ca168e5a001d8933de26e2f68
ms.sourcegitcommit: e0a1238596690b3b6eedd86c2ac14099948a5e25
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "6072545"
---
<span data-ttu-id="c66f0-101">يعد استخدام الملحقات لتطوير تطبيقات Finance and Operations أمراً أساسياً لاستراتيجية Microsoft الخاصة بإصدار واحد، والذي يسمح لجميع العملاء بالاطلاع على أحدث إصدار من خلال الحصول دائماً على التحديثات المستمرة التي تديرها Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c66f0-101">Using extensions to develop for Finance and Operations apps is fundamental to Microsoft’s strategy of One Version, which allows all customers to be on the latest release by always acquiring continuous updates that are managed by Microsoft.</span></span> 

<span data-ttu-id="c66f0-102">تتضمن بعض مزايا هذا التغيير الجديد ما يلي:</span><span class="sxs-lookup"><span data-stu-id="c66f0-102">Some of the benefits to this new change include:</span></span> 

- <span data-ttu-id="c66f0-103">تدعم تطبيقات Finance and Operations التحديثات المستمرة، لذا فإن الترقيات أسهل بكثير وأقل تكلفة.</span><span class="sxs-lookup"><span data-stu-id="c66f0-103">Finance and Operations apps supports continuous updates, so upgrades are much easier and less expensive.</span></span> 
- <span data-ttu-id="c66f0-104">من خلال التواجد دائماً على أحدث إصدار، يمكنك تحسين الإنتاجية دون إعاقة إمكانية الترقية.</span><span class="sxs-lookup"><span data-stu-id="c66f0-104">By always being on the latest version, you can improve productivity without impeding upgradability.</span></span> 
- <span data-ttu-id="c66f0-105">تم تحسين إمكانية الدعم وإمكانية الخدمة.</span><span class="sxs-lookup"><span data-stu-id="c66f0-105">Supportability and serviceability are improved.</span></span> 
- <span data-ttu-id="c66f0-106">يتم تقليل تكاليف تنفيذ عمليات التخصيص والتخصيص بلا رمز.</span><span class="sxs-lookup"><span data-stu-id="c66f0-106">Implementation costs for no-code personalization and customizations are reduced.</span></span> 
- <span data-ttu-id="c66f0-107">يُعد الابتكار جنباً إلى جنب مع Microsoft أسهل لموردي البرامج المستقلين (ISVs).</span><span class="sxs-lookup"><span data-stu-id="c66f0-107">Innovating alongside Microsoft is easier for independent software vendors (ISVs).</span></span> 

<span data-ttu-id="c66f0-108">هذا التغيير أساسي إذا كنت قادماً من Dynamics AX ‏2012 للبنية التحتية والخدمات المستخدمة، وللتطوير.</span><span class="sxs-lookup"><span data-stu-id="c66f0-108">This change is fundamental if you are coming from Dynamics AX 2012 for infrastructure and services used, and for development.</span></span> <span data-ttu-id="c66f0-109">في تطبيقات Finance and Operations، لم يعد بإمكانك العمل على تراكب الرمز الأساسي والحصول على تخصيصات متداخلة عند التطوير.</span><span class="sxs-lookup"><span data-stu-id="c66f0-109">In Finance and Operations apps, you can no longer overlayer base code and have intrusive customizations when developing.</span></span> 

<span data-ttu-id="c66f0-110">تستعرض النقاط التالية لماذا يجب عليك استخدام الملحقات للتطوير.</span><span class="sxs-lookup"><span data-stu-id="c66f0-110">The following bullet points review why you must use extensions for development.</span></span> 

- <span data-ttu-id="c66f0-111">يمكن أن تؤدي التخصيصات التي يتم تنفيذها باستخدام التراكب إلى حدوث مشكلات في المنتج يصعب تشخيصها وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="c66f0-111">Customizations that are implemented by using overlayering can create product issues that are difficult to diagnose and fix.</span></span>
- <span data-ttu-id="c66f0-112">يعد دمج التعارضات بين التخصيصات وبيانات تعريف Microsoft أو ISV المحدثة ورمز المصدر مهمة تطوير يدوية.</span><span class="sxs-lookup"><span data-stu-id="c66f0-112">Merging conflicts between the customizations and the updated Microsoft or ISV metadata and source code is a manual development task.</span></span> <span data-ttu-id="c66f0-113">تحدث هذه المشكلة حتى إذا لم يكن التخصيص متداخلاً لأن التغييرات مختلطة مع الرمز الأصلي.</span><span class="sxs-lookup"><span data-stu-id="c66f0-113">This issue occurs even if the customization isn’t intrusive because the changes are mixed in with the original code.</span></span>

- <span data-ttu-id="c66f0-114">التكلفة الإجمالية للملكية عالية.</span><span class="sxs-lookup"><span data-stu-id="c66f0-114">Total cost of ownership is high.</span></span> 

<span data-ttu-id="c66f0-115">أثناء الترقية إلى تطبيقات Finance and Operations، ستستخدم أداة ترقية الرمز لنقل الرمز الخاص بك من مخزن نماذج Dynamics AX ‏2012 الخاص بك إلى رمز جديد سيكون متوافقاً مع تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="c66f0-115">During your upgrade to Finance and Operations apps, you will use the Code Upgrade Tool to move your code from your Dynamics AX 2012 model store to new code that will be compatible with Finance and Operations apps.</span></span> <span data-ttu-id="c66f0-116">يجب على المطورين نقل الرمز ومنطق الأعمال من التراكب إلى الملحقات.</span><span class="sxs-lookup"><span data-stu-id="c66f0-116">Developers must move the code and business logic from overlayering to extensions.</span></span> 

<span data-ttu-id="c66f0-117">لمزيد من المعلومات، راجع [أدوات ترقية البيانات والرمز من Dynamics AX ‏2012 إلى تطبيقات Finance and Operations.](https://docs.microsoft.com/learn/modules/tools-code-data-upgrade-ax-2012-finance-operations//?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="c66f0-117">For more information, see [Tools for code and data upgrade from Dynamics AX 2012 to Finance and Operations apps.](https://docs.microsoft.com/learn/modules/tools-code-data-upgrade-ax-2012-finance-operations//?azure-portal=true).</span></span>

