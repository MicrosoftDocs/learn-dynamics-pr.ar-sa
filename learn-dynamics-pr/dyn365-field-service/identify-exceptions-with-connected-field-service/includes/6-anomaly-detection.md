---
ms.openlocfilehash: e2532fd9fd7bd40b16140947f8c1330a77a7598520518578344ce1b4d0b0c175
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7434026"
---
في هذا التدريب العملي، ستقوم بتعديل المنطق المستخدم لإنشاء تنبيه IoT ليكون أكثر ديناميكية باستخدام ميزة معاينة اكتشاف الحالات الخارجة عن المألوف في Azure Stream Analytics.  حالياً، يتم إنشاء تنبيه IoT عندما تصل درجة الحرارة من الجهاز إلى حد الترميز الثابت.  باستخدام إمكانات الكشف الخارج عن المألوف، ستقوم بتعديل استعلامات وظيفة الدفق للكشف عن كلٍ من اتجاه العلوي والسفلي في درجة الحرارة.  سيكون هذا النوع من الكشف مثالياً في المكان الذي تريد فيه الإخطار المبكر عن التغيير من الحالة المتوقعة ولكن ليس لديه قيمة مضمنة بترميز ثابت والتي تشير إلى الوقت الذي تصبح فيه مشكلة.

## <a name="exercise-1-building-new-query"></a>التدريب 1: إنشاء استعلام جديد 

في هذا التدريب، ستقوم بإنشاء استعلام جديد لاستبدال استعلام مهمة Azure Stream Analytics الموجودة. ستقوم ببناء هذا الاستعلام الجديد بشكل تدريجي، حتى يمكنك مشاهدة ما تقوم به الأجزاء. تم تصميم هذا المعمل للعمل مع جهازك الفعلي، إذا لم يكن لديك جهاز فعلي، يمكنك تغيير الاستعلام لاستخدام الحقول من جهاز المحاكاة.

### <a name="task-1-add-anomaly-data-collection-to-azure"></a>المهمة 1: إضافة تجميع بيانات خارج عن المألوف إلى Azure

لحفظ نتائج التفاصيل التي تم إنشاؤها من ‏‫اكتشاف الخارج عن المألوف‬، فإننا نحتاج إلى إنشاء مجموعة أخرى في Azure Cosmos DB التي استخدمناها في وحدة التدريب العملي السابق. نقوم بذلك لتسهيل رؤية القيم التي تم إنشاؤها من عامل كشف الخارج هن المألوف.

1.  انتقل إلى مدخل **Azure** وحدد مجموعات الموارد، ثم افتح مجموعة الموارد التي قمت بإنشائها عند نشر Connected Field Service.

1.  افتح **Azure Cosmo DB** التي قمت بإنشائها.

1.  حدد **مستكشف البيانات** وانقر فوق ... زر من قاعدة بيانات قياس تتبع الاستخدام وحدد **حاوية جديدة.**

1.  أدخِل **AnomalyData** لـ **معرف الحاوية** وأدخِل **معرف الجهاز** إلى **مفتاح التقسيم** ثم انقر فوق **موافق**.

### <a name="task-2-add-new-output"></a>المهمة 2: إضافة إخراج جديد

في هذه المهمة، ستقوم بإضافة إخراج جديد لمجموعة AnomalyData.

1.  قم بإغلاق الريشة الخاصة بـ **Azure Cosmos DB** .

1.  حدد موقع **وظيفة Stream Analytics**.

1.  انقر فوق **إيقاف**. يجب إيقاف مهمة Stream Analytics قبل أن تتمكن من تغيير الاستعلام والمدخلات/المخرجات.

1.  انقر فوق **نعم**.

1.  بعد توقف الوظيفة، حدد **إخراج** انقر فوق **+ إضافة** وحدد **Cosmo DB**.

