---
ms.openlocfilehash: 6f27927c626b1cb59e401840b17f1f91faff9853
ms.sourcegitcommit: 971396efb8e68a74511ae8ca417a67c4d9cef8ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/04/2021
ms.locfileid: "7599848"
---
يجري التعامل مع الاتفاقات التجارية والخصومات والسيناريوهات الأخرى التي تعتمد على المعالجات الثانوية في Supply Chain Management من خلال بيانات التدبير. بالنسبة لكل أمر شراء، يستخدم محرك التدبير مجموعة معقدة من المعايير لإيجاد السعر الأمثل المطلوب تحميله. حتى عند تمكين الكتابة المزدوجة للمحافظة على مزامنة البيانات في بيئتين، لا يكون هذا السيناريو دائماً، لا سيما في الحالات التي جرى فيها إنشاء صف أو تحديثه من Dataverse وقد يشغل إجراءات متابعة في بيئة Supply Chain Management بعد ذلك.

## <a name="sync-the-procurement-data-from-supply-chain-management"></a>مزامنة بيانات التدبير من Supply Chain Management

لمزامنة بيانات التدبير من Supply Chain Management، اتبع الخطوات التالية:

1. في Dataverse، انتقل إلى  **المخزون > أمر الشراء**.

1. حدد  **جديد**  لإنشاء أمر شراء جديد أو حدد صف أمر شراء موجود.

1. في جزء الإجراء، حدد **مزامنة**.

ستجري مزامنة كافة الأعمدة من Dataverse وField Service التي تشاركها Supply Chain Management.

شاهد مقطع الفيديو التالي للاطلاع على خطوات مزامنة البيانات من Supply Chain Management.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RWMga6]

قد ترغب في استخدام دالة **المزامنة** عند:

- إجراء عده تغييرات متسلسلة لنفس الصف من Dataverse.

- لا تكون متأكداً مما إذا كان التغيير هو التغيير المتتابع الثاني من Dataverse.

- يمكن حل إخطار الخطأ المتعلق بتحديث قيمة من Supply Chain Management بتشغيل دالة **المزامنة** ثم محاولة إجراء التحديث مرةً أخرى.
