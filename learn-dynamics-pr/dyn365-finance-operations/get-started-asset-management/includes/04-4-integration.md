---
ms.openlocfilehash: 12fd01f11cc9cb33bec46acc31be08c5bb4d6f6d
ms.sourcegitcommit: c23f80e4732f19cd5136470607376672a2219ddb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/11/2020
ms.locfileid: "6072107"
---
<span data-ttu-id="351a5-101">تقدم هذه الوحدة نظرة عامة حول عمليات التكامل المتوفرة مع إدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="351a5-101">This unit provides an overview of integrations that are available with Asset Management.</span></span>

## <a name="dynamics-365-field-service-integration-with-asset-management"></a><span data-ttu-id="351a5-102">تكامل Dynamics 365 Field Service مع إدارة الأصول</span><span class="sxs-lookup"><span data-stu-id="351a5-102">Dynamics 365 Field Service integration with Asset Management</span></span>

<span data-ttu-id="351a5-103">يعمل Supply Chain Management على تسهيل مزامنة تدفقات عمليات دورة الحياة مع Dynamics 365 Field Service.</span><span class="sxs-lookup"><span data-stu-id="351a5-103">Supply Chain Management facilitates the synchronization of lifecycle process flows with Dynamics 365 Field Service.</span></span> <span data-ttu-id="351a5-104">يتم تكوين عمليات التكامل باستخدام قوالب مكامل البيانات الموسعة وMicrosoft Dataverse.</span><span class="sxs-lookup"><span data-stu-id="351a5-104">The integrations are configured using extensible Data integrator templates and Microsoft Dataverse.</span></span> <span data-ttu-id="351a5-105">يمكن للمؤسسات الاستفادة من الإمكانات المجمّعة لإدارة الأصول وField Service وإدارة كل من الأصول الداخلية والخارجية.</span><span class="sxs-lookup"><span data-stu-id="351a5-105">Organizations can leverage the combined capabilities of Asset Management and Field Service and manage both internal and external assets.</span></span> <span data-ttu-id="351a5-106">ويعتمد تكامل Field Service على وظيفة "العميل المتوقع إلى النقد" الحالية.</span><span class="sxs-lookup"><span data-stu-id="351a5-106">The Field Service integration builds on top of the existing prospect-to-cash functionality.</span></span> 

<span data-ttu-id="351a5-107">يمكن استخدام القوالب القياسية لإنشاء مشاريع تكامل مخصصة، حيث يمكن تعيين حقول وكيانات قياسية ومخصصة إضافية لتعديل التكامل وتلبية احتياجات العمل الخاصة.</span><span class="sxs-lookup"><span data-stu-id="351a5-107">Standard templates can be used to create custom integration projects, where additional standard and custom fields and entities can be mapped to adjust the integration and meet specific business needs.</span></span>

<span data-ttu-id="351a5-108">تركز عملية التكامل الأولي بين Field Service وSupply Chain Management على تمكين فوترة أوامر العمل والاتفاقيات الموجودة في Field Service في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="351a5-108">Initial integration between Field Service and Supply Chain Management is focused on enabling work orders and agreements in Field Service to be invoiced in Supply Chain Management.</span></span> <span data-ttu-id="351a5-109">يبدأ التدفق المدعوم في Field Service، حيث تتم مزامنة المعلومات من أوامر العمل مع Supply Chain Management كأوامر مبيعات.</span><span class="sxs-lookup"><span data-stu-id="351a5-109">The supported flow starts in Field Service, where information from work orders is synchronized to Supply Chain Management as sales orders.</span></span> <span data-ttu-id="351a5-110">في Supply Chain Management، تتم فوترة أوامر المبيعات لإنشاء مستندات فاتورة، كما هو موضح في الرسم التخطيطي.</span><span class="sxs-lookup"><span data-stu-id="351a5-110">In Supply Chain Management, the sales orders are invoiced to generate invoice documents, as shown in the diagram.</span></span> 

![رسم تخطيطي يوضح نقاط التكامل بين Field Service وSupply Chain Management.](../media/field-service-integration-c.png)

 
<span data-ttu-id="351a5-112">توفر الوظائف الإضافية للفنيين الميدانيين نتيجة تحليلات لمعلومات المخزون من Supply Chain Management، مما يسمح لهم بتحديث مستويات المخزون وإجراء عمليات نقل المواد.</span><span class="sxs-lookup"><span data-stu-id="351a5-112">Additional functionality gives field technicians insight into the inventory information from Supply Chain Management, allowing them to update inventory levels and do material transfers.</span></span> <span data-ttu-id="351a5-113">ويمكن للشركات التي تقوم بتثبيت البضائع المبيعة أو صيانتها الاستفادة من التحكم والرؤية بشكل أفضل لعملية المبيعات والخدمة الكاملة بالتكامل من المشاريع.</span><span class="sxs-lookup"><span data-stu-id="351a5-113">Companies installing or servicing sold goods can benefit from better control and visibility to the full sales and service process with integration from projects.</span></span>

