---
ms.openlocfilehash: 75387301fdcec56fca00dfd813672c576ffbb510
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071232"
---
يمكنك استخدام `GetExecutionSummaryStatus` لكل من مهام الاستيراد والتصدير. يستخدم هذا للتحقق من حالة وظيفة تشغيل مشروع البيانات. واجهة برمجة التطبيقات (API) هذه قابلة للتطبيق على عمليات النشر السحابية وعمليات النشر المحلية. ضع في اعتبارك أن الملف سيبقى في مساحة تخزين الكائنات الثنائية كبيرة الحجم لمدة سبعة أيام، وبعد ذلك سيتم حذفه تلقائياً.

للتحقق من حالة واجهة برمجة التطبيقات (API)، استخدم `GetExecutionSummaryStatus` ثم حدد معرف التنفيذ.

على سبيل المثال:

```csharp
POST /data/DataManagementDefinitionGroups/Microsoft.Dynamics.DataEntities.GetExecutionSummaryStatus
BODY
{"executionId":"<executionId>"}
```
سيتم إرسال رسالة رد JSON بنجاح وسيتم عرض حالة التنفيذ. هناك العديد من المخرجات التي قد تتلقاها في هذه الرسالة:

-   غير معروف
-   ‏‫ليس قيد التشغيل‬
-   جارٍ التنفيذ
-   ناجح
-   نجح جزئياً
-   فشل
-   ‏‫تم الإلغاء‬
 