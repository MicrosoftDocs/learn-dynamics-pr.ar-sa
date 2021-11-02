---
ms.openlocfilehash: e7f90c2aa031637b0c82e02b7f140155238d6868
ms.sourcegitcommit: 7dfc0768b02855de806a520a0ae1edd2f4de5093
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/12/2021
ms.locfileid: "7625609"
---
لتثبيت Connected Customer Service، يلزمك توفير الآتي:

- Dynamics 365 Customer Service مع بيانات اعتماد مسؤول النظام

- الوصول إلى اشتراك Azure

## <a name="installing-connected-customer-service-for-azure-iot-hub"></a>تثبيت Connected Customer Service من أجل Azure IoT Hub

يتم توزيع Connected Customer Service من أجل Azure IoT Hub عن طريق اتباع معالج خطوة بخطوة يتم تشغيله عن طريق الانتقال إلى [‎ تطبيق توزيع IoT](https://iotdeployment.dynamics.com/?azure-portal=true) في مستعرض وتسجيل الدخول باستخدام بيانات اعتماد Dynamics 365.

> [!div class="mx-imgBorder"]
> ![لقطة شاشة توضح تطبيق توزيع IoT.](../media/3-cs-iot-deployment-app-screen.png)

في تطبيق توزيع IoT، ستحدد بيئة Dynamics 365 واشتراك Azure. وعندئذٍ، يمكنك تحديد موارد Azure الموجودة أو مطالبة التطبيق بتوزيع موارد Azure جديدة من القالب.

> [!div class="mx-imgBorder"]
> ![لقطة شاشة لتطبيق توزيع IoT مع خيارات موارد Azure.](../media/3-cs-iot-deployment-app-options.png)

> [!Important]
> لتوزيع Connected Customer Service من أجل Azure، تحتاج إلى بيانات اعتماد حساب المؤسسة لـ Azure مع القدرة على إنشاء مجموعة موارد Azure وموارد Azure.

سيقوم التطبيق بتوزيع الموارد التي تظهر التقدم كما هو موضح في لقطة الشاشة الآتية.

> [!div class="mx-imgBorder"]
> ![لقطة شاشة لتطبيق توزيع IoT الذي يقوم بإنشاء الموارد.](../media/3-cs-iot-deployment-app-summary.png)

عندما يتم توزيع الموارد، يمكنك بدء اتصال الأجهزة بـ Dynamics 365 Customer Service.

## <a name="installing-connected-customer-service-for-azure-iot-central"></a>تثبيت Connected Customer Service من أجل IoT Central Azure

أولاً، يتطلب تثبيت Connected Customer Service من أجل IoT Central Azureإنشاء تطبيق IoT Central .Azure

أولاً، انتقل إلى [Azure IoT Central](https://apps.azureiotcentral.com/?azure-portal=true) في مستعرض وقم بتسجيل الدخول باستخدام بيانات اعتماد Dynamics 365. ضمن **إنشاء**، حدد **تطبيق مخصص**.

> [!div class="mx-imgBorder"]
> ![لقطة شاشة توضح تحديد تطبيق مخصص من أجل IoT Central.](../media/3-cs-iot-central-custom-app.png)

انقر فوق **إنشاء تطبيق** وسيتم عرض الشاشة الآتية.

> [!div class="mx-imgBorder"]
> ![لقطة شاشة توضح شاشة خيارات إنشاء تطبيق IoT Central.](../media/3-cs-iot-central-custom-app-options.png)

يجب منح التطبيق اسمًا والتأكد من أن عنوان URL فريدًا.

> [!IMPORTANT]
> يجب عدم استخدام خطة التسعير المجانية. يجب اختيار أحد خطط التسعير القياسية لتتمكن من توصيل IoT Central بـ Dynamics 365 باستخدام تدفقات سحابة Power Automate.

يجب اختيار خطة التسعير وتحديد اشتراك Azure. سيؤدي النقر فوق **إنشاء** إلى توفير تطبيق IoT Central.

بعد بضع ثوانٍ، سيتم عرض لوحة معلومات التطبيق.

> [!div class="mx-imgBorder"]
> ![لقطة شاشة توضح تطبيق IoT Central مخصص.](../media/3-cs-iot-central-custom-app-dashboard.png)

أنت الآن على استعداد لإضافة أجهزة إلى Connected Customer Service.
