---
ms.openlocfilehash: 02b0d927148e9311192627741776110e89e2e199e48c05a3eaf6455efaf575d8
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7094419"
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
 