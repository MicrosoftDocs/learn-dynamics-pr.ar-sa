---
ms.openlocfilehash: bb74de10c8be576347eafa32786da0c308e5060f
ms.sourcegitcommit: bfcf3cb276d50978eba5dd4b8268a26abfd9783a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/17/2021
ms.locfileid: "7436394"
---
تم اعتماد القدرة على إنشاء بطاقة معلومات لا تحتوي على أي إجراءات/أزرار وهي متاحة حاليًا في المعاينة.

تمت الإضافة إلى عملية **إنشاء بطاقة للمساعد V3 (معاينة)**.

> [!div class="mx-imgBorder"]
> [![Dynamics 365 Sales Insights يظهر إجراء إنشاء بطاقة للمساعد V3 في علامة تبويب "الإجراءات".](../media/tutorial-9-create-card-assistant-ss.png)](../media/tutorial-9-create-card-assistant-ss.png#lightbox)

## <a name="step-1-create-a-trigger-to-start-the-flow"></a>الخطوة 1: إنشاء مشغل لبدء التدفق

قم بتعيين مشغل يعمل كل صباح في 8 صباحًا.

1.  في البحث، أدخل **تكرار**. من نتائج البحث، ضمن الخيار المشغلات، حدد **تكرار**.

    > [!div class="mx-imgBorder"]
    > [![نتائج البحث عن التكرارات تعرض جدول التكرارات في علامة تبويب "مشغلات".](../media/tutorial-9-select-recurrence-ss.png)](../media/tutorial-9-select-recurrence-ss.png#lightbox)

1.  ستري المشغل أدناه. أدخل **الفاصل الزمني** كـ **1** وحدد **التكرار** كـ **يوم**.  يضمن ذلك تشغيل المشغل مرة واحدة في اليوم.

    يمكن تعيين الأعمدة الأخرى وفقًا لمتطلباتك. في هذا المثال، نقوم بتعيين **في هذه الساعات** كـ **8**، حيث إننا نريد تشغيل المشغل كل صباح في الساعة 8 ص.

    > [!div class="mx-imgBorder"]
    > [![مع الفاصل الزمني المعين إلى 1، يتم تعيين "التكرار" إلى يوم، وعند تعيين هذه الساعات إلى 8، فإنها تعمل كل صباح في الساعة 8 صباحًا.](../media/tutorial-9-run-every-morning-ss.png)](../media/tutorial-9-run-every-morning-ss.png#lightbox)

## <a name="step-2-add-an-action-to-the-flow"></a>الخطوة 2: إضافة إجراء إلى المسار

1.  حدد **خطوة جديدة** وفي مربع البحث، أدخل **Sales Insights** أو **المساعد**.

1.  حدد موصل **Dynamics 365 Sales Insights**.

1.  ضمن الإجراءات، حدد **إنشاء بطاقة للمساعد V3**.

    > [!div class="mx-imgBorder"]
    > [![ضمن الإجراءات، حدد إنشاء بطاقة للمساعد V3.](../media/tutorial-9-choose-create-card-assistant-ss.png)](../media/tutorial-9-choose-create-card-assistant-ss.png#lightbox)

## <a name="step-3-enter-details-and-choose-action-type-none"></a>الخطوة 3: إدخال التفاصيل واختيار نوع الإجراء "لا شيء"

1.  أدخل البيئة والتفاصيل الأخرى حسب الحاجة.

1.  حدد **لا شيء** من القائمة المنسدلة **نوع الإجراء "أساسي"** للتأكد من عدم إضافة أي إجراء في بطاقة المعلومات.

    > [!div class="mx-imgBorder"]
    > [![يتم تحديد "لا شيء" لنوع الإجراء "أساسي".](../media/tutorial-9-primary-action-type-none-ss.png)](../media/tutorial-9-primary-action-type-none-ss.png#lightbox)

## <a name="step-4-save-the-flow-and-test-the-flow"></a>الخطوة 4: حفظ التدفق واختباره

تشغيل المسار يدويًا أو عند تشغيله كما هو مجدول، يجب أن تكون بطاقة المعلومات الجديدة متوفرة في التطبيق.

> [!div class="mx-imgBorder"]
> [![مظهر بطاقة المعلومات الجديدة عند تشغيلها.](../media/tutoria-9-new-insight-card-ss.png)](../media/tutoria-9-new-insight-card-ss.png#lightbox)
