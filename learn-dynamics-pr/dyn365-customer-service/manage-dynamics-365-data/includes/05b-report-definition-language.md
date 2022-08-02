---
ms.openlocfilehash: 8b4a456447dd25111881557990fc110a58c57a121b04c9cdfda8d191bf6c9c6a
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7054276"
---
يجب تمتلك أدوات التطوير المطلوبة والامتيازات المناسبة في تطبيقات Dynamics 365 for Customer Engagement لكتابة تقرير ونشره. أيضاً، يجب أن تكون على دراية بما يلي:

- Visual Studio

- إنشاء تقارير SQL Server Reporting Services باستخدام SQL Server Data Tools (SSDT)

- لكتابة تقارير تستند إلى الإحضار، لغة FetchXML في تطبيقات Dynamics 365 for Customer Engagement

## <a name="required-tools"></a>الأدوات المطلوبة

يلزم ما يلي لكتابة تقرير مخصص لتطبيقات Dynamics 365 for Customer Engagement:

 - Visual Studio. عليك مراجعة متطلبات Report Authoring Extension، في بعض الإصدارات الخاصة

 - SQL Server Data Tools - هذه بيئة لتأليف التقرير تتوفر كمكوّن إضافي باستخدام Visual Studio.

 - Dynamics 365 Report Authoring Extension - يلزم توفير هذا إذا كنت تكتب تقارير مخصصة تستند إلى الإحضار. لاحظ أن تطبيقات Dynamics 365 Customer Engagement، مثل Dynamics 365 Sales وDynamics 365 Customer Service، تدعم فقط التقارير التي تستند إلى الإحضار. يجب تثبيت Dynamics 365 Report Authoring Extension على الكمبيوتر المُثبت عليه Visual Studio وSQL Server Data Tools.

 - ملحق Microsoft Reporting Services Projects - يُستخدم لإنشاء مشروعات خادم التقرير. ويتم تضمين هذا الملحق مع Visual Studio 2015. بالنسبة للإصدارات الأحدث، راجع ملحق Report Services Projects.

 > [!NOTE]
 > لا يمكنك استخدام SQL Server Reporting Services Report Builder لتأليف تقارير FetchXML. يُستخدم Dynamics 365 Report Authoring Extension لـ SQL Server Data Tools لتأليف تقارير FetchXML. لا يتوفر Dynamics 365 Report Authoring Extension إلا في إصدار 32 بت.

## <a name="required-privileges"></a>الامتيازات المطلوبة

لنشر تقارير مخصصة إلى Dynamics 365 for Customer Engagement، يجب أن يكون لديك حساب تطبيقات Dynamics 365 for Customer Engagement ودور أمان مخصصين لك يتضمن امتياز **PublishReport**. بشكل افتراضي، يشتمل دور مخصص النظام ودور أمان مسؤول النظام على هذه الامتيازات.

## <a name="report-development-process"></a>عملية تطوير التقرير

يسرد ما يلي خطوات تطوير تقارير Dynamics 365 for Customer Engagement المخصصة. قد تضطر إلى تكرار بعض الخطوات أثناء تطوير التقرير:

1. قم بتطوير مفهوم التقرير أو المواصفات بناءً على معلومات العمل التي سيتم عرضها.

1. قم بإنشاء تقرير مخصص أو استخدم تقريراً موجوداً للتعديل باستخدام SQL Server Data Tools في Visual Studio.

    - أنشئ تقريراً (مخصصاً) جديداً. قم بإنشاء تقارير مخصصة باستخدام SQL Server Data Tools.
    
    - قم بتنزيل ملف تعريف تقرير موجود لتطبيقات Dynamics 365 for Customer Engagement (.rdl). للقيام بذلك، افتح تطبيق Customer Engagement، وحدد علامة التبويب **التقارير**، وحدد التقرير الذي تريده، ثم حدد **تحرير** من شريط الأوامر. في صفحة خصائص التقرير، حدد **تنزيل التقرير** من شريط الأدوات **الإجراءات**.
 
1. أنشئ معلمات التقرير الأساسي.

1. حدد مجموعات البيانات ومعايير التصفية لاسترداد البيانات: قم بتمكين التصفية المسبقة للكيانات الأساسية. 

1. حدد التخطيط الأساسي للتقرير، بما في ذلك الرؤوس والتذييلات.

1. أضف عناصر التقرير كما هو مطلوب بناءً على مواصفات التقرير.

1. عاين التقرير في Visual Studio، وقم بحل أية أخطاء. 

1. انشر التقرير إلى خادم التقارير باستخدام تطبيقات Dynamics 365 for Customer Engagement.

1. قم بتشغيل التقرير المنشور للتحقق.

 




