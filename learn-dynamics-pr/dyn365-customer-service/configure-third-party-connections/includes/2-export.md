---
ms.openlocfilehash: ed95c02bfbd96698a111eefa64de202ea51c1dd8
ms.sourcegitcommit: c9e4fdec30906fc4b8686ea5c65b335ca5b68c26
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2021
ms.locfileid: "7933563"
---
تتمثل إحدى الإمكانيات الرئيسية لبرنامج Customer Insights في القدرة على استخدام بيانات Customer Insights في تطبيقات أخرى. تعد تطبيقات Microsoft Dynamics 365، مثل Dynamics 365 Sales وDynamics 365 Marketing، أمثلة رئيسية حيث يمكن أن يوفر تطبيق بيانات Customer Insights تجربة محسنة ويسمح لك بالوصول إلى العملاء واستهدافهم بشكل أفضل.

## <a name="dynamics-365-marketing"></a>Dynamics 365 Marketing

يساعد Dynamics 365 Marketing المؤسسات على الارتقاء بتجارب العملاء من خلال السماح لك بتنظيم رحلات مخصصة عبر جميع نقاط الاتصال لتقوية العلاقات وكسب الولاء.

بالإضافة إلى إمكانات إدارة الأحداث، يتكون Dynamics 365 Marketing من وحدتين أساسيتين:

-   **التسويق في الوقت الفعلي** - يتيح لك بدء رحلات العملاء في الوقت الفعلي بناءً على الإشارات وبيانات الملف الشخصي الغنية التي تجمعها من عملائك. بالإضافة إلى ذلك، يمكنك اختيار القناة الصحيحة لكل فرد والتواصل في اللحظات المهمة.

-   **التسويق الخارجي** - يوفر [التسويق عبر البريد الإلكتروني](/dynamics365/marketing/prepare-marketing-emails/?azure-portal=true)، [رحلات العميل](/dynamics365/marketing/customer-journeys-create-automated-campaigns/?azure-portal=true)، [تسجيل نقاط رئيسية](/dynamics365/marketing/set-up-lead-scoring/?azure-portal=true)، [وصفحات التسويق](/dynamics365/marketing/create-deploy-marketing-pages/?azure-portal=true)، [والنشر في مواقع التواصل الاجتماعي](/dynamics365/marketing/social-posting/?azure-portal=true)، والتي تتيح لك ربط عمليات التسويق والمبيعات الخاصة بك بسلاسة.

## <a name="outbound-marketing"></a>التسويق الصادر

بينما يمكنك إنشاء شرائح العملاء في Dynamics 365 Marketing، فإن المعايير والبيانات المستخدمة في إنشاء هذه المقاطع تقتصر على البيانات المخزنة في Dynamics 365 Marketing. باستخدام رؤى الجمهور، يمكنك استخدام ملفات تعريف العملاء الموحدة التي تتضمن بيانات من بيانات Dynamics 365 Marketing والتطبيقات الأخرى. باستخدام إمكانات إثراء رؤى الجمهور، مثل تضمين البيانات من البائعين، يمكنك بناء فهم أعمق عن هوية عملاؤك بحيث يمكنك إنشاء مقاطع مستهدفة أكثر مما لو كنت تخطط لاستخدام Dynamics 365 Marketing فقط.

يتيح لك الحل المتكامل بين Dynamics 365 Marketing وCustomer Insights:

-   **تضمين بيانات Dynamics 365 Marketing في ملف تعريف العميل الموحد** - تحميل البيانات من Dynamics 365 Marketing إلى Customer Insights بحيث يمكنه دمج معلومات العميل مع البيانات من مصادر أخرى.

-   **إثراء البيانات** - استخدم أدوات مثل Microsoft Graph والبيانات من خدمات أخرى، مثل التجربة، حتى تتمكن من بناء فهم كامل للعميل وبناء المزيد من مقاطع العملاء المستهدفة.

-   **استخدم بيانات Customer Insights في رحلات عميل Dynamics 365 Marketing** - استيراد المقاطع التي تم إنشاؤها في Customer Insights إلى Dynamics 365 Marketing ثم أدخلها في رحلات العميل.

