---
ms.openlocfilehash: 09bb43747d8ddedd0a8bdd3ed8ee0c129239c5d81a2700025d4612636893348a
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7438292"
---
LinkedIn Talent Hub عبارة عن نظام أساسي لتتبع المتقدمين (ATS). يتيح لك البحث عن الموظفين وإدارتهم وتوظيفهم في مكان واحد. خلال دمج Dynamics 365 Human Resources يمكنك بسهولة إنشاء سجلات للموظفين في الموارد البشرية للمتقدمين الذين تم تعيينهم لشغل منصب.

## <a name="setup"></a>الإعداد

يجب على مسؤول النظام إكمال مهام الإعداد لتمكين التكامل مع LinkedIn Talent Hub. أولاً، في بيئة Power Apps يجب عليك إعداد دور المستخدم والأمان لمنح LinkedIn Talent Hub الأذونات المناسبة لكتابة البيانات في الموارد البشرية.

يتضمن إعداد Dynamics 365 Human Resources مع LinkedIn Talent Hub الخطوات التالية:

1.  اربط بيئتك بـ LinkedIn Talent Hub.
2.  قم بإنشاء دور أمان Power Apps.
3.  قم بإنشاء مستخدم تطبيق Power Apps.
4.  تعيين دور أمان للمستخدم الجديد.
5.  أضف تطبيق Azure Active Directory في الموارد البشرية.
6.  أنشئ كيان في Microsoft Dataverse.

## <a name="exporting-candidate-records"></a>تصدير سجلات مرشحين

عد اكتمال الإعداد، يمكن لموظفي التوظيف ومحترفي الموارد البشرية استخدام وظيفة **تصدير إلى HRIS** في LinkedIn Talent Hub لتصدير سجلات المرشحين المستأجرين من LinkedIn Talent Hub إلى الموارد البشرية.

### <a name="export-records-from-linkedin-talent-hub"></a>تصدير السجلات من LinkedIn Talent Hub

بعد انتقال المرشح خلال عملية التوظيف وتم تعيينه، يمكنك تصدير سجل المرشح من LinkedIn Talent Hub إلى الموارد البشرية.:::image type="content" source="../media/3-5-human-resources-admin-integration-linkedin-talent-hub-export-callout-ce115dc8.png" alt-text="لقطة شاشة توضح التصدير إلى شاشة HRIS في الموارد البشرية المستخدمة لتصدير سجل المرشح من LinkedIn Talent Hub بعد انتقال المرشح خلال عملية التوظيف وتم تعيينه.":::


## <a name="complete-onboarding-in-human-resources"></a>إكمال إعداد الموارد البشرية

تظهر سجلات المرشحين التي تم تصديرها من LinkedIn Talent Hub إلى الموارد البشرية في قسم **المرشحين للتعيين** في صفحة **إدارة شؤون الموظفين**.
