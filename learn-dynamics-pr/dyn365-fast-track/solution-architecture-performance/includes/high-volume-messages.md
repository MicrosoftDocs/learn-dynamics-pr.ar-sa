---
ms.openlocfilehash: c70a30bc23d32fb6a599918c79376d4854c35168
ms.sourcegitcommit: 20c987e5ad19236137f3bdbaaae524d0864711b2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/01/2022
ms.locfileid: "9393356"
---
يحتوي مثيل تطبيقات التمويل والعمليات الخاص بالعميل عَلى تكامل لأمر مبيعات كبير الحجم يستخدم نمط OData فِي الوقت الفعلي. حجم بيانات الذروة 500،000 بند فِي الساعة. تكتفي الشركة باستيراد البيانات كل ست ساعات. لا يعمل التكامل بالشكل المتوقع ويؤثر عَلى قابلية استخدام النظام.

## <a name="pattern---select-an-asynchronous-integration-pattern"></a>النمط - حدد نمط تكامل غير متزامن

عند إدارة حجم كبير من الرسائل، يجب تحديد نمط تكامل غير متزامن للأسباب التالية:
- يمكن ضبطه للتعامل مع الأحجام ذات الذروة العالية.
- إنه نمط غير محظور، حيث يقدم المتصل الطلب ثم يواصل دون انتظار استجابة.

تتضمن أمثلة الأنماط غير المتزامنة ما يلي:
- [واجهة برمجة تطبيقات REST لحزمة إدارة البيانات](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-management-api/?azure-portal=true)
- [واجهة API لعمليات تكرار التكامل](/dynamics365/fin-ops-core/dev-itpro/data-entities/recurring-integrations/?azure-portal=true)

تأكد من توفر الكيان الداعم الذي يدعم الواردات القائمة عَلى المجموعة أو الموازية.

لمزيد من المعلومات، راجع [التكامل بين تطبيقات التمويل والعمليات وخدمات الجهات الخارجية - Finance & Operations | Dynamics 365 | Microsoft Docs](/dynamics365/fin-ops-core/dev-itpro/data-entities/integration-overview/?azure-portal=true).

## <a name="anti-patterns"></a>الأنماط المضادة

ضع فِي اعتبارك الأنماط المضادة (المزالق) التالية عند تحديد تكامل غير متزامن:
- استمر فِي استخدام نمط الوقت الحقيقي لـ OData.
- استخدم نمطًا غير متزامن، لكن لا تختبره وتحسِّنه قبل استخدامه فِي الإنتاج.