لاستخدام مقاطع Dynamics 365 Customer Insights مع Dynamics 365 Marketing، أكمل الخطوات التالية:

1.  **أحضر جهات اتصال Marketing الخاصة بك إلى Customer Insights**. من خلال إعداد Dynamics 365 Marketing كمصدر بيانات، يمكنك تضمين جهات اتصال Marketing في ملف تعريف العميل الموحد الخاص بك. لمزيد من المعلومات، راجع [جلب جهات اتصال Marketing إلى Customer Insights](/dynamics365/marketing/customer-insights-segments?azure-portal=true#bring-your-marketing-contacts-into-customer-insights).

1.  **حدد تطبيق Marketing الخاص بك على أنه تصدير**. لكي تتوفر مقاطع Customer Insights في Dynamics 365 Marketing، قم بإعداد مثيل Marketing الخاص بك كوجهة تصدير. ما عليك سوى إكمال هذه الخطوة مرة واحدة. [تعرف على كيفية تحديد تطبيق Marketing الخاص بك كوجهة تصدير](/dynamics365/marketing/customer-insights-segments?azure-portal=true#set-your-marketing-app-as-an-export-destination-in-customer-insights).

1.  **أنشئ مقاطعك في Customer Insights**. يمكنك إنشاء مقاطع في Customer Insights لاستخدام عناصر مثل بيانات الإثراء والذكاء والعناصر الأخرى. [تعرف على كيفية بناء مقاطع العملاء](/dynamics365/marketing/segmentation-lists-subscriptions/?azure-portal=true). 

1.  **قم بإعداد مقطع للتصدير إلى Marketing**. أضف أي مقطع تريد تصديره إلى Marketing إلى وجهة التصدير المناسبة بحيث يمكنك إتاحته في مثيل Marketing الذي يتصل به. [تعرف على المزيد حول إعداد مقطع للتصدير إلى Marketing](/dynamics365/marketing/customer-insights-segments?azure-portal=true#configure-a-customer-insights-segment-to-export-to-marketing).

بالإضافة إلى ذلك، يمكنك تعديل الأجزاء المتاحة للتصدير وتعديل حالة تحديث التصدير. لمزيد من المعلومات، راجع [استخدام مقاطع Customer Insights مع Dynamics 365 Marketing](/dynamics365/marketing/customer-insights-segments/?azure-portal=true).

## <a name="real-time-marketing"></a>التسويق في الوقت الحقيقي

من الناحية التاريخية، كان Dynamics 365 Marketing تطبيقاً للمسوقين. الآن، بمساعدة الذكاء الاصطناعي واللغة الطبيعية، يمكن لمستخدمي الأعمال بناء رحلات قائمة على الأحداث تصل إلى العملاء عبر نقاط اتصال متعددة وتنمي العلاقات من العملاء المحتملين من خلال المبيعات والدعم.

من خلال التسويق في الوقت الفعلي، يمكنك تخصيص تفاعل العملاء باستخدام بيانات المعاملات والسلوكية والديموغرافية من [Dynamics 365 Customer Insights](/customer-insights/?azure-portal=true). باستخدام بيانات Customer Insights، يُمكنك:

-   استهدف ملفات تعريف العملاء الموحدة في Customer Insights ومقاطعها، والتي ستساعدك على إشراك كل عميل، بغض النظر عما إذا كانت بيانات العميل في Marketing أو Customer Insights.

-   المحتوى الديناميكي الأساسي (مثل الرموز المميزة المخصصة) في رسائل البريد الإلكتروني والرسائل النصية والإخطارات المؤقتة عن بعض الإجراءات مثل حالة الولاء أو تاريخ تجديد الاشتراك أو الحساب الأصلي أو أي إجراء آخر قمت باتخاذه في ملف تعريف العميل الموحّد.

على سبيل المثال، ضع في اعتبارك سيناريو يكون لديك فيه موقع ويب للتجارة الإلكترونية. تتمثل ممارستك في الحصول على معلومات حول الزوار والمتسوقين على موقع الويب كملفات تعريف العملاء في Customer Insights. الآن، قررت أيضاً استهداف الزوار الذين تخلوا عن عرباتهم أثناء التسوق.

للتأكد من أنه يمكنك استخدام بيانات Customer Insights في Dynamics 365 Marketing، تأكد من أنك قمت بتمكين مشاركة البيانات بين بيئة Customer Insights ومثيل Microsoft Dataverse الذي يدعم Dynamics 365 Marketing. عادةً، يمكن تنفيذ هذه المهمة عند إنشاء بيئتك، ولكن يمكنك إضافتها لاحقاً إذا لزم الأمر. لمزيد من المعلومات، راجع [اتصل بـ Microsoft Dataverse](/dynamics365/customer-insights/audience-insights/manage-environments?azure-portal=true#create-an-environment-in-an-existing-organization).

بعد تمكين مشاركة البيانات وإكمال عملية **الخريطة والمطابقة والدمج** وإنشاء مقطع واحدة على الأقل، يمكنك البدء في استخدام البيانات في Marketing. يمكنك إعداد الاتصال في Dynamics 365 Marketing عن طريق تحديد **الإعدادات > إدارة البيانات > موصل Customer Insights**. 

> [!div class="mx-imgBorder"]
> [![لقطة شاشة للموصل Customer Insights في Dynamics 365 Marketing.](../media/customer-insights-connector.png)](../media/customer-insights-connector.png#lightbox)

لمزيد من المعلومات، راجع [استخدام ملفات تعريف Customer Insights والقطاعات في التسويق في الوقت الفعلي](/dynamics365/marketing/real-time-marketing-ci-profile?azure-portal=true#set-up-default-properties-for-unified-customer-profiles).

## <a name="dynamics-365-sales"></a>Dynamics 365 Sales

يُمكّن Dynamics 365 Sales مندوبي المبيعات من بناء علاقات قوية مع عملائهم، واتخاذ الإجراءات بناءً على الرؤى، وإغلاق الصفقات بشكل أسرع. يمكنك استخدام Dynamics 365 Sales لتتبع حساباتك وجهات اتصالك، وتعزيز مبيعاتك من العميل المتوقع إلى الطلب، وإنشاء ضمانات المبيعات. علاوة على ذلك، يمكنك إنشاء قوائم وحملات تسويقية، ويمكنك متابعة حالات الخدمة المرتبطة بحسابات أو فرص معينة.

يمكن للمؤسسات التي تستخدم Customer Insights استخدام بيانات العملاء لإنشاء قوائم التسويق ومتابعة مهام سير العمل وإرسال العروض الترويجية في Dynamics 365 Sales.

على غرار إمكانات التصدير الأخرى، إذا كنت تريد استخدام بيانات Customer Insights في Dynamics 365 Sales، فأنت بحاجة إلى إكمال خطوتين:

-   **قم بإعداد الاتصال بـ Sales** - ضمن **المسؤول > اتصالات**، أضف اتصالاً ثم حدد **Dynamics 365 Sales**. بعد تحديد عنوان الخادم والمصادقة، سيكون الاتصال متاحاً في المستقبل لعمليات التصدير. [تعرف على كيفية إعداد اتصال بـ Dynamics 365 Sales](/dynamics365/customer-insights/audience-insights/export-dynamics365-sales/?azure-portal=true).

-   **قم بإعداد التصدير** - ضمن **البيانات> الصادرات**، أضف وجهة تصدير جديدة تشير إلى اتصال Dynamics 365 Sales الذي قمت بإنشائه مسبقاً. في التصدير، حدد المقاطع المراد تضمينها في التصدير. [تعرف على كيفية إعداد تصدير إلى Dynamics 365 Sales](/dynamics365/customer-insights/audience-insights/export-dynamics365-sales?azure-portal=true#configure-an-export).

الآن بعد أن تعلمت كيفية استخدام ملف تعريف العميل وبيانات المقطع من Customer Insights مع Dynamics 365 Marketing وDynamics 365 Sales، يمكنك معرفة كيفية عرض بيانات Customer Insights في سجلات Dynamics 365.

