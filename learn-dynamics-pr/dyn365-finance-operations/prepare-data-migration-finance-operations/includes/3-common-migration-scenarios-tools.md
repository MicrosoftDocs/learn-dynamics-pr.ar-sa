---
ms.openlocfilehash: 6a49d2fe4fefa7fde80bd2e03860d439dca50b0b
ms.sourcegitcommit: 2475a4326b76fa8838c2e4e6885473bdd6fe6270
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/02/2021
ms.locfileid: "6072172"
---
<span data-ttu-id="26a6d-101">فيما يلي سيناريوهان وتوصيات لاستخدام نمط التكامل.</span><span class="sxs-lookup"><span data-stu-id="26a6d-101">The following are two scenarios, and recommendations for which integration pattern to use.</span></span> 

## <a name="scenario-1"></a><span data-ttu-id="26a6d-102">السيناريو 1</span><span class="sxs-lookup"><span data-stu-id="26a6d-102">Scenario 1</span></span>

<span data-ttu-id="26a6d-103">يعمل لدى شركة طاقة عمال ميدانيون يقومون بجدولة مهام تركيب السخانات.</span><span class="sxs-lookup"><span data-stu-id="26a6d-103">An energy company has field workers who schedule installation jobs for heaters.</span></span> <span data-ttu-id="26a6d-104">تستخدم هذه الشركة تطبيقات Finance and Operations لمكتب الشئون الإدارية وبرامج الجهات الخارجية كخدمة (SaaS) لجدولة المواعيد.</span><span class="sxs-lookup"><span data-stu-id="26a6d-104">This company uses Finance and Operations apps for the back office and third-party software as a service (SaaS) to schedule appointments.</span></span> <span data-ttu-id="26a6d-105">عندما يقوم العاملون الميدانيون بجدولة المواعيد، فيجب عليهم النظر في مدى توفر المخزون للتأكد من توفر أجزاء التركيب الخاصة بالمهمة.</span><span class="sxs-lookup"><span data-stu-id="26a6d-105">When field workers schedule appointments, they must look up inventory availability to make sure that installation parts are available for the job.</span></span> 

<span data-ttu-id="26a6d-106">بيانات الوقت الحقيقي المطلوبة:</span><span class="sxs-lookup"><span data-stu-id="26a6d-106">The real-time data required:</span></span> 

- <span data-ttu-id="26a6d-107">حجم البيانات الذروة هو 1،000 سجل في الساعة</span><span class="sxs-lookup"><span data-stu-id="26a6d-107">Peak data volume is 1,000 records per hour</span></span>
- <span data-ttu-id="26a6d-108">التردد مخصص.</span><span class="sxs-lookup"><span data-stu-id="26a6d-108">Frequency is Ad hoc.</span></span>

<span data-ttu-id="26a6d-109">يمكن تنفيذ هذا السيناريو باستخدام نمط تكامل خدمة مخصص.</span><span class="sxs-lookup"><span data-stu-id="26a6d-109">This scenario can be implemented by using a custom service integration pattern.</span></span>

<span data-ttu-id="26a6d-110">في Finance and Operations، اطلب من مطور إنشاء خدمة مخصصة لحساب المخزون الفعلي المتاح لصنف محدد.</span><span class="sxs-lookup"><span data-stu-id="26a6d-110">In Finance and Operations, have a developer create a custom service to calculate the physical on-hand inventory for a given item.</span></span>

<span data-ttu-id="26a6d-111">في تطبيق الجدولة، قم بإجراء استدعاء في الوقت الحقيقي لنقطة نهاية خدمة مخصصة، من خلال SOAP أو REST، لاسترداد معلومات المخزون للصنف المحدد.</span><span class="sxs-lookup"><span data-stu-id="26a6d-111">In the scheduling application, make a real-time call to a custom service endpoint, through either SOAP or REST, to retrieve inventory information for the selected item.</span></span>

## <a name="scenario-2"></a><span data-ttu-id="26a6d-112">السيناريو 2</span><span class="sxs-lookup"><span data-stu-id="26a6d-112">Scenario 2</span></span>

