---
ms.openlocfilehash: 8eb4d73a197b22a1a0c1024359aaff3240ec30f2
ms.sourcegitcommit: df34fe229bb726628154d95627564ff46adf703a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/23/2021
ms.locfileid: "6656570"
---
في Dynamics 365 Human Resources، تسمح لك معالجة التعويض احتساب مبالغ التعويض الأساسية الجديدة لموظفيك استناداً إلى تعديلات الأسهم وأهداف زيادة الجدارة والأداء. في هذا الوحدة، ستقوم بما يلي:

- إنشاء عملية تعويض.

- تشغيل العملية.

- عرض النتائج.

## <a name="set-up-the-compensation-process"></a>إعداد عملية التعويض

يتيح لك حدث العملية تحديد معلمات معالجة التعويض، بما في ذلك فترة التاريخ لتقييم تحديد مبالغ التعويض والتاريخ الذي يجب أن تدخل فيه مبالغ التعويض الجديدة حيز التنفيذ.

1. في مساحة العمل **إدارة التعويض**، حدد **الارتباطات > عمليات التعويض**.

1. حدد **جديد**.

1. أدخِل قيم **العملية** و **الوصف**، ثم حدد **نوع العملية**.

1. أدخِل تواريخ الحقول ضمن **إعداد التاريخ**.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لعملية إنشاء التعويض في الموارد البشرية.](../media/human-resources-compensation-create-process.png)](../media/human-resources-compensation-create-process.png#lightbox)

1. حدد **حفظ**.

1. حدد **الإعداد** في شريط التنقل.

1. ضمن **الخطط**، حدد **إضافة** لإضافة خطة تعويض إلى حدث العملية.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لخطط إضافة تعويضات لعملية التعويض في الموارد البشرية.](../media/human-resources-compensation-process-add-plans.png)](../media/human-resources-compensation-process-add-plans.png#lightbox)

1. ضمن **الإجراءات**، حدد **إضافة** لإضافة إجراءات تعويض ثابتة للخطة المحددة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لإجراءات إضافة تعويض لعملية التعويض في الموارد البشرية.](../media/human-resources-compensation-process-add-actions.png)](../media/human-resources-compensation-process-add-actions.png#lightbox)

1. حدد **حفظ**.

## <a name="run-the-compensation-process"></a>تشغيل عملية التعويض

لتشغيل عملية التعويض، اتبع الخطوات التالية:

1. في الصفحة **عمليات التعويض**، حدد **تشغيل العملية**.

1. قم بتغيير القيم في جزء **تشغيل عملية التعويض** حسب الضرورة.

   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لعملية تشغيل التعويض في الموارد البشرية.](../media/human-resources-compensation-run-process.png)](../media/human-resources-compensation-run-process.png#lightbox)

1. حدد **موافق**.

## <a name="view-the-process-results"></a>عرض نتائج العملية

في الصفحة **عمليات التعويض**، حدد **نتائج العملية**.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لخيار عرض نتائج العملية في إدارة تعويض الموارد البشرية.](../media/human-resources-compensation-view-process-results.png)](../media/human-resources-compensation-view-process-results.png#lightbox)

تحتوي صفحة **نتائج العملية** على معلومات حول تشغيل العملية، بما في ذلك وقت التشغيل، والمستخدم الذي قام بتشغيل العملية، وما إذا كانت الأخطاء قد حدثت عند تشغيل العملية. يمكنك أيضاً تحديد الخيار **تأمين** لتعطيل الزر **تحميل التعويض** ومنع أي شخص من تحميل أحداث التعويض إلى سجلات الموظف.
يؤدي تحديد الزر **نتائج الموظف** إلى عرض قائمة الموظفين المضمنين في التشغيل.

للحصول على مزيد من المعلومات، راجع [عملية التعويض](/dynamics365/human-resources/hr-compensation-process/?azure-portal=true).