1.  أدخِل **AnomalyDB** للحصول على **مخرج الاسم المستعار** ثم قم بتحديد **الاشتراك** وحدد **Cosmo DB** الذي قمت بإنشائه **وقاعدة البيانات** التي قمت بإنشائها وقم بإدخال **AnomalyData** لـ **اسم الحاوية** ثم انقر فوق **حفظ**.

يتكون كل تدريب من سيناريو وأهداف تعليمية، ويصف السيناريو الغرض من التدريبات، بينما يتم سرد الأهداف ولها نقاط.

### <a name="task-3-prepare-and-build-the-new-query"></a>المهمة 3: إعداد الاستعلام الجديد وإنشاءه

1.  حدد **استعلام**.

1.  قم بنسخ الاستعلام الموجود وحفظه في حالة رغبتك في الرجوع إليه لاحقاً.

1.  قم بإلغاء تحديد الاستعلام الموجود، سنقوم بإنشاء حقل جديد خطو بخطوة.

1.  ألصق القصاصة الموجودة أدناه في محرر الاستعلام.

    ```csharp
    WITH AlertData AS 
    (
    
    SELECT
        IoTHub.ConnectionDeviceId as Device,
        System.Timestamp as tumblingWindowEnd,
           AVG(Stream.temp) as TempC,
           AVG(((Stream.temp*1.8)+32)) as TempF,
           AVG(Stream.accelerometerX) as accelerometerX,
           AVG(Stream.accelerometerY) as accelerometerY,
           AVG(Stream.accelerometerZ) as accelerometerZ
        
    FROM
        IoTStream Stream TIMESTAMP BY IoTHub.EnqueuedTime
    GROUP BY IoTHub.ConnectionDeviceId, TumblingWindow(second, 10)
    ),
    ```

    ![لقطة شاشة للقصاصة البرمجية التي تم لصقها إلى محرر الاستعلام.](../media/snippet-querry-editor.png)

    > [!NOTE]
    > سيؤدي ذلك إلى معالجة البيانات الأولية خارج الجهاز والمجموعة في نافذة متقلبة كل 10 ثواني التي سيتم تقييمها لحالات الكشف عن العيوب. نختار استخدام متوسط البيانات الموجودة في النافذة، ويمكنك استخدام أي تجميع تم إجراؤه يتناسب مع الخاص بك.

1.  قم بلصق ما يلي مباشرة بعد الاستعلام السابق، سيؤدي ذلك إلى استخدام البيانات من الاستعلام الأخير وزيادتها.

    ```csharp
    FillInMissingValuesStep AS
        (
              SELECT                
                    System.Timestamp AS hoppingWindowEnd,
                    TopOne() OVER (ORDER BY tumblingWindowEnd DESC) AS lastEvent
             FROM AlertData
             GROUP BY HOPPINGWINDOW(second, 300, 5)
    
        ),
    ```

    > [!NOTE]
    > للمساعدة في ضمان توحيد البيانات بحيث لا تتوفر لدينا أي فجوات، حددنا تعبئة الفجوات عن طريق الحصول على آخر حدث في كل نافذة من إطارات القفزات.

1.  قم بلصق الخطوة التالية لإجراء تسجيل الخارج عن المألوف بالفعل.

    ```csharp
    AnomalyDetectionStep AS (
    SELECT
         lastevent.Device as lastEventDevice,
         hoppingWindowEnd,
                    lastEvent.tumblingWindowEnd as lastTumblingWindowEnd,
                    lastEvent.TempC as lastEventTempC,
                    lastEvent.TempF as lastEventTempF,
                    lastEvent.accelerometerY as lastEventaccelerometerY,
                    lastEvent.accelerometerX as lastEventaccelerometerX,
                    lastEvent.accelerometerZ as lastEventaccelerometerZ,                
                    system.timestamp as anomalyDetectionStepTimestamp,
         ANOMALYDETECTION(lastEvent.TempC) OVER (PARTITION BY lastevent.Device LIMIT DURATION(mi, 2)) as  scores
    FROM FillInMissingValuesStep
    ),
    ```

    > [!NOTE]
    > يستخدم هذا الاستعلام عامل تشغيل ANOMALYDETECTION في قيمة TempC.  يتم القيام بذلك على كل جهاز ويتم قياسه لمدة دقيقتين.  يتسبب ذلك في جعل تدريب كشف عن الخارج عن المألوف بالأجهزة خاصاً وقد يستوعب الفروق في درجات الحرارة الأساسية في كل موقع من مواقع الأجهزة. المخرج من هذه النتائج تتم إضافته إلى المخرجات للتقييم في الاستعلام التالي.

