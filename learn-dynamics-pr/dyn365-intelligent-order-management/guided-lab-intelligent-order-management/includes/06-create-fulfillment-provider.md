---
ms.openlocfilehash: ae956258f45e1605361bab844bcad40130a13b30
ms.sourcegitcommit: 70e51e3ba609b4f9cf6b7a3b2770f4a0916c051a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2022
ms.locfileid: "8091314"
---
تصف هذه الوحدة الخطوات المطلوبة لإنشاء موفر تنفيذ في Intelligent Order Management.

## <a name="create-a-new-provider-definition"></a>إنشاء تعريف موفر جديد

لإنشاء تعريف موفر جديد، اتبع هذه الخطوات:

1. انتقل إلى **الموفرون‬ > الكتالوج**.
1. حدد **تعريف موفر جديد**.
1. في **اسم العرض**، أدخل **LabFulfillmentProvider**.
1. في **الاسم المنطقي**، أدخل **msdyn_LabFulfillmentProvider**.
1. في **الوصف**، أدخل **موفر التنفيذ المعملي**.
1. في **الشعار‬**، حدد **Lab.png**.
1. في **نوع الخدمة**، أدخل **التنفيذ**.
1. حدد **حفظ وإغلاق**.

## <a name="add-a-provider-definition-to-the-solution"></a>إضافة تعريف موفر إلى الحل

لإضافة تعريف موفر إلى الحل، اتبع الخطوات التالية:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com) وانتقل إلى الحل **LabProviders** الذي تم إنشاؤه مؤخراً.
1. حدد **إضافة موجود > تعريف موفر IOM**.
1. حدد **LabFulfillmentProvider**، ثم حدد **إضافة** لإضافته إلى الحل. 

## <a name="create-a-provider-action-to-send-a-fulfillment-payload-to-outlook"></a>إنشاء اجراء موفر لإرسال حمولة تنفيذ إلى Outlook

