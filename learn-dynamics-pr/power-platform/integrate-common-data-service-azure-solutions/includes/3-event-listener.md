---
ms.openlocfilehash: 03a5aa4e8df5e6b44e46804066602d5e871b95ee
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7457562"
---
## <a name="types-of-supported-service-bus-contracts"></a>أنواع عقود "ناقل الخدمة" المدعومة  

يدعم Microsoft Dataverse مجموعة متنوعة من الأساليب لاستخدام الرسائل الموجودة في قائمة انتظار ناقل خدمة المراسلة في Azure: قائمة الانتظار أو العقود أحادية الاتجاه أو العقود ثنائية الاتجاه أو REST. إذا كنت تستخدم أسلوبي العقود ثنائية الاتجاه وREST، فيمكنك إرجاع مجموعة من المعلومات مرة أخرى إلى Dataverse.

### <a name="queue"></a>قائمة الانتظار

وحدات إصغاء قائمة الانتظار غير مطلوبة لهذا النوع من قوائم الانتظار. ويمكنك استخدام الرسائل الموجودة في قائمة الانتظار في قراءة "تحديد القدرة" أو "ليست لتحديد القدرة". وستقوم قراءة تحديد القدرة بقراءة الرسالة من قائمة الانتظار وإزالتها، بينما لا تقوم القراءة التي ليست لتحديد القدرة بإزالة الرسالة من قائمة الانتظار. وتفيد هذه الطريقة لسيناريوهات "الإرسال والنسيان" التي ليس من المهم فيها تلقي الرسالة في وقت معين.

### <a name="topic"></a>الموضوع

تُعد وحدات إصغاء الموضوع مماثلة لوحدات إصغاء قائمة الانتظار، باستثناء أنه يمكن لوحدة إصغاء واحدة أو أكثر الاشتراك لتلقي رسائل لموضوع معين. ويكون هذا النوع مفيدًا في حالة الحاجة إلى عدة عملاء لرسالة معينة.

### <a name="one-way"></a>العقود أحادية الاتجاه

تتطلب العقود أحادية الاتجاه توفُّر وحدة إصغاء نشطة للحدث من أجل استخدام رسالة يتم ترحيلها إلى قائمة الانتظار "ناقل الخدمة". وفي حالة عدم توفُّر أي وحدة إصغاء نشطة، ستفشل عملية الترحيل. وإذا فشل الترحيل، سيقوم Dataverse بإعادة محاولة ترحيل الرسالة في فترات زمنية أكبر بأضعاف كثيرة حتى يتم إلغاء وظيفة النظام غير المتزامنة في النهاية. وفي هذه الحالة، سيتم تعيين حالة "وظيفة النظام" الخاصة بهذا الحدث إلى **فشلت**.

### <a name="two-way"></a>العقود ثنائية الاتجاه

تتشابه العقود ثنائية الاتجاه مع العقود أحادية الاتجاه، باستثناء أنها توفر أيضًا القدرة على إرجاع قيمة سلسلة من وحدة الإصغاء. إذا كنت قد سجلت مكونًا إضافيًا مخصصًا متوافقًا مع Azure لترحيل رسالتك، فإنه يمكنك استخدام هذه البيانات التي تم إرجاعها في المكون الإضافي. وقد يتمثل الاستخدام الشائع لهذا السيناريو فيما إذا كنت ترغب في استرداد معرف السجل الذي تم إنشاؤه في نظام خارجي كجزء من عملية وحدة الإصغاء للحفاظ عليه في بيئة Dataverse لديك.

### <a name="rest"></a>REST

تتشابه عقود REST مع العقود ثنائية الاتجاه باستثناء أنها تُعرض على نقطة نهاية REST.

## <a name="write-a-queue-listener"></a>كتابة وحدة إصغاء قائمة الانتظار

في التمرين السابق، قمت بتسجيل "نقطة نهاية خدمة" تقوم بنشر الرسائل إلى "نقطة نهاية ناقل خدمة" كلما تم تحديث بيانات الحساب في بيئة Dataverse الخاصة بك. ويوضح هذا التمرين الآن كيفية استخدام هذه الرسائل.

1.  إنشاء تطبيق وحدة التحكم رقم "ج" في Visual Studio الذي يستهدف إطار .NET 4.6.2 أو إصدارًا أعلى.

3.  أضف حزم NuGet الآتية:

    -  Azure.Messaging.ServiceBus

    -  Microsoft.CrmSdk.CoreAssemblies

4.  في الطريقة الرئيسية للتطبيق، الصق الكود الآتي. استبدل عنوان URL لنقطة النهاية بعنوان URL لنقطة النهاية الخاصة بمساحة اسم ناقل خدمة Azure لديك واسم قائمة الانتظار إذا كان مختلفًا:

    ```csharp
    string connectionString =@"[ENDPOINT URL]";
    string queueName = "mslearnsamplequeue";
    QueueClient queueClient = QueueClient.CreateFromConnectionString(connectionString, queueName, ReceiveMode.PeekLock);
    ```

5.  لاستخدام الرسالة، استخدم الطريقة "OnMessage"، والتي توفر إمكانية معالجة رسالة قائمة انتظار ناقل الخدمة في مضخة رسائل تستند إلى الحدث. وفي هذا التمرين، ستستخدم طرق "أداة التسلسل" التي توفرها حزمة Microsoft.Xrm.Sdk بحيث يمكنك إجراء تسلسل للرسالة الواردة في نوع البيانات RemoteExecutionContext Dataverse‎. واستنادًا إلى نوع الرسالة التي تم تسجيلها، تحتاج إلى إجراء تسلسل بناءً على تنسيق الرسائل المطابق (‎.NETBinary أو JSON أو XML).

    ```csharp
    queueClient.OnMessage(message =>
                {
                    //get RemoteExecutionContext based on Message Format
                    RemoteExecutionContext context = null;
    
                    if (message.ContentType == "application/msbin1") //.NETBinary Message Format
                    {
                        context = message.GetBody<RemoteExecutionContext>();
                    }
                    else if (message.ContentType == "application/json") //JSON Message Format
                    {
                        context = message.GetBody<RemoteExecutionContext>(
                                          new DataContractJsonSerializer(typeof(RemoteExecutionContext)));
                    }
                    else if (message.ContentType == "application/xml") //XML Message Format
                    {
                        context = message.GetBody<RemoteExecutionContext>(
                            new DataContractSerializer(typeof(RemoteExecutionContext)));
                    }
                    try
                    {
    //serialize the entire context leveraging the SerializeContext extension method
                        Console.WriteLine(context.SerializeContext());
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine(ex.ToString());
                    }
                });
    ```

6.  وأخيرًا، سنقوم بإضافة Console.ReadLine()‎ إلى طريقتنا الرئيسية للسماح بمعالجة العديد من الرسائل.  ملحوظة: هذه ليست طريقة قابلة للتحجيم للتعامل مع معالجة الحدث، ولكنها تكفي لأغراض التمرين الخاصة بنا.  وستحتاج إلى الحصول على حل أكثر قابلية للتحجيم تستضيفه في وظيفة Azure Durable أو خدمة أخرى حسب تفضيلاتك.  

    ```csharp
    Console.ReadLine();
    ```

7.  اضغط على F5 لتشغيل التطبيق.  في حالة وجود رسائل بالفعل في قائمة الانتظار الخاصة بك من التمرين السابق، تجب معالجتها وعرض محتويات رسائلها في شاشة وحدة التحكم.  وإذا لم توجد رسائل، فيمكنك استدعاء تحديث من خلال إجراء تحديث لأحد الحسابات في بيئة Dataverse.

