---
ms.openlocfilehash: 75f775bb5466aabac522615fb563ef79361a2c61
ms.sourcegitcommit: b214fdb68f932da234d60906b9fe7a1d294c0af0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2022
ms.locfileid: "9515226"
---
يمكن دمج كلٍّ من Dynamics 365 Field Service وDynamics 365 Supply Chain Management (وحدة إدارة الأصول) في Dynamics 365 Guides

## <a name="integrate-dynamics-365-field-service-with-dynamics-365-guides"></a>دمج Dynamics 365 Field Service مع Dynamics 365 Guides
يعمل تكامل Dynamics 365 Field Service على تمكين عملاء Field Service من إرفاق الأدلة بمهام Field Service. عند تعيين أوامر العمل للفنيين، يمكن للفنيين استخدام علامة التبويب **Field Service** المخصصة في تطبيق Dynamics 365 Guides HoloLens لتشغيل الدليل المخصص والقيام بعملهم.

> [!NOTE]
> >لإرفاق الأدلة بمهام الخدمة في Dynamics 365 Field Service، يلزمك الحصول على مثيل Dynamics 365 Customer Engagement ‏(CRM) مع إصدار Dynamics 365 Field Service رقم 8.6.0.183 أو إصدار لاحق. كما تحتاج إلى التحديث إلى حل Dynamics 365 Guides الإصدار 104.1907.0.33 أو إصدار لاحق وكمبيوتر Dynamics 365 Guides وإصدارات التطبيق HoloLens أرقام 104.1907.19001.

### <a name="enable-your-technicians-to-use-dynamics-365-guides-for-work-orders"></a>تمكين الفنيين من استخدام Dynamics 365 Guides لأوامر العمل

1.  أنشئ دليلاً باستخدام كمبيوتر Dynamics 365 Guides وتطبيقات HoloLens. للحصول على معلومات حول إنشاء دليل، راجع [دليل المؤلف في Dynamics 365 Guides](/training/modules/author-guides/?azure-portal=true).
    
1.  أنشئ أمر عمل Field Service وأرفق مهمة خدمة به.

    1.  لإنشاء أمر عمل جديد في Dynamics 365 Field Service، حدد **أوامر العمل** في التنقل الأيسر، ثم حدد **أمر العمل الجديد**.

    1.  في طريقة عرض **مهام الخدمة**، حدد **الأوامر الإضافية** (**…**)، ثم حدد **إضافة مهمة خدمة أمر عمل جديدة**.
    
        [ ![لقطة شاشة لعرض مهام الخدمة مع تحديد إضافة مهمة خدمة أمر العمل الجديدة.](../media/add-new-task-ssm.png) ](../media/add-new-task-ssm.png#lightbox) 

    1.  في طريقة عرض **مهمة خدمة أمر العمل الجديدة**، حدد نوع المهمة، وقدم وصفاً اختيارياً، ثم حدد دليلاً للإقران بمهمة الخدمة. حدد **حفظ** عند الانتهاء.

1.  تعيين أمر العمل إلى مورد (الفني). للقيام بذلك، تحتاج إلى إنشاء حجز للمورد:

    1.  في طريقة عرض **أمر العمل**، قم بالتمرير لأسفل إلى علامة التبويب **حجوزات**، وحدد **الأوامر الإضافية (...)**، ثم حدد **إضافة مورد قابل للحجز جديد**.

    1.  في طريقة عرض **حجز مورد قابل للحجز جديد**، حدد مهمة الخدمة في الوقت المناسب للفني، ثم حدد فني مناسب كمورد.
 
        [![لقطة شاشة لطريقة عرض "حجز مورد جديد قابل للحجز".](../media/schedule-select-resource-ssm.png) ](../media/schedule-select-resource-ssm.png#lightbox)

1.  اطلب من الفني الخاص بك تشغيل تطبيق Dynamics 365 Guides على HoloLens. بعد تسجيل الدخول، سيرى الفني علامة التبويب **Field Service**. تعرض علامة التبويب الدليل (وأي أدلة أخرى مخصصة لهم) جنباً إلى جنب مع وصف موجز للحجز ومتى تمت جدولة هذا الطلب.

![لقطة شاشة لصفحة تحديد الدليل مع عرض علامة التبويب Field Service.](../media/select-guide-3-ss.png)  

ضع في اعتبارك النقاط التالية:

- يعرض تطبيق Dynamics 365 Guides HoloLens أوامر العمل المجدولة لليوم الحالي والأيام الثمانية التالية.
- تستمر أوامر العمل في الظهور على HoloLens حتى يتم تمييزها على أنها **مكتملة** أو في Field Service أو تم تعيينها لشخص آخر.

## <a name="integrate-dynamics-365-supply-chain-management-asset-management-module-with-dynamics-365-guides"></a>دمج Dynamics 365 Supply Chain Management (وحدة إدارة الأصول) في Dynamics 365 Guides

يمكنك أيضاً دمج وحدة إدارة الأصول في Dynamics 365 Supply Chain Management مع Dynamics 365 Guides للاستفادة من أدلة الواقع المختلط في عمليات سير عمل الصيانة والخدمة اليومية. 

إذا كان هناك دليل مرتبط بأمر عمل إدارة الأصول، فعندما يفتح العامل قائمة فحص الصيانة لأمر العمل في تطبيق التمويل والعمليات ‏(Dynamics 365) للأجهزة المحمولة (1)، تُظهر تفاصيل البند أن الدليل متوفر (2). يمكن للعامل بعد ذلك العثور على الدليل وفتحه في تطبيق Dynamics 365 Guides HoloLens ‏(3).

[ ![لقطات من قائمة مراجعة الصيانة وتفاصيل الخط في الدليل والدليل في تطبيق HoloLens.](../media/asset-management-integration-ssm.jpg)](../media/asset-management-integration-ssm.jpg#lightbox)

لمعرفه المزيد حول تكامل إدارة الأصول مع Dynamics 365 Guides، انتقل إلى [دمج Dynamics 365 Supply Chain Management (إدارة الأصول) مع Dynamics 365 Guides](/dynamics365/supply-chain/asset-management/asset-management-guides-integration/?azure-portal=true).
