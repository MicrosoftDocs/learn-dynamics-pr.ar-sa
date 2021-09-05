---
ms.openlocfilehash: 9f3c58400aa76849f4030aa8297b6aa0a183c44c
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7365905"
---
عندما تحتاج إلى تعديل الكود الأساسي، استخدم إطار عمل قابلية التوسعة. يمكنك توسيع الكود الأساسي باستخدام المفاهيم التالية:

- **الأحداث** – يتم رفع الأحداث كعمليات سابقة ولاحقة حول الأساليب الأساسية، مما يعني أنه يمكنك تشغيل الكود قبل استدعاء الطريقة الأساسية وبعد اكتمالها. قدم Dynamics AX 2012 أحداث XPP، والتي تتوفر أيضاً في هذا الإصدار ويمكن الاشتراك فيها في ملحقاتك. لمزيد من المعلومات، راجع [‏‫تخصيص من خلال الملحق وتراكب الطبقات‬](/dynamics365/fin-ops-core/dev-itpro/extensibility/customization-overlayering-extensions?azure-portal=true#event-argument-types).

- **المكونات الإضافية** – المكونات الإضافية هي نقاط الملحق التي يتم تحديدها بواسطة التطبيق الأساسي. باستخدام نمط مصنع الفئة، تمكنك المكونات الإضافية من استبدال الوظيفة الأساسية. يمكنك التعرف على كيفية تنفيذ المكونات الإضافية في البرنامج التعليمي [‏‫تخصيص عناصر النموذج من خلال الملحقات](/dynamics365/fin-ops-core/dev-itpro/extensibility/customize-model-elements-extensions/?azure-portal=true).

- **ملحقات الفئة** – تتيح لك ملحقات الفئة زيادة فئة عن طريق إضافة أساليب ومتغيرات للفئات والجداول والنماذج الموجودة. لمزيد من المعلومات، راجع [نموذج ملحق الفئة في X++](/dynamics365/fin-ops-core/dev-itpro/extensibility/class-extensions/?azure-portal=true).

