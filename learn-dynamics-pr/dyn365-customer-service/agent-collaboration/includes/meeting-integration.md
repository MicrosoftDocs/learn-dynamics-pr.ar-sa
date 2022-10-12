---
ms.openlocfilehash: 5b5ef645b7850161bfe31358ede742b0397d44ed
ms.sourcegitcommit: b553b85e16cc744acb7223ab5348070f6e26a4fe
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/21/2022
ms.locfileid: "9567190"
---
تتيح ميزة تكامل اجتماعات Microsoft Teams لمندوبي Dynamics 365 Customer Service إمكانية الوصول بسرعة إلى السجلات وتحديثها في Microsoft Teams قبل الاجتماع وخلاله وبعده مع عملائهم. بمجرد تمكينها، يتم تزويد المندوبين والمشرفين في مؤسستك بتجربة متماسكة وسلسة بين Dynamics 365 وTeams. يمكن للعملاء استخدام وظيفة الاجتماعات لتلبية احتياجات العملاء بكفاءة أكبر.

يتم تمكين تكامل الاجتماعات في تطبيق **مركز مسؤولي Customer Service**. حدد **التعاون** ضمن مجموعة **خبرة المندوب** واختر **إدارة** بجوار **تكامل الاجتماعات باستخدام Teams**. قم بتعيين مفتاح التبديل على **تشغيل‏‎**.

للتأكد من أن الميزة ستعمل بشكل صحيح، ستحتاج إلى تكوين الوظائف التالية:

-   **مزامنة التقويمات:** يضمن هذا الإعداد الاختياري إضافة الاجتماعات التي تم إنشاؤها في Dynamics 365 إلى Microsoft Outlook وTeams، وظهورها في تقويمات المندوب. لمزيد من المعلومات، راجع [إعداد المزامنة على جانب الخادم للبريد الإلكتروني والمواعيد وجهات الاتصال والمهام - Power Platform](/power-platform/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks/?azure-portal=true).

-   **إضافة الاجتماعات والانضمام إليها:** يضمن هذا الإعداد المطلوب قيام أحد المندوبين بإنشاء اجتماعات Microsoft Teams والانضمام إليها مباشرة من Dynamics 365. 
    لمزيد من المعلومات، راجع [إدارة إعدادات الميزات - Power Platform](/power-platform/admin/settings-features/?azure-portal=true).

**استخدام تكامل اجتماعات Microsoft Teams في Customer Service**

توفر ميزة تكامل اجتماعات Teams تجربة اجتماع موحدة تساعدك، بصفتك مندوباً، على تقليل عبء العمل الإداري وزيادة الإنتاجية. يمكن الوصول إلى سجلات Dynamics 365 أثناء إجراء اجتماع عبر Microsoft Teams، والتي يمكنك الرجوع إليها وإجراء محادثات ذات صلة بالسياق مع عملائك. يمكنك أيضاً تدوين الملاحظات للمساعدة على توفير الوقت وزيادة الإنتاجية واستخدام بيانات أفضل داخل مؤسستك.

كمندوب، يمكنك:

-   إنشاء اجتماعات Microsoft Teams والانضمام إليها مباشرةً من Dynamics 365.

-   الوصول إلى سجلات Dynamics 365 وتحديثها بسلاسة داخل سياق اجتماع Microsoft Teams.

-   تسجيل الملاحظات والمهام بسلاسة أثناء اجتماع Microsoft Teams، ومزامنة هذه الملاحظات والمهام تلقائياً مع السجلات في Dynamics 365.

## <a name="meeting-lifecycle"></a>دورة حياة الاجتماع

يمكن تقسيم دورة حياة الاجتماع إلى المراحل التالية، مع تلبية كل مرحلة لمهام بعينها:

