---
ms.openlocfilehash: 426e8d75b9b2001e966fb54a4806417a36c4a2fc
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7457473"
---
يوفر API العميل كائن يمكن الوصول إليه بشكل عمومي (Xrm)، وهو متوفر للاستخدام في التعليمات البرمجية الخاصة بك للقيام بأنشطة مختلفة. على مستوى عالٍ، يوضح الرسم التالي كل من الخصائص والطرق المتاحة. للحصول على نظرة عامة متعمقة لهذا الكائن، راجع [كائن Xrm API العميل](/powerapps/developer/model-driven-apps/clientapi/clientapi-xrm/?azure-portal=true).

![نموذج كائن Xrm يوضح كل من الخصائص والطرق المتاحة.](../media/xrm-object.png)

## <a name="device-object"></a>كائن الجهاز

يكشف كائن Xrm.Device عن إمكانيات الجهاز الأصلية المرتبطة بتفاعلات الجهاز المحمول، باستثناء طريقة pickFile، والتي يمكن الوصول إليها أيضاً من خلال عملاء الويب. توفر تطبيقات اللوحة أيضاً إطاراً موسعاً لتطوير الأجهزة المحمولة ويجب أيضاً أخذها في الاعتبار في هذه السيناريوهات. الجدول التالي هو ملخص للطرق المتوفرة داخل كائن Xrm.Device.

| الطريقة             | الوصف                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------|
| [captureAudio](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-device/captureaudio/?azure-portal=true)       | يستدعي ميكروفون الجهاز لتسجيل الصوت.                                                         |
| [captureImage](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-device/captureimage/?azure-portal=true)       | يستدعي كاميرا الجهاز لالتقاط صورة.                                                         |
| [captureVideo](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-device/capturevideo/?azure-portal=true)       | يستدعي كاميرا الجهاز لتسجيل الفيديو.                                                             |
| [getBarcodeValue](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-device/getbarcodevalue/?azure-portal=true)    | يستدعي كاميرا الجهاز لمسح معلومات الرمز الشريطي، مثل رقم المنتج.                   |
| [getCurrentPosition](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-device/getcurrentposition/?azure-portal=true) | إرجاع الموقع الحالي باستخدام إمكانية تحديد الموقع الجغرافي للجهاز.                                 |
| [pickFile](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-device/pickfile/?azure-portal=true)           | يفتح مربع حوار لتحديد الملفات من جهاز الكمبيوتر (عميل الويب) أو الجهاز المحمول (عملاء الهاتف المحمول).  |

## <a name="encoding-object"></a>كائن ترميز

يتم استخدام كائن Xrm.Encoding لترميز سلاسل XML وHTML وفك ترميزها. يمكن أن يكون هذا الترميز وفك التشفير ذا قيمة عندما تتفاعل مع موارد ويب HTML، وترميز معلمات سلسلة الاستعلام وفك تشفيرها، وأيضاً عندما تتفاعل مع FetchXML الذي يحتوي على أحرف خاصة في سلسلة البحث.

## <a name="navigation-object"></a>كائن التنقل

يوفر كائن التنقل طرقاً مرتبطة بالتنقل يمكن استخدامها داخل تطبيق يستند إلى نموذج. لا تُعتبر الأنشطة مثل عرض مربعات حوار التنبيه والتأكيد والخطأ تجربة مستخدم مثالية، ولكنها لا تزال متاحة للاستخدام. في هذه السيناريوهات، نوصي بأن تضع في اعتبارك إعلامات النموذج و/أو آليات أخرى لتحذير المستخدمين من مشكلة ما. فيما يلي ملخص للطرق المتاحة داخل كائن Xrm.Navigation.

| الطريقة            | الوصف                                                               |
|-------------------|---------------------------------------------------------------------------|
| [openAlertDialog](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openalertdialog/?azure-portal=true)   | يعرض مربع حوار تنبيه يحتوي على رسالة وزر.               |
| [openConfirmDialog](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openconfirmdialog/?azure-portal=true) | يعرض مربع حوار للتأكيد يحتوي على رسالة وزرين.  |
| [openErrorDialog](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openerrordialog/?azure-portal=true)   | يعرض مربع حوار خطأ.                                                 |
| [openFile](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openfile/?azure-portal=true)          | يفتح ملف.                                                             |
| [openForm](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openform/?azure-portal=true)          | يفتح نموذج كيان أو نموذج إنشاء سريع.                              |
| [openUrl](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openurl/?azure-portal=true)           | يفتح عنوان URL، بما في ذلك عناوين URL للملف.                                         |
| [openWebResource](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-navigation/openwebresource/?azure-portal=true)   | يفتح مورد ويب HTML.                                           |