لإنشاء إجراء موفر لإرسال حمولة تنفيذ إلى Outlook، اتبع هذه الخطوات:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com)، ثم انتقل إلى **الحلول**.
1. افتح **الحل الافتراضي**.
1. حدد **جديد**.
1. حدد **سير العمل السحابي‬‏‫**، ثم قم بتسميته **تمرين عملي - إرسال إلى التنفيذ (Outlook)**.
1. حدد نوع التشغيل باعتباره **‬‏‫تشغيل سير عمل يدوياً‬‏‫** ثم أكمل هذه الإجراءات.
    - حدد **إضافة إدخال**، وحدد **النص**، ثم قم بإدخال **ProviderActionExecutionEventId** في الحقل الأول.
    - حدد **إضافة إدخال**، وحدد **النص**، ثم قم بإدخال **EntityRecordId** في الحقل الأول.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة خصائص تشغيل تدفق يدوياً.](../media/manual-trigger-flow-ss.png)](../media/manual-trigger-flow-ss.png#lightbox)

1. إنشاء إجراء تهيئة متغير:
    - في **الاسم**، أدخل **ExecutionResult‎**.
    - في **النوع**، حدد **منطقي**.
    - في **القيمة**، أدخل **صحيح‬**.  
1. إنشاء إجراء تهيئة متغير ثانٍ:
    - في **الاسم**، أدخل **ProcessedSaleOrderLines**.
    - في **النوع**، حدد **صفيف**.
1. إنشاء إجراء تهيئة متغير ثالث:
    - في **الاسم**، أدخل **ProcessedFulfillmentOrderLines**.
    - في **النوع**، حدد **صفيف**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لخيارات إجراءات "تهيئة متغير".](../media/variable-initialization-actions-ss.png)](../media/variable-initialization-actions-ss.png#lightbox)

1. أضف نطاق **المحاولة‏‎**.
1. ضمن نطاق **المحاولة**، أضف **تنفيذ إجراء غير مرتبط** عن طريق توفير المعلومات التالية:
    - **ProviderActionExecutionEventId** - ضمن **المحتوى الديناميكي**، حدد **ProviderActionExecutionEventId**.
    - **PowerAutomateRunId** - حدد التعبير على الشكل التالي: `workflow()['run']?['name']`.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة نطاق "المحاولة".](../media/try-scope-ss.png)](../media/try-scope-ss.png#lightbox)

1. أضف إجراء **‏‫الحصول على صف حسب المعرف** ثم أدخل المعلومات التالية:
    - في **اسم الجدول**، أدخل **أوامر التنفيذ**.
    - في **معرف الصف**، حدد **EntityRecordId** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لحقل إجراء "معرف الصف" في صفحة "المحاولة".](../media/get-fulfillment-order-ss.png)](../media/get-fulfillment-order-ss.png#lightbox)

1. أضف إجراء **إرسال رسالة إلكترونية** من موصل Outlook.com، لأن هذا هو الاتصال الذي قمت بإعداده في وقت سابق.
    - على السطر **إلى**، يتم استخدام *placeholder@placeholder.com* كعنصر نائب للنص. ستستبدل نص العنصر النائب هذا بمعلمة موفر في الخطوات اللاحقة.
    - على سطر **الموضوع**، يمكنك الحصول على **الاسم** من الخطوة **الحصول على أمر التنفيذ** ضمن **المحتوى الديناميكي**.
    - في **النص الأساسي**، حدد التعبير التالي: `outputs('Get_fulfillment_order')['body']`
    
    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة الإجراء "إرسال رسالة إلكترونية".](../media/send-email-ss.png)](../media/send-email-ss.png#lightbox)

1. أضف إجراء **إدراج صفوف** كما يلي:
    - في **اسم الجدول**، أدخل **منتجات أوامر التنفيذ**.
    - في **استعلام إحضار XML** أدخل التعليمات البرمجية التالية: 

    ```XML
    <fetch>  
      <entity name="msdyn_fulfillmentorderdetail">  
       <all-attributes />
         <filter>
         <condition attribute="msdyn_fulfillmentid" operator="eq" value="@{triggerBody()['text_1']}"/>
         </filter>
      </entity>  
    </fetch>
    ```

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة "الحصول على بنود أمر التنفيذ".](../media/get-fulfilment-lines-ss.png)](../media/get-fulfilment-lines-ss.png#lightbox)

1. أضف عنصر تحكم **تطبيق على كل‬‏‫** باستخدام إجراء **إرسال رسالة إلكترونية** كما يلي:   
    - احصل على **القيمة** من خطوة **الحصول على بند أمر التنفيذ** ضمن **المحتوى الديناميكي**. 
    - احصل على **الاسم** من خطوة **الحصول على بند أمر التنفيذ** ضمن **المحتوى الديناميكي**. 
    - حدد **الصنف الحالي** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة عنصر التحكم "تطبيق على كل".](../media/apply-to-each-control-ss.png)](../media/apply-to-each-control-ss.png#lightbox)

1. ضمن التكرار الحلقي، أضف إجراء **إلحاق بمتغير الصفيف** كما يلي:
    - في **الاسم**، أدخل **ProcessedFulfillmentOrderLines**.
    - في **القيمة**، حدد **معرف بند التنفيذ** ضمن **المحتوى الديناميكي**. 

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للصفحة "إلحاق ببنود التنفيذ التي تمت معالجتها".](../media/append-processed-fulfillment-lines-ss.png)](../media/append-processed-fulfillment-lines-ss.png#lightbox)

1. ضمن التكرار الحلقي، أضف إجراء **إلحاق بمتغير صفيف** آخر كما يلي:
    - في **الاسم**، أدخل **ProcessedSalesOrderLines**.
    - في **القيمة**، حدد **معرف سطر المبيعات** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة للصفحة "إلحاق ببنود الأمر التي تمت معالجتها".](../media/append-processed-order-lines-ss.png)](../media/append-processed-order-lines-ss.png#lightbox)

1. قم بطي نطاق **المحاولة** عن طريق تحديد شريط عنوانه. 
1. حدد **خطوة جديد**، ثم أضف نطاقاً آخر باسم **التقاط**.
1. في النطاق **التقاط**، حدد علامة الحذف (**...**)، وحدد **تكوين التشغيل بعد**، ثم أكمل إجراءات الإعداد التالية:
    - حدد خانة الاختيار **فشل**.
    - حدد خانة الاختيار **انتهت مهلته‬‏‫**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة النطاق "التقاط".](../media/catch-scope-ss.png)](../media/catch-scope-ss.png#lightbox)

1. في النطاق **التقاط**، حدد **إضافة إجراء**. أضف إجراء **تعيين متغير**، ثم غيّر اسمه إلى **تعيين نتيجة التنفيذ إلى فاشلة**.
1. قم بإعداد الخصائص على النحو التالي:
    - في **الاسم**، أدخل **ExecutionResult‎**.
    - في **القيمة**، أدخل **خطأ**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة "تعيين نتيجة التنفيذ إلى فاشلة"‬‏‫.](../media/set-execution-failed-ss.png)](../media/set-execution-failed-ss.png#lightbox)

1. حدد **‎خطوة جديدة**، ثم أضف نطاقاً آخر باسم **أخيراً**.
1. في النطاق **أخيراً**، حدد علامة الحذف (**...**)، وحدد **تكوين التشغيل بعد**، ثم أكمل الإجراءات التالية:
    - حدد خانة الاختيار **هو ناجح**.
    - حدد خانة الاختيار **انتهت مهلته‬‏‫**.
    - حدد خانة الاختيار **تم تخطيه**.
    - حدد خانة الاختيار **انتهت مهلته‬‏‫**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة النطاق "أخيراً".](../media/finally-scope-ss.png)](../media/finally-scope-ss.png#lightbox)

1. في صفحة النطاق **أخيراً**، أضف خطوة **شرط**، ثم قارن المتغير **ExecutionResult** مع **صحيح** كما يلي:
    - في الحقل الأول، حدد المتغير **ExecutionResult‎**.
    - في الحقل الثاني، حدد **يساوي**.
    - في الحقل الثالث، حدد **صحيح**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لخطوة الشرط تُظهر الحقول الثلاثة.](../media/check-processed-lines-raise-business-events-ss.png)](../media/check-processed-lines-raise-business-events-ss.png#lightbox)

1. في الفرع **إذا كانت الإجابة نعم**، أضف إجراء **تشغيل سير عمل تابع‬‏‫** وغيّر اسمه إلى **تنفيذ أحداث الأعمال لبنود أمر التنفيذ التي تمت معالجتها**.
1. قم بإعداد الخصائص على النحو التالي:
    - في **سير العمل التابع**، أدخل **تنفيذ حدث أعمال**.
    - في **BusinessEventDefinitionId**، أدخل **063d85c8-60a4-eb11-9443-000d3a313675**.
    - في **EntityRecordId**، حدد التعبير التالي: `string(variables('ProcessedFulfillmentOrderLines'))`

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لصفحة تنفيذ أحداث الأعمال لبنود أمر التنفيذ التي تمت معالجتها مع إجراء تشغيل سير عمل تابع‬ (أحداث الأعمال).](../media/raise-business-events-processed-fulfillment-order-lines-ss.png)](../media/raise-business-events-processed-fulfillment-order-lines-ss.png#lightbox)

1. في الفرع **إذا كانت الإجابة نعم**، أضف إجراء **تشغيل سير عمل تابع** آخر وغيّر اسمه إلى **تنفيذ الأحداث المجمّعة لأمر المبيعات**.
1. قم بإعداد الخصائص على النحو التالي:
   - في **LineBusinessEventDefinitionId**، أدخل **ccf64002-61a4-eb11-9443-000d3a313675**.
   - في **LineRecordId**، حدد التعبير على الشكل التالي: `string(variables('ProcessedSalesOrderLines'))`
   - في **OrderBusinessEventDefinitionId**، أدخل **48688716-61a4-eb11-9443-000d3a313675**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لإجراء تشغيل سير عمل تابع‬ (الأحداث المجمّعة).](../media/run-child-flow-action-2-ss.png)](../media/run-child-flow-action-2-ss.png#lightbox)

1. قم بطي خطوة الشرط.  
1. أضف **تنفيذ اجراء غير مرتبط** باتباع الخطوات التالية:
    - في **اسم الإجراء**، أدخل **msdyn_CompleteProviderActionExecution**.
    - في **ExecutionResult**، حدد المتغير **ExecutionResult** ضمن **المحتوى الديناميكي**.
    - في **ProviderActionExecutionEventId**، حدد **ProviderActionExecutionEventId** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لتنفيذ إجراء غير مرتبط.](../media/perform-unbound-action-ss.png)](../media/perform-unbound-action-ss.png#lightbox)

1. حدد **حفظ**.

## <a name="add-a-provider-definition-logic-definition-to-the-outlook-provider-definition"></a>إضافة تعريف منطق تعريف الموفر إلى تعريف موفر Outlook

لإضافة تعريف منطق تعريف الموفر إلى تعريف موفر Outlook، اتبع الخطوات التالية:

1. انتقل إلى **الموفرون‬ > الكتالوج**.
1. حدد **LabFulfillmentProvider** الذي تم إنشاؤه مؤخراً.
1. حدد **تحرير‬** من شريط القوائم. 
1. حدد علامة التبويب **تعريفات المنطق**.
1. حدد **+ تعريف منطق تعريف موفر IOM الجديد**.
1. في **اسم العرض**، أدخل **تمرين عملي - إرسال إلى التنفيذ (Outlook)**.
1. في **الاسم المنطقي**، أدخل **msdyn_LabSentToFulfillmentOutlook**.
1. في **تعريف الموفر**، أدخل **LabFulfillmentProvider**.
1. في **نوع المنطق**، أدخل **إجراء الموفر**.
1. في **اسم سير العمل**، أدخل **تمرين عملي - إرسال إلى التنفيذ (Outlook)**.
1. في **دقائق المهلة**، أدخل **2**.
1. في **‫الحد الأقصى لعدد عمليات إعادة المحاولة‬**، أدخل **3**.
1. في **الوصف‏‎‬**، أدخل **تمرين عملي - إرسال إلى التنفيذ (Outlook)**.
1. بالنسبة إلى **نوع الإجراء**، أدخل **الإرسال إلى التنفيذ**.
1. حدد **حفظ**. ستؤدي هذه الخطوات إلى إنشاء تمثيل JSON لسير العمل السحابي لمعالج الرسائل وتعبئة حقل **بيانات العميل**.
1. استبدل البريد الإلكتروني للعنصر النائب بمعلمة الموفر عن طريق نسخ كتلة النص في حقل **بيانات العميل** ثم لصقها في المفكرة. 
1. في كتلة النص، ابحث عن **placeholder@placeholder.com** واستبدله بـ **{{LabOutboundFulfillmentEmail}}**.
1. انسخ كتلة النص المعدّلة مرة أخرى إلى حقل **بيانات العميل**.
1. حدد **حفظ وإغلاق**.
1. حدد **الاتصالات**. يجب أن تكون الآن تعريفات مرجع اتصال **Microsoft Dataverse** و **Outlook.com** مدرجة.

## <a name="add-a-provider-definition-logic-definition-to-the-outlook-labproviders-solution"></a>إضافة تعريف منطق تعريف الموفر إلى حل Outlook LabProviders

لإضافة تعريف منطق تعريف الموفر إلى حل Outlook LabProviders، اتبع الخطوات التالية:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com) وانتقل إلى الحل **LabProviders** الذي تم إنشاؤه مؤخراً.
1. حدد **إضافة موجود > تعريف منطق تعريف موفر IOM**.
1. حدد **تمرين عملي - إرسال إلى التنفيذ (Outlook)** ثم حدد **إضافة‏‎‏‎** لإضافته إلى الحل. 

