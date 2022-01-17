---
ms.openlocfilehash: 09f1f77bf74deecb8678a2632eec74bd910626d7
ms.sourcegitcommit: 178639e9a46ac1ef2cba985875f0d21d1baee52e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/03/2022
ms.locfileid: "7948535"
---
ستقوم في هذا التمرين بإعداد مقاييس الرضا والتنبيهات لأحد المشروعات في Dynamics 365 Customer Voice.

> [!NOTE]
> يمكنك استكمال تلك المهام في أي إصدار تجريبي أو بيئة اختبار معزولة.

## <a name="task-1-create-a-new-project"></a>المهمة 1: إنشاء مشروع جديد

في هذه المهمة، ستقوم بإنشاء مشروع جديد باستخدام قالب المشروع **زيارة الخدمة** في Dynamics 365 Customer Voice..

1. انتقل إلى [Dynamics 365 Customer Voice](https://customervoice.microsoft.com/?azure-portal=true) وسجّل الدخول باستخدام بيانات الاعتماد الخاصة بك.

1. حدّد **الشروع في العمل**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر لوحة المعلومات الرئيسية في Dynamics 365 Customer Voice مع تمييز الزر "الشروع في العمل".](../media/get-started.png)](../media/get-started.png#lightbox)

1. حدد القالب **زيارة الخدمة** من قائمة خيارات قوالب المشروعات.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر سلسلة من قوالب المشروعات في Dynamics 365 Customer Voice، مع تحديد قالب زيارة الخدمة.](../media/service-visit.png)](../media/service-visit.png#lightbox)

1. من الجزء السفلي للشاشة، حدد زر **التالي**.

1. حدد **مراجعة جميع البيئات**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر شاشة اختيار الموقع لأحد المشروعات في Customer Voice. تم تمييز ارتباط "مراجعة جميع البيئات".](../media/see-all-environments.png)](../media/see-all-environments.png#lightbox)

1. حدد بيئة من القائمة. في الزاوية اليمنى السفلية من الشاشة، عند عرض الرسالة **تم منح الإذن**، حدد الزر **تحديد وإغلاق**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر قائمة تتضمن جميع البيئات المتوفرة في أي مؤسسة. وقد تم تمييز إحدى البيئات الموجودة في القائمة، وتم تمييز الزر "تحديد وإغلاق".](../media/select-and-close-all-environments.png)](../media/select-and-close-all-environments.png#lightbox)

1. حدد الزر **إنشاء**.

اكتمل المشروع الآن، وسيتم عرض استطلاع **ملاحظات الخدمة الميدانية** من قالب المشروع **زيارة الخدمة**.

## <a name="task-2-create-a-satisfaction-metric"></a>المهمة 2: إنشاء مقياس رضا

في هذه المهمة، ستقوم بإنشاء مقياس رضا للمشروع الذي أنشأته في المهمة 1.

1. من الصفحة الرئيسية في Dynamics 365 Customer Voice، حدد **جميع المشروعات**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر لوحة المعلومات الرئيسية في Dynamics 365 Customer Voice. تم تمييز قائمة "جميع المشروعات".](../media/customer-voice-all-projects.png)](../media/customer-voice-all-projects.png#lightbox)

1. حدد المشروع **زيارة الخدمة** الذي قمتَ بإنشائه في المهمة 1 لفتحه.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر قائمة مشروعات في Dynamics 365 Customer Voice، مع تمييز المشروع "زيارة الخدمة".](../media/service-visit-my-projects-select.png)](../media/service-visit-my-projects-select.png#lightbox)

1. قم بالتمرير لأسفل الاستطلاع‬، ثم حدد الزر **إضافة جديد**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر الجزء السفلي من أحد الاستطلاعات في Customer Voice. يتم تمييز الزر "إضافة جديد".](../media/add-new.png)](../media/add-new.png#lightbox)

1. حدد السهم ثم حدد **Net Promoter Score** من القائمة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر كل خيارات الأسئلة المتوفرة في Customer Voice. يتم تمييز نوع سؤال Net Promoter Score.](../media/net-promoter-score.png)](../media/net-promoter-score.png#lightbox)

1. حدد القائمة **تخصيص** من الجانب الأيمن للاستطلاع.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر القائمة "تخصيص" في أحد الاستطلاعات في Dynamics 365 Customer Voice.](../media/customization.png)](../media/customization.png#lightbox)

1. حدد **‏‫مقاييس الرضا** من القائمة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر اللوحة "تخصيص" مفتوحة في أحد الاستطلاعات في Customer Voice. يتم تمييز خيار "مقاييس الرضا".](../media/satisfaction-metrics.png)](../media/satisfaction-metrics.png#lightbox)

1. يوجد بالفعل مقياسان للرضا. تم تضمين هذه المقاييس كجزء من قالب المشروع. حدد **إضافة مقياس** لإنشاء واحد جديد.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر اللوحة "مقاييس الرضا" مفتوحة في Customer Voice. يتم تمييز الزر "إضافة مقياس".](../media/add-metric.png)](../media/add-metric.png#lightbox)

1. حدد **Net Promoter Score** من القائمة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر الزر "إضافة مقياس" محددًا في Customer Voice، وتعرض سلسلة من الخيارات، بما في ذلك خيار Net Promoter Score.](../media/net-promoter-score-add-metric.png)](../media/net-promoter-score-add-metric.png#lightbox)

1. قم بتغيير اسم المقياس إلى **NPS**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر مقياسًا جديدًا للرضا تتم إضافته واسم المقياس كـ Net Promoter Score.](../media/name-net-promoter-score.png)](../media/name-net-promoter-score.png#lightbox)

1. حدد السؤال الجديد الذي قمتَ بإضافته إلى الاستطلاع في هذه المهمة ثم حدد الزر **حفظ**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر قائمه منسدلة تعرض جميع الأسئلة التي يمكنها التعيين إلى مقياس جديد في Customer Voice.](../media/field-service-feedback.png)](../media/field-service-feedback.png#lightbox)

يجب أن يظهر إعلام للإشارة إلى أنه تم حفظ المقياس، وسيكون مقياس NPS الجديد مرئيًا في القائمة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر أنه تم حفظ مقياس رضا جديد في Customer Voice. يتم تمييز المقياس الجديد في قائمة المقاييس.](../media/metric-saved.png)](../media/metric-saved.png#lightbox)

## <a name="task-3-create-new-alerts"></a>المهمة 3: إنشاء تنبيهات‬ جديدة

في هذه المهمة، ستقوم بإنشاء تنبيهين جديدين للمشروع الذي قمت بإنشائه في المهمة 1.

1. من الصفحة الرئيسية في Dynamics 365 Customer Voice، حدد **جميع المشروعات**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر لوحة المعلومات الرئيسية في Customer Voice، مع تمييز قائمة "جميع المشروعات".](../media/all-projects.png)](../media/all-projects.png#lightbox)

1. حدد المشروع **زيارة الخدمة** الذي قمتَ بإنشائه في المهمة 1 لفتحه.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر قائمة مشروعات، مع تمييز المشروع "زيارة الخدمة".](../media/service-visit-my-projects.png)](../media/service-visit-my-projects.png#lightbox)

1. من قائمة المشروع الموجودة على الجانب الأيسر، حدد **التنبيهات‬‬**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر القائمة الرئيسية في مشروع ما في Customer Voice وقد تم تمييز الخيار "التنبيهات".](../media/alerts.png)](../media/alerts.png#lightbox)

1. حدد **إنشاء قاعدة تنبيه** من منتصف الشاشة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر معلومات حول إنشاء تنبيهات في Customer Voice. يتم تمييز الزر "إنشاء قاعدة تنبيه".](../media/create-alert-rule.png)](../media/create-alert-rule.png#lightbox)

1. قم بإطلاق الاسم التالي على قاعدة التنبيه: **التوجه السلبي**.
   حدد **توجه العميل** من القائمة **مقاييس الرضا**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر نموذج قاعدة تنبيه يتم إنشاؤه في Dynamics 365 Customer Voice.](../media/detractor-satisfaction-metric.png)](../media/detractor-satisfaction-metric.png#lightbox)

1. قم بتعيين الشرط إلى **يساوي** والقيمة إلى **سلبي**.
   حدد الزر **حفظ**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر شرطًا تتم إضافته إلى مقياس رضا. يظهر الشرط "يساوي" والقيمة المحددة هي "سلبي".](../media/condition-negative.png)](../media/condition-negative.png#lightbox)

1. من منطقه التنبيهات الأساسية، حدد **إنشاء قاعدة تنبيه**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر الزر "إنشاء قاعدة تنبيه" يتم تمييزه في مشروع ما في Dynamics 365 Customer Voice](../media/create-alert-rule-select.png)](../media/create-alert-rule-select.png#lightbox)

1. قم بتسمية القاعدة **المنتقص** وحدد **NPS** من القائمة **مقياس الرضا**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر قاعدة تنبيه جديدة يتم إنشاؤها في Customer Voice. اسم القاعدة هو "المنتقص" ومقياس الرضا هو NPS.](../media/detractor-satisfaction-metric.png)](../media/detractor-satisfaction-metric.png#lightbox)

1. قم بتعيين الشرط إلى **يساوي** والقيمة إلى **منتقصون**.
   حدد الزر **حفظ**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر شرطًا تتم إضافته إلى مقياس رضا. يُظهر الشرط "يساوي" والقيمة المحددة هي "منتقصون".](../media/condition-detractor.png)](../media/condition-detractor.png#lightbox)

1. من قائمة المشروع الرئيسية، حدد الاستطلاع **ملاحظات الخدمة الميدانية‬**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر القائمة الرئيسية في مشروع ما، ويتم تمييز الاستطلاع حول "ملاحظات الخدمة الميدانية" في القسم "الاستطلاعات".](../media/field-service-feedback-alerts.png)](../media/field-service-feedback-alerts.png#lightbox)

1. حدد الزر **معاينة** من أعلى الاستطلاع.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر الزر "معاينة" وقد تم تمييزه في استطلاع في Dynamics 365 Customer Voice.](../media/preview.png)](../media/preview.png#lightbox)

1. املأ الأسئلة الموجودة في الاستطلاع. بالنسبة للسؤال 4، أدخل النص التالي:

   **كانت الخدمة سيئة للغاية، ولم نكن سعداء بطريقة التعامل مع مشكلتنا.**

   بالنسبة للسؤال 5، حدد الرقم 6 أو أقل ثم **إرسال** الاستطلاع.

## <a name="task-4-assign-and-resolve-an-alert"></a>المهمة 4: تعيين أحد التنبيهات وحلها

في هذه المهمة، ستقوم بمراجعة التنبيهات التي قمت بإنشائها في المهمة 3 ثم تعيين أحد التنبيهات وحلها.

1. حدد الخيار **التنبيهات** من قائمة المشروع الرئيسية من المشروع الذي قمت بإنشائه في المهمة 1.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر منطقة "التنبيهات" الرئيسية في مشروع ما في Dynamics 365 Customer Voice.](../media/alerts-anonymous.png)](../media/alerts-anonymous.png#lightbox)

1. حدد كلمة **مجهول** للتنبيه الأول في القائمة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر تنبيهين في إحدى الشبكات على اللوحة "التنبيهات" في Customer Voice. يتم تمييز واحد من التنبيهين في القائمة.](../media/anonymous-alerts.png)](../media/anonymous-alerts.png#lightbox)

1. حدد الزر **تعيين‬**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لصفحة "تفاصيل التنبيه"، مع تمييز الزر "تعيين".](../media/assign-alert-details.png)](../media/assign-alert-details.png#lightbox)

1. ابدأ كتابة اسم أحد المستخدمين في بيئة Dataverse لديك.
   يمكنك إدخال اسم المستخدم الخاص بك في حال عدم وجود مستخدمين آخرين. بعد العثور على المستخدم، حدده من القائمة المقترحة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر المستخدم الذي تم البحث عنه لتعيين تنبيه له في Dynamics 365 Customer Voice.](../media/assign-alert-peter-suggested.png)](../media/assign-alert-peter-suggested.png#lightbox)

1. حدد الزر **تعيين‬**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة للشاشة "تعيين تنبيه إلى‬"، مع تمييز الزر "تعيين".](../media/assign-alert-2-peter.png)](../media/assign-alert-2-peter.png#lightbox)

   يجب أن يظهر التنبيه الآن على أنه تم تعيينه للمستخدم الذي حددتَه.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة للشاشة "تفاصيل التنبيه"، تُظهر أنه تم تعيين التنبيه في المنطقة "تم التعيين إلى".](../media/assigned.png)](../media/assigned.png#lightbox)

1. حدد علامة التبويب **ملاحظات** في شاشة **تفاصيل التنبيه**. أدخل النص التالي في الحقل:

   **اتصلتُ بالعميل ولم أتلقَّ ردًا. سأتابع مرة أخرى الأسبوع القادم.**

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لعلامة التبويب "ملاحظات" في الشاشة "تفاصيل التنبيه"، تُظهر التعليقات التي تمت إضافتها إلى الحقل.](../media/alert-details-summary.png)](../media/alert-details-summary.png#lightbox)

1. حدد الزر **حفظ**.

1. حدد شبكة التنبيهات، ثم قم بتمرير المؤشر فوق نشاط التنبيه الآخر الذي لم يتم تعيينه بعد. حدد علامة الحذف (**...**) ثم حدد الخيار **تعيين**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر أحد أنشطة التنبيه في الشبكة "التنبيهات" مع فتح قائمة علامة الحذف. يتم تمييز الزر "تعيين".](../media/assign-anonymous.png)](../media/assign-anonymous.png#lightbox)

1. ابدأ كتابة اسم أحد المستخدمين في بيئة Dataverse لديك.
   يمكنك استخدام اسم المستخدم لديك في حال عدم وجود مستخدمين آخرين. بعد العثور على المستخدم، حدده من القائمة المقترحة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة للشاشة "التعيين إلى"، مع إدخال أحد الأسماء في مربع البحث للعثور على شخص ما لتعيين تنبيه إليه.](../media/assign-alert-peter.png)](../media/assign-alert-peter.png#lightbox)

1. حدد الزر **تعيين‬**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر مستخدمًا تم تحديده لتعيين تنبيه إليه. يتم تمييز الزر "تعيين".](../media/assign.png)](../media/assign.png#lightbox)

1. حدد قائمة علامة الحذف مرة أخرى، وفي هذه المرة حدد الخيار **حل**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة للشبكة "التنبيهات" مع فتح قائمة علامة الحذف وتمييز الزر "حل".](../media/resolve-anonymous-alert.png)](../media/resolve-anonymous-alert.png#lightbox)

1. أضف النص التالي في المربع **التعليقات**:

   **تم التحدث مع العميل. وتم حل المشكلة معه، وأصبح الآن مسرورًا بمتابعة العمل في المشروع.**

   في الجزء السفلي من اللوحة، حدد الزر **حل**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر شاشة التنبيهات "حل" مفتوحة مع إضافة نص إلى المربع "التعليقات".](../media/resolve-alert-comments.png)](../media/resolve-alert-comments.png#lightbox)

1. حدد علامة التبويب **تم الحل**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة للشبكة "التنبيهات" مع تمييز علامة التبويب "تم الحل".](../media/resolved-tab.png)](../media/resolved-tab.png#lightbox)

سيظهر الآن التنبيه الذي قمت بحله مع تفاصيل من قام بحل المشكلة، بالإضافة إلى وقت حلها وتفاصيل الحل.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة تُظهر علامة التبويب "تم الحل" تسرد جميع أنشطة التنبيهات التي تم حلها لأحد المشروعات في Dynamics 365 Customer Voice.](../media/alert-details-resolution.png)](../media/alert-details-resolution.png#lightbox)
