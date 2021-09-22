---
ms.openlocfilehash: 49c0fb737b8c46980b498e31afa565ef3d7b944c
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7324654"
---
استخدم Dynamics 365 App for Outlook للاستفادة من قوة تطبيقات Dynamics 365 Customer Engagement أثناء استخدام Outlook على سطح المكتب أو الويب أو الهاتف. عندما يتم تثبيت Dynamics 365 App for Outlook، استناداً إلى إصدار التطبيق الذي قمت بتثبيته، سترى جزءاً أو نافذة بجوار رسالة بريد إلكتروني محددة من Outlook، أو عند إنشاء رسالة بريد إلكتروني أو إعداد اجتماع أو موعد.

باستخدام Dynamics 365 App for Outlook، يمكنك:

- عرض معلومات حول جهات الاتصال والعملاء المتوقعين أثناء العمل في Outlook. يمكنك عرض هذه المعلومات في سياق رسالة بريد إلكتروني أو اجتماع أو موعد. على سبيل المثال، عرض أرقام الهواتف واسم الشركة والأنشطة الأخيرة والأنشطة التالية والسجلات الحديثة.

- ربط رسائل البريد الإلكتروني والاجتماعات والمواعيد بسجل بنقرة واحدة. على سبيل المثال، ربط رسالة بريد إلكتروني بحساب أو فرصة أو حالة معينة. كما يدعم Dynamics 365 App for Outlook الكيانات المخصصة.

- فتح السجلات مباشرةً للبحث عن معلومات أكثر تفصيلاً أو إدخالها.

- إضافة مكالمة هاتفية أو مهمة أو نشاط موعد.

- إنشاء سجل جديد لأي كيان (نوع السجل).

- إضافة قوالب البريد الإلكتروني والمقالات المعرفية ومطبوعات المبيعات عند إنشاء رسالة بريد إلكتروني أو إعداد اجتماع.

- تعقب جهات اتصال Outlook.

### <a name="before-you-deploy-the-dynamics-365-app-for-outlook"></a>قبل توزيع Dynamics 365 App for Outlook

قبل أن نتعمق في كل ما تحتاج إلى معرفته لتمكين وتوزيع تطبيق Dynamics 365 App for Outlook، من المهم ملاحظة أن الإصدار الأخير من Dynamics 365 App for Outlook يعمل فقط مع إصدار 9.0 من تطبيقات Dynamics 365 Customer Engagement أو أحدث.

### <a name="requirements"></a>المتطلبات

| **المتطلب**                   |    **الوصف**     |
|-----------------------------------|-----------------------------------|
| **خادم البريد الإلكتروني**                  | Exchange Server 2013 CU 14 أو أكبر |
|                                   | Exchange Server 2016          |
|                                   | Exchange Online               |
| **عميل البريد الإلكتروني**                  | إصدار Outlook 2016 (MSI) 16.0.4266.1001 أو أحدث (على نظام التشغيل Windows 7 أو نظام تشغيل العميل الأحدث مع تثبيت IE 11) |                   
|                                   | إصدار Outlook 2016 (C2R) 16.0.93330.2073 أو أحدث (على نظام التشغيل Windows 7 أو نظام تشغيل العميل الأحدث مع تثبيت IE 11)                  |
|                                   | إصدار Outlook 2016 (MSI) 15.0.5023.1000 أو أحدث (على نظام التشغيل Windows 7 أو نظام تشغيل العميل الأحدث مع تثبيت IE 11)                  |
|                                   | Outlook for MAC               |
|                                   | Outlook لـ iOS (Apple iPhone 6S أو أحدث، يعمل بنظام iOS الإصدار 8 أو أحدث)     |
|                                   | Outlook لـ Android (مع Exchange Online، على هواتف Android التي تعمل بنظام Android 4 4.4 أو 5.0 أو 6.0 أو 7.0)        |
| **المستعرض (Outlook web access)**  | Microsoft Edge (مع Exchange المحلي 2016 أو أحدث وExchange Online)              |
|                                   | Internet Explorer 11 (مع Exchange المحلي 2016 أو أحدث وExchange Online)   |
|                                   | Google Chrome                 |
|                                   | Mozilla Firefox               |


- الإصدار 9.0 من تطبيقات Dynamics 365 Customer Engagement أو أحدث.

- مزامنة رسالة البريد الإلكتروني الواردة من خلال مزامنة على جانب الخادم. لمزيد من المعلومات، راجع [‎إعداد المزامنة على جانب الخادم للبريد الإلكتروني والمواعيد وجهات الاتصال والمهام](/dynamics365/customer-engagement/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks).

