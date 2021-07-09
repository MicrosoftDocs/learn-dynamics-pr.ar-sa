---
ms.openlocfilehash: f8b8170faddef4fdbe828f097d657d9fc3bb7044
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072404"
---
<span data-ttu-id="9a00c-101">خلال رحلة الترقية، يجب أن تكون قادراً على اتخاذ قرارات مدروسة بشأن سيناريوهات تكامل البيانات عند تنفيذ تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="9a00c-101">Throughout your upgrade journey, you need to be able to make thoughtful decisions about data integration scenarios when implementing Finance and Operations apps.</span></span> 

<span data-ttu-id="9a00c-102">عند اختيار نمط تكامل، تجب مراعاة عدة عوامل، مثل تلك التي تجب مراعاتها عند تنفيذ Dynamics AX 2012.</span><span class="sxs-lookup"><span data-stu-id="9a00c-102">When choosing an integration pattern, you should consider several factors, as you would have when implementing Dynamics AX 2012.</span></span> <span data-ttu-id="9a00c-103">والفرق أنك تعمل، الآن، على تطبيق قائم على السحابة داخل Azure.</span><span class="sxs-lookup"><span data-stu-id="9a00c-103">The difference is that, now, you are working on a cloud-based application within Azure.</span></span> 

## <a name="latency"></a><span data-ttu-id="9a00c-104">زمن الانتقال</span><span class="sxs-lookup"><span data-stu-id="9a00c-104">Latency</span></span> 

<span data-ttu-id="9a00c-105">ضع في اعتبارك العوامل الآتية المتعلقة بزمن الانتقال:</span><span class="sxs-lookup"><span data-stu-id="9a00c-105">Consider the following factors regarding latency:</span></span>

- <span data-ttu-id="9a00c-106">**متزامن** يتم تشغيل التكامل مع الاستجابة الفورية المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-106">**Synchronous** - Integration is triggered with an immediate response that is required.</span></span> 
- <span data-ttu-id="9a00c-107">**غير متزامن** يتم تشغيل التكامل مع الاستجابة المتأخرة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-107">**Asynchronous** - Integration is triggered with a delayed response that is required.</span></span> 
    - <span data-ttu-id="9a00c-108">قريب من الوقت الحقيقي - يُسمح بأقل زمن انتقال (أقل من دقيقة واحدة) بين المشغل والإرسال.</span><span class="sxs-lookup"><span data-stu-id="9a00c-108">Near real-time - Minimal latency (<1 minute) is allowed between trigger and transmission.</span></span> 
    - <span data-ttu-id="9a00c-109">الدُفعة المجدولة - سيحدث التكامل على أساس مجدول مع تكرار محدد سابقاً.</span><span class="sxs-lookup"><span data-stu-id="9a00c-109">Scheduled batch - Integration will occur on a scheduled basis with a pre-determined recurrence.</span></span>


## <a name="message-routing"></a><span data-ttu-id="9a00c-110">توجيه الرسائل</span><span class="sxs-lookup"><span data-stu-id="9a00c-110">Message routing</span></span>

<span data-ttu-id="9a00c-111">ضع في اعتبارك العوامل المتعلقة بتوجيه الرسائل الآتية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-111">Consider the following factors regarding message routing:</span></span>

- <span data-ttu-id="9a00c-112">**نقطة إلى نقطة** Dynamics 365إلى نظام قديم</span><span class="sxs-lookup"><span data-stu-id="9a00c-112">**Point-to-Point** - Dynamics 365 to Legacy System</span></span>
- <span data-ttu-id="9a00c-113">**ناقل خدمة المؤسسة** - خادم BizTalk وأخرى</span><span class="sxs-lookup"><span data-stu-id="9a00c-113">**Enterprise Service Bus** - BizTalk Server and others</span></span>
- <span data-ttu-id="9a00c-114">**وسيط، المركز والمتحدث أو استخراج، نقل، تحميل (ETL)** - على سبيل المثال، برنامج SQL Server Integration Services</span><span class="sxs-lookup"><span data-stu-id="9a00c-114">**Broker, Hub & Spoke, or Extract, Transform, Load (ETL)** - For example, SQL Server Integration Services</span></span> 


