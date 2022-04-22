---
ms.openlocfilehash: 57f92e25c5097b5ae8495161497dcf45f6c68c9b
ms.sourcegitcommit: 638bab9b0642ad3d3698e559bdfe044fb14354f7
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2022
ms.locfileid: "8548419"
---
في هذه المرحلة من التمرين العملي للبدء السريع، يجب على الموفر أن يعرض المكونات كما يظهر في لقطة الشاشة التالية.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لمكونات حل الموفر.](../media/export-components-ss.png)](../media/export-components-ss.png#lightbox)

لمزيد من المعلومات، راجع [تصدير الحلول](/power-apps/maker/data-platform/export-solutions).

## <a name="clean-up-after-export"></a>التنظيف بعد التصدير

للتنظيف بعد التصدير، اتبع هذه الخطوات:

1. انتقل إلى [مدخل المنشئ في Power Apps](https://make.powerapps.com)، انتقل إلى **الحلول > الحل الافتراضي**، ثم قم بالتصفية على **سير العمل السحابي**.
1. أوقف مهام سير العمل السحابية التالية التي تم إنشاؤها لتهيئة تعريف منطق تعريف الموفر: 
    - تمرين عملي IOM - معالج طلبات الرسائل لاستلام الأمر
    - تمرين عملي IOM - إرسال إلى التنفيذ (Outlook)
    - تمرين عملي IOM - إرسال إلى التنفيذ (RequestBin)

> [!NOTE]
> سيتم إنشاء مهام سير عمل جديدة عند إنشاء مثيل عن الموفر. إذا لم توقف تشغيل مهام سير العمل هذه، فسيتم إرسال أكثر من الحمولة الصادرة المتوقعة.
