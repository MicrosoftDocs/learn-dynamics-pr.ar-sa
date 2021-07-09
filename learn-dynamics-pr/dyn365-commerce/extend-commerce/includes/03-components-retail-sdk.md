---
ms.openlocfilehash: b176f7ddd99e137cb55af0840a5daaecbb30cdd8
ms.sourcegitcommit: 2475a4326b76fa8838c2e4e6885473bdd6fe6270
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/02/2021
ms.locfileid: "6070443"
---
<span data-ttu-id="6d1d2-101">توفر الجداول التالية معلومات حول المكونات الموجودة في عدة تطوير البرامج (SDK) التي يجب تخصيصها لسيناريوهات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-101">The following tables provide information about the components in the software development kit (SDK) that must be customized for different scenarios.</span></span> <span data-ttu-id="6d1d2-102">يمكن فقط تعديل المشروعات النموذجية داخل Retail SDK\SampleExtensions لأغراض الملحق.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-102">Only the sample projects inside the Retail SDK\SampleExtensions can be modified for extension purposes.</span></span> <span data-ttu-id="6d1d2-103">يجب عدم تعديل أي ملفات أو مشروعات أو نصوص برمجية أخرى في Retail SDK.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-103">No other files, projects, or scripts should be modified in the Retail SDK.</span></span>


## <a name="client-pos"></a><span data-ttu-id="6d1d2-104">العميل (نقطة البيع)</span><span class="sxs-lookup"><span data-stu-id="6d1d2-104">Client (POS)</span></span>


| <span data-ttu-id="6d1d2-105">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-105">**Item**</span></span> | <span data-ttu-id="6d1d2-106">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-106">**Description**</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="6d1d2-107">**السيناريوهات**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-107">**Scenarios**</span></span> | <span data-ttu-id="6d1d2-108">توسيع نقطة البيع لتغييرات تجربة المستخدم ومنطق العميل وسير العمل وعمليات التحقق البسيطة.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-108">Extend the point of sale (POS) for user experience changes, client logic, workflow, and simple validations.</span></span>|
 |  <span data-ttu-id="6d1d2-109">**مرجع Commerce SDK**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-109">**Commerce SDK reference**</span></span> | <span data-ttu-id="6d1d2-110">\RetailSDK\POS.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-110">\RetailSDK\POS.</span></span> <span data-ttu-id="6d1d2-111">افتح الملف **ModernPos.sln** أو **CloudPos.sln**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-111">Open the **ModernPos.sln** or **CloudPos.sln** file.</span></span> <span data-ttu-id="6d1d2-112">أضف الملحق إلى المشروع **POS.Extension**، ولكن لا تقم بتعديل أي شيء في مشروعات تطبيق نقطة البيع/الويب الأساسية.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-112">Add the extension to the **POS.Extension** project, but don't modify anything in the core POS app/web projects.</span></span>|
|  <span data-ttu-id="6d1d2-113">**التقنية**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-113">**Technology**</span></span> | <span data-ttu-id="6d1d2-114">Typescript وHTML وCSS</span><span class="sxs-lookup"><span data-stu-id="6d1d2-114">Typescript, HTML, and CSS</span></span>|
|  <span data-ttu-id="6d1d2-115">**الوثائق**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-115">**Documentation**</span></span> | [<span data-ttu-id="6d1d2-116">تشغيل نماذج نقطة البيع</span><span class="sxs-lookup"><span data-stu-id="6d1d2-116">Run the point of sale (POS) samples</span></span>]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-run-samples/?azure-portal=true)|
    

## <a name="commerce-runtime-crt"></a><span data-ttu-id="6d1d2-117">Commerce runtime (CRT)</span><span class="sxs-lookup"><span data-stu-id="6d1d2-117">Commerce runtime (CRT)</span></span>


| <span data-ttu-id="6d1d2-118">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-118">**Item**</span></span> | <span data-ttu-id="6d1d2-119">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-119">**Description**</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="6d1d2-120">**السيناريوهات**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-120">**Scenarios**</span></span> | <span data-ttu-id="6d1d2-121">توسيع commerce runtime لإضافة منطق الأعمال أو تعديله، على سبيل المثال، حساب الضريبة والسعر والخصم وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-121">Extend the commerce runtime to add or modify business logic, for example, calculating tax, price, discount, and so on.</span></span>|
 |  <span data-ttu-id="6d1d2-122">**مرجع Commerce SDK**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-122">**Commerce SDK reference**</span></span> | <span data-ttu-id="6d1d2-123">\RetailSDK\SampleExtensions\CommerceRuntime.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-123">\RetailSDK\SampleExtensions\CommerceRuntime.</span></span> <span data-ttu-id="6d1d2-124">افتح الملف **CommerceRuntimeSamples.sln**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-124">Open the **CommerceRuntimeSamples.sln** file.</span></span>|
