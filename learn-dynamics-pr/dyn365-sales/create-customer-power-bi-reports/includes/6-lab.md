---
ms.openlocfilehash: 2320b1de2cce0b9e9f3fe683b63b5d77a4085a83
ms.sourcegitcommit: bfcf3cb276d50978eba5dd4b8268a26abfd9783a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/17/2021
ms.locfileid: "7436329"
---
في هذا التمرين، ستستخدم Microsoft Power BI للاتصال بالبيانات Dynamics 365 Customer Voice، والتي ستمنحك التحضير اللازم لإنشاء تقاريرك الخاصة.

### <a name="task-1-install-power-bi-desktop"></a>المهمة 1: تثبيت Power BI Desktop

في هذه المهمة، ستقوم بتثبيت العميل Power BI Desktop.

1.  انتقل إلى صفحة [Power BI التنزيلات](https://powerbi.microsoft.com/downloads/?azure-portal=true).

1.  من قسم **Microsoft Power BI من قسم** حدد **تنزيل**.

    > [!div class="mx-imgBorder"]
    > [![قم بتنزيل مربع حوار Power B I Desktop مع سهم يشير إلى أمر التنزيل.](../media/lab-1-ssm.png)](../media/lab-1-ssm.png#lightbox)

1.  سيتم فتح نافذة جديدة، مع مربع حوار يوضح أن الموقع يحاول فتح متجر Microsoft. حدد **فتح** للسماح بهذا الإجراء. 

    > [!NOTE]
    > تأكد من إيقاف تشغيل أدوات حظر النوافذ المنبثقة في متصفحك حتى لا يتم حظر هذا الحوار.

    > [!div class="mx-imgBorder"]
    > [![حاول هذا الموقع فتح مربع حوار Microsoft Store بسهم يشير إلى الزر "فتح".](../media/lab-2-ssm.png)](../media/lab-2-ssm.png#lightbox)

1.  يجب أن يفتح متجر Microsoft Store ويوجهك إلى التطبيق Power BI Desktop. حدد **تثبيت**.

    > [!div class="mx-imgBorder"]
    > [![قم بتثبيت Power B I بسهم يشير إلى زر التثبيت.](../media/lab-3-ssm.png)](../media/lab-3-ssm.png#lightbox)

1.  سيتم الآن تنزيل التطبيق Power BI Desktop على محطة العمل الخاصة بك. انتظر حتى يكتمل هذا التنزيل.

    > [!div class="mx-imgBorder"]
    > [![مربع حوار التقدم في تنزيل Power B I على سطح المكتب.](../media/lab-4-ss.png)](../media/lab-4-ss.png#lightbox)

1.  بعد تثبيت المنتج، حدد الزر **تشغيل**.

    > [!div class="mx-imgBorder"]
    > [![رسالة تثبيت هذا المنتج مع سهم يشير إلى زر التشغيل.](../media/lab-5-ssm.png)](../media/lab-5-ssm.png#lightbox)

### <a name="task-2-access-microsoft-power-platform-admin-center"></a>المهمة 2: الوصول إلى مركز الإدارة Microsoft Power Platform

في هذه المهمة، ستصل إلى مركز الإدارة Microsoft Power Platform للعثور على عنوان URL للخادم لبيئتك Microsoft Dataverse.

1.  انتقل إلى [Microsoft Power Platform مركز الإدارة](https://admin.powerplatform.microsoft.com/?azure-portal=true).

1.  سيتم إدراج البيئة Dataverse للمثيل Dynamics 365 Customer Voice في مركز الإدارة. حدد الاسم **البيئة** الذي تريد استخدامه.

    > [!div class="mx-imgBorder"]
    > [![افتح البيئة من قائمة البيئات.](../media/lab-6-ssm.png)](../media/lab-6-ssm.png#lightbox)

1.  سيتم عرض عنوان URL الخاص بالبيئة. انقر بزر الماوس الأيمن فوق عنوان URL الخاص بالبيئة.

    > [!div class="mx-imgBorder"]
    > [![حدد موقع U R L في جزء تفاصيل البيئة.](../media/lab-7-ssm.png)](../media/lab-7-ssm.png#lightbox)

1.  حدد **نسخ الرابط**. افتح المفكرة أو أداة تحرير أخرى والصق الرابط. سوف تستخدم هذا الارتباط في المهمة التالية.

    > [!div class="mx-imgBorder"]
    > [![النقر بزر الماوس الأيمن فوق U R L مع سهم يشير إلى خيار نسخ الرابط.](../media/lab-8-ssm.png)](../media/lab-8-ssm.png#lightbox)

### <a name="task-3-connect-to-dynamics-365-customer-voice-data"></a>المهمة 3: الاتصال ببيانات Dynamics 365 Customer Voice

في هذه المهمة، ستقوم بالاتصال بالبيانات Dynamics 365 Customer Voice في بيئتك Dataverse وإضافة جداول الجداول إلى تقرير.

1.  إذا لم يعد لديك Power BI Desktop فافتحه.

1.  حدد **الحصول على البيانات** من شاشة الترحيب.

    > [!div class="mx-imgBorder"]
    > [![Power B I Desktop مع تمييز الزر "الحصول على البيانات".](../media/lab-9-ssm.png)](../media/lab-9-ssm.png#lightbox)

1.  حدد **Microsoft Power Platform** من قائمة خيارات فئة البيانات.

    > [!div class="mx-imgBorder"]
    > [![احصل على خيارات البيانات مع سهم يشير إلى الخيار Microsoft Power Platform.](../media/lab-10-ssm.png)](../media/lab-10-ssm.png#lightbox)

1.  حدد **Microsoft Dataverse** من قائمة الخيارات Microsoft Power Platform.

    > [!div class="mx-imgBorder"]
    > [![Microsoft Power Platform خيارات مع سهم يشير إلى Dataverse.](../media/lab-11-ssm.png)](../media/lab-11-ssm.png#lightbox)

1.  حدد **اتصال**.

1.  استخدم الارتباط الذي قمت بالوصول إليه في المهمة 2 والصقه في عمود **عنوان URL للخادم**.

    > [!div class="mx-imgBorder"]
    > [![Dataverse مربع حوار مع سهم يشير إلى قيمة Server U R L.](../media/lab-13-ssm.png)](../media/lab-13-ssm.png#lightbox)

1.  حدد **موافق**.

1.  إذا قمت بتسجيل الدخول بالفعل، فستتجاوز الخطوة التالية ولن يُطلب منك اسم المستخدم وكلمة المرور. إذا لم تكن قد قمت بتسجيل الدخول، حدد **الزر تسجيل الدخول**.

    > [!div class="mx-imgBorder"]
    > [![سجّل الدخول إلى Dataverse حساب المؤسسة.](../media/lab-15-ssm.png)](../media/lab-15-ssm.png#lightbox)

1.  سيُطلب منك تسجيل الدخول. ادخل اسم المستخدم، ثم حدد **التالي**.

    > [!div class="mx-imgBorder"]
    > [![أدخل اسم المستخدم مع سهم إلى الزر "التالي.](../media/lab-16-ssm.png)](../media/lab-16-ssm.png#lightbox)

1. ادخل كلمه المرور الخاصة بك ثم حدد **تسجيل الدخول**.

    > [!div class="mx-imgBorder"]
    > [![أدخل كلمة المرور مع سهم إلى زر تسجيل الدخول.](../media/lab-17-ssm.png)](../media/lab-17-ssm.png#lightbox)

1. تظهر الشاشة التالية أنك قمت بتسجيل الدخول حالياً. حدد **اتصال** للمتابعة

    > [!div class="mx-imgBorder"]
    > [![أنت مسجّل الدخول حالياً. حدد زر الاتصال للمتابعة.](../media/lab-18-ssm.png)](../media/lab-18-ssm.png#lightbox)

1. في مربع البحث **Navigator** أدخل **msfp**، والذي سيؤدي إلى تصفية جداول الجدول وعرض جداول Dynamics 365 Customer Voice فقط.

    > [!div class="mx-imgBorder"]
    > [![Navigator مع نتائج بحث msfp تعرض جداول الجدول التي تبدأ بـ msfp.](../media/lab-19-ssm.png)](../media/lab-19-ssm.png#lightbox)

1. حدد المربعات بجانب الجداول التالية: **msfp_question**، **msfp_questionresponse**، **msfp_survey**، **msfp_surveyinvite**، and **msfp_surveyresponse**.

    > [!div class="mx-imgBorder"]
    > [![مربعات الاختيار المحددة بجوار الجداول المحددة.](../media/lab-20-ssm.png)](../media/lab-20-ssm.png#lightbox)

1. في مربع البحث **Navigator** أدخل الكلمة **جهة اتصال** ثم حدد المربع المجاور لجدول **جهة الاتصال**.

    > [!div class="mx-imgBorder"]
    > [![مربع بحث المستكشف مع نتائج البحث عن جهات الاتصال التي تعرض جداول الجداول التي تبدأ بجهة الاتصال.](../media/lab-21-ssm.png)](../media/lab-21-ssm.png#lightbox)

1. في مربع البحث **Navigator** أدخل **activityparty**. حدد المربع المجاور لجدول **ActivityParty**.

    > [!div class="mx-imgBorder"]
    > [![مربع بحث Navigator مع نتائج بحث نشاط طرف يعرض جدول ActivityParty المحدد.](../media/lab-22-ssm.png)](../media/lab-22-ssm.png#lightbox)

1. حدد الزر **تحميل**.

1. انتظر حتى يتم تحميل الجداول.

    > [!div class="mx-imgBorder"]
    > [![يظهر مؤشر تقدم التحميل "إنشاء اتصال في النموذج ..." أسفل كل جدول.](../media/lab-24-ss.png)](../media/lab-24-ss.png#lightbox)

1. ضمن قسم **أعمدة** في تقرير Power BI يجب أن تشاهد الآن جميع جداول الجدول التي تم تحديدها في الخطوات السابقة.

    > [!div class="mx-imgBorder"]
    > [![يظهر مصمم Power BI بالجداول المحددة في قائمة الأعمدة.](../media/lab-25-ssm.png)](../media/lab-25-ssm.png#lightbox)

### <a name="task-4-link-table-tables-in-a-power-bi-report"></a>المهمة 4: ربط جداول الجداول في تقرير Power BI

في هذه المهمة، ستقوم بربط جداول الجداول التي تم تحديدها في المهمة 3 عن طريق إنشاء علاقات فيما بينها.

1.  حدد رمز الطراز من القائمة الموجودة على الجانب الأيسر من Power BI.

    > [!div class="mx-imgBorder"]
    > [![سهم يشير إلى رمز الطراز في القائمة.](../media/lab-26-ssm.png)](../media/lab-26-ssm.png#lightbox)

1.  باستخدام شريط التمرير في الجزء السفلي من الشاشة، قم بالتمرير إلى اليمين حتى تجد جدول **msfp_survey table**.

    > [!div class="mx-imgBorder"]
    > [![تم تمييز جدول msfp_survey المميز بسهم يشير إلى شريط التمرير.](../media/lab-27-ssm.png)](../media/lab-27-ssm.png#lightbox)

1.  باستخدام الماوس، حدد مع الاستمرار أعلى جدول msfp_survey ثم اسحبه إلى اليسار بحيث يصبح الآن الجدول الأول في العرض.

    > [!div class="mx-imgBorder"]
    > [![يظهر الجدول يتم سحبه إلى موقع جديد.](../media/lab-28-ssm.png)](../media/lab-28-ssm.png#lightbox)

1.  حرك جميع الجداول حولها حتى يبدو التخطيط كما هو موضح في الشكل التالي. سيؤدي هذا الإجراء إلى تسهيل الخطوة التالية عند ربط الجداول ببعضها البعض.

    > [!div class="mx-imgBorder"]
    > [![جداول منظمة مع msfp_survey إلى اليسار، والباقي في صفين إلى اليمين. يحتوي الصف العلوي على msfp_surveyinvite و ActivityParty و Contact. الصف الثاني به msfp_question و msfp_surveyresponse و msfp_questionresponse.](../media/lab-29-ss.png)](../media/lab-29-ss.png#lightbox)

1.  في جدول msfp_survey، قم بالتمرير لأسفل حتى تجد العمود **msfp_surveyid**. ثم، في جدول msfp_question، قم بالتمرير لأسفل حتى تجد العمود **msfp_survey**. حدد العمود **msfp_surveyid** واسحبه إلى العمود **msfp_survey** في الجدول الآخر. ثم حرر الماوس.

    > [!div class="mx-imgBorder"]
    > [![يُظهر إنشاء علاقة بين الجداول عن طريق سحب العمود m s f p_survey I D من m s f p_question إلى العمود m s f p_survey m s f p_surveyid.](../media/lab-30-ssm.png)](../media/lab-30-ssm.png#lightbox)

1.  سيكون خط الاتصال مرئياً الآن بين الجدولين. سيؤدي تحريك الماوس فوق الخط إلى تمييز العمودين المستخدمين للاتصال.

    > [!div class="mx-imgBorder"]
    > [![يظهر خط اتصال بين الجداول مع سهم ثنائي الاتجاه في وسطه..](../media/lab-31-ss.png)](../media/lab-31-ss.png#lightbox)

1.  باستخدام العمود **msfp_surveyid**، قم بتوصيل جدول msfp_survey بجدول msfp_surveyinvite في العمود **msfp_surveyid**.

1.  باستخدام العمود **msfp_survey ID** قم بتوصيل جدول msfp_survey بجدول msfp_surveyresponse في العمود **msfp_surveyid**.

1.  باستخدام العمود **activityid** قم بتوصيل جدول msfp_surveyinvite بجدول activityparty في العمود **activityid**.

1. باستخدام العمود **partyid** قم بتوصيل جدول activityparty بجدول جهات الاتصال في العمود **contactid**.

1. باستخدام العمود **activityid**، قم بتوصيل جدول msfp_surveyinvite بجدول msfp_surveyresponse في العمود **msfp_surveyinviteid**.

1. باستخدام العمود **activityid** قم بتوصيل جدول msfp_surveyresponse بجدول msfp_questionresponse في العمود **msfp_surveyresponseid** .

1. باستخدام العمود **msfp_questionid** ، قم بتوصيل جدول msfp_question بجدول msfp_questionresponse في العمود **msfp_questionid**.

   يجب أن يبدو النموذج الآن مشابهاً للصورة التالية.

    > [!div class="mx-imgBorder"]
    > [![العلاقات المكتملة بين كافة الجداول.](../media/lab-32-ss.png)](../media/lab-32-ss.png#lightbox)

1. حدد أيقونة الإبلاغ من شريط التنقل الأيمن.

    > [!div class="mx-imgBorder"]
    > [![يعرض سهماً يشير إلى علامة التبويب "تقرير" في شريط القائمة الجانبية.](../media/lab-33-ssm.png)](../media/lab-33-ssm.png#lightbox)

تم الآن ربط جداولك بشكل صحيح، وأنت مستعد لبدء إنشاء تقرير Power BI.

> [!div class="mx-imgBorder"]
> [![" Power B I إظهار قائمة الأعمدة المملوءة بالجداول المحددة.](../media/lab-25-ssm.png)](../media/lab-25-ssm.png#lightbox)