- يعد Dynamics 365 App for Outlook وظيفة إضافية في Outlook تستخدم خدمات Exchange عبر الويب (EWS) للتفاعل مع Microsoft Exchange. يتطلب هذا تمكين OAuth على Microsoft Exchange. لمزيد من المعلومات حول هذه التبعية، راجع [المصادقة واعتبارات الإذن للأسلوب makeEwsRequestAsync](/outlook/add-ins/web-services#authentication-and-permission-considerations-for-the-makeewsrequestasync-method).

- على عملاء Windows، يجب تثبيت Internet Explorer 11 وتمكينه ولكن ليس بالضرورة المستعرض الافتراضي. لمزيد من المعلومات حول هذه التبعية، راجع [متطلبات تشغيل وظائف Office الإضافية](/office/dev/add-ins/concepts/requirements-for-running-office-add-ins#client-requirements-windows-desktop-and-tablet).

### <a name="required-privileges"></a>الامتيازات المطلوبة

توفر تطبيقات Dynamics 365 Customer Engagement إمكانية الوصول إلى تطبيق Dynamics 365 App for Outlook من خلال امتياز **استخدام Dynamics 365 App for Outlook** . إذا لم يكن لدى المستخدم هذا الامتياز، فسيتلقى الخطأ التالي:

"غير مسموح لك باستخدام هذا التطبيق. تحقق مع مسؤول النظام لتحديث إعداداتك.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWs2f1]

### <a name="supported-configurations-with-microsoft-exchange"></a>التكوينات المدعومة مع Microsoft Exchange

اعتباراً من تحديث ديسمبر 2016 لـ Dynamics 365 (عبر الإنترنت والأماكن المحلية)، يمكنك استخدام التطبيق مع أي مجموعة من تطبيقات Dynamics 365 Customer Engagement أو تطبيقات Dynamics 365 Customer Engagement (المحلية) وكذلك Exchange Online أو Exchange Server (المحلي)، بما في ذلك التكوينات المختلطة.

لمعرفة المزيد، راجع [التكوينات المعتمدة](/dynamics365/customer-engagement/outlook-app/deploy-dynamics-365-app-for-outlook#supported-configurations-with-microsoft-exchange) وكذلك [دعم الميزة لكل عميل](/dynamics365/customer-engagement/outlook-app/deploy-dynamics-365-app-for-outlook#feature-support-per-client).

### <a name="deploying-the-dynamics-365-app-for-outlook"></a>توزيع Dynamics 365 App for Outlook

بعد إعداد المزامنة على جانب الخادم وتعيين الامتيازات المطلوبة، يمكنك دفع Dynamics 365 App for Outlook لبعض المستخدمين أو جميعهم، أو يمكنك جعل المستخدمين يثبتونه بأنفسهم حسب الحاجة.

### <a name="troubleshooting-installation-problems"></a>استكشاف أخطاء التثبيت وإصلاحها

- إذا كنت لا ترى تطبيق Dynamics 365 App for Outlook عند النقر على الزر **إعدادات** ، فتحقق من تمكين الميزة. لمزيد من المعلومات، راجع [تمكين](/dynamics365/customer-engagement/outlook-app/deploy-dynamics-365-app-for-outlook#enable).

- إذا واجهت أنت أو المستخدمون لديك مشكلة في تثبيت Dynamics 365 App for Outlook، فقد يكون ذلك بسبب أن صندوق بريد Exchange الخاص بهم مرتبط حالياً بمؤسسة أخرى. يمكن لصندوق بريد Exchange (عنوان البريد الإلكتروني) مزامنة المواعيد وجهات الاتصال والمهام مع مؤسسة واحدة فقط، ويمكن للمستخدم الذي ينتمي إلى تلك المؤسسة فقط مزامنة المواعيد وجهات الاتصال والمهام مع صندوق بريد واحد في Exchange. يمكنك الكتابة فوق الإعداد المخزن في Exchange إذا أردت تغيير مؤسسة المزامنة الأولية. لمزيد من المعلومات، راجع [مقالة قاعدة المعارف هذه.](https://support.microsoft.com/help/3211627/incomingemailrejected-error-when-attempting-to-install-dynamics-365-app-for-outlook)

### <a name="customizing-the-dynamics-365-app-for-outlook"></a>تخصيص Dynamics 365 App for Outlook

تخصيص Dynamics 365 App for Outlook هو جزء من نطاق هذه الوحدة النمطية. إذا كنت ترغب في الحصول على مزيد من المعلومات حول عملية تخصيص التطبيق، فراجع الروابط التالية:

- [تخصيص البطاقة المتعلقة بالتعقب](/dynamics365/customer-engagement/outlook-app/customize-the-track-regarding-card)
- [تخصيص الكيانات التي تظهر في الإنشاء السريع](/dynamics365/customer-engagement/outlook-app/add-a-custom-entity-to-quick-create)
- [تخصيص حقل البحث "بخصوص" لإضافة كيانات أو إزالتها](/dynamics365/customer-engagement/outlook-app/enable-a-custom-entity-to-appear-in-the-regarding-lookup)
- [توسيع البحث في حقول البحث "بخصوص"](/dynamics365/customer-engagement/outlook-app/search-on-custom-field-regarding-lookup)
- [تصفية الكيانات وطرق العرض التي تظهر في Dynamics 365 App for Outlook](/dynamics365/customer-engagement/outlook-app/filter-entities-and-views)
- [القيود عند تخصيص التطبيق](/dynamics365/customer-engagement/outlook-app/limitations-when-customizing-app-for-outlook)
