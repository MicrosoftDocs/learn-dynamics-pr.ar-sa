---
ms.openlocfilehash: 929eb2c6002fbf69748b1e9b525455ae09bfdd14
ms.sourcegitcommit: 42a0faa4dc64a860f6457449b0792257c2254757
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/23/2022
ms.locfileid: "9584035"
---
في الآونة الأخيرة، بدأ أحد العملاء استخدام Dynamics 365 Finance. قام المستخدمون برفع تذاكر الدعم الداخلي، مدعين أن النظام بطيء ويمنعهم من إكمال عملهم.

## <a name="pattern---collect-information-and-analyze-telemetry"></a>النمط - جمع المعلومات وتحليل القياس عن بُعد

الاستجابة لتفاعلات المستخدم البطيئة من خلال جمع المعلومات وتحليل القياس عن بُعد. في هذا السيناريو، ستكون أفضل ممارساتك هي:

- تأكد من أن المستخدمين يقدمون المعلومات المناسبة للسماح بمزيد من التحقيق. إذا لم يكن المستخدمون عَلى دراية بالمعلومات المطلوبة، فقم بتثقيفهم.
- راجع المعلومات لتحديد ما إذا كانت الأنماط الشائعة موجودة.
- قم بجمع القياس عن بعد من المصادر ومراجعته، مثل Lifecycle Services وQuery Store وTraces.
- التخفيف من الاختناقات التي تؤثر عَلى المستخدمين.
- راجع [اختبار الأداء فِي سلسلة الأحاديث التقنية من Microsoft Dynamics 365 - مدونة Microsoft Dynamics](https://community.dynamics.com/365/dynamics-365-fasttrack/b/techtalks/posts/performance-testing-in-microsoft-dynamics-365-techtalk-series/?azure-portal=true).
- راجع المقالات التالية حول استكشاف الأخطاء وإصلاحها باستخدام Lifecycle Services Microsoft Dynamics:

  - [استكشاف أخطاء الأداء وإصلاحها باستخدام الأدوات الموجودة في Lifecycle Services](/dynamics365/fin-ops-core/dev-itpro/lifecycle-services/performancetroubleshooting/?azure-portal=true)
  - [كتاب تعليمات الاستعلام](/dynamics365/fin-ops-core/dev-itpro/lifecycle-services/querycookbook/?azure-portal=true)

## <a name="anti-pattern"></a>النمط المضاد

من بين النمط المضاد (المزلق) الاستجابة لتفاعلات المستخدم البطيئة أن نفترض أن مشكلات الأداء مرتبطة بالبنية الأساسية وبالتالي لا يمكن للعملاء و/أو الشركاء فعل أي شيء لإصلاحها.