## <a name="add-provider-definition-connection-references-to-the-labproviders-solution"></a>إضافة مراجع اتصال تعريف الموفر إلى حل LabProviders

لإضافة مراجع اتصال تعريف الموفر إلى حل LabProviders، اتبع هذه الخطوات:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com) وانتقل إلى الحل **LabProviders** الذي تم إنشاؤه مؤخراً.
1. حدد **إضافة موجود > مرجع اتصال تعريف موفر IOM**.
1. حدد مراجع اتصال تعريف موفر **Microsoft Dataverse** و **Outlook.com**، ثم حدد **إضافة** لإضافتها إلى الحل. 

## <a name="create-a-provider-action-to-send-a-fulfillment-payload-to-requestbin"></a>إنشاء إجراء موفر لإرسال حمولة تنفيذ إلى RequestBin

لإنشاء إجراء موفر لإرسال حمولة تنفيذ إلى RequestBin، اتبع هذه الخطوات:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com)، ثم انتقل إلى **الحلول**.
1. افتح **الحل الافتراضي**.
1. حدد **جديد**.
1. حدد **سير العمل السحابي**، ثم قم بتسميته **تمرين عملي - إرسال إلى التنفيذ (RequestBin)**.
1. حدد نوع المشغّل باعتباره **‬‏‫تشغيل سير عمل يدوياً‬‏‫** ثم أدخل المعلومات التالية:
    - حدد **إضافة إدخال**، وحدد **النص**، ثم قم بإدخال **ProviderActionExecutionEventId** في الحقل الأول.
    - حدد **إضافة إدخال**، وحدد **النص**، ثم قم بإدخال **EntityRecordId** في الحقل الأول.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لكيفية تشغيل خصائص التدفق يدوياً (RequestBin).](../media/manual-trigger-flow-properties-ss.png)](../media/manual-trigger-flow-properties-ss.png#lightbox)

1. إنشاء إجراء تهيئة متغير:
    - في **الاسم**، أدخل **ExecutionResult‎**.
    - في **النوع**، حدد **منطقي**.
    - في **القيمة**، أدخل **صحيح‬**.  
1. إنشاء إجراء تهيئة متغير ثانٍ:
    - في **الاسم**، أدخل **ProcessedSaleOrderLines**.
    - في **النوع**، حدد **صفيف**.
1. إنشاء إجراء تهيئة متغير ثالث:
    - في **الاسم**، أدخل **ProcessedFulfillmentOrderLines**.
    - في **النوع**، حدد **صفيف**.

     > [!div class="mx-imgBorder"]
     > [![لقطة شاشة لإجراءات تهيئة متغير (RequestBin).](../media/variable-initialization-actions-ss.png)](../media/variable-initialization-actions-ss.png#lightbox)

1. أضف نطاق **المحاولة‏‎**.
1. ضمن نطاق **المحاولة**، أضف **تنفيذ إجراء غير مرتبط** كما يلي:
    - **ProviderActionExecutionEventId** - ضمن **المحتوى الديناميكي**، حدد **ProviderActionExecutionEventId**.
    - **PowerAutomateRunId** - حدد التعبير على الشكل التالي: `workflow()['run']?['name']`

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لنطاق المحاولة (RequestBin).](../media/try-scope-ss.png)](../media/try-scope-ss.png#lightbox)

1. أضف إجراء **‏‫الحصول على صف حسب المعرف** وقم بإعداده على النحو التالي:
    - في **اسم الجدول**، أدخل **أوامر التنفيذ**.
    - في **معرف الصف**، حدد **EntityRecordId** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لإجراء الحصول على معرف صف (RequestBin).](../media/get-row-id-action-ss.png)](../media/get-row-id-action-ss.png#lightbox)

1. أضف إجراء **إنشاء أمر تنفيذ** من موصل RequestBin عن طريق تحديد **النص الأساسي** من ضمن **المحتوى الديناميكي** من أجل **النص الأساسي**. 
   
    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لإجراء إنشاء أمر تنفيذ.](../media/create-fulfillment-order-ss.png)](../media/create-fulfillment-order-ss.png#lightbox)

1. أضف إجراء **إدراج صفوف** كما يلي:
    - في **اسم الجدول**، أدخل **منتجات أوامر التنفيذ**.
    - في **استعلام إحضار XML**، أدخل ما يلي: </br>

    ```XML
    <fetch>  
      <entity name="msdyn_fulfillmentorderdetail">  
       <all-attributes />
         <filter>
         <condition attribute="msdyn_fulfillmentid" operator="eq" value="@{triggerBody()['text_1']}"/>
         </filter>
      </entity>  
    </fetch>
    ```

    
    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لإجراء إدراج صفوف.](../media/list-rows-action-ss.png)](../media/list-rows-action-ss.png#lightbox)

1. أضف عنصر تحكم **تطبيق على كل** باستخدام إجراء **إنشاء بنود أمر التنفيذ** من اتصال RequestBin كما يلي:
    - احصل على **القيمة** من خطوة **الحصول على بند أمر التنفيذ** ضمن **المحتوى الديناميكي**. 
    - حدد **الصنف الحالي** ضمن **المحتوى الديناميكي**.

     > [!div class="mx-imgBorder"]
     > [![لقطة شاشة لعنصر تحكم "تطبيق على كل" (Requestbin).](../media/apply-to-each-control-2-ss.png)](../media/apply-to-each-control-2-ss.png#lightbox)

1. ضمن التكرار الحلقي، أضف إجراء **إلحاق بمتغير الصفيف** كما يلي:
    - في **الاسم**، أدخل **ProcessedFulfillmentOrderLines**.
    - في **القيمة**، حدد **معرف بند التنفيذ** ضمن **المحتوى الديناميكي**. 

    > [!div class="mx-imgBorder"]
    > > [![لقطة شاشة لإجراء الإلحاق بالصفيف (تنفيذ).](../media/append-to-array-1-ss.png)](../media/append-to-array-1-ss.png#lightbox)

1. ضمن التكرار الحلقي، أضف إجراء **إلحاق بمتغير صفيف** آخر كما يلي:
    - في **الاسم**، أدخل **ProcessedSalesOrderLines**.
    - في **القيمة**، حدد **معرف سطر المبيعات** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لإجراء الإلحاق بالصفيف (مبيعات).](../media/append-to-array-2-ss.png)](../media/append-to-array-2-ss.png#lightbox)

1. قم بطي نطاق **المحاولة** عن طريق تحديد شريط عنوانه. 
1. حدد **خطوة جديدة** ثم أضف نطاقاً مختلفاً تمت إعادة تسميته إلى **التقاط‏‎**.
1. في النطاق **التقاط**، حدد علامة الحذف (**...**)، وحدد **تكوين التشغيل بعد**، ثم اتبع هذه الخطوات:
    - حدد خانة الاختيار **فشل**.
    - حدد خانة الاختيار **انتهت مهلته‬‏‫**.

     > [!div class="mx-imgBorder"]
     > [![لقطة شاشة لصفحة النطاق "التقاط".](../media/catch-scope-ss.png)](../media/catch-scope-ss.png#lightbox)

1. في صفحة النطاق **التقاط**، حدد **إضافة إجراء**، وأضف الإجراء **تعيين متغير**، ثم غيّر اسمه إلى **تعيين نتيجة التنفيذ إلى فاشلة**.
1. قم بإعداد الخصائص على النحو التالي:
    - في **الاسم**، أدخل **ExecutionResult‎**.
    - في **القيمة**، أدخل **خطأ**.

     > [!div class="mx-imgBorder"]
     > [![لقطة شاشة لإجراء "تعيين متغير".](../media/set-variable-ss.png)](../media/set-variable-ss.png#lightbox)

1. حدد **‎خطوة جديدة**، ثم أضف نطاقاً آخر تم تغيير اسمه إلى **أخيراً**.
1. في النطاق **أخيراً**، حدد علامة الحذف (**...**)، وحدد **تكوين التشغيل بعد**، ثم اتبع هذه الخطوات:
    - حدد خانة الاختيار **هو ناجح**.
    - حدد خانة الاختيار **انتهت مهلته‬‏‫**.
    - حدد خانة الاختيار **تم تخطيه**.
    - حدد خانة الاختيار **انتهت مهلته‬‏‫**.

     > [!div class="mx-imgBorder"]
     > [![لقطة شاشة لصفحة النطاق "أخيراً".](../media/finally-scope-ss.png)](../media/finally-scope-ss.png#lightbox)

1. في النطاق **أخيراً**، أضف خطوة **شرط**، ثم قارن المتغير **ExecutionResult** مع **صحيح** كما يلي:
    - في الحقل الأول، حدد المتغير **ExecutionResult‎**.
    - في الحقل الثاني، حدد **يساوي**.
    - في الحقل الثالث، حدد **صحيح**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لخطوة "الشرط".](../media/condition-step-ss.png)](../media/condition-step-ss.png#lightbox)

1. في الفرع **إذا كانت الإجابة نعم**، أضف إجراء **تشغيل سير عمل تابع** وغيّر اسمه إلى **تنفيذ أحداث الأعمال لبنود أمر التنفيذ التي تمت معالجتها**.
1. قم بإعداد الخصائص على النحو التالي:
    - في **سير العمل التابع**، أدخل **تنفيذ حدث أعمال**.
    - في **BusinessEventDefinitionId**، أدخل **063d85c8-60a4-eb11-9443-000d3a313675**.
    - في **EntityRecordId**، حدد التعبير التالي: `string(variables('ProcessedFulfillmentOrderLines'))`

1. في الفرع **إذا كانت الإجابة نعم**، أضف إجراء **تشغيل سير عمل تابع** آخر وغيّر اسمه إلى **تنفيذ الأحداث المجمّعة لأمر المبيعات**.
1. قم بإعداد الخصائص على النحو التالي:
   - في **LineBusinessEventDefinitionId**، أدخل **ccf64002-61a4-eb11-9443-000d3a313675**.
   - في **LineRecordId**، حدد التعبير التالي: `string(variables('ProcessedSalesOrderLines'))`.
   - في **OrderBusinessEventDefinitionId**، أدخل **48688716-61a4-eb11-9443-000d3a313675**.

    
    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لإجراء تشغيل سير عمل تابع‬ (الأحداث المجمّعة).](../media/run-child-flow-action-2-ss.png)](../media/run-child-flow-action-2-ss.png#lightbox)

1. قم بطي خطوة الشرط.  
1. أضف **تنفيذ إجراء غير مرتبط** كما يلي:
    - في **اسم الإجراء**، أدخل **msdyn_CompleteProviderActionExecution**.
    - في **ExecutionResult**، حدد المتغير **ExecutionResult** ضمن **المحتوى الديناميكي**.
    - في **ProviderActionExecutionEventId**، حدد **ProviderActionExecutionEventId** ضمن **المحتوى الديناميكي**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لتنفيذ إجراء غير مرتبط.](../media/perform-unbound-action-ss.png)](../media/perform-unbound-action-ss.png#lightbox)

1. حدد **حفظ**.

## <a name="add-a-provider-definition-logic-definition-to-the-provider-definition-requestbin"></a>إضافة تعريف منطق تعريف الموفر إلى تعريف الموفر (RequestBin)

لإضافة تعريف منطق تعريف الموفر إلى تعريف موفر RequestBin، اتبع الخطوات التالية:

1. انتقل إلى **الموفرون‬ > الكتالوج**.
1. حدد **LabFulfillmentProvider** الذي تم إنشاؤه مؤخراً.
1. حدد **تحرير‬** من شريط القوائم. 
1. حدد علامة التبويب **تعريفات المنطق**.
1. حدد **+ تعريف منطق تعريف موفر IOM الجديد**.
1. في **اسم العرض**، أدخل **تمرين عملي - إرسال إلى التنفيذ (RequestBin)**.
1. في **الاسم المنطقي**، أدخل **msdyn_LabSentToFulfillmentRequestBin**.
1. في **تعريف الموفر**، أدخل **LabFulfillmentProvider**.
1. في **نوع المنطق**، أدخل **إجراء الموفر**.
1. في **اسم سير العمل**، أدخل **تمرين عملي - إرسال إلى التنفيذ (RequestBin)**.
1. في **دقائق المهلة**، أدخل **2**.
1. في **‫الحد الأقصى لعدد عمليات إعادة المحاولة‬**، أدخل **3**.
1. في **الوصف‏‎‬**، أدخل **تمرين عملي - إرسال إلى التنفيذ (RequestBin)**.
1. بالنسبة إلى **نوع الإجراء**، أدخل **الإرسال إلى التنفيذ**.
1. حدد **حفظ**. ستؤدي هذه الخطوات إلى إنشاء تمثيل JSON لسير العمل السحابي لمعالج الرسائل وتعبئة حقل **بيانات العميل**.
1. حدد **حفظ وإغلاق**.
1. حدد **الاتصالات**. يجب أن تكون تعريفات مراجع اتصال **Microsoft Dataverse** و **Outlook.com** و **RequestBin** مدرجة.

## <a name="add-a-provider-definition-parameter-to-the-provider-definition"></a>إضافة معلمة تعريف الموفر إلى تعريف الموفر

لإضافة معلمة تعريف موفر إلى تعريف الموفر، اتبع هذه الخطوات:

1. حدد **المعلمات**. 
1. حدد **+ معلمة تعريف موفر IOM جديد**.
1. في **اسم العرض**، أدخل **LabOutboundFulfillmentEmail**.
1. في **نوع البيانات**، أدخل **نص**.
1. في **تعريف الموفر**، أدخل **LabFulfillmentProvider**.
1. في **المفتاح**، أدخل **LabOutboundFulfillmentEmail**.
1. في **الاسم المنطقي**، أدخل **msdyn_LabOutboundFulfillmentEmail**.
1. في **مطلوب‬**، أدخل **نعم**.
1. حدد **حفظ وإغلاق**.

## <a name="add-a-provider-definition-logic-definition-to-the-labproviders-solution-requestbin"></a>إضافة تعريف منطق تعريف الموفر إلى حل LabProviders‏ (RequestBin)

لإضافة تعريف منطق تعريف الموفر إلى حل RequestBin LabProviders، اتبع الخطوات التالية:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com) وانتقل إلى الحل **LabProviders** الذي تم إنشاؤه مؤخراً.
1. حدد **إضافة موجود > تعريف منطق تعريف موفر IOM**.
1. حدد **تمرين عملي - إرسال إلى التنفيذ (RequestBin)** ثم حدد **إضافة‏‎‏‎** لإضافته إلى الحل. 

## <a name="add-a-provider-definition-connection-reference-to-the-labproviders-solution"></a>إضافة مرجع اتصال تعريف الموفر إلى حل LabProviders

لإضافة مرجع اتصال تعريف الموفر إلى حل LabProviders، اتبع هذه الخطوات:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com) وانتقل إلى الحل **LabProviders** الذي تم إنشاؤه مؤخراً.
1. حدد **إضافة موجود > مرجع اتصال تعريف موفر IOM**.
1. حدد **RequestBin‎**، ثم حدد **إضافة** لإضافته إلى الحل.

## <a name="add-a-provider-definition-parameter-to-the-labproviders-solution"></a>إضافة معلمة تعريف الموفر إلى حل LabProviders

لإضافة معلمة تعريف موفر إلى حل LabProviders، اتبع هذه الخطوات:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com) وانتقل إلى الحل **LabProviders** الذي تم إنشاؤه مؤخراً.
1. حدد **إضافة موجود > معلمة تعريف موفر IOM**.
1. حدد **LabOutboundFulfillmentEmail**، ثم حدد **إضافة** لإضافته إلى الحل.