## <a name="frequency"></a><span data-ttu-id="9a00c-115">التكرار</span><span class="sxs-lookup"><span data-stu-id="9a00c-115">Frequency</span></span>

<span data-ttu-id="9a00c-116">يمكن تصنيف طلب التكامل في التكرارات الآتية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-116">The integration request can be classified into the following frequencies:</span></span> 

- <span data-ttu-id="9a00c-117">**مرتفع** ثوانٍ أو دقائق</span><span class="sxs-lookup"><span data-stu-id="9a00c-117">**High** - Seconds or minutes</span></span> 
- <span data-ttu-id="9a00c-118">**متوسط** ساعات أو أيام</span><span class="sxs-lookup"><span data-stu-id="9a00c-118">**Medium** - Hours or days</span></span> 
- <span data-ttu-id="9a00c-119">**منخفض** - أسابيع أو أشهر</span><span class="sxs-lookup"><span data-stu-id="9a00c-119">**Low** - Weeks or months</span></span>


## <a name="trigger"></a><span data-ttu-id="9a00c-120">المشغِّل</span><span class="sxs-lookup"><span data-stu-id="9a00c-120">Trigger</span></span>

<span data-ttu-id="9a00c-121">ضع في اعتبارك العوامل المتعلقة بالمشغِّل الآتية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-121">Consider the following factors regarding trigger:</span></span>

- <span data-ttu-id="9a00c-122">**عند الطلب/يدوي** - تكامل يبدأ يدوياً بواسطة المستخدم النهائي أو مستخدم تقنية المعلومات.</span><span class="sxs-lookup"><span data-stu-id="9a00c-122">**On-Demand/Manual** - Integration is manually initiated by an end user or an IT user.</span></span> 
- <span data-ttu-id="9a00c-123">**الحدث المُشغَّل** - تكامل يتم تشغيله استناداً إلى حدث أو حالة في النظام المصدر أو النظام الوجهة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-123">**Event Triggered** - Integration is triggered based on an event or condition in the source or destination system.</span></span> 
- <span data-ttu-id="9a00c-124">**الوقت/التاريخ المجدول** تكامل يتم تشغيله بناء على جدول محدد سابقاً.</span><span class="sxs-lookup"><span data-stu-id="9a00c-124">**Time/Date Scheduled** - Integration is triggered based on a predetermined schedule.</span></span> 


## <a name="interactionoperations"></a><span data-ttu-id="9a00c-125">التفاعل/العمليات</span><span class="sxs-lookup"><span data-stu-id="9a00c-125">Interaction/Operations</span></span>

<span data-ttu-id="9a00c-126">ضع في اعتبارك العوامل المتعلقة بالتفاعل/العمليات الآتية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-126">Consider the following factors regarding interaction/operations:</span></span>

<span data-ttu-id="9a00c-127">**إنشاء** -سجل سيتم إنشاؤه في النظام الوجهة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-127">**Create** - Record will be created in the destination system.</span></span>
<span data-ttu-id="9a00c-128">**قراءة** تكامل سوف يستعلم عن المصدر ويعيد جزء البيانات المطلوب على وجه التحديد.</span><span class="sxs-lookup"><span data-stu-id="9a00c-128">**Read** - Integration will query the source and return a specifically requested piece of data.</span></span> 
<span data-ttu-id="9a00c-129">**تحديث** - تكامل سيقوم بتحديث سجل موجود في النظام الوجهة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-129">**Update** - Integration will update an existing record in the destination system.</span></span> 
<span data-ttu-id="9a00c-130">**حذف** - النتائج في حذف سجل في النظام الوجهة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-130">**Delete** - Results in the deletion of a record in the destination system.</span></span>
<span data-ttu-id="9a00c-131">**إجراء** - تكامل سيقوم بتشغيل حدث نظام، مثل **حساب سعر أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="9a00c-131">**Action** -Integration will trigger a system event, for example, **Calculate sales order price**.</span></span>

