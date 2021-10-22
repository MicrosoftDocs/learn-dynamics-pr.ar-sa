---
ms.openlocfilehash: 9ca38618d557dc45604c6aaf83ed79047a70e45a
ms.sourcegitcommit: 971396efb8e68a74511ae8ca417a67c4d9cef8ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/04/2021
ms.locfileid: "7599849"
---
لتحقيق تكامل Supply Chain Management مع Field Service، ثبّت المكونات التالية:

- إصدار Field Service 8.8.31.60 أو إصدار أحدث لتحقيق التكامل الشامل لأوامر الشراء

- إصدار Supply Chain Management 10.0.14 أو أحدث

- الكتابة المزدوجة، لتشغيل حل OneFSSCM

للحصول على إرشادات التثبيت، راجع الوثائق التالية:

- **الكتابة المزدوجة**  - لمزيد من المعلومات، راجع  [الصفحة الرئيسية للكتابة المزدوجة](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page?azure-portal=true).

- **Dynamics 365 Field Service** - لمزيد من المعلومات، راجع  [كيفية تثبيت Dynamics 365 Field Service](/dynamics365/field-service/install-field-service?azure-portal=true).

تضيف الكتابة المزدوجة وField Service طبقات حل متعددة تعمل على توسيع البيئة ببيانات تعريف ونماذج وطرق عرض ومنطق جديد عند التمكين في Microsoft Dataverse. يمكن تفعيل هذه الحلول بأي ترتيب. بشكل عام، يجب عليك تثبيتها بالترتيب التالي:

1. **Field Service Common** - يتم تثبيت هذا الحل عند تثبيت Field Service في البيئة. لمزيد من المعلومات، راجع [الحل Field Service Common](/dynamics365/customer-engagement/web-api/fieldservicecommon?azure-portal=true).

1. **Field Service ‏(Anchor)** - يتم تثبيت هذا الحل عند تثبيت Field Service في البيئة.

1. **Supply Chain Management Extended** - - يتم تثبيت هذا الحل تلقائيًا عند تمكين الكتابة المزدوجة في بيئة ما.

1. **الحل OneFSSCM ‏(Field Service/Supply Chain Management)** - يتم تثبيت هذا الحل تلقائيًا بأي حل تم تثبيته أخيرًا (Field Service أو Supply Chain Management).

    - إذا تم تثبيت Field Service بالفعل في البيئة، وقمت بتمكين الكتابة المزدوجة، والتي تقوم بتثبيت Supply Chain Management Extended، يتم تثبيت OneFSSCM.

    - إذا تم تثبيت Supply Chain Management Extended بالفعل في البيئة، وقمت بتثبيت Field Service، فسيتم تثبيت OneFSSCM.