<span data-ttu-id="351a5-114">يتمتع كل من Supply Chain Management وField Service بنقاط التكامل التالية:</span><span class="sxs-lookup"><span data-stu-id="351a5-114">Supply Chain Management and Field Service have the following integration points:</span></span>

- <span data-ttu-id="351a5-115">أوامر عمل Field Service مع ارتباطات إلى مشاريع Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="351a5-115">Field Service work orders with links to Supply Chain Management projects.</span></span> <span data-ttu-id="351a5-116">يمكنك تطبيق رقم المشروع على أمر المبيعات للسماح بالفوترة من المشروع.</span><span class="sxs-lookup"><span data-stu-id="351a5-116">You can apply the project number to the sales order to allow invoicing from the project.</span></span>
- <span data-ttu-id="351a5-117">مشاريع Supply Chain Management المتصلة بأوامر عمل Field Service.</span><span class="sxs-lookup"><span data-stu-id="351a5-117">Supply Chain Management projects connected with Field Service work orders.</span></span>
- <span data-ttu-id="351a5-118">معلومات المستودع</span><span class="sxs-lookup"><span data-stu-id="351a5-118">Warehouse information</span></span>
- <span data-ttu-id="351a5-119">معلومات المخزون المتاح</span><span class="sxs-lookup"><span data-stu-id="351a5-119">On-hand inventory information</span></span>
- <span data-ttu-id="351a5-120">عمليات نقل المخزون</span><span class="sxs-lookup"><span data-stu-id="351a5-120">Inventory transfers</span></span>
- <span data-ttu-id="351a5-121">تعديلات المخزون</span><span class="sxs-lookup"><span data-stu-id="351a5-121">Inventory adjustments</span></span>

## <a name="business-events-uptake-for-asset-management"></a><span data-ttu-id="351a5-122">تنفيذ أحداث الأعمال لإدارة الأصول</span><span class="sxs-lookup"><span data-stu-id="351a5-122">Business events uptake for Asset Management</span></span>
<span data-ttu-id="351a5-123">توفر ‏‫أحداث الأعمال‬ إطار عمل يسمح للأنظمة الخارجية بتلقي الإعلامات من Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="351a5-123">Business events provide a framework that allows external systems to receive notifications from Supply Chain Management.</span></span> <span data-ttu-id="351a5-124">وباستخدام هذه الوظيفة، يمكن للأنظمة تنفيذ إجراءات العمل استجابةً لأحداث الأعمال عند تشغيل إجراءات العمل.</span><span class="sxs-lookup"><span data-stu-id="351a5-124">Using this functionality, systems can perform business actions in response to business events when a business process is run.</span></span>

<span data-ttu-id="351a5-125">لمزيد من المعلومات حول أحداث الأعمال، راجع وحدة [استهلاك أحداث الأعمال في تطبيقات Finance and Operations](https://docs.microsoft.com/learn/modules/business-events-finance-operations//?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="351a5-125">For more information about business events, see the [Consume business events in Finance and Operations apps](https://docs.microsoft.com/learn/modules/business-events-finance-operations//?azure-portal=true) module.</span></span>

<span data-ttu-id="351a5-126">يتيح استخدام وظائف أحداث الأعمال مع إدارة الأصول للمستخدمين إمكانية الوصول إلى مستندات الأعمال من خلال الاستفادة من Microsoft Power Automate والتطبيقات المنطقية.</span><span class="sxs-lookup"><span data-stu-id="351a5-126">Using Business events functionality with Asset management enables users to access business documents by leveraging Microsoft Power Automate and logic apps.</span></span> <span data-ttu-id="351a5-127">ويتم تضمين مشغلات لطلبات الصيانة وتغييرات حالة أمر العمل في إطار عمل ‏‫أحداث الأعمال.</span><span class="sxs-lookup"><span data-stu-id="351a5-127">Triggers for maintenance requests and work order state changes are included in the business events framework.</span></span> 

![رسم تخطيطي يوضح كيفية حصول الأنظمة الخارجية على إعلامات من Supply Chain Management عبر Power Automate.](../media/business-events-c.png) 

<span data-ttu-id="351a5-129">تشمل أحداث الأعمال المدعومة:</span><span class="sxs-lookup"><span data-stu-id="351a5-129">Supported business events include:</span></span>

- <span data-ttu-id="351a5-130">تم إنشاء طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="351a5-130">Maintenance request is created.</span></span>
- <span data-ttu-id="351a5-131">تم تغيير خاصية الأصل.</span><span class="sxs-lookup"><span data-stu-id="351a5-131">Asset property is changed.</span></span>
- <span data-ttu-id="351a5-132">تم إنشاء أمر عمل الصيانة لطلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="351a5-132">Maintenance work order created for maintenance request.</span></span>
- <span data-ttu-id="351a5-133">تم الإبلاغ عن اكتمال أمر عمل الصيانة.</span><span class="sxs-lookup"><span data-stu-id="351a5-133">Maintenance work order reported completed.</span></span>
- <span data-ttu-id="351a5-134">تمت جدولة أمر عمل الصيانة.</span><span class="sxs-lookup"><span data-stu-id="351a5-134">A maintenance work order is scheduled.</span></span>