## <a name="batching"></a><span data-ttu-id="9a00c-132">الدفعات</span><span class="sxs-lookup"><span data-stu-id="9a00c-132">Batching</span></span>

<span data-ttu-id="9a00c-133">ضع في اعتبارك العوامل المتعلقة بالتجميع الآتية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-133">Consider the following factors regarding batching:</span></span>

- <span data-ttu-id="9a00c-134">**غير مجمَّع** سجلات فردية يتم إرسالها في طلب التكامل.</span><span class="sxs-lookup"><span data-stu-id="9a00c-134">**Unbatched** - Individual records are sent in the integration request.</span></span> 
- <span data-ttu-id="9a00c-135">**مجمَّع** سجلات يتم توحيدها للإرسال من خلال طلب التكامل.</span><span class="sxs-lookup"><span data-stu-id="9a00c-135">**Batched** - Records are consolidated for transmission through the integration request.</span></span>

## <a name="volume"></a><span data-ttu-id="9a00c-136">المقدار</span><span class="sxs-lookup"><span data-stu-id="9a00c-136">Volume</span></span>

<span data-ttu-id="9a00c-137">يجب أن يكون عدد السجلات لكل طلب مجمَّع إما **منخفض** أو **متوسط** أو **مرتفع** المقدار.</span><span class="sxs-lookup"><span data-stu-id="9a00c-137">The number of records for each batched request should be either **Low**, **Medium**, or **High** volume.</span></span> 

## <a name="transport-protocol"></a><span data-ttu-id="9a00c-138">بروتوكول النقل</span><span class="sxs-lookup"><span data-stu-id="9a00c-138">Transport protocol</span></span>

<span data-ttu-id="9a00c-139">ضع في اعتبارك العوامل المتعلقة ببروتوكول النقل الآتية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-139">Consider the following factors regarding transport protocol:</span></span>

- <span data-ttu-id="9a00c-140">خدمة Windows File وFTP/SFTP</span><span class="sxs-lookup"><span data-stu-id="9a00c-140">Windows File Service and FTP/SFTP</span></span>
- <span data-ttu-id="9a00c-141">بروتوكول HTTP/HTTPS وخدمة ويب WCF وخدمة ويب SOAP</span><span class="sxs-lookup"><span data-stu-id="9a00c-141">HTTP/HTTPS, WCF Web Service, and SOAP Web Service</span></span>
- <span data-ttu-id="9a00c-142">واجهة ODBC واستعلام Direct SQL</span><span class="sxs-lookup"><span data-stu-id="9a00c-142">ODBC and Direct SQL Query</span></span>

## <a name="file-formats-and-schemadata-dictionary"></a><span data-ttu-id="9a00c-143">تنسيقات الملفات وقاموس المخطط/البيانات</span><span class="sxs-lookup"><span data-stu-id="9a00c-143">File formats and Schema/Data Dictionary</span></span>

<span data-ttu-id="9a00c-144">تجب مراعاة العوامل الآتية المتعلقة بتنسيقات الملفات وقاموس المخطط/البيانات:</span><span class="sxs-lookup"><span data-stu-id="9a00c-144">Consider the following factors regarding file formats and Schema/Data Dictionary:</span></span>

- <span data-ttu-id="9a00c-145">**تنسيقات الملفات** ملف ثابت و.NET TCP وXML وما شابه ذلك</span><span class="sxs-lookup"><span data-stu-id="9a00c-145">**File formats** - Flat file, .NET TCP, XML, and so on</span></span> 
- <span data-ttu-id="9a00c-146">**مخطط الرسالة/واجهة برمجة التطبيقات (API)** - XSD / WSDL / OpenAPI (Swagger)</span><span class="sxs-lookup"><span data-stu-id="9a00c-146">**Message/API Schema** - XSD / WSDL / OpenAPI (Swagger)</span></span>

## <a name="data-mappingmetadata-definition"></a><span data-ttu-id="9a00c-147">تعيين البيانات/تحديد بيانات التعريف</span><span class="sxs-lookup"><span data-stu-id="9a00c-147">Data mapping/metadata definition</span></span>

