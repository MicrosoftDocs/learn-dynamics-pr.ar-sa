---
ms.openlocfilehash: 2613d68c17135fb223d1d3b39334e8861febc4e7
ms.sourcegitcommit: 20c987e5ad19236137f3bdbaaae524d0864711b2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/01/2022
ms.locfileid: "9393366"
---
يحتاج العميل إلَى وظيفة دفعية مخصصة للتشغيل كل ليلة ومعالجة آلاف السجلات. يبني الشريك الوظيفة الدفعية المطلوبة، وتعمل عَلى النحو المطلوب. ومع ذلك، فإن الوظيفة تستغرق وقتًا طويلاً وتمنع إكمال الوظائف الليلية خلال الوقت المخصص.

## <a name="pattern---design-batch-jobs-with-parallelism"></a>النمط - تصميم الوظائف الدفعية بالتوازي

يعني الحل القابل للتطوير أنه يمكنك تقسيم مهمة دفعية إلَى أجزاء أصغر، ويمكنك تشغيل كلّ منها بشكل مستقل وبالتوازي للسماح بإنتاجية أسرع. تتوفر تقنيات مختلفة لتختار من بينها، وتتم مناقشتها بالتفصيل فِي المقالات التالية:

- **توازي الدُفعات** - [التوازي الدُفعي فِي AX – الجزء الأول | Microsoft Docs](/archive/blogs/axperf/batch-parallelism-in-ax-part-i/?azure-portal=true)
- **نمذجة المهام الفردية** - [التوازي الدُفعي فِي AX – الجزء الثاني | Microsoft Docs](/archive/blogs/axperf/batch-parallelism-in-ax-part-ii/?azure-portal=ture)
- **أهم عمليات الانتقاء** - [التوازي الدُفعي فِي AX – الجزء الثالث | Microsoft Docs](/archive/blogs/axperf/batch-parallelism-in-ax-part-iii/?azure-portal=true)

## <a name="anti-patterns"></a>الأنماط المضادة

ضع فِي اعتبارك الأنماط المضادة (المزالق) التالية عند تصميم قابلية التوسع:
- لا تختبر الوظائف الدفعية ببيانات تمثل أحجامًا حقيقية.
- لا تصمم وظائف دفعية مع وضع التوازي فِي الاعتبار.
