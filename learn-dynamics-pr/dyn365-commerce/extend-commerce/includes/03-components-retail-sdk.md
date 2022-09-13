---
ms.openlocfilehash: 538dda5f7f82c4b4876125df98acb5acbfd02334
ms.sourcegitcommit: 719553652dcf44322f1628d12e79bc870ba0ddd1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/15/2022
ms.locfileid: "9300815"
---
توفر الجداول التالية معلومات حول المكونات الموجودة في عدة تطوير البرامج (SDK) التي يجب تخصيصها لسيناريوهات مختلفة. يمكن فقط تعديل المشروعات النموذجية داخل Retail SDK\SampleExtensions لأغراض الملحق. يجب عدم تعديل أي ملفات أو مشروعات أو نصوص برمجية أخرى في Retail SDK.


## <a name="store-commerce"></a>Store Commerce


| **الصنف** | **الوصف‏‎** |
 | ------------- | ------------- |
 | **السيناريوهات** | توسيع Store Commerce لتغييرات تجربة المستخدم ومنطق العميل وسير العمل وعمليات التحقق من الصحة البسيطة.|
 |  **مرجع Commerce SDK** | \RetailSDK\POS. افتح الملف **ModernPos.sln** أو **CloudPos.sln**. أضف الملحق إلى مشروع **POS.Extension**، ولكن لا تقم بتعديل أي شيء في مشروعات تطبيق Store Commerce/الويب الأساسية.|
|  **التقنية** | Typescript وHTML وCSS|
|  **الوثائق** | [تشغيل نماذج Store Commerce]( /dynamics365/commerce/dev-itpro/pos-run-samples/?azure-portal=true)|
    

## <a name="commerce-runtime-crt"></a>Commerce runtime (CRT)


| **الصنف** | **الوصف‏‎** |
 | ------------- | ------------- |
 | **السيناريوهات** | توسيع commerce runtime لإضافة منطق الأعمال أو تعديله، على سبيل المثال، حساب الضريبة والسعر والخصم وما إلى ذلك.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\CommerceRuntime. افتح الملف **CommerceRuntimeSamples.sln**.|
|  **التقنية** | C#|
|  **الوثائق** | [قابلية توسعة Commerce runtime (CRT) وRetail Server](/dynamics365/commerce/dev-itpro/commerce-runtime-extensibility/?azure-portal=true) |


## <a name="retail-server-rs"></a>Retail server (RS)


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | إنشاء ملحق Retail Server جديد لعرض واجهات Commerce API الجديدة للعميل.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\RetailServer. افتح أي من الملحقات النموذجية في المجلد **RetailServer**.|
|  **التقنية** | OData، C#|
|  **الوثائق** |[إنشاء واجهة API جديدة لملحق Retail Server (الإصدار 10.0.11 والإصدارات اللاحقة من Retail SDK)](/dynamics365/commerce/dev-itpro/retail-server-extension/?azure-portal=true) |


## <a name="typescript-proxy"></a>وكيل Typescript


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | يكون وكيل Typescript مطلوباً إذا كانت هناك حاجة إلى استهلاك ملحقات RS جديدة في عملاء Store Commerce أو التجارة الإلكترونية.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\RetailServer. افتح أي من الملحقات النموذجية في المجلد **RetailServer**. |
 |  **التقنية** | OData، C#|
|  **الوثائق** | [إنشاء وكيل Typescript لـ Store Commerce]( /dynamics365/commerce/dev-itpro/retail-server-icontroller-extension/?azure-portal=true#generate-the-typescript-proxy-for-pos) (Retail SDK إصدار 10.0.11 والأحدث)|


## <a name="hardware-station"></a>محطة الأجهزة


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | محطة أجهزة لإضافة المنطق المتعلق بالأجهزة الطرفية أو تعديله.|
 |  **مرجع Commerce SDK** | \RetailSDK\ \SampleExtensions\HardwareStation. افتح الملف **HardwareStationSamples.sln**.|
|  **التقنية** | C#|
|  **الوثائق** | [دمج Store Commerce مع جهاز جديد](/dynamics365/commerce/dev-itpro/hardware-device-extension/?azure-portal=true)|


## <a name="payment"></a>الدفع


| **الصنف** | **الوصف‏‎** |
 | ------------- | ------------- |
 | **السيناريوهات** | دمج Store Commerce مع موصل مدفوعات جديد.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\HardwareStation\Extension.PaymentSample. افتح الملف **HardwareStation.Extension.PaymentSample.sln**.|
|  **التقنية** | C#|
|  **الوثائق** |[ إنشاء تكامل الدفع الشامل للوحدة الطرفية للدفع](/dynamics365/commerce/dev-itpro/end-to-end-payment-extension/?azure-portal=true)