<span data-ttu-id="26a6d-113">تتلقى الشركة حجماً كبيراً من أوامر المبيعات من نظام الواجهة الأمامية الذي يعمل محلياً.</span><span class="sxs-lookup"><span data-stu-id="26a6d-113">A company receives a large volume of sales orders from a front-end system that runs on-premises.</span></span> <span data-ttu-id="26a6d-114">وبشكل دوري، يجب إرسال هذه الأوامر إلى Finance and Operations للمعالجة والإدارة.</span><span class="sxs-lookup"><span data-stu-id="26a6d-114">Periodically, these orders must be sent to Finance and Operations for processing and management.</span></span>

<span data-ttu-id="26a6d-115">لا يلزم توفر بيانات الوقت الحقيقي.</span><span class="sxs-lookup"><span data-stu-id="26a6d-115">The real-time data is not required.</span></span> <span data-ttu-id="26a6d-116">حجم البيانات الذروة هو 20،000 سجل في الساعة والتكرار مرة واحدة كل خمس دقائق.</span><span class="sxs-lookup"><span data-stu-id="26a6d-116">Peak data volume is 20,000 records per hour and the Frequency is One time every five minutes.</span></span>

<span data-ttu-id="26a6d-117">يتم تنفيذ هذا السيناريو بشكل أفضل باستخدام نمط تكامل واجهات برمجة التطبيقات (API) لبيانات الدُفعات.</span><span class="sxs-lookup"><span data-stu-id="26a6d-117">This scenario is best implemented by using a batch data APIs integration pattern.</span></span>

<span data-ttu-id="26a6d-118">حدد جميع الكيانات المطلوبة للتكامل، وتأكد من تمكين إدارة البيانات للكيانات.</span><span class="sxs-lookup"><span data-stu-id="26a6d-118">Determine all the entities that are required for the integration, and make sure that data management is enabled for the entities.</span></span>

## <a name="finance-and-operations-apps-integration-tools"></a><span data-ttu-id="26a6d-119">أدوات تكامل تطبيقات Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="26a6d-119">Finance and Operations apps integration tools</span></span>

<span data-ttu-id="26a6d-120">توفر تطبيقات Finance and Operations أدوات لترحيل البيانات، مثل:</span><span class="sxs-lookup"><span data-stu-id="26a6d-120">Finance and Operations apps offer tools for data migration, such as:</span></span>

- <span data-ttu-id="26a6d-121">مساحة عمل إدارة البيانات</span><span class="sxs-lookup"><span data-stu-id="26a6d-121">Data management workspace</span></span>
- <span data-ttu-id="26a6d-122">تكامل Office</span><span class="sxs-lookup"><span data-stu-id="26a6d-122">Office integration</span></span>
- <span data-ttu-id="26a6d-123">مصمم مصنفات Excel</span><span class="sxs-lookup"><span data-stu-id="26a6d-123">Excel workbook designer</span></span>


<span data-ttu-id="26a6d-124">لمعرفة المزيد حول تكنولوجيا واجهة برمجة التطبيقات (API) لتطبيقات Finance and Operations، راجع وحدتي [تكامل تطبيقات Finance and Operations مع Microsoft Azure](https://docs.microsoft.com/learn/modules/integrate-azure-finance-operations/?azure-portal=true)، و[نفذ واجهة برمجة تطبيقات (API) حزمة إدارة البيانات لتطبيقات Finance and Operations](https://docs.microsoft.com/learn/modules/data-package-api-finance-operations/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="26a6d-124">To learn more about API technology for Finance and Operations apps, see the [Integrate Finance and Operations apps with Microsoft Azure](https://docs.microsoft.com/learn/modules/integrate-azure-finance-operations/?azure-portal=true), and [Implement the Data management package API for Finance and Operations apps](https://docs.microsoft.com/learn/modules/data-package-api-finance-operations/?azure-portal=true) modules.</span></span>
 
