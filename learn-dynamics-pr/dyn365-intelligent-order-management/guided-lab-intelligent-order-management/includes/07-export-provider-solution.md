---
ms.openlocfilehash: ae234c9f33945bf8d8cb4b39cd801849b99215b8
ms.sourcegitcommit: 28b5b81155de28693455114a5fc5941cb314c9ef
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/31/2022
ms.locfileid: "8075794"
---
في هذه المرحلة من معمل البدء السريع ، يجب أن ترى الآن المكونات التالية في حل الموفر.

> [!div class="mx-imgBorder"]
> [![موفر مكونات الحل](../media/export-components-ss.png)](../media/export-components-ss.png#lightbox)

للحصول على إرشادات حول تصدير الحل الخاص بك، راجع [تصدير الحلول](/powerapps/maker/data-platform/export-solutions).

## <a name="clean-up-after-export"></a>التنظيف بعد التصدير

للتنظيف بعد التصدير، اتبع هذه الخطوات.

1. انتقل إلى [مدخل منشئ Power App](https://make.powerapps.com)، وانتقل إلى **الحلول \> الحلول الافتراضية**، ثم قم بالتصفية على **تدفق السحابة**.
1. أوقف تدفقات السحابة التالية التي تم إنشاؤها لتهيئة تعريف منطق تعريف الموفر. 
    - معالج طلبات الحصول على طلب رسالة من معمل IOM.
    - تمرين عملي IOM - إرسال إلى التنفيذ (Outlook).
    - تمرين عملي IOM - إرسال إلى التنفيذ (RequestBin).

> [!NOTE]
> يتم إنشاء تدفقات جديدة عند إنشاء مثيل للمزود. إذا لم يتم إيقاف تشغيل هذه التدفقات، فسيتم إرسال أكثر من الحمولة الصادرة المتوقعة.
