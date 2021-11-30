---
ms.openlocfilehash: 7a0ac971dcb86e4191c1d452409b69b63512b395
ms.sourcegitcommit: c95922edfc4783b70b93a09d3c31693ebcad174e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/04/2021
ms.locfileid: "7752219"
---
كما ذكر سابقاً، يمكنك تضمين تقارير Power BI ولوحات المعلومات والإطارات المتجانبة في Dynamics 365 Customer Service. وتقوم هذه الوحدة باستكشاف كيف يمكن لـ Power BI استهلاك البيانات من Dynamics 365 لإنشاء تقارير ولوحات معلومات Power BI.

> [!NOTE]
> لا توضح هذه الوحدة النمطية كيفية إنشاء تقارير Power BI بالتفصيل؛ ويكون التركيز على كيفية اتصال Power BI ببيانات Dynamics 365 Customer Service.

## <a name="overview-of-power-bi"></a>نظرة عامة على Power BI

Microsoft Power BI عبارة عن مجموعة من أدوات تحليل الأعمال التي تقدم رؤى من خلال مؤسستك. يساعد Power BI على الاتصال بمئات من مصادر البيانات، ويبسط عملية إعداد البيانات، ويقود التحليل الفوري.
باستخدام الأدوات التي توفرها Power BI، يمكنك إنتاج تقارير مقنعة ثم نشرها حتى تتمكن مؤسستك من استهلاكها على الويب وعبر الأجهزة المحمولة.

يمكن للجميع إنشاء لوحات معلومات مخصصة تمنحهم عرضاً فريداً بزاوية 360 درجة لأعمالهم، والتي تتسع عبر المؤسسة، والتي تشتمل على الحوكمة وميزات الأمان. تتوفر هذه الميزات والأدوات من خلال موقع ويب Power BI. يوفر موقع الويب هذا موقعاً يمكنك فيه إنشاء لوحات معلومات مخصصة. بالإضافة إلى ذلك، يشتمل موقع الويب على لوحات معلومات Power BI المكونة مسبقاً التي تم إنشاؤها خصيصاً لـ Microsoft Dynamics 365 Customer Service.

Power BI هي أداة مفيدة لمساعدتك في تحليل بيانات Microsoft Dynamics 365. نظراً لأنه تطبيق تحليلات كامل للمؤسسات، فإن له نظاماً بيئياً خاصاً به. تتصل التطبيقات المتوفرة لـ Power BI بمئات من مصادر البيانات المختلفة، بما في ذلك Dynamics 365. لذلك، من السهل عليك الاتصال والحصول على بيانات مفيدة على الفور.

يمكنك توصيل Dynamics 365 الخاص بك باستخدام تطبيق Power BI تم تكوينه مسبقاً أو عن طريق إنشاء تقارير Power BI الخاصة بك.

## <a name="power-bi-app"></a>تطبيق Power BI

يحتوي تطبيق Customer Service Analytics for Dynamics 365 من Power BI على العديد من التقارير ولوحات المعلومات للحالات وقوائم الانتظار والمندوبين. يمكنك استخدام هذا التطبيق لتحليل بيانات خدمة العملاء.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتطبيق Customer Service Analytics من Power BI.](../media/5-power-bi-app.png)](../media/5-power-bi-app.png#lightbox)

تم شرح هذا التطبيق بمزيد من التفصيل في وحدة الشروع في العمل مع Customer Service Insights.

## <a name="connect-power-bi-to-dynamics-365-customer-service"></a>قم بتوصيل Power BI بـ Dynamics 365 Customer Service

Power BI Desktop هو تطبيق Microsoft Windows الذي يمكنك من الاتصال بالبيانات وإنشاء التقارير قبل النشر إلى خدمة Power BI على powerbi.com.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتطبيق Power BI Desktop.](../media/5-power-bi-desktop.png)](../media/5-power-bi-desktop.png#lightbox)

حدد رمز **Dataverse** الموجود في شريط الأدوات لتلقي المطالبة بمجال المؤسسة الخاص ببيئة Dynamics 365 Customer Service.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة تعرض الاتصال بشاشة Microsoft Dataverse.](../media/5-connect-to-dataverse.png)](../media/5-connect-to-dataverse.png#lightbox)

> [!NOTE]
> يمكنك تحديد خيار **الاستيراد**، حيث يتم نسخ البيانات في Power BI ثم تحديثها على أساس مجدول. وبدلاً من ذلك، يمكنك تحديد الخيار **DirectQuery** حيث يتم الاستعلام عن البيانات في الوقت الحقيقي من Dataverse عند وصول أحد المستخدمين إلى تقرير Power BI.

انسخ عنوان URL الخاص ببيئتك ثم حدد **موافق**. إذا طُلب منك ذلك، سجّل الدخول باستخدام بيانات اعتماد Dynamics 365 الخاصة بك.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة توضح أنك متصل بـ Dataverse.](../media/5-connected-to-dataverse.png)](../media/5-connected-to-dataverse.png#lightbox)

حدد **اتصال**.

> [!div class="mx-imgBorder"]
> [![لقطة الشاشة التي تظهر عدد قليل من الجداول المحددة في Dataverse.](../media/5-select-tables.png)](../media/5-select-tables.png#lightbox)

حدد الجداول في Dataverse التي تريد استخدامها في التقارير الخاصة بك.
تتطلب هذه العملية فهم نموذج البيانات الخاص بتطبيق Dynamics 365 Customer Service. يمكنك تحديد **التحميل** لاستيراد جميع الجداول والأعمدة والبيانات. بدلاً من ذلك، حدد **تحويل البيانات** لبدء **Power Query**، حيث يمكنك تنظيف بياناتك وتحويلها.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة تعرض شاشة التحميل.](../media/5-loading-data.png)](../media/5-loading-data.png#lightbox)

بعد تحميل البيانات، يمكنك استخدام وظيفة Power BI لإنشاء الرسوم المرئية، كما هو موضح في لقطة الشاشة التالية.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة تعرض نموذجاً لتقرير Power BI.](../media/5-power-bi-report.png)](../media/5-power-bi-report.png#lightbox)

## <a name="considerations"></a>الاعتبارات

نظراً لأن Power BI يتصل بـ Dynamics 365، فهناك بعض القيود التي يجب مراعاتها عندما تقرر استخدام Power BI:

- لا يعمل Power BI في سياق السجلات أو المستخدمين. على عكس المخططات ولوحات المعلومات، لا يتم تشغيل Power BI في سياق سجل أو مستخدم.
ومع ذلك، باستخدام موصل Dataverse، يتم تنفيذ سياق الأمان الخاص بالمستخدم من خلال Power BI بحيث يتمكن المستخدمون فقط من رؤية البيانات التي يحق لهم الحصول عليها.

- تظهر تحديثات البيانات في كل ساعة أو يومياً إذا كنت تستخدم خيار **الاستيراد**. لا يُظهر Power BI عرض الوقت الفعلي لبيانات Dynamics 365. يتم تحديث البيانات على فترات زمنية محددة تعتمد على فئة التسعير الخاصة بك.

- ويتم فصل تطبيق Dynamics 365 وخدمة Power BI. Power BI هو تطبيق منفصل يتصل ببيانات Dynamics 365. قد يتطلب الأمر تراخيصاً أخرى بالإضافة إلى تراخيص Dynamics 365 الخاص بك.
