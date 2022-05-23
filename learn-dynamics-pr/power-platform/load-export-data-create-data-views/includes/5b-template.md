---
ms.openlocfilehash: 967642597dbf1f17adb3d660131c4190d6062372
ms.sourcegitcommit: d923ddcaa6b0e6740cbcf77535cb6de781dc6b19
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/03/2022
ms.locfileid: "8666623"
---
يمكنك إنشاء تدفقات بيانات Microsoft Power Platform من الاستعلامات في أوراق عمل Microsoft Excel للاستفادة من تدفقات البيانات المدعومة من السحابة التي تقوم بتحديث البيانات ومعالجتها على فترات منتظمة بدلاً من إجراء هذه العمليات يدويًا في Excel.

يمكن أن يكون العمل مع مجموعات البيانات الكبيرة أو الاستعلامات طويلة الأمد مرهقًا في كل مرة يتعين عليك فيها تشغيل تحديث البيانات يدويًا في Excel لأنه يأخذ موارد من جهاز الكمبيوتر لديك للقيام بذلك، وعليك الانتظار حتى يتم إجراء الحساب للحصول على أحدث البيانات . يعد نقل عمليات البيانات هذه إلى تدفق بيانات Power Platform طريقة فعالة لتحرير موارد الكمبيوتر الخاص بك ولإتاحة أحدث البيانات بسهولة لتستهلكها في Excel.

## <a name="exporting-queries-in-excel-to-a-power-query-template"></a>تصدير الاستعلامات في Excel إلى قالب Power Query
    
>[!NOTE]
>يتوفر قالب التصدير التالي [للمشتركين في Office Insider](https://insider.office.com/?azure-portal=true) فقط.

تتمثل الخطوة الأولى في إنشاء قالب Power Query باستخدام استعلاماتك في Excel. 
    

1. ابدأ بفتح Excel ثم محرر Power Query من علامة التبويب البيانات > الحصول على البيانات > **تشغيل محرر Power Query**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لتشغيل ميزة محرر Power Query.](../media/5b-template-excel-power-query.png)](../media/5b-template-excel-power-query.png#lightbox)

1. بمجرد تحميل Power Query، حدد الملف > **تصدير قالب**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لميزة قالب التصدير.](../media/5b-excel-power-query-export.png)](../media/5b-excel-power-query-export.png#lightbox)

1. قم بتسميه القالب الخاص بك وإضافة وصف، ثم حدد **موافق**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لحقل اسم قالب تصدير power query.](../media/5b-excel-power-query-export-name.png)](../media/5b-excel-power-query-export-name.png#lightbox)

## <a name="creating-a-power-platform-dataflow-from-the-power-query-template"></a>إنشاء تدفق بيانات Power Platform من قالب Power Query

1.  قم بتسجيل الدخول إلى مدخل Power Apps.

1.  تحديد بيئة.

1.  في جزء التنقل الأيمن، حدد **Dataverse** > **تدفقات البيانات**.

1. من شريط الأدوات، حدد **تدفقات البيانات الجديدة** > **استيراد قالب**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لقالب الاستيراد في قائمة تدفق البيانات الجديدة.](../media/5b-template-excel-import-template.png)](../media/5b-template-excel-import-template.png#lightbox)

1. حدد قالب Power Query الذي قمت بإنشائه مسبقاً. سيتم ملء اسم تدفق البيانات مع اسم القالب المقدم. بمجرد الانتهاء من شاشة إنشاء تدفق البيانات، حدد **التالي** لرؤية استعلاماتك من Excel في محرر الاستعلام.

1. من الآن، اتبع الخطوات الموجودة في الفصل السابق حول إنشاء تدفق البيانات وعملية التكوين حتى تتمكن من إجراء المزيد من التحويل لبياناتك، وتعيين جداول التحديث في تدفق البيانات، وأي عملية تدفق بيانات أخرى ممكنة.
