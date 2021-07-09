---
ms.openlocfilehash: 714016b9db5373df6679ac925c507b45fd7baf53
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072400"
---
<span data-ttu-id="2dfd6-101">تحتوي تطبيقات Finance and Operations على واجهات برمجة تطبيقات (API) متعددة تدعم سيناريوهات التكامل:</span><span class="sxs-lookup"><span data-stu-id="2dfd6-101">Finance and Operations apps contain multiple APIs that support integration scenarios:</span></span>
 
- <span data-ttu-id="2dfd6-102">بروتوكول البيانات المفتوحة (OData)</span><span class="sxs-lookup"><span data-stu-id="2dfd6-102">Open Data Protocol (OData)</span></span>
- <span data-ttu-id="2dfd6-103">الخدمات المخصصة</span><span class="sxs-lookup"><span data-stu-id="2dfd6-103">Custom services</span></span>
- <span data-ttu-id="2dfd6-104">خدمات الويب الخارجية</span><span class="sxs-lookup"><span data-stu-id="2dfd6-104">External web services</span></span>
- <span data-ttu-id="2dfd6-105">عمليات تكامل Office‬‏‫</span><span class="sxs-lookup"><span data-stu-id="2dfd6-105">Office integrations</span></span>
- <span data-ttu-id="2dfd6-106">عمليات تكامل متكررة</span><span class="sxs-lookup"><span data-stu-id="2dfd6-106">Recurring integrations</span></span>
- <span data-ttu-id="2dfd6-107">واجهة برمجة التطبيقات (API) لحزمة إدارة البيانات</span><span class="sxs-lookup"><span data-stu-id="2dfd6-107">Data management package API</span></span>

<span data-ttu-id="2dfd6-108">تعمل واجهة برامج التطبيقات لعمليات التكامل المتكررة وواجهة برمجة التطبيقات (API) لـ Data Management Framework‏ (DMF) على دعم سيناريوهات التكامل المستندة إلى الملفات.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-108">Recurring integrations API and the Data Management Framework (DMF) API support file-based integration scenarios.</span></span> <span data-ttu-id="2dfd6-109">يأتي DMF بشكل جاهز في Finance and Operations ويدعم استيراد البيانات وتصديرها.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-109">The DMF comes out of the box with Finance and Operations and supports data import and export.</span></span> <span data-ttu-id="2dfd6-110">كما تدعم عمليات التكامل المتكررة سيناريوهات استيراد البيانات وتصديرها.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-110">Recurring integrations also support data import and export scenarios.</span></span>

<span data-ttu-id="2dfd6-111">عند تحديد واجهة برمجة تطبيقات (API) التكامل، سيكون لديك العديد من التقديرات.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-111">When selecting an integration API, you will have many considerations.</span></span> <span data-ttu-id="2dfd6-112">ويمكن أن تساعدك بعض نقاط القرار الخاصة بـ DMF وعمليات التكامل المتكررة على اختيار سيناريو تكامل التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-112">Some of the decision points for the DMF and recurring integrations can help you chose your implementation integration scenario.</span></span>

