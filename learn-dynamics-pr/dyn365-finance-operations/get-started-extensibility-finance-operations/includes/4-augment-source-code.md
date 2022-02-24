---
ms.openlocfilehash: 7b4f6fcfed6c5a75138fedacc237cc7f6a325c6b
ms.sourcegitcommit: e0a1238596690b3b6eedd86c2ac14099948a5e25
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "6072539"
---
عندما تحتاج إلى تعديل الكود الأساسي، استخدم إطار عمل قابلية التوسعة. يمكنك توسيع الكود الأساسي باستخدام المفاهيم التالية:

- **الأحداث** – يتم رفع الأحداث كعمليات سابقة ولاحقة حول الأساليب الأساسية، مما يعني أنه يمكنك تشغيل الكود قبل استدعاء الطريقة الأساسية وبعد اكتمالها. قدم Dynamics AX 2012 أحداث XPP، والتي تتوفر أيضاً في هذا الإصدار ويمكن الاشتراك فيها في ملحقاتك. لمزيد من المعلومات، راجع [‏‫تخصيص من خلال الملحق وتراكب الطبقات‬](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/extensibility/customization-overlayering-extensions#event-argument-types/?azure-portal=true).

- **المكونات الإضافية** – المكونات الإضافية هي نقاط الملحق التي يتم تحديدها بواسطة التطبيق الأساسي. باستخدام نمط مصنع الفئة، تمكنك المكونات الإضافية من استبدال الوظيفة الأساسية. يمكنك التعرف على كيفية تنفيذ المكونات الإضافية في البرنامج التعليمي [‏‫تخصيص عناصر النموذج من خلال الملحقات](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/extensibility/customize-model-elements-extensions/?azure-portal=true).

- **ملحقات الفئة** – تتيح لك ملحقات الفئة زيادة فئة عن طريق إضافة أساليب ومتغيرات للفئات والجداول والنماذج الموجودة. لمزيد من المعلومات، راجع [نموذج ملحق الفئة في X++](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/extensibility/class-extensions/?azure-portal=true).

