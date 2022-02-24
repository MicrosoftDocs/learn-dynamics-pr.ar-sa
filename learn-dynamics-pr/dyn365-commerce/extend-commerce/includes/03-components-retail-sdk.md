---
ms.openlocfilehash: b176f7ddd99e137cb55af0840a5daaecbb30cdd8
ms.sourcegitcommit: 2475a4326b76fa8838c2e4e6885473bdd6fe6270
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/02/2021
ms.locfileid: "6070443"
---
توفر الجداول التالية معلومات حول المكونات الموجودة في عدة تطوير البرامج (SDK) التي يجب تخصيصها لسيناريوهات مختلفة. يمكن فقط تعديل المشروعات النموذجية داخل Retail SDK\SampleExtensions لأغراض الملحق. يجب عدم تعديل أي ملفات أو مشروعات أو نصوص برمجية أخرى في Retail SDK.


## <a name="client-pos"></a>العميل (نقطة البيع)


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | توسيع نقطة البيع لتغييرات تجربة المستخدم ومنطق العميل وسير العمل وعمليات التحقق البسيطة.|
 |  **مرجع Commerce SDK** | \RetailSDK\POS. افتح الملف **ModernPos.sln** أو **CloudPos.sln**. أضف الملحق إلى المشروع **POS.Extension**، ولكن لا تقم بتعديل أي شيء في مشروعات تطبيق نقطة البيع/الويب الأساسية.|
|  **التقنية** | Typescript وHTML وCSS|
|  **الوثائق** | [تشغيل نماذج نقطة البيع]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-run-samples/?azure-portal=true)|
    

## <a name="commerce-runtime-crt"></a>Commerce runtime (CRT)


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | توسيع commerce runtime لإضافة منطق الأعمال أو تعديله، على سبيل المثال، حساب الضريبة والسعر والخصم وما إلى ذلك.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\CommerceRuntime. افتح الملف **CommerceRuntimeSamples.sln**.|
|  **التقنية** | C#|
|  **الوثائق** | [قابلية توسعة Commerce runtime (CRT) وRetail Server](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/commerce-runtime-extensibility/?azure-portal=true) |


## <a name="retail-server-rs"></a>Retail server (RS)


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | إنشاء ملحق Retail Server جديد لعرض واجهات Commerce API الجديدة للعميل.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\RetailServer. افتح أي من الملحقات النموذجية في المجلد **RetailServer**.|
|  **التقنية** | OData، C#|
|  **الوثائق** |[إنشاء واجهة API جديدة لملحق Retail Server (الإصدار 10.0.11 والإصدارات اللاحقة من Retail SDK)](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/retail-server-extension) |


## <a name="typescript-proxy"></a>وكيل Typescript


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | يكون وكيل Typescript مطلوباً إذا كانت ملحقات RS الجديدة بحاجة إلى أن يتم استهلاكها في عملاء نقطة البيع أو التجارة الإلكترونية.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\RetailServer. افتح أي من الملحقات النموذجية في المجلد **RetailServer**. |
 |  **التقنية** | OData، C#|
|  **الوثائق** | [إنشاء وكيل Typescript لنقطة البيع]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/retail-server-icontroller-extension/?azure-portal=true#generate-the-typescript-proxy-for-pos) (الإصدار 10.0.11 والإصدارات اللاحقة من Retail SDK)|


## <a name="hardware-station"></a>محطة الأجهزة


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | محطة أجهزة لإضافة المنطق المتعلق بالأجهزة الطرفية أو تعديله.|
 |  **مرجع Commerce SDK** | \RetailSDK\ \SampleExtensions\HardwareStation. افتح الملف **HardwareStationSamples.sln**.|
|  **التقنية** | C#|
|  **الوثائق** | [دمج نقطة البيع مع جهاز جديد](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/hardware-device-extension/?azure-portal=true)|


## <a name="payment"></a>الدفع


| **الصنف** | **الوصف** |
 | ------------- | ------------- |
 | **السيناريوهات** | دمج نقطة البيع مع موصل مدفوعات جديد.|
 |  **مرجع Commerce SDK** | \RetailSDK\SampleExtensions\HardwareStation\Extension.PaymentSample. افتح الملف **HardwareStation.Extension.PaymentSample.sln**.|
|  **التقنية** | C#|
|  **الوثائق** |[ إنشاء تكامل الدفع الشامل للوحدة الطرفية للدفع](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/end-to-end-payment-extension/?azure-portal=true)

