---
ms.openlocfilehash: cd4350643aa2ae6cc2eaf592efef7e409c0a9313
ms.sourcegitcommit: b364f2e6dabd073ec1c9fd9d1bb6efe295ce9d2f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/28/2022
ms.locfileid: "9596665"
---
حدد سيناريو عمليات المشروع للمورد أو غير المخزن إذا كنت جديدًا في Project Operations وإذا لم تقم بنشر تطبيقات المالية والعمليات وتطبيقات Microsoft Dynamics 365 Customer Engagement.

عملية نشر Project Operations لسيناريو مورد أو غير مخزّن كما يلي:

1. استرداد اشتراكات البرامج لـ:

    - Project Operations‏ (CRM)
    - Office 365 Project Operations
    - تطبيقات التمويل والعمليات
    - تعيين التراخيص للمستخدمين
    - سجل لأجل الاشتراك في Microsoft Azure

1. توفير بيئة التمويل والعمليات:

    - قم بإنشاء مشروع جديد في Lifecycle Services
    - يوافق المسؤول على اشتراك Azure
    - قم بتكوين التحكم في الوصول إلى Azure
    - إضافة موصل Azure إلى مشروع Lifecycle Services
    - نشر بيئة تمويل وعمليات
     
1. إجراءات ما بعد النشر:
    - قم بتأسيس اتصال ثنائي الكتابة.
    - تحديث إعدادات الأمان في بيئة Project Operations.
    - تكوين خرائط جدول ثنائية الكتابة وتشغيلها.
    - استيراد بيانات التكوين والعروض التوضيحية (هذه الخطوة اختيارية.)

## <a name="redeem-software-subscriptions"></a>استرداد اشتراكات البرامج

لتحسين تجربة التعلم الخاصة بك في هذه الوحدة، يمكنك الوصول إلى بيئة تجريبية لـ Project Operations عن طريق تحديد **البدء** في الزاوية العلوية اليمنى من صفحة [Dynamics 365 Project Operations ](https://dynamics.microsoft.com/project-operations/overview/?azure-portal=true).

## <a name="provision-a-finance-and-operations-environment"></a>توفير بيئة التمويل والعمليات:

شاهد الفيديو التالي للحصول على عرض توضيحي لكيفية توفير بيئة التمويل والعمليات باستخدام Lifecycle Services.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWzk1O]

## <a name="establish-a-dual-write-connection"></a>قم بتأسيس اتصال ثنائي الكتابة

يتم إجراء الاتصال تلقائيًا عند استخدام Lifecycle Services لنشر التمويل والعمليات التي تتضمن نشر بيئة Dataverse.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لإعدادات النشر (التمويل والعمليات) Sandbox بقالب Power Platform تم تعيينه إلى معيار Dynamics 365.](../media/power-platform-integration-ss.png)](../media/power-platform-integration-ss.png#lightbox)

يمكنك أيضاً إعداد اتصال الكتابة المزدوجة يدوياً باستخدام معالج في التمويل والعمليات.

شاهد الفيديو التالي للحصول على عرض توضيحي لكيفية إعداد اتصال الكتابة المزدوجة باستخدام المعالج.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWzk24]

## <a name="update-security-settings-on-the-project-operations-environment"></a>تحديث إعدادات الأمان في بيئة Project Operations

يتطلب **مستخدم التطبيق ثنائي الكتابة** امتيازات **قراءة** و **إلحاق بـ** التي تم تعيينها لـ تنظيم الجداول التالية:

- جدول الحسابات

- نوع سعر صرف العملات

- التقويم المالي

- دفتر الأستاذ

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لصفحة Dynamics 365 Security Roles مع تحديد مستخدم تطبيق الكتابة المزدوجة.](../media/security-roles-ss.png)](../media/security-roles-ss.png#lightbox)

يتطلب الفريق الافتراضي تعيين الدور **مستخدم التطبيق ثنائي** الكتابة.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لمربع حوار إدارة أدوار الفريق مع تحديد مستخدم تطبيق الكتابة المزدوجة.](../media/manage-team-roles-ss.png)](../media/manage-team-roles-ss.png#lightbox)

شاهد الفيديو التالي للحصول على عرض توضيحي لكيفية تحديث إعدادات الأمان.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWzdRL]

## <a name="configure-and-run-dual-write-table-maps"></a>تكوين خرائط جدول ثنائية الكتابة وتشغيلها

لتكوين خرائط الكتابة المزدوجة وتشغيلها، اتبع الخطوات التالية:

1. في صفحة **الكتابة المزدوجة** في التمويل والعمليات، في خانة **البحث** (الزاوية اليمنى العليا)، أدخل **Project Res** لتضييق النتائج.

1. حدد **أدوار موارد المشروع لجميع الشركات (فئات الموارد القابلة للحجز)**، ثم حدد **تشغيل**.

1. في جزء **عمليات الكتابة الأولية وخريطة (خرائط) الجدول ذات الصلة**، تأكد من أن تم مسح خانة **المزامنة الأولية**.

1. حدد **تشغيل**.

شاهد مقطعي الفيديو التاليين للحصول على عروض توضيحية حول كيفية تكوين خرائط جدول الكتابة المزدوجة وتشغيلها.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWzdRM]

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWzdRO]

## <a name="import-configuration-and-demo-data"></a>استيراد التكوين والبيانات التجريبية

تكوين الاستيراد والبيانات التجريبية اختيارية.

يمكنك اختيارياً استيراد بيانات Microsoft التجريبية إلى بيئتك بحيث يكون لديك بيانات لاستخدامها عند ممارسة التمارين. اتبع هذه الخطوات:

1. افتح علامة تبويب جديدة في متصفح الويب الخاص بك، وانسخ الارتباط التالي في مربع عنوان الويب، ثم اضغط على **Enter** مفتاح: [https://aka.ms/AAbf3j5](https://aka.ms/AAbf3j5/?azure-portal=true)

1. في الجزء السفلي من الشاشة، حدد علامة القطع (**...**) ثم حدد **إظهار في المجلد**.

1. انقر بزر الماوس الأيمن فوق ملف.zip ثم حدد **استخراج الكل...**

1. في مربع الحوار **استخراج المجلدات المضغوطة (المضغوطة)**، قم بإلغاء تحديد خانة الاختيار **إظهار الملفات المستخرجة عند الاكتمال** ثم حدد **استخراج**.

1. في نافذة **File Explorer** الجديدة انقر مرتين فوق ملف **DataMigrationUtility.exe**.

1. في نافذة **ترحيل التهيئة**، حدد **استيراد البيانات** ثم حدد **متابعة**.

1. في نافذة **تسجيل الدخول** حدد **Office 365**، وتأكد من أن **إظهار خيارات متقدمة** تم تحديد خانة الاختيار، أكمل النموذج، ثم حدد **تسجيل الدخول**.

1. في المربع **ملف مضغوط** حدد علامة القطع (**...**)، حدد **SampleSetupAndConfigData.zip** ملف، ثم حدد **فتح**.

1. في نافذة **ترحيل التهيئة** حدد **استيراد البيانات**. ستستغرق عملية الاستيراد ثلاث دقائق تقريباً حتى تكتمل.

شاهد الفيديو التالي للحصول على عرض توضيحي لكيفية استيراد بيانات التكوين والعروض التوضيحية.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWzdRQ]