1.  قم بلصق ما يلي في الاستعلام الذي تقوم بإنشائه.

    ```csharp
    AnomalyDetectionFilter AS (
    SELECT lastEventDevice as DeviceId,
        CAST(GetRecordPropertyValue(scores, 'BiLevelChangeScore') as float) as BiLevelChangeScore,
        CAST(GetRecordPropertyValue(scores, 'SlowPosTrendScore') as float) as SlowPosTrendScore,
        CAST(GetRecordPropertyValue(scores, 'SlowNegTrendScore') as float) as SlowNegTrendScore,
        lastEventTempC as Reading,
        'Tempature' as ReadingType,
        'Trend Up ' as Threshold,
        'EventToken' as EventToken,
        lastTumblingWindowEnd as time
    
    FROM AnomalyDetectionStep 
    WHERE 
           CAST(GetRecordPropertyValue(scores, 'SlowPosTrendScore') as float) >= 10      
    union
    SELECT lastEventDevice as DeviceId,
        CAST(GetRecordPropertyValue(scores, 'BiLevelChangeScore') as float) as BiLevelChangeScore,
        CAST(GetRecordPropertyValue(scores, 'SlowPosTrendScore') as float) as SlowPosTrendScore,
        CAST(GetRecordPropertyValue(scores, 'SlowNegTrendScore') as float) as SlowNegTrendScore,
        lastEventTempC as Reading,
        'Tempature' as ReadingType,
        'Trend Down ' as Threshold,
        'EventToken' as EventToken,
        lastTumblingWindowEnd as time
    
    FROM AnomalyDetectionStep 
    WHERE       
          CAST(GetRecordPropertyValue(scores, 'SlowNegTrendScore') as float) >= 10
    )
    ```

    > [!NOTE]
    > يؤدي ذلك إلى تقييم كل من SlowPosTrendScore وSlowNegTrendScore.  القيمة التي تقوم بفحصها هي الحساسية.  قد يكون من الممكن البدء بالمخاطرة عند 3.25، ولكننا نختار أن تنتظر حتى يصبح الأمر أكثر أهمية عند 10.  وفي الحقيقة، ستقوم بضبط ذلك للسيناريو الخاص بك.  لاحظ أيضاً لن لدينا حقول محددة لـ Reading، وReadingType، وThreshold، وEventToken.  وهذه هي البيانات التي يتوقعها تطبيق Logic لأي رسالة يتم إخراجها إلى تنبيهات AlertsQueue الذي ستقوم به في الاستعلام التالي.  في حالة عدم الاحتفاظ بهذه الحقول، يجب تعديل تطبيق Logic App بحيث لا يتوقع وجوده.

1.  قم بلصق القصاصة البرمجية التي تلي القصاصة الأخيرة.

    ```tsql
    SELECT *
    INTO AlertsQueue
    FROM AnomalyDetectionFilter data
    WHERE LAG(data.DeviceID) OVER (PARTITION BY data.DeviceId, CAST(data.Reading as bigint), data.ReadingType LIMIT DURATION(minute, 1)) IS NULL
    ```
    > [!NOTE]
    > وهذا يقوم بالإدراج الفعلي في تنبيهات AlertsQueue الذي سيتم انتقاؤها بواسطة تطبيق Logic App لإنشاء سجل تنبيه IoT.  لاحظ أننا نحتفظ بعامل LAG في المكان الذي يتم فيه تقييد عدد المرات التي نضع فيها الرسائل في قائمة الانتظار فقط عندما يكون لدى نفس الجهاز لدرجات حرارة مستديرة بيانات جديدة في غضون دقيقة.