|  <span data-ttu-id="6d1d2-125">**التقنية**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-125">**Technology**</span></span> | <span data-ttu-id="6d1d2-126">C#</span><span class="sxs-lookup"><span data-stu-id="6d1d2-126">C#</span></span>|
|  <span data-ttu-id="6d1d2-127">**الوثائق**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-127">**Documentation**</span></span> | [<span data-ttu-id="6d1d2-128">قابلية توسعة Commerce runtime (CRT) وRetail Server</span><span class="sxs-lookup"><span data-stu-id="6d1d2-128">Commerce runtime (CRT) and Retail Server extensibility</span></span>](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/commerce-runtime-extensibility/?azure-portal=true) |


## <a name="retail-server-rs"></a><span data-ttu-id="6d1d2-129">Retail server (RS)</span><span class="sxs-lookup"><span data-stu-id="6d1d2-129">Retail server (RS)</span></span>


| <span data-ttu-id="6d1d2-130">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-130">**Item**</span></span> | <span data-ttu-id="6d1d2-131">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-131">**Description**</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="6d1d2-132">**السيناريوهات**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-132">**Scenarios**</span></span> | <span data-ttu-id="6d1d2-133">إنشاء ملحق Retail Server جديد لعرض واجهات Commerce API الجديدة للعميل.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-133">Create a new Retail Server extension to expose new Commerce APIs to the client.</span></span>|
 |  <span data-ttu-id="6d1d2-134">**مرجع Commerce SDK**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-134">**Commerce SDK reference**</span></span> | <span data-ttu-id="6d1d2-135">\RetailSDK\SampleExtensions\RetailServer.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-135">\RetailSDK\SampleExtensions\RetailServer.</span></span> <span data-ttu-id="6d1d2-136">افتح أي من الملحقات النموذجية في المجلد **RetailServer**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-136">Open any of the sample extensions inside the **RetailServer** folder.</span></span>|
|  <span data-ttu-id="6d1d2-137">**التقنية**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-137">**Technology**</span></span> | <span data-ttu-id="6d1d2-138">OData، C#</span><span class="sxs-lookup"><span data-stu-id="6d1d2-138">OData, C#</span></span>|
|  <span data-ttu-id="6d1d2-139">**الوثائق**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-139">**Documentation**</span></span> |[<span data-ttu-id="6d1d2-140">إنشاء واجهة API جديدة لملحق Retail Server (الإصدار 10.0.11 والإصدارات اللاحقة من Retail SDK)</span><span class="sxs-lookup"><span data-stu-id="6d1d2-140">Create a new Retail Server extension API (Retail SDK version 10.0.11 and later)</span></span>](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/retail-server-extension) |


## <a name="typescript-proxy"></a><span data-ttu-id="6d1d2-141">وكيل Typescript</span><span class="sxs-lookup"><span data-stu-id="6d1d2-141">Typescript proxy</span></span>


| <span data-ttu-id="6d1d2-142">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-142">**Item**</span></span> | <span data-ttu-id="6d1d2-143">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-143">**Description**</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="6d1d2-144">**السيناريوهات**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-144">**Scenarios**</span></span> | <span data-ttu-id="6d1d2-145">يكون وكيل Typescript مطلوباً إذا كانت ملحقات RS الجديدة بحاجة إلى أن يتم استهلاكها في عملاء نقطة البيع أو التجارة الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-145">Typescript proxy is required if new RS extensions need to be consumed in POS or e-Commerce clients.</span></span>|
 |  <span data-ttu-id="6d1d2-146">**مرجع Commerce SDK**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-146">**Commerce SDK reference**</span></span> | <span data-ttu-id="6d1d2-147">\RetailSDK\SampleExtensions\RetailServer.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-147">\RetailSDK\SampleExtensions\RetailServer.</span></span> <span data-ttu-id="6d1d2-148">افتح أي من الملحقات النموذجية في المجلد **RetailServer**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-148">Open any of the sample extensions inside the **RetailServer** folder.</span></span> |
 |  <span data-ttu-id="6d1d2-149">**التقنية**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-149">**Technology**</span></span> | <span data-ttu-id="6d1d2-150">OData، C#</span><span class="sxs-lookup"><span data-stu-id="6d1d2-150">OData, C#</span></span>|
