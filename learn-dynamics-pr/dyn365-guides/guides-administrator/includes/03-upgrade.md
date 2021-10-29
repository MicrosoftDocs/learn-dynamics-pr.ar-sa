---
ms.openlocfilehash: 4fabddd3aca7d477adf1ccb7147916ae2c9aa213
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7587022"
---
تتطلب بعض إصدارات Dynamics 365 Guides تحديثاً لحل Dynamics 365 Guides.

> [!Important]
> لترقية حل Guides، يجب أن يكون لديك **دور مجموعة أمان مسؤول النظام** وترخيص Guides معين. راجع [تكوين أمان المستخدم للموارد في بيئة](/power-platform/admin/database-security/?azure-portal=true).

عندما يكون التحديث مطلوباً، سيرى المستخدم إشعاراً في لوحة **ما الجديد**.
ضع في اعتبارك ما يلي:

- قبل تحديث الحل في مركز إدارة Microsoft Power Platform، تأكد من تحديث تطبيقي الكمبيوتر الشخصي Dynamics 365 Guides وHoloLens إلى أحدث إصدار من Microsoft Store.

- يجب إجراء تحديثات الحل عندما لا يكون تطبيقي الكمبيوتر الشخصي وHoloLens قيد الاستخدام.

لترقية الحل:

1.  انتقل إلى [مركز إدارة Microsoft Power Platform]( https://admin.powerplatform.microsoft.com/environments/?azure-portal=true)، وقم بتسجيل الدخول باستخدام أذونات **دور أمان مسؤول النظام** لـ Dynamics 365 Guides. كما يجب أن يكون لدى المسؤولين ترخيص Dynamics 365 Guides تم تعيينه لحساب المستخدم الخاص بهم.
2.  لتحديد البيئة، حدد **الموارد**، ثم حدد **تطبيقات Dynamics 365**.
3.  بجوار **Dynamics 365 Guides**، حدد **المزيد من إجراءات التطبيقات** (**...**)، ثم حدد **تثبيت**.
    ![لقطة شاشة لزر المزيد من التطبيقات.](../media/more-application-actions-install-ssm.png) 

4.  في مربع الحوار الذي يظهر، حدد البيئة التي تريد ترقية الحل لـ (1)، وحدد خانة الاختيار **أوافق على شروط الخدمة** ‏(2)، ثم حدد **تثبيت** ‏(3).

    ![لقطة شاشة لمربع حوار تثبيت Dynamics 365 Guides.](../media/solution-install-button-ssm.png). 

## <a name="troubleshooting"></a>استكشاف الأخطاء وإصلاحها
إذا واجهت مشكلات أثناء ترقية الحل، فتأكد من أن لديك دور أمان **مسؤول النظام** وراجع[تكوين أمان المستخدم للموارد في بيئة](/power-platform/admin/database-security/?azure-portal=true). يجب أن يكون لديك دور أمان **مسؤول النظام** لترقية الحل.

إذا واجهت رسالة الخطأ **لا يمكن فتح الدليل**، فراجع قسم **استكشاف الأخطاء وتصحيحها** في [ترقية حل Dynamics 365 Guides](/dynamics365/mixed-reality/guides/upgrade/?azure-portal=true)


## <a name="compatibility-between-dynamics-365-guides-solutions-and-apps-pc-and-hololens"></a>التوافق بين حلول وتطبيقات Dynamics 365 Guides (الكمبيوتر الشخصي وHoloLens)

نوصي بأن تقوم دائماً بتحديث حل Dynamics 365 Guides في كل إصدار، بحيث يمكنك الوصول إلى أحدث الميزات والتحديثات. ومع ذلك، إذا كنت تشك في أن لديك إصداراً أقدم من الحل، ويجب عليك التحقق من توافقه مع تطبيقي الكمبيوتر الشخصي وHoloLens اللذين تستخدمهما، فراجع الجدول الموجود في قسم **توافق التطبيقات/الحلول** في [التوافق بين حلول وتطبيقات Dynamics 365 Guides (الكمبيوتر الشخصي وHoloLens)](/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility/?azure-portal=true).

للعثور على التطبيق وإصدارات الحلول التي تستخدمها، في تطبيق الكمبيوتر الشخصي، حدد الأمر **حول**. يجب عليك تسجيل الدخول لمشاهدة كلا رقمي الإصدار.