-   ما قبل الاجتماع: في هذه المرحلة، تحتاج إلى تنفيذ المهام التالية:

    -   [إنشاء اجتماع Teams](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#create-a-teams-meeting)

    -   [الانضمام إلى اجتماع Teams](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#join-a-teams-meeting)

    -   [إضافة تطبيق Dynamics 365 إلى اجتماع Teams](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#add-dynamics-365-app-to-a-teams-meeting)

    -   [استخدام تطبيق Dynamics 365 لعرض معلومات السجل وتحديثها](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#work-with-the-dynamics-365-app)

-   أثناء الاجتماع: في هذه المرحلة، تحتاج إلى تنفيذ المهام التالية:

    -   استخدام اللوحة الجانبية لعرض معلومات السجل وتحديثها

    -   [التعامل مع الملاحظات أثناء الاجتماع](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#work-with-notes-during-a-meeting)

    -   [التعامل مع المهام أثناء الاجتماع](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#work-with-tasks-during-a-meeting)

    -   [التعامل مع الأنشطة أثناء الاجتماع](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#work-with-activities-during-a-meeting)

-   بعد الاجتماع: في هذه المرحلة، تحتاج إلى تنفيذ المهمة التالية:

    -   [استخدام تطبيق Dynamics 365 لعرض معلومات السجل وتحديثها](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#work-with-the-dynamics-365-app)


### <a name="create-a-teams-meeting"></a>إنشاء اجتماع Teams

يمكنك إنشاء اجتماع Teams إما من Dynamics 365 أو Microsoft Outlook. أثناء إنشاء اجتماع Teams، تأكد من ربط سجل Dynamics 365 بالاجتماع. يتيح لك ربط أحد السجلات بالاجتماع عرض تفاصيل السجل قبل الاجتماع، وفي اللوحة الجانبية أثناء الاجتماع، وبعد الاجتماع.

يمكنك ربط سجل Dynamics 365 من خلال تحديد السجل ذي الصلة. عند ربط سجل قبل الاجتماع ، تتم إضافة تطبيق Dynamics 365 تلقائياً إلى الاجتماع، ويمكنك الاطّلاع على تفاصيل السجل المرتبط في اللوحة الجانبية. إذا لم يكن السجل مرتبطاً بالاجتماع، فلن تتمكن من الاطّلاع على تفاصيل السجل المرتبط. في مثل هذه الحالة، يجب إضافة تطبيق Dynamics 365 إلى الاجتماع قبل البدء فيه، وذلك للحصول على تجربة أفضل.

#### <a name="create-teams-meetings-in-dynamics-365"></a>إنشاء اجتماعات Teams في Dynamics 365

يمكنك إنشاء اجتماع Teams إما من المخطط الزمني لأحد السجلات أو من خلال صفحة الأنشطة. للحصول على إرشادات خطوة بخطوة لإنشاء اجتماع Teams، راجع [إنشاء اجتماع Teams](/dynamics365/customer-service/use-teams-meetings?azure-portal=true#create-a-teams-meeting).

#### <a name="create-teams-meetings-in-microsoft-outlook"></a>إنشاء اجتماعات Teams في Microsoft Outlook

يمكنك إنشاء اجتماع Teams في Microsoft Outlook، ولكن لن يتم ربط الاجتماع بسجل Dynamics 365 تلقائياً. يجب تثبيت تطبيق Dynamics 365 app for Outlook لربط الاجتماع بسجل Dynamics 365. بعد تثبيت التطبيق، افتحه وابحث عن السجل في حقل **تعيين بخصوص** .

للحصول على معلومات حول إنشاء اجتماع Teams في Microsoft Outlook، راجع [جدولة اجتماع Teams من Outlook](https://support.microsoft.com/office/schedule-a-teams-meeting-from-outlook-883cc15c-580f-441a-92ea-0992c00a9b0f).

للحصول على معلومات حول استخدام تطبيق Dynamics 365 App for Outlook، راجع 
[التنقل الأساسي في App for Outlook (تطبيقات Dynamics 365)](/dynamics365/outlook-app/user/basic-navigation/?azure-portal=true).

## <a name="add-dynamics-365-app-to-a-teams-meeting"></a>إضافة تطبيق Dynamics 365 إلى اجتماع Teams

يمكن إضافة تطبيق Dynamics 365 بإحدى طريقتين:

-   **إضافة التطبيق تلقائياً**: إذا قمت بربط سجل Dynamics 365 باجتماع أثناء إنشائه في Dynamics 365 أو Microsoft Outlook، تتم إضافة تطبيق Dynamics 365 تلقائياً إلى الاجتماع. يتيح لك ذلك عرض تفاصيل السجل قبل الاجتماع وخلاله وبعده.

-   **إضافة التطبيق يدوياً**: إذا لم تقم بربط سجل Dynamics 365 باجتماع أثناء إنشائه في Dynamics 365 أو Microsoft Outlook، فمن المستحسن إضافة التطبيق إلى الاجتماع قبل الانضمام إلى اجتماع Teams للحصول على تجربة أفضل.

لإضافة تطبيق قبل اجتماع، أرسل دعوة الاجتماع أولاً، ثم افتح الاجتماع في Teams. حدد **إضافة علامة تبويب**، وابحث عن تطبيق Dynamics 365، ثم أضفه.

لإضافة تطبيق أثناء اجتماع، بعد بدء الاجتماع، حدد 
**إضافة تطبيق** في عناصر تحكم الاجتماع في المنطقة العلوية اليسرى من الشاشة، وابحث عن تطبيق Dynamics 365 وأضفه.

### <a name="work-with-the-dynamics-365-app"></a>العمل مع تطبيق Dynamics 365

يسمح لك تطبيق Dynamics 365 بعرض معلومات السجل المرتبطة بأحد الاجتماعات. يمكن عرض تفاصيل السجل قبل الاجتماع وفي اللوحة الجانبية أثناء الاجتماع وبعد الاجتماع. افتح الاجتماع في Teams، ثم حدد علامة التبويب **Dynamics 365** . يمكنك تنفيذ كافة الإجراءات على السجل المرتبط كما تفعل في Dynamics 365 Customer Service.

لعرض تفاصيل السجل أثناء الاجتماع، حدد رمز تطبيق Dynamics 365 في شريط أدوات الاجتماع الموجود في المنطقة اليسرى العليا من الشاشة. يتم عرض تفاصيل السجل في لوحة جانبية. يمكنك عرض المعلومات وتحديثها مثل الملاحظات والمهام.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتفاصيل الاتصال في التطبيق.](../media/contact-details.png)](../media/contact-details.png#lightbox)

أثناء وجودك في Teams، إذا كنت تريد الوصول إلى سجل مباشرة في تطبيق Dynamics 365، فيمكنك فتح السجل عن طريق تحديد رمز النافذة المنبثقة على اللوحة الجانبية.

### <a name="join-a-teams-meeting"></a>الانضمام إلى اجتماع Teams

يمكنك إنشاء اجتماع Teams إما من Dynamics 365 أو Microsoft Outlook أو Microsoft Teams.

#### <a name="join-a-teams-meeting-from-dynamics-365"></a>الانضمام إلى اجتماع Teams من Dynamics 365

1.  افتح سجل الاجتماع من **المخطط الزمني** أو من صفحة 
    **الأنشطة** .

1.  نفذ أحد الإجراءات التالية:

    -   في "شريط الأوامر" في الجزء العلوي، حدد **الانضمام إلى اجتماع Teams**.

    -   في الحقل **اجتماع Teams** ، حدد **الانضمام إلى اجتماع Teams**.

    -   انتقل إلى منطقة **الوصف،** واضغط باستمرار على المفتاح **Ctrl** ، ثم حدد 
        **انقر هنا للانضمام إلى الاجتماع**.

#### <a name="join-a-teams-meeting-from-microsoft-outlook"></a>الانضمام إلى اجتماع Teams من Microsoft Outlook

1.  افتح حدث التقويم.

1.  نفذ أحد الإجراءات التالية:

    -   ضمن علامة التبويب **اجتماع** في الشريط، حدد **الانضمام إلى اجتماع Teams**.

    -   في نص الرسالة، حدد **انقر هنا للانضمام إلى الاجتماع**.
