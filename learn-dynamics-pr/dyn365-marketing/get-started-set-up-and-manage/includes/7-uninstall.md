---
ms.openlocfilehash: 3e888b6d1ca382a68bc9960c969be6540e757974
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7435401"
---
يُمكنك إزالة تطبيق Marketing من أي بيئة Dynamics 365 قد ثبّته فيها. بعد إزالة التثبيت، ستحصل على استحقاق (ترخيص) Marketing مجاني. يُمكنك تثبيت الترخيص في بيئة Dynamics 365 أخرى إذا لزم الأمر.

## <a name="uninstall-process-steps"></a>خطوات عملية أزاله التثبيت

1.  إزالة تثبيت خدمات Marketing عن طريق تشغيل معالج إزالة التثبيت.

2.  إعادة تعيين جميع مداخل Dynamics 365 أو مداخل Power Apps التي كانت متصلة بتطبيق Marketing (إن وجد).

3.  تنظيف حلول Marketing في Dynamics 365.

يُدير مُعالج إزالة تثبيت Marketing معظم عملية إزالة التثبيت. 

-   يُزيل المعالج جميع خدمات Marketing وإدارة الأحداث و Dynamics 365 Connector for LinkedIn Lead Gen Forms من خادم تطبيق Dynamics 365

-   إزالة خدمة المعلومات التسويقية وبياناتها

-   إيقاف مزامنة المستخدم من Microsoft 365 لمستخدمي Marketing فقط.

-   تحرير استحقاق (ترخيص) Dynamics 365 Marketing لاستخدامه مع مثيل Dynamics 365 آخر إذا لزم الأمر.

اتبع [الخطوات الواردة هنا](/dynamics365/marketing/uninstall-marketing?azure-portal=true#uninstall-the-marketing-services) لتشغيل معالج إزالة التثبيت. وتأكد أيضًا من [إعادة تعيين أي مداخل Dynamics 365 متصلة بتطبيق Marketing غير المثبت](/dynamics365/marketing/uninstall-marketing?azure-portal=true#reset-any-dynamics-365-portals-connected-to-the-uninstalled-marketing-app) و [إزالة حلول Marketing في Dynamics 365](/dynamics365/marketing/uninstall-marketing?azure-portal=true#remove-marketing-solutions-in-dynamics-365).
