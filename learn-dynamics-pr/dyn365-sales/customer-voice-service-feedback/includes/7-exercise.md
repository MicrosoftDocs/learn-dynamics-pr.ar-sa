---
ms.openlocfilehash: db98549975bf24f2682b75f82988dc2e605b8f69
ms.sourcegitcommit: eebec3c189448605c3b1045c399fbe2d89e729ac
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/27/2021
ms.locfileid: "7712726"
---
في هذا التمرين، ستقوم بإنشاء قالب بريد إلكتروني وتخصيصه، بما في ذلك متغيرات الاستبيان.

> [!IMPORTANT]
> يُمكنك إكمال هذا التمرين باستخدام Dynamics 365 Customer Service في بيئتك أو دونه. ومع ذلك، إذا كنت ترغب في استكمال المهمة الثانية في التمرين 3، فسيلزمك استكمال هذه الخطوات في بيئة تتضمن Dynamics 365 Customer Service أيضاً. يمكنك استكمال هذه التمارين في إصدار تجريبي أو بيئة الاختبار المعزولة.

## <a name="exercise-1-create-a-new-project"></a>التمرين 1: إنشاء مشروع جديد

في هذا التمرين، ستقوم بإنشاء مشروع جديد.

1. انتقل إلى [Dynamics 365 Customer Voice](https://customervoice.microsoft.com/?azure-portal=true) وسجّل الدخول باستخدام بيانات الاعتماد الخاصة بك.

1. حدّد **الشروع في العمل**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للصفحة المنتقل إليها من أجل Dynamics 365 Customer Voice وزر "الشروع في العمل".](../media/get-started.png)](../media/get-started.png#lightbox)

1. حدد قالب مشروع **الدعم**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لخيارات قالب المشروع، والتي تظهر قالب مشروع "الدعم" المحدد.](../media/support-project-template.png)](../media/support-project-template.png#lightbox)

1. حدّد **إصدار أولي**، والذي سيوفر نظرة عامة على الاستبيان المرتبط بهذا المشروع.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقالب مشروع "الدعم" المحدد، مع تمييز زر "إصدار أولي".](../media/preview.png)](../media/preview.png#lightbox)

1. وعند الانتهاء من مراجعة الاستبيان، حدد **إقفال**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للإصدار الأولى لاستبيان تعليقات خدمة العملاء.](../media/close.png)](../media/close.png#lightbox)

1. حدد زر **التالي** للمتابعة.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقالب مشروع "الدعم"، توضح زر "التالي" المحدد.](../media/next.png)](../media/next.png#lightbox)

1. من نافذة **‏‫أين تريد إنشاء المشروع‬**، يُمكنك تحديد الموقع الذي تود إضافة المشروع إليه. حدد الرابط **راجع جميع البيئات**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للنافذة التي يمكنك خلالها تحديد مكان إضافة مشروع، مع تمييز رابط "راجع جميع البيئات".](../media/environments.png)](../media/environments.png#lightbox)

1. سيتم توجيهك إلى نافذة **‏‫جميع البيئات‬**، والتي توفر قائمة بجميع بيئات Common Data Service التي يحق لك الوصول إليها. حدد البيئة التي تستخدمها لاستكمال هذا التمرين. إذا كان لديك حق الوصول إلى البيئة، فسيتم عرض رسالة توضح أنه تم منح الإذن. حدد زر **تحديد وإغلاق**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقائمة بجميع بيئات Common Data Service التي يمكنك الوصول إليها، مع تمييز زر "تحديد وإغلاق".](../media/select-close.png)](../media/select-close.png#lightbox)

    > [!NOTE]
    > نظراً إلى استخدامك Customer Voice لفترة من الوقت، سيتم ملء قائمة المواقع الأخيرة بأحدث البيئات التي استخدمتها. وبعد ذلك، يُمكنك تحديد البيئة مباشرة من هذه القائمة بدلاً من ذلك.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لمواقع مختلفة يمكنك إضافة المشروع إليها Dynamics 365 Customer Voice.](../media/locations.png)](../media/locations.png#lightbox)

1. حدد زر **إنشاء**. في حالة تعذُّر تحديد الزر، يجب التأكيد باستخدام الخطوة السابقة ثم التأكّد من تحديد موقع واحد.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر أن Customer Voice متصل بـ Microsoft Dynamics 365، مع تحديد زر "إنشاء".](../media/create.png)](../media/create.png#lightbox)

## <a name="exercise-2-add-survey-variables"></a>تمرين 2: إضافة متغيرات الاستبيان

في هذا التدريب، ستتعلم كيفية إنشاء المتغيرات وإضافتها إلى الاستبيان.

### <a name="task-1-create-variables"></a>المهمة 1: إنشاء متغيرات

في هذه المهمة، ستقوم بإنشاء المتغيرات.

1. حدد لوحة **تخصيص** الموجودة في أعلى الزاوية اليمنى من استبيان "دقة الحالة" في مشروعك.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لاستبيان تعليقات خدمة العملاء، مع تحديد لوحة "تخصيص".](../media/customization.png)](../media/customization.png#lightbox)

1. من القائمة التي تفتح، حدد **تخصيص**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقائمة "تخصيص" مع قائمة بالخيارات والتخصيص المحدديْن.](../media/personalization.png)](../media/personalization.png#lightbox)

1. ستعرض شاشة **تخصيص** جميع المتغيرات الموجودة لاستبيان "دقة الحالة". حدد **‏‫إضافة متغير‬**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة من شاشة "تخصيص" تعرض زر "إضافة متغير" المحدد.](../media/add-variable.png)](../media/add-variable.png#lightbox)

1. اكتب **CaseNumber‎** في اسم المتغير. تأكد من عدم تضمين مسافة بين الكلمتين. في حالة القيام بذلك، سيتم عرض رسالة توضح "الأحرف القياسية مطلوبة". أزل المسافة لإزالة رسالة الخطأ. حدد **‏‫إضافة متغير‬** مرة أخرى.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لمتغير بالإدخال CaseNumber على أنه اسم المتغير.](../media/add-variable-2.png)](../media/add-variable-2.png#lightbox)

1. اكتب **‎CaseTitle‎** في اسم المتغير. حدد زر **حفظ** لإضافة المتغيرين الجديدين.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقائمة تضم متغيرين وخيار "إضافة متغير" وزر "حفظ" تم تمييزها.](../media/save.png)](../media/save.png#lightbox)

    سيتم عرض رسالة تأكيد في لوحة **تخصيص** للإشارة إلى إضافة المتغيرين.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لرسالة التأكيد توضح إضافة المتغيرين.](../media/variables-added.png)](../media/variables-added.png#lightbox)

1. حدد زر **إغلاق** لإغلاق هذا القسم.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لزر "إغلاق" في الجزء السفلي من لوحة "تخصيص".](../media/close-2.png)](../media/close-2.png#lightbox)

1. حدد السهم لتصغير لوحة **تخصيص**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة توضح السهم المستخدم لتصغير لوحة "تخصيص".](../media/arrow.png)](../media/arrow.png#lightbox)

لقد نجحت في إضافة متغيرين جديدين لاستخدامهما في الاستبيان.

### <a name="task-2-add-variables-to-the-survey"></a>المهمة 2: إضافة متغيرات إلى الاستبيان

في هذه المهمة، ستقوم بإضافة متغيرات إلى وصف الاستبيان.

1. حدد وصف الاستبيان لتمييز النص ثم احذف النص.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر استبيان تعليقات خدمة العملاء مع تمييز الوصف.](../media/customer-service-feedback.png)](../media/customer-service-feedback.png#lightbox)

1. حدد القائمة المنسدلة **المتغيرات** ثم حدد **First Name**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للقائمة المنسدلة الخاصة بالمتغيرات، مع تحديد المتغيرات > First Name.](../media/variables-menu.png)](../media/variables-menu.png#lightbox)

1. ستتم إضافة **{{First Name}}** إلى الوصف. أضف فاصلة بعد المتغير ثم أضف النص التالي: **نحن نقدر عملك. لقد أغلقنا مؤخراً بطاقة دعم لك، وسنكون ممتنين لتعليقاتك على هذه التجربة. وكمرجع لك، إليك معلومات حالتك:**

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للنص المطلوب إدخاله لوصف الاستبيان.](../media/survey-description.png)](../media/survey-description.png#lightbox)

1. حدد القائمة المنسدلة **المتغيرات**، وهذه المرة حدد **رقم الحالة**. أضف واصلة ثم حدد القائمة المنسدلة **المتغيرات** مرة أخرى لتحديد **عنوان الحالة**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للقائمة المنسدلة "المتغيرات"، مع تحديد رقم الحالة.](../media/case-number.png)](../media/case-number.png#lightbox)

يجب أن يشبه وصف الاستبيان المكتمل لقطة الشاشة التالية.

> [!div class="mx-imgBorder"]
> [![لقطة لوصف الاستبيان المكتمل.](../media/description-text-box.png)](../media/description-text-box.png#lightbox)

لقد نجحت في إضافة متغيرات إلى وصف الاستبيان.

## <a name="exercise-3-customize-the-email-template"></a>تمرين 3: تخصيص قالب بريد إلكتروني 

في هذا التدريب، ستتعلم كيفية تخصيص قالب البريد الإلكتروني وإضافة متغيرات الاستبيان إلى الموضوع والنص الأساسي للبريد الإلكتروني.

### <a name="task-1-add-variables-to-the-email-template"></a>المهمة 1: إضافة متغيرات إلى قالب البريد الإلكتروني

في هذه المهمة، ستقوم بإضافة متغيرات إلى قالب البريد الإلكتروني.

1. من استبيان دقة الحالة الرئيسي، حدد علامة تبويب **إرسال** من أعلى الجزء الأيمن من الشاشة.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لاستبيان دقة الحالة مع تمييز علامة تبويب "إرسال".](../media/send-tab.png)](../media/send-tab.png#lightbox)

1. حدد خيار **البريد الإلكتروني**.

    > [!div class="mx-imgBorder"]
    > [![لقطة لخيار البريد الإلكتروني المحدد في علامة تبويب "إرسال" من استبيان دقة الحالة.](../media/email-option.png)](../media/email-option.png#lightbox)

1. حدد القائمة المنسدلة **قالب**. سيتم تحديد قالب **تعليقات الدعم** بالفعل وهو القالب الذي سيتم عرضه في منطقة **البريد الإلكتروني**. حدد القائمة المنسدلة **القالب** مرة أخرى لإغلاقها.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للقائمة المنسدلة "القالب" مع تحديد "تعليقات الدعم".](../media/template-menu.png)](../media/template-menu.png#lightbox)

1. حدد **الموضوع** ثم حدد النص الموجود في موضعه بالفعل. احذف النص.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للموضوع المحدد مع تمييز نص "‏‫كيف سار الأمر؟‬".](../media/subject.png)](../media/subject.png#lightbox)

1. حدد القائمة **إدراج** ثم مرّر المؤشر فوق خيار **المتغيرات المخصصة**. سيتم عرض قائمة المتغيرات المتاحة. حدد **First Name** لإضافته إلى الموضوع.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للقائمة المنسدلة "إدراج" مع تحديد المتغيرات المخصصة > First Name.](../media/first-name.png)](../media/first-name.png#lightbox)

1. بعد متغير "First Name"، أضف النص التالي: **هل يمكنك مشاركة تعليقات في تجربتك الأخيرة؟**

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للحقلين "المستلمين" و"الموضوع" مع إضافة نص "هل يمكنك مشاركة تعليقات في تجربتك الأخيرة؟".](../media/share-feedback-subject.png)](../media/share-feedback-subject.png#lightbox)

1. في النص الأساسي للبريد الإلكتروني، حدد متغير **Last Name** ثم احذفه.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر استبيان تعليقات الدعم مع تمييز متغير "Last Name".](../media/last-name.png)](../media/last-name.png#lightbox)

1. بعد الجملة الثانية التي تنتهي بكلمة *المستقبل*، أضف النص التالي: **قمنا بإغلاقه مؤخراً**.

1. حدد قائمة **إدراج**، ومرّر المؤشر فوق خيار **المتغيرات المخصصة**، ثم حدد **CaseNumber‎**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر تحديد CaseNumber‎ كمتغير مخصص.](../media/case-number-variable.png)](../media/case-number-variable.png#lightbox)

1. أضف واصلة ثم حدد **CaseTitle‎** لإضافته كمتغير أيضاً. يجب أن يكون قالب بريدك الإلكتروني مشابهاً للقطة الشاشة التالية.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقالب البريد الإلكتروني مع زر "بدء الاستبيان".](../media/begin-survey-button.png)](../media/begin-survey-button.png#lightbox)

1. حدد زر **حفظ** من الجزء السفلي من قالب البريد الإلكتروني.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لزر "حفظ" في قالب البريد الإلكتروني.](../media/save-button.png)](../media/save-button.png#lightbox)

سيظهر إخطار في الجزء العلوي من الشاشة، والذي يشير إلى أن القالب قد تم حفظه بنجاح.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لرسالة "تم حفظ القالب" في شاشة "استبيان دقة الحالة".](../media/template-saved.png)](../media/template-saved.png#lightbox)

### <a name="task-2-send-an-email-with-variables-populated"></a>المهمة 2: إرسال بريد إلكتروني يحتوي على متغيرات تم ملؤها

في هذه المهمة، ستقوم بإرسال بريد إلكتروني يحتوي على المتغيرات التي تم ملؤها لأحد المستلمين. لإكمال هذه المهمة، ستحتاج إلى استخدام عنوان بريد إلكتروني يمكنك الوصول إليه.

1. حدد علامة التبويب **إرسال** من استبيان دقة الحالة الرئيسي.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر تمييز علامة التبويب "إرسال" في شاشة "استبيان دقة الحالة".](../media/send-tab-2.png)](../media/send-tab-2.png#lightbox)

1. حدد خيار **البريد الإلكتروني**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لخيار "البريد الإلكتروني" المحدد في علامة تبويب "إرسال" من شاشة "استبيان دقة الحالة".](../media/email-option.png)](../media/email-option.png#lightbox)

1. حدد الرابط **استيراد جهات الاتصال** في أعلى الجزء الأيمن من قالب البريد الإلكتروني.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقالب البريد الإلكتروني مع تحديد رابط "استيراد جهات الاتصال".](../media/import-contacts.png)](../media/import-contacts.png#lightbox)

1. حدد **الخيارات المتقدمة**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر شاشة "استيراد جهات الاتصال" مع تمييز "الخيارات المتقدمة".](../media/advanced-options.png)](../media/advanced-options.png#lightbox)

1. في قسم **الخيارات المتقدمة**، يمكنك تنزيل قالب يتضمن جميع المتغيرات من الاستبيان ذي الصلة. حدد تنزيل **القالب المتقدم**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لرابط "تنزيل القالب المتقدم" في نافذة "الخيارات المتقدمة".](../media/download-advanced-template.png)](../media/download-advanced-template.png#lightbox)

1. سيتم تنزيل ملف CustomerVoiceSample.csv. انتقل إلى مجلد التنزيلات الخاص بك وافتح الملف. قم بتعبئة الحقول بعنوان البريد الإلكتروني (الذي تتوفر لديك صلاحية الوصول إليه) والاسم الأول واسم العائلة ورقم الحالة ومعلومات عنوان الحالة.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لجدول بيانات Microsoft Excel يحتوي على سجل جهة الاتصال وبيانات سجل الحالة من Dynamics 365 Customer Engagement.](../media/contact-record.png)](../media/contact-record.png#lightbox)

1. إذا كانت لديك صلاحية الوصول إلى Dynamics 365 Customer Service مع جدول الحالة، يمكنك أيضاً إكمال العمودين **RegardingID‎** و **RegardingEntityName‎**. إذا قمت بفتح حالة في Dynamics 365، فسوف تشتمل نهاية عنوان URL على المعرف الفريد من الحالة.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لعنوان URL من مستعرض ويب مع تمييز الجزء الأخير من عنوان URL.](../media/url.png)](../media/url.png#lightbox)

1. أضف معرف الحالة في حقل **RegardingID‎** ثم اكتب كلمة **حدث** في عمود **RegardingEntityName‎**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للعمودين "RegardingID" و"RegardingEntityName" من جدول بيانات Excel.](../media/excel-data.png)](../media/excel-data.png#lightbox)

1. احفظ ملف CSV إلى سطح المكتب (أو في أي مجلد يتوفر لديك حق الوصول إليه).

1. حدد زر **تحميل** من شاشة **استيراد جهات الاتصال**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لزر "تحميل" في شاشة "استيراد جهات الاتصال".](../media/upload-button.png)](../media/upload-button.png#lightbox)

1. استعرض حتى تصل إلى المكان الذي قمت فيه بحفظ الملف، وحدده، ثم حدد **فتح** من عنصر تحكم البحث.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لمستعرض Microsoft Explorer مع تحديد ملف Excel وتمييز زر "فتح".](../media/open-button.png)](../media/open-button.png#lightbox)

1. سيتم استيراد الملف وسيظهر إخطار يوضح بأنه كان ناجحاً. يجب عرض البريد الإلكتروني والاسم الأول واسم العائلة لجهة الاتصال.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لرسالة الملف الذي تم تحميله بنجاح في شاشة استيراد جهات الاتصال.](../media/successful-upload.png)](../media/successful-upload.png#lightbox)

1. حدد زر **استيراد** من شاشة **استيراد جهات الاتصال**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لزر "استيراد" في شاشة "استيراد جهات الاتصال".](../media/import-button.png)](../media/import-button.png#lightbox)

1. من المفترض أن يعرض حقل **المستلمين** مستلماً واحداً. حدد زر **إرسال** من الجزء السفلي للبريد الإلكتروني.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة توضح حقل "المستلمين" يظهر مستلماً واحداً.](../media/recipient.png)](../media/recipient.png#lightbox)

1. افتح علبة الوارد الخاصة بعنوان البريد الإلكتروني الذي استخدمته. يجب أن تكون قد تلقيت رسالة إلكترونية تتضمن الاسم الأول في "الموضوع". ويجب أيضاً عرض رقم الحالة وعنوان الحالة. حدد زر **بدء الاستبيان**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لرسالة بريد إلكتروني مع عرض الاسم الأول للمستلم في "الموضوع" والنص الأساسي للبريد الإلكتروني.](../media/email-recipient.png)](../media/email-recipient.png#lightbox)

   ومن المفترض كذلك أن يعرض الاستبيان نفس المتغيرات الثلاثة التي تم ملؤها في الوصف.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تظهر استبيان تعليقات خدمة العملاء مع تمييز الوصف.](../media/survey-description-2.png)](../media/survey-description-2.png#lightbox)

1. إذا كان ملف الاستيراد الخاص بك تضمن العمودين **RegardingID‎** و **RegardingEntityName‎**، فيمكنك الانتقال إلى الحالة في Dynamics 365. سيتم عرض دعوة الاستبيان في الخط الزمني في الحالة.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لخط زمني من سجل حالة مع تمييز نشاط دعوة الاستبيان.](../media/active.png)](../media/active.png#lightbox)
    
