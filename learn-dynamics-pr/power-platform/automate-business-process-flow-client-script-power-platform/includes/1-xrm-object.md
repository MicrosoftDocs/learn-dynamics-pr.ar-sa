---
ms.openlocfilehash: 99f966021be29b907dfdc534bc8e8bfa1ad61ed7
ms.sourcegitcommit: 638bab9b0642ad3d3698e559bdfe044fb14354f7
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2022
ms.locfileid: "8548623"
---
توفر API الخاصة بالعميل كائن **Xrm** والذي يكون متوفراً بشكل عام في التعليمات البرمجية الخاصة بك للقيام بأنشطة مختلفة دون الحاجة إلى استخدام سياق التنفيذ. على مستوى عالٍ، يوضح الرسم التالي كل من الخصائص والطرق المتاحة. للحصول على نظرة عامة متعمقة لهذا الكائن، راجع [كائن Xrm API الخاص بالعميل](/power-apps/developer/model-driven-apps/clientapi/clientapi-xrm/?azure-portal=true).

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لمساحات الاسم في نموذج كائن API لبرنامج العميل النصي وXrm والتطبيق والجهاز والترميز والتنقل واللوحة والأداة المساعدة وWebAPI.](../media/xrm-object.png)](../media/xrm-object.png#lightbox)

## <a name="app-object"></a>كائن التطبيق

باستخدام addGlobalNotification من كائن التطبيق، يمكنك عرض إخطار بالخطأ أو المعلومات أو التحذير أو النجاح لأحد التطبيقات وتحديد الإجراءات التي سيتم تنفيذها استناداً إلى الاخطار. يتشابه هذا النموذج مع الإخطارات ولكن يمكن استخدامه خارج سياق النموذج. على سبيل المثال، يمكن أن يستخدم البرنامج النصي لشريط الأوامر هذا العنصر لإخطار المستخدم باكتمال تنفيذ الإجراء. استخدم أسلوب clearGlobalNotification لمسح إخطار في التطبيق.

## <a name="device-object"></a>كائن الجهاز

يكشف كائن Xrm.Device عن إمكانيات الجهاز الأصلية المرتبطة بتفاعلات الجهاز المحمول، باستثناء طريقة pickFile، والتي يمكن الوصول إليها أيضاً من خلال عملاء الويب. توفر تطبيقات اللوحة أيضاً إطار عمل موسع لتطوير الأجهزة المحمولة ويجب أيضاً أخذها في الاعتبار في هذه السيناريوهات. الجدول التالي هو ملخص للطرق المتوفرة داخل كائن Xrm.Device.

|     الطريقة                |     الوصف                                                                                                |
|---------------------------|----------------------------------------------------------------------------------------------------------------|
|     [captureAudio](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-device/captureaudio/?azure-portal=true)          |     يستدعي ميكروفون الجهاز لتسجيل الصوت.                                                             |
|     [captureImage](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-device/captureimage/?azure-portal=true)          |     يستدعي كاميرا الجهاز لالتقاط صورة.                                                             |
|     [captureVideo](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-device/capturevideo/?azure-portal=true)          |     يستدعي كاميرا الجهاز لتسجيل مقطع فيديو.                                                               |
|     [getBarcodeValue](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-device/getbarcodevalue/?azure-portal=true)       |     يستدعي كاميرا الجهاز لمسح معلومات الرمز الشريطي، مثل رقم المنتج.                     |
|     [getCurrentPosition](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-device/getcurrentposition/?azure-portal=true)    |     إرجاع الموقع الحالي باستخدام إمكانية تحديد الموقع الجغرافي للجهاز.                                 |
|     [pickFile](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-device/pickfile/?azure-portal=true)              |     يفتح مربع حوار لتحديد الملفات من جهاز الكمبيوتر (عميل الويب) أو الجهاز المحمول (عملاء الأجهزة المحمولة).    |

ووفقاً لتكوين الجهاز، لن تتوفر بعض الوظائف. قد تكون موافقة المستخدم مطلوبة أيضاً حتى يتمكن التطبيق من الوصول إلى إمكانيات معينة للجهاز. على سبيل المثال، قد يكون المستخدم قد قام بتعطيل إمكانيات موقع الجهاز بشكل عام أو أنه رفض الوصول إلى كاميرا التطبيق. عند تطوير تطبيق احذر من فشل إحدى هذه الطرق بسبب إمكانيات الجهاز أو التكوين أو نقص الأذونات أو الموافقة.

## <a name="encoding-object"></a>كائن ترميز

يتم استخدام كائن Xrm.Encoding لترميز سلاسل XML وHTML وفك ترميزها. يمكن أن يكون هذا الترميز وفك التشفير ذا قيمة عندما تتفاعل مع موارد ويب HTML، وتشفير معلمات سلسلة الاستعلام وفك تشفيرها، وأيضاً عندما تتفاعل مع FetchXML الذي يحتوي على أحرف خاصة مثل "&" أو '\<' في سلسلة البحث.

## <a name="navigation-object"></a>كائن التنقل

يوفر كائن التنقل طرقاً مرتبطة بالتنقل يمكن استخدامها داخل تطبيق يستند إلى نموذج. نظراً لطبيعة الحظر، لا تُعتبر الأنشطة مثل عرض مربعات حوار التنبيه والتأكيد والخطأ تجربة مستخدم مثالية، ولكنها لا تزال متاحة للاستخدام. في هذه السيناريوهات، عليك أن تضع في اعتبارك إخطارات النموذج أو آليات أخرى غير محظورة لتحذير المستخدمين من مشكلة ما. فيما يلي ملخص للطرق المتاحة داخل كائن Xrm.Navigation.

 |     الطريقة               |     الوصف                                                                      |
|--------------------------|--------------------------------------------------------------------------------------|
|     [openAlertDialog](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openalertdialog/?azure-portal=true)      |     يعرض مربع حوار التنبيه الذي يحتوي على رسالة وزر.                 |
|     [openConfirmDialog](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openconfirmdialog/?azure-portal=true)    |     يعرض مربع حوار للتأكيد الذي يحتوي على رسالة وزرين.    |
|     [openErrorDialog](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openerrordialog/?azure-portal=true)      |     يعرض مربع حوار الخطأ.                                                        |
|     [openFile](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openfile/?azure-portal=true)             |     فتح ملف.                                                                    |
|     [openForm](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openform/?azure-portal=true)             |     فتح نموذج جدول أو نموذج إنشاء سريع.                                       |
|     [openUrl](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openurl/?azure-portal=true)              |     فتح عنوان URL، بما في ذلك عناوين URL للملف.                                                |
|     [openWebResource](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openwebresource/?azure-portal=true)      |     فتح مورد ويب بتنسيق HTML.                                                      |

## <a name="panel-object"></a>كائن لوحة

يوفر كائن Xrm.Panel طريقة لعرض صفحة ويب في الجزء الجانبي لنموذج تطبيق يستند إلى النموذج. هذه الميزة موجودة حالياً في الإصدار الأولي ولن يتم تناولها بالتفصيل هنا. لمزيد من المعلومات، راجع [لوحة Xrm.](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-panel/?azure-portal=true).

## <a name="utility-object"></a>كائن الأداة المساعدة

يعد كائن Xrm.Utility حاوية للعديد من الأساليب المفيدة. الجدول التالي هو ملخص للطرق المتوفرة داخل كائن Xrm.Utility. لمزيد من المعلومات، راجع [Xrm.Utility (مرجع API الخاص بالعميل)](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/?azure-portal=true)

  |     الطريقة                          |     الوصف                                                                                                                                                                   |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|     [closeProgressIndicator](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/closeprogressindicator/?azure-portal=true)          |     يقوم المؤشر بإغلاق مربع حوار التقدم الذي تم فتحه باستخدام showProgressIndicator.                                                                                         |
|     [getAllowedStatusTransitions](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/getallowedstatustransitions/?azure-portal=true)     |     إرجاع انتقالات الحالة الصالحة للجدول ورمز الحالة المحددين.                                                                                                 |
|     [getEntityMetadata](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/getentitymetadata/?azure-portal=true)               |     يعيد بيانات تعريف الكيان للكيان المحدد.                                                                                                                         |
|     [getGlobalContext](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/getglobalcontext/?azure-portal=true)                |     الحصول على السياق العمومي الذي يمكنه توفير معلومات وقت التشغيل بما في ذلك إعدادات المؤسسة وإعدادات المستخدم والتطبيق ومعلومات العميل.                              |
|     [getLearningPathAttributeName](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/getlearningpathattributename/?azure-portal=true)    |     إرجاع اسم سمة DOM المتوقعة من مصمم محتوى مسار التعليم (التعليمات الإرشادية) لتحديد عناصر تحكم واجهة المستخدم في نماذج التطبيقات المستندة إلى النموذج.    |
|     [getResourceString](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/getresourcestring/?azure-portal=true)               |     إرجاع السلسلة المترجمة لمفتاح محدد مقترن مع مورد الويب المحدد.                                                                            |
|     [invokeProcessAction](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/invokeprocessaction/?azure-portal=true)             |     استدعاء اجراء استناداً إلى المعلمات المحددة. يمكن أيضاً استخدام هذا لاستدعاء واجهات برمجة التطبيقات المخصصة (APIs) التي تم إنشاؤها من قبل المطورين.                                            |
|     [lookupObjects](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/lookupobjects/?azure-portal=true)                   |     يستخدم هذا الزر في فتح عنصر تحكم بحث لتحديد صنف واحد أو أكثر.                                                                                                                           |
|     [refreshParentGrid](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/refreshparentgrid/?azure-portal=true)               |     تحديث الشبكة الأصل التي تحتوي على السجل المحدد.                                                                                                               |
|     [showProgressIndicator](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility/showprogressindicator/?azure-portal=true)           |     يعرض مربع حوار التقدم مع الرسالة المحددة.                                                                                                                        |

هناك أيضاً العديد من الأساليب غير المدرجة أعلاه التي قد تكون موجودة في التعليمات البرمجية القديمة [والتي تم إهمالها الآن](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-utility?azure-portal=true#deprecated-methods) بسبب أنها انتقلت إلى مساحة اسم Xrm.Navigation. في حالة العثور على هذه الأساليب يجب تحديث الكود لاستخدام أساليب Xrm.Navigation الجديدة.

## <a name="xrmwebapi-object"></a>كائن Xrm.WebApi

يوفر كائن Xrm.WebApi خصائص وأساليب لاستخدام عنوان API للويب لعمليات CRUD التقليدية داخل البرنامج النصي الخاص بالعميل. عند استخدام Xrm.WebAPI، تتم معالجة المصادقة تلقائياً في سياق المستخدم الحالي باستخدام التطبيق. يمكن استخدام عنوان API للويب سواءً كان التطبيق متصلاً أو غير متصل (إذا تم تكوين البيئة). تتضمن مساحة الاسم مجموعة معينة من الأساليب المتصلة بالإنترنت وغير المتصلة ومع ذلك فإن استخدام هذه الطرق يتطلب منك تعقب حالة العميل. إذا كنت تستخدم Xrm.WebAPI ،Xrm.WebAPI.createRecord، تحدد واجهة برمجة التطبيقات (API) ما إذا كان يجب أن تستخدم أساليب مساحة الاسم المتصلة أو غير المتصلة.

الجدول التالي هو ملخص للطرق المتوفرة داخل كائن Xrm.WebApi. لمزيد من المعلومات، راجع [Xrm.WebApi (مرجع API الخاص بالعميل)](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/?azure-portal=true).

|     الطريقة                     |     الوصف                                                                                                               |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------|
|     [createRecord](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/createrecord/?azure-portal=true)               |     إنشاء صف جدول.                                                                                                      |
|     [deleteRecord](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/deleterecord/?azure-portal=true)               |     يتيح حذف صف جدول باستخدام معرف الصف.                                                                              |
|     [retrieveRecord](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/retrieverecord/?azure-portal=true)             |     يتيح استرجاع صف باستخدام معرف الصف.                                                                                  |
|     [retrieveMultipleRecords](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/retrievemultiplerecords/?azure-portal=true)    |     استرداد مجموعة من صفوف الجدول المطابقة لخيارات الاستعلام أو إحضار XML المتوفر.                                  |
|     [updateRecord](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord/?azure-portal=true)               |     تحديث صف جدول.                                                                                                      |
|     [isAvailableOffline](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/isavailableoffline/?azure-portal=true)         |     إرجاع القيمة المنطقية التي تشير إلى ما إذا كان الجدول موجوداً في ملف تعريف المستخدم ومتاحاً في وضع عدم الاتصال.    |
|     [تنفيذ](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/online/execute/?azure-portal=true)                    |     تشغيل اجراء أو وظيفة واحدة أو عملية CRUD.                                                                         |
|     [executeMultiple](/power-apps/developer/model-driven-apps/clientapi/reference/xrm-webapi/online/executemultiple/?azure-portal=true)            |     تشغيل مجموعة من الإجراءات أو الوظائف أو عمليات CRUD.                                                             |

باستخدام خصائص وأساليب كائن **Xrm**، يمكنك تنفيذ عمليات الأعمال تلقائياً وتحسين تجربة المستخدم الكلية.
