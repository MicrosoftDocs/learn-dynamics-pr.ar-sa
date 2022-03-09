---
ms.openlocfilehash: 931331799b3b57010acf57473d779963111ec8e4
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7355972"
---
قبل أن تتمكن من استخدام إدارة المزايا، يجب عليك تمكينها في مساحة عمل **إدارة الميزات**، التي توفر قائمة بالميزات التي يتم تقديمها في كل إصدار. بشكل افتراضي، يتم إيقاف تشغيل الميزات الجديدة.

> [!IMPORTANT]
> تأكد من التدرب على إدارة المزايا في بيئة وضع حماية قبل تمكينها في بيئة الإنتاج الخاصة بك. يمكنك تمكين وتعطيل إدارة المزايا بقدر ما تريد في بيئة وضع الحماية. ومع ذلك، بعد تشغيل إدارة المزايا في بيئة إنتاج، لا يمكنك إيقاف تشغيل الميزة. لمزيد من المعلومات، راجع [إدارة الميزات](/dynamics365/human-resources/hr-admin-manage-features/?azure-portal=true).

## <a name="enable-benefits-management"></a>تمكين إدارة المزايا

لتمكين إدارة المزايا، اتبع الخطوات التالية:

1. في Human Resources، حدد إطار متجانب **إدارة النظام**.
   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لـ Human Resources مع تمييز زر إدارة النظام](../media/benefits-management-system-administration.png)](../media/benefits-management-system-administration.png#lightbox)

1. في صفحة **إدارة النظام**، حدد إطار متجانب **إدارة الميزات**.
   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لصفحة إدارة النظام مع تمييز إدارة الميزات.](../media/benefits-management-feature-management.png)](../media/benefits-management-feature-management.png#lightbox)

1. في صفحة **إدارة الميزات**، حدد **إدارة المزايا**، ثم حدد **تمكين الآن**.
   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لإدارة المزايا مع تمييز الزر "تمكين الآن".](../media/benefits-management-enable-now.png)](../media/benefits-management-enable-now.png#lightbox)

1. في جزء **تمكين إدارة المزايا**، حدد **تمكين**.

تحل إدارة المزايا محل الوظائف في مساحة عمل **المزايا** القديمة. بعد قيامك بتمكين إدارة المزايا، لن تتمكن من الوصول إلى النماذج التالية في مساحة عمل **المزايا**:

- **المزايا‬**

- **عناصر المزايا**

- **نسب حساب المساهمة**

- **نتائج تسجيل الميزات**

- **نتائج التمديد أو انتهاء صلاحية الميزات**

- **أنواع قواعد سياسات استحقاق المزايا**

- **سياسات استحقاق المزايا**

- **أحداث الاستحقاق**

يمكنك عرض المعلومات في هذه النماذج في وضع القراءة فقط. إذا كنت ترغب في تحرير المعلومات، يجب عليك أولاً تعطيل إدارة المزايا (في بيئات وضع الحماية فقط).

بعد تمكين إدارة المزايا، سيتوفر الإطاران المتجانبان **إدارة الميزات** و **المزايا** في Human Resources.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة للإطارين المتجانبين إدارة المزايا والمزايا.](../media/benefits-management-tiles.png)](../media/benefits-management-tiles.png#lightbox)

## <a name="hide-legacy-benefit-forms"></a>إخفاء نماذج المزايا القديمة

يمكنك إيقاف تشغيل نماذج المزايا القديمة إذا لم تعد بحاجة إلى رؤيتها في بيئتك.

1. في Human Resources، حدد إطار متجانب **إدارة المزايا**.

1. في مساحة عمل **إدارة المزايا**، حدد **المعلمات المشتركة لـ Human Resources‬**.
   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة لمساحة عمل إدارة المزايا مع تمييز المعلمات المشتركة لـ Human Resources.](../media/benefits-management-shared-parameters.png)](../media/benefits-management-shared-parameters.png#lightbox)

1. في صفحة **المعلمات المشتركة لـ Human Resources**، حدد علامة التبويب **إدارة المزايا**.

1. قم بتعيين تبديل **إخفاء نماذج المزايا القديمة** إلى **نعم**.
   > [!div class="mx-imgBorder"]
   > [![لقطة شاشة للمعلمات المشتركة لـ Human Resources مع تشغيل تبديل إخفاء نماذج المزايا القديمة.](../media/benefits-management-hide-legacy.png)](../media/benefits-management-hide-legacy.png#lightbox)

## <a name="disable-benefits-management"></a>تعطيل إدارة المزايا

تتشابه خطوات تعطيل إدارة المزايا تقريباً مع خطوات تمكينها. تذكر، لا يمكنك تعطيل إدارة المزايا في بيئة إنتاج.

1. في Human Resources، حدد إطار متجانب **إدارة النظام**.

1. في صفحة **إدارة النظام**، حدد إطار متجانب **إدارة الميزات**.

1. في صفحة **إدارة الميزات**، حدد **إدارة المزايا**، ثم حدد **تعطيل**.