## <a name="panel-object"></a>كائن لوحة

يوفر كائن Xrm.Panel طريقة لعرض صفحة ويب على الجزء الجانبي من نموذج تطبيق يستند إلى نموذج. هذه الميزة قيد المعاينة حالياً ولن يتم تناولها بالتفصيل هنا. لمزيد من المعلومات، راجع [لوحة Xrm](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-panel/?azure-portal=true).

## <a name="utility-object"></a>كائن الأداة المساعدة

يوفر كائن Xrm.Utility حاوية لمختلف الأساليب المفيدة.
الجدول التالي هو ملخص للطرق المتوفرة داخل كائن Xrm.Utility. لمزيد من المعلومات، راجع [Xrm.Utility (مرجع واجهة API العميل)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/?azure-portal=true)

| الطريقة                       | الوصف                                                                                                                                                    |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [closeProgress](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/closeprogressindicator/?azure-portal=true)                | المؤشر يغلق مربع حوار التقدم.                                                                                                                        |
| [getAllowedStatusTransitions](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/getallowedstatustransitions/?azure-portal=true)  | ترجع انتقالات الحالة الصالحة لنوع الكيان المحدد ورمز الحالة.                                                                              |
| [getEntityMetadata](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/getentitymetadata/?azure-portal=true)            | ترجع بيانات تعريف الكيان للكيان المحدد.                                                                                                          |
| [getGlobalContext](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/getglobalcontext/?azure-portal=true)             | يحصل على السياق العمومي.                                                                                                                                       |
| [getLearningPathAttributeName](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/getlearningpathattributename/?azure-portal=true) | يُرجع اسم سمة DOM التي يتوقعها مصمم محتوى مسار التعلم (تعليمات إرشادية) لتحديد عناصر تحكم واجهة المستخدم في نماذج التطبيقات المستندة إلى النموذج. |
| [getResourceString](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/getresourcestring/?azure-portal=true)            | ترجع السلسلة المترجمة لمفتاح معين مرتبط بمورد الويب المحدد.                                                                       |
| [invokeProcessAction](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/invokeprocessaction/?azure-portal=true)          | يستدعي إجراءً بناءً على المعلمات المحددة.                                                                                                           |
| [lookupObjects](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/lookupobjects/?azure-portal=true)                | يفتح عنصر تحكم بحث لتحديد صنف واحد أو أكثر.                                                                                                            |
| [refreshParentGrid](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/refreshparentgrid/?azure-portal=true)            | يجدد الشبكة الرئيسية التي تحتوي على السجل المحدد.                                                                                                     |
| [showProgressIndicator](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-utility/showprogressindicator/?azure-portal=true)        | يعرض حوار التقدم بالرسالة المحددة.                                                                                                         |

## <a name="xrmwebapi-object"></a>كائن Xrm.WebApi

يوفر كائن Xrm.WebApi خصائص وأساليب لاستخدام واجهة API الويب لعمليات CRUD التقليدية داخل برنامج نصي للعميل. الجدول التالي هو ملخص للطرق المتوفرة في كائن Xrm.WebApi. لمزيد من المعلومات، راجع [Xrm.WebApi (مرجع واجهة API العميل)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/?azure-portal=true).

| الطريقة              | الوصف                                                                                                                           |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| [createRecord](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/createrecord/?azure-portal=true)              | يقوم بإنشاء سجل كيان.                                                                                                      |
| [deleteRecord](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/deleterecord/?azure-portal=true)              | يحذف سجل الكيان.                                                                                                      |
| [retrieveRecord](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/retrieverecord/?azure-portal=true)            | يسترجع سجل الكيان.                                                                                                    |
| [retrieveMultipleRecords](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/retrievemultiplerecords/?azure-portal=true)            | يسترجع مجموعة من سجلات الكيانات.                                                                             |
| [updateRecord](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord/?azure-portal=true)              | يحدّث سجل الكيان.                                                                                                      |
| [isAvailableOffline](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/isavailableoffline/?azure-portal=true)  | ترجع قيمة منطقية تشير إلى ما إذا كان الكيان موجوداً في ملف تعريف المستخدم ومتاحاً في وضع عدم الاتصال. |
| [تنفيذ](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/online/execute/?azure-portal=true)             | قم بتشغيل إجراء أو وظيفة واحدة أو عملية CRUD.                                                                                 |
| [executeMultiple](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/online/executemultiple/?azure-portal=true)             | قم بتشغيل مجموعة من الإجراءات أو الوظائف أو عمليات CRUD.                                                                | 
