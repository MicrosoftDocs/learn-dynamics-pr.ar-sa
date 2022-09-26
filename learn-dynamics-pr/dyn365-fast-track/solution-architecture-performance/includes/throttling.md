---
ms.openlocfilehash: 503970c6c2f3223a53ddf33f858ff51d54b1f34f
ms.sourcegitcommit: 20c987e5ad19236137f3bdbaaae524d0864711b2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/01/2022
ms.locfileid: "9393361"
---
يحتوي مثيل إنتاج تطبيقات التمويل والعمليات للعميل عَلى العديد من OData فِي الوقت الفعلي والتكاملات المخصصة القائمة عَلى الخدمة مع الأنظمة الخارجية. بعض عمليات الدمج أكثر أهمية من غيرها. لاحظ العميل أنه خلال ساعات العمل، يتم تقييد طلبات عمليات الدمج المهمة، ما أدى إلَى حدوث حالة خطأ.

## <a name="pattern---split-and-set-up-priorities-for-integrations"></a>النمط - تقسيم أولويات عمليات الدمج وإعدادها
ضع فِي اعتبارك الأنماط التالية (أفضل الممارسات) عند تقسيم أولويات عمليات الدمج وتحديدها:
- توزيع أحمال عمل تكامل مختلفة عبر مبادئ خدمة متعددة.
- [حدد الأولويات المناسبة](/dynamics365/fin-ops-core/dev-itpro/data-entities/priority-based-throttling/?azure-portal=true) لضمان أن عمليات التكامل ذات الأولوية المنخفضة سيتم تقييدها قبل التكامل ذي الأولوية العالية.
- قم بتنفيذ [عمليات إعادة المحاولة](/dynamics365/fin-ops-core/dev-itpro/data-entities/service-protection-retry-operations/?azure-portal=true) واستخدم الفاصل الزمني **Retry-After** لإعادة المحاولة الذي يوفره الخادم.
- استمر فِي [المراقبة](/dynamics365/fin-ops-core/dev-itpro/data-entities/service-protection-monitoring/?azure-portal=true) وأنماط تكامل الخدمة المخصصة باستخدام Microsoft Dynamics 365 Lifecycle Services.
- افتح تذكرة دعم مع Microsoft لمراجعة البنية الأساسية إذا لم تحل الإجراءات السابقة المشكلة.
- قم بالتجهيز لـ [حدود واجهة برمجة التطبيقات لحماية الخدمة المستندة إلَى المستخدم](/dynamics365/fin-ops-core/dev-itpro/data-entities/service-protection-api-limits/?azure-portal=true) لتطبيقات التمويل والعمليات، والمخصصة لكل مستخدم، لكل خادم ويب.

لمزيد من المعلومات، راجع [حدود API لحماية الخدمة - Finance and Operations | Dynamics 365 | Microsoft Docs](/dynamics365/fin-ops-core/dev-itpro/data-entities/service-protection-api-limits/?azure-portal=true).

## <a name="anti-patterns"></a>الأنماط المضادة 

ضع فِي اعتبارك الأنماط المضادة (المزالق) التالية عند تقسيم أولويات وإنشائها لعمليات التكامل:
- استخدم نفس مبدأ الخدمة لأحمال عمل تكامل مختلفة.
- لا تضع أولويات.
- لا تنفذ عمليات **إعادة المحاولة**.
- لا تستخدم الفاصل الزمني **Retry-After** المتوفرة من خلال الخادم عندما تكون بصدد تنفيذ عمليات **Retry**.