|  <span data-ttu-id="6d1d2-151">**الوثائق**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-151">**Documentation**</span></span> | <span data-ttu-id="6d1d2-152">[إنشاء وكيل Typescript لنقطة البيع]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/retail-server-icontroller-extension/?azure-portal=true#generate-the-typescript-proxy-for-pos) (الإصدار 10.0.11 والإصدارات اللاحقة من Retail SDK)</span><span class="sxs-lookup"><span data-stu-id="6d1d2-152">[Generate the Typescript proxy for POS]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/retail-server-icontroller-extension/?azure-portal=true#generate-the-typescript-proxy-for-pos) (Retail SDK version 10.0.11 and later)</span></span>|


## <a name="hardware-station"></a><span data-ttu-id="6d1d2-153">محطة الأجهزة</span><span class="sxs-lookup"><span data-stu-id="6d1d2-153">Hardware station</span></span>


| <span data-ttu-id="6d1d2-154">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-154">**Item**</span></span> | <span data-ttu-id="6d1d2-155">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-155">**Description**</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="6d1d2-156">**السيناريوهات**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-156">**Scenarios**</span></span> | <span data-ttu-id="6d1d2-157">محطة أجهزة لإضافة المنطق المتعلق بالأجهزة الطرفية أو تعديله.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-157">Hardware station to add or modify logics that are related to peripherals.</span></span>|
 |  <span data-ttu-id="6d1d2-158">**مرجع Commerce SDK**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-158">**Commerce SDK reference**</span></span> | <span data-ttu-id="6d1d2-159">\RetailSDK\ \SampleExtensions\HardwareStation.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-159">\RetailSDK\ \SampleExtensions\HardwareStation.</span></span> <span data-ttu-id="6d1d2-160">افتح الملف **HardwareStationSamples.sln**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-160">Open the **HardwareStationSamples.sln** file.</span></span>|
|  <span data-ttu-id="6d1d2-161">**التقنية**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-161">**Technology**</span></span> | <span data-ttu-id="6d1d2-162">C#</span><span class="sxs-lookup"><span data-stu-id="6d1d2-162">C#</span></span>|
|  <span data-ttu-id="6d1d2-163">**الوثائق**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-163">**Documentation**</span></span> | [<span data-ttu-id="6d1d2-164">دمج نقطة البيع مع جهاز جديد</span><span class="sxs-lookup"><span data-stu-id="6d1d2-164">Integrate POS with a new hardware device</span></span>](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/hardware-device-extension/?azure-portal=true)|


## <a name="payment"></a><span data-ttu-id="6d1d2-165">الدفع</span><span class="sxs-lookup"><span data-stu-id="6d1d2-165">Payment</span></span>


| <span data-ttu-id="6d1d2-166">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-166">**Item**</span></span> | <span data-ttu-id="6d1d2-167">**الوصف**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-167">**Description**</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="6d1d2-168">**السيناريوهات**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-168">**Scenarios**</span></span> | <span data-ttu-id="6d1d2-169">دمج نقطة البيع مع موصل مدفوعات جديد.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-169">Integrate POS with a new payment connector.</span></span>|
 |  <span data-ttu-id="6d1d2-170">**مرجع Commerce SDK**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-170">**Commerce SDK reference**</span></span> | <span data-ttu-id="6d1d2-171">\RetailSDK\SampleExtensions\HardwareStation\Extension.PaymentSample.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-171">\RetailSDK\SampleExtensions\HardwareStation\Extension.PaymentSample.</span></span> <span data-ttu-id="6d1d2-172">افتح الملف **HardwareStation.Extension.PaymentSample.sln**.</span><span class="sxs-lookup"><span data-stu-id="6d1d2-172">Open the **HardwareStation.Extension.PaymentSample.sln** file.</span></span>|
|  <span data-ttu-id="6d1d2-173">**التقنية**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-173">**Technology**</span></span> | <span data-ttu-id="6d1d2-174">C#</span><span class="sxs-lookup"><span data-stu-id="6d1d2-174">C#</span></span>|
|  <span data-ttu-id="6d1d2-175">**الوثائق**</span><span class="sxs-lookup"><span data-stu-id="6d1d2-175">**Documentation**</span></span> |[<span data-ttu-id="6d1d2-176"> إنشاء تكامل الدفع الشامل للوحدة الطرفية للدفع</span><span class="sxs-lookup"><span data-stu-id="6d1d2-176"> Create an end-to-end payment integration for a payment terminal</span></span>](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/end-to-end-payment-extension/?azure-portal=true)