1.  للتأكد من أننا قمنا بتسجيل نفس بيانات التفصيل من الجهاز، قم بإضافة الاستعلام التالي مرة أخرى.

    ```tsql
    SELECT 
    IoTHub.ConnectionDeviceId as DeviceID, humidity, temp, pressure, magnetometerX, magnetometerY, magnetometerZ, accelerometerX, accelerometerY, accelerometerZ, gyroscopeX, gyroscopeY, gyroscopeZ
    Into CosmosDB
    FROM IoTStream TIMESTAMP BY IoTHub.EnqueuedTime
    ```

10. قم بإضافة ما يلي. سيؤدي ذلك إلى حفظ النتائج من عامل كشف الخارج عن المألوف، بحيث يمكنك بسهولة رؤية البيانات عبر مستكشف بيانات Azure Cosmos DB.

    ```tsql
    SELECT 
    lasteventdevice as DeviceID, hoppingwindowend, lasteventtempc, lasteventtempf, lasteventaccelerometery, lasteventaccelerometerx, lasteventaccelerometerz, anomalydetectionsteptimestamp, scores
    Into AnomalyDB
    FROM AnomalyDetectionStep
    ```

1. احفظ **الاستعلام**.

1. انقر فوق **نعم**.

1. حدد علامة التبويب **نظرة عامة** وانقر فوق **البدء**.

1. حدد **الآن** وانقر فوق **البدء** مرة أخرى.

1. تأكد من نجاح المهمة.

## <a name="exercise-2-testing-the-query"></a>تدريب 2: اختبار الاستعلام 

في هذا التدريب، ستحاول التسبب في تغيير درجة الحرارة الموجودة على الجهاز المادي لاختبار كشف الخارج عن المألوف.

يتكون كل تدريب من سيناريو وأهداف تعليمية، ويصف السيناريو الغرض من التدريبات، بينما يتم سرد الأهداف ولها نقاط.

### <a name="task-1-test-the-query"></a>المهمة 1: اختبار الاستعلام

والآن هو جزء التحدي، أنت بحاجة إلى شيء لتغيير درجة الحرارة التي يقرأها الجهاز ببطء.  تعمل أكياس الثلج بشكل جيد، مثلها مثل علب الهواء المضغوط.  قد يعمل أيضاً مجفف الشعر أو مدفئ اليد.  تأكد فقط من حماية جهازك حتى لا\'يبتل أو يؤدي ذلك إلى إتلافه.

1.  استخدام إحدى الأدوات المذكورة لتغيير درجة حرارة جهازك.

1.  أغلق ريش **Stream Analytics**.

1.  قم بفتح Azure Cosmos DB.

1.  حدد **مستكشف البيانات** وقم بتوسيع **AnomalyData** وحدد **العناصر**.

1.  يجب أن تحصل على قائمة بالتنبيهات. انقر فوق أحد التنبيهات.

1.  يجب أن تتوفر لديك بيانات المستشعر من جهازك.

    ![لقطة شاشة لمعلومات المستشعر من جهازك.](../media/sensor-information-from-device.png)

1.  انتقل إلى [Power Apps](https://make.powerapps.com/?azure-portal=true) وتأكد من أنك في البيئة الصحيحة.

1.  حدد **التطبيقات**، وانقر لفتح تطبيق **Connected Field Service**.

1.  حدد **تنبيهات IoT**.

1. افتح أحد التنبيهات.

1. انتقل إلى قسم **بيانات التنبيه** وسترى معلومات المستشعر من جهازك.

    ![لقطة شاشة لقسم بيانات التنبيه مع معلومات المستشعر من الجهاز.](../media/alert-data-device-sensor-information.png)