<span data-ttu-id="2dfd6-113">للحصول على مزيد من المعلومات، راجع [سيناريوهات تكامل البيانات](https://docs.microsoft.com/learn/modules/integration-patterns-finance-operations/4-scenarios/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="2dfd6-113">For more information, see [Data integration scenarios](https://docs.microsoft.com/learn/modules/integration-patterns-finance-operations/4-scenarios/?azure-portal=true).</span></span>

<span data-ttu-id="2dfd6-114">يجب تقييم هذه التقديرات بحيث يمكنك تحديد إستراتيجية التكامل الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-114">These considerations should be evaluated so that you can determine your integration strategy.</span></span> <span data-ttu-id="2dfd6-115">تظهر الصورة الآتية بعض التوصيات لسيناريوهات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-115">The following image shows some recommendations for different scenarios.</span></span>

![جدول التوصيات لسيناريوهات التكامل المختلفة.](../media/strategy.png)

<span data-ttu-id="2dfd6-117">لمساعدتك على تحديد إستراتيجية التكامل الخاصة بك، تقوم الأقسام الآتية بمراجعة بعض سيناريوهات التكامل للترقية من AX ‏2012.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-117">To help you determine your integration strategy, the following sections review some integration scenarios for upgrading from AX 2012.</span></span>

## <a name="system-services-scenario"></a><span data-ttu-id="2dfd6-118">سيناريو خدمات النظام</span><span class="sxs-lookup"><span data-stu-id="2dfd6-118">System services scenario</span></span>

<span data-ttu-id="2dfd6-119">لدعم مجموعة من الخيارات للتخصيص والبرمجة، يوفر Dynamics AX‏ 2012 أنواع الخدمات الآتية:</span><span class="sxs-lookup"><span data-stu-id="2dfd6-119">To support a range of options for customization and programmability, Dynamics AX 2012 provides the following types of services:</span></span>

- <span data-ttu-id="2dfd6-120">خدمة الاستعلام، والتي توفر الوصول إلى البيانات التي تم إرجاعها في استعلامات AOT</span><span class="sxs-lookup"><span data-stu-id="2dfd6-120">Query Service, which provides access to data that is returned in AOT queries</span></span>
- <span data-ttu-id="2dfd6-121">بيانات التعريف لكائنات AOT مثل الجداول وأنواع البيانات الملحقة (أنواع EDT)</span><span class="sxs-lookup"><span data-stu-id="2dfd6-121">Metadata for AOT objects such as tables and extended data types (EDTs)</span></span>
- <span data-ttu-id="2dfd6-122">بيانات حول المستخدم المستدعي، مثل اللغة الافتراضية والشركة الافتراضية</span><span class="sxs-lookup"><span data-stu-id="2dfd6-122">Data about the calling user, such as default language and default company</span></span>

<span data-ttu-id="2dfd6-123">تستخدم تطبيقات Finance and Operations خدمة بيانات التعريف REST ‏(‎http;‎//\[‎baseURL]/metadata).</span><span class="sxs-lookup"><span data-stu-id="2dfd6-123">Finance and Operations apps uses REST metadata service (http;//\[baseURL]/metadata).</span></span> 

- <span data-ttu-id="2dfd6-124">**التسميات** – تقوم بإرجاع التسميات من النظام.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-124">**Labels** – Returns labels from the system.</span></span> <span data-ttu-id="2dfd6-125">وتحتوي التسميات على زوج ثنائي من مفتاح اللغة والمعرف بحيث يمكنك استرداد قيمة التسمية.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-125">Labels have a dual pair key of language and ID so that you can retrieve the value of the label.</span></span>
- <span data-ttu-id="2dfd6-126">**كيانات البيانات** – تقوم بإرجاع قائمة بتنسيق JSON لكافة كيانات البيانات في النظام.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-126">**Data entities** – Returns a JSON-formatted list of all data entities in the system.</span></span>

## <a name="custom-service-scenario"></a><span data-ttu-id="2dfd6-127">سيناريو الخدمة المخصصة</span><span class="sxs-lookup"><span data-stu-id="2dfd6-127">Custom service scenario</span></span>


<span data-ttu-id="2dfd6-128">يسمح Dynamics AX ‏2012 بإنشاء الخدمات المخصصة التي يتم عرضها عبر نقاط نهاية SOAP.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-128">Dynamics AX 2012 allows the creation of custom services that are exposed through SOAP endpoints.</span></span> <span data-ttu-id="2dfd6-129">ويسمح السيناريو للأنظمة الخارجية باستدعاء منطق أعمال Dynamics.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-129">The scenario allows external systems to call Dynamics business logics.</span></span>

<span data-ttu-id="2dfd6-130">خصائص الخدمة المخصصة هي:</span><span class="sxs-lookup"><span data-stu-id="2dfd6-130">Characteristics of custom service are:</span></span> 

- <span data-ttu-id="2dfd6-131">متزامنة</span><span class="sxs-lookup"><span data-stu-id="2dfd6-131">Synchronous</span></span>
- <span data-ttu-id="2dfd6-132">قابلة للتخصيص</span><span class="sxs-lookup"><span data-stu-id="2dfd6-132">Customizable</span></span>
- <span data-ttu-id="2dfd6-133">تسمح بمعلمات التمرير</span><span class="sxs-lookup"><span data-stu-id="2dfd6-133">Allows passing parameters</span></span>
- <span data-ttu-id="2dfd6-134">تتطلب معالجة المنفذ</span><span class="sxs-lookup"><span data-stu-id="2dfd6-134">Requires port handling</span></span>
- <span data-ttu-id="2dfd6-135">WCF المستندة إلى SOAP</span><span class="sxs-lookup"><span data-stu-id="2dfd6-135">SOAP-based WCF</span></span>

<span data-ttu-id="2dfd6-136">مثال: تقوم خدمة خارجية (صفحة ويب الواجهة الأمامية) بإرسال أمر لتحديث كمية الأمر وتأكيدها.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-136">Example: External service (front end webpage) sends a command to update the order quantity and confirm it.</span></span>


<span data-ttu-id="2dfd6-137">تسمح تطبيقات Finance and Operations بتنشيط منطق العمل من نظام خارجي باستخدام أساليب مختلفة:</span><span class="sxs-lookup"><span data-stu-id="2dfd6-137">Finance and Operations apps allow business logics activation from an external system by using different techniques:</span></span>

- <span data-ttu-id="2dfd6-138">الخدمة المخصصة المستندة إلى JSON</span><span class="sxs-lookup"><span data-stu-id="2dfd6-138">JSON-based custom service</span></span>
- <span data-ttu-id="2dfd6-139">إجراءات كيان OData</span><span class="sxs-lookup"><span data-stu-id="2dfd6-139">OData entity’s actions</span></span>
- <span data-ttu-id="2dfd6-140">الخدمة المخصصة المستندة إلى SOAP</span><span class="sxs-lookup"><span data-stu-id="2dfd6-140">SOAP-based custom service</span></span>

<span data-ttu-id="2dfd6-141">تتشارك الأساليب في الخصائص الآتية:</span><span class="sxs-lookup"><span data-stu-id="2dfd6-141">The techniques share the following characteristics:</span></span>

- <span data-ttu-id="2dfd6-142">متزامنة</span><span class="sxs-lookup"><span data-stu-id="2dfd6-142">Synchronous</span></span>
- <span data-ttu-id="2dfd6-143">قابلة للتخصيص</span><span class="sxs-lookup"><span data-stu-id="2dfd6-143">Customizable</span></span>
- <span data-ttu-id="2dfd6-144">تسمح بمعلمات التمرير</span><span class="sxs-lookup"><span data-stu-id="2dfd6-144">Allow passing parameters</span></span> 
- <span data-ttu-id="2dfd6-145">لا تتطلب معالجة المنفذ</span><span class="sxs-lookup"><span data-stu-id="2dfd6-145">Do not require port handling</span></span>
- <span data-ttu-id="2dfd6-146">مصادقة Azure AD</span><span class="sxs-lookup"><span data-stu-id="2dfd6-146">Azure AD authentication</span></span>

## <a name="application-integration-framework-aif-file-based-exchange-or-msmq"></a><span data-ttu-id="2dfd6-147">التبادل المستند إلى الملفات لإطار عمل تكامل التطبيق (AIF) أو MSMQ</span><span class="sxs-lookup"><span data-stu-id="2dfd6-147">Application Integration Framework (AIF) file-based exchange or MSMQ</span></span> 

<span data-ttu-id="2dfd6-148">يتم دفع المستندات في Dynamics AX2012 باستخدام تنسيق XML القياسي، أو باستخدام تحويل XSLT.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-148">Documents are pushed in Dynamics AX 2012 by using XML standard format, or by using XSLT transformation.</span></span> <span data-ttu-id="2dfd6-149">يتم إدراج الرسائل في قائمة الانتظار ومعالجتها بشكل غير متزامن.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-149">The messages are enqueued and processed asynchronously.</span></span>

- <span data-ttu-id="2dfd6-150">مستوى صوت عالٍ</span><span class="sxs-lookup"><span data-stu-id="2dfd6-150">High volume</span></span>
- <span data-ttu-id="2dfd6-151">غير متزامنة</span><span class="sxs-lookup"><span data-stu-id="2dfd6-151">Asynchronous</span></span> 
- <span data-ttu-id="2dfd6-152">التحويل (اختياري)</span><span class="sxs-lookup"><span data-stu-id="2dfd6-152">Transformation (optional)</span></span>


<span data-ttu-id="2dfd6-153">مثال: استيراد بيانات الحركة من مستودع تلقائي، والذي تم إرساله كملفات بتنسيق ‎.csv.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-153">Example: Importing movement data from an automated warehouse, which was sent as .csv files.</span></span>

<span data-ttu-id="2dfd6-154">في تطبيقات Finance and Operations، يمكنك استخدام خدمات Azure أو Data Management Framework‏ (DMF):</span><span class="sxs-lookup"><span data-stu-id="2dfd6-154">In Finance and Operations apps, you can use Azure Services or the Data Management Framework (DMF):</span></span>

- <span data-ttu-id="2dfd6-155">يسمح **Data Management Framework‏** بآلية الإدراج في قائمة الانتظار/إزالة من قائمة الانتظار وعمليات التحويل المدمجة.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-155">**Data Management Framework** allows compact enqueuing/dequeuing mechanism and transformations.</span></span> <span data-ttu-id="2dfd6-156">ويتطلب آلية خارجية لإرسال الملفات إلى Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-156">It requires an external mechanism to send the files to Dynamics 365.</span></span>
- <span data-ttu-id="2dfd6-157">من خلال **خدمات Azure** باستخدام برنامج وسيط خارجي (على سبيل المثال، Logic Apps)، والتي تسمح بفصل الأعمال في منطق الأعمال ERP من منطق التحويل وتوفير المزيد من المرونة.</span><span class="sxs-lookup"><span data-stu-id="2dfd6-157">Through **Azure Services** by using an external middleware (for example, Logic Apps), which allows decoupling the ERP business logics from the transformation logics and provides more flexibility.</span></span>

