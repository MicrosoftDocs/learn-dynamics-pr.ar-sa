---
ms.openlocfilehash: 6e1ce9af4aa96c62179cd2315998c2a21c7db3243fe4059b6d062fd24c5dedb7
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7582704"
---
توضح الخطوات التالية كيفية تكوين نموذج التطبيق باستخدام مثيل Fraud Protection الخاص بك.

1. حدد [نماذج Dynamics 365 Fraud Protection](https://github.com/microsoft/Dynamics-365-Fraud-Protection-Samples/tree/master/src/?azure-portal=true) لفتح نماذج مستندات Fraud Protection في GitHub.

2.  حدد **الرمز** في الزاوية العلوية اليسرى من صفحة الويب.

3.  حدد زر **الرمز** الأخضر.
    
    ![لقطة شاشة لصفحة نماذج Dynamics 365 Fraud Protection التي تميز زر الرمز.](../media/code-button-ssm.png)

4.  حدد لنسخ عنوان موقع المستودع الذي تريد استنساخه.
    ![لقطة شاشة لصفحة نماذج Dynamics 365 Fraud Protection تعرض عنواناً يُراد استنساخه.](../media/address-to-clone-ssm.png)

5.  افتح مثيل Visual Studio الخاص بك، وحدد **استنساخ مستودع** في إطار البدء.

6.  في حقل **موقع المستودع**، الصق موقع المستودع الذي نسخته مسبقاً من صفحة ويب GitHub. حدد المسار المحلي، ثم حدد **استنساخ**.

    ![لقطة شاشة لصفحة نسخ صفحة مستودع تبرز حقل موقع المستودع.](../media/clone-repository-ssm.png)

7.  عند تحديد **استنساخ**، سيقوم Visual Studio بمسح الحل ضوئياً وتحميله في **مستكشف الحلول**. وبدلاً من ذلك، يمكنك فتح الحل في Visual Studio عن طريق تحديد **فتح المشروع أو الحل** في نافذة البدء.

8.  حدد موقع المستودع المستنسخ، ثم حدد **فتح**.

9.  حدد ملف **Contoso.FraudProtection.sln** من قائمة **الاسم**، ثم حدد **فتح**.

10. عند تحميل الحل في **مستكشف الحلول**، حدد **المصدر**، ثم حدد **ويب**.
    ![لقطة شاشة لـ Solution Explorer مع تمييز المصدر والويب.](../media/src-web-ssm.png)

11. قم بالتمرير لأسفل وحدد ملف **appsettings.json**.

    ![لقطة شاشة لـ Solution Explorer تبرز ملف JSON لإعدادات التطبيق.](../media/app-settings-json-ssm.png)

12. أدخل المعلومات التي تلقيتها من لوحة معلومات مدخل Fraud Protection في ملف appsettings.json. يقوم الجدول التالي بتعيين المعلومات من مدخل Fraud Protection إلى الحقول القليلة الأولى في حقول appsettings.json:

    | **مدخل Fraud Protection** | **إعداد JSON** |
     | ------------- | ------------- |
     | **معرف المثيل** | معرف المثيل |
     | **معرف المثيل** | DeviceFingerprintingCustomerId |
     | **نقطة نهاية API** | ApiBaseUrl |
 
    اختبر أيضاً إعداد **DeviceFingerprintingDomain** لمجموعة بصمات الجهاز على https:\//fpt.dfp.microsoft.com.

    لا يُنصح بهذا الإعداد للإنتاج، ولكنه مناسب تماماً لمساعدتك في التعرف على بصمات الجهاز.

    تُظهر لقطة الشاشة التالية حقول appsettings.json الأربعة هذه، والتي تم تمييزها بالمربع الأحمر.

    ![لقطة شاشة لحقول JSON لإعدادات التطبيق الأربعة.](../media/app-settings-json-fields-ssm.png)

13. يوضح الجدول التالي مكان إدخال بقية المعلومات من مدخل Fraud Protection إلى ملف appsettings.json.

    |**مدخل Fraud Protection** | **إعداد JSON**|
    | ------------- | ------------- |
     | **معرف الدليل** | المرجع|
     | **عنوان URI لمورد API** | المورد |
    | **معرف التطبيق (العميل)** | ClientID |
    | **سر العميل** | ClientSecret |


    > [!NOTE]
    > ضع **معرف الدليل** من مدخل Fraud Protection في عنوان URL التالي [https://login.microsoftonline.com/[Directory_ID]](https://login.microsoftonline.com/?azure-portal=true)، ثم قم بتعيين إعداد **المرجع** في ملف appsettings.json إلى عنوان URL هذا. 

    تُظهر لقطة الشاشة التالية حقول appsettings.json الأربعة هذه، والتي تم تمييزها بالمربعات الحمراء.

    ![لقطة شاشة لحقول JSON لإعدادات التطبيق الأربعة المتبقية.](../media/remaining-app-settings-json-fields-ssm.png)

14. اكتمل الآن تكوين نموذج الموقع. في Visual Studio، اضغط على مفتاح **F5** أو حدد زر التشغيل الأخضر أعلى الشاشة لتشغيل نموذج الموقع من خلال تكوين **IIS Express**.
 
    ![لقطة شاشة تبرز زر IIS Express.](../media/iis-express-ssm.png)

    يعرض نموذج الموقع، جاهز للاستخدام.

    ![لقطة شاشة لنموذج الموقع الذي تم إنشاؤه.](../media/sample-site-ss.png)