<span data-ttu-id="9a00c-148">ضع في اعتبارك العوامل الآتية المتعلقة بتعيين البيانات/تحديد بيانات التعريف:</span><span class="sxs-lookup"><span data-stu-id="9a00c-148">Consider the following factors regarding data mapping/metadata definition:</span></span>

- <span data-ttu-id="9a00c-149">**نموذج متعارف عليه** - تكامل يتم تعيينه إلى نموذج قياسي في وسيط أو ESB.</span><span class="sxs-lookup"><span data-stu-id="9a00c-149">**Canonical model** - Integration is mapped to a standardized model in a broker or ESB.</span></span> 
- <span data-ttu-id="9a00c-150">**تنسيق خاص بالتطبيق** - تعيين مباشر بين النظام المصدر والنظام الوجهة.</span><span class="sxs-lookup"><span data-stu-id="9a00c-150">**Application specific format** - Direct mapping between the source and destination systems.</span></span> 

## <a name="transformation-and-translation-point"></a><span data-ttu-id="9a00c-151">نقطة التحويل والترجمة</span><span class="sxs-lookup"><span data-stu-id="9a00c-151">Transformation and translation point</span></span>

<span data-ttu-id="9a00c-152">تجب مراعاة العوامل الآتية فيما يتعلق بنقطة التحويل والترجمة:</span><span class="sxs-lookup"><span data-stu-id="9a00c-152">Consider the following factors regarding transformation and translation point:</span></span>

- <span data-ttu-id="9a00c-153">**ESB/وسيط** - يحدث في نظام الوسيط أثناء عملية التكامل (في حالة عدم طلب منطق).</span><span class="sxs-lookup"><span data-stu-id="9a00c-153">**ESB/Broker** - Occurs in the broker system during the integration process (if no logic is required).</span></span>
- <span data-ttu-id="9a00c-154">**الوجهة** - تحدث في النظام الوجهة (إذا كان منطق العمل مطلوباً للتحويل).</span><span class="sxs-lookup"><span data-stu-id="9a00c-154">**Destination** - Occurs in the destination system (if business logic is required for the transformation).</span></span>
- <span data-ttu-id="9a00c-155">**المصدر** - يحدث في النظام المصدر قبل إرسال البيانات (إذا كان المنطق مطلوباً).</span><span class="sxs-lookup"><span data-stu-id="9a00c-155">**Source** - Occurs in the source system before the data is transmitted (if logic is required).</span></span> 

## <a name="error-handling-and-reconciliation"></a><span data-ttu-id="9a00c-156">معالجة الأخطاء والتسوية</span><span class="sxs-lookup"><span data-stu-id="9a00c-156">Error handling and reconciliation</span></span>

<span data-ttu-id="9a00c-157">تجب مراعاة العوامل الآتية فيما يتعلق بمعالجة الأخطاء والتسوية:</span><span class="sxs-lookup"><span data-stu-id="9a00c-157">Consider the following factors regarding error handling and reconciliation:</span></span>

- <span data-ttu-id="9a00c-158">**إخطارات** - البريد الكتروني ولوحة المعلومات والرسائل النصية وما شابه ذلك</span><span class="sxs-lookup"><span data-stu-id="9a00c-158">**Notifications** - Email, Dashboard, SMS, and so on</span></span> 
- <span data-ttu-id="9a00c-159">**نقطة التسوية** - التطبيق والبرنامج الوسيط وأداة المراقبة المساعدة وما شابه ذلك</span><span class="sxs-lookup"><span data-stu-id="9a00c-159">**Reconciliation point** - Application, Middleware, Monitoring utility, and so on</span></span>
- <span data-ttu-id="9a00c-160">**أدوات التسوية** خدمات جودة البيانات والتقارير والاستعلامات وما إلى ذلك</span><span class="sxs-lookup"><span data-stu-id="9a00c-160">**Reconciliation tools** - Data quality services, reports, queries, and so on</span></span>


