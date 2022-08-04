---
ms.openlocfilehash: 628a348e18c73f6bcc5e3ce02fc41cbb347bb363
ms.sourcegitcommit: 387570c3e18c5bac18992a0b71b9740aa99cba9a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/30/2022
ms.locfileid: "9092582"
---
في Dynamics 365 Marketing، يُمكن للمستخدمين إنشاء صفحات منتقل إليها وأنواع أخرى من صفحات الويب التي تعرض محتوى مخصصاً لجهات الاتصال المعروفة.

يستخدم الحل الأساليب الآتية:

-   يُحدد ملف تعريف الارتباط، الذي يتم تعيينه في المستعرض، جهات الاتصال المعروفة.

-   يُستخدم JavaScript لإحضار القيم من سجل جهة الاتصال المعني إلى صفحه التسويق.

-   يجب تشغيل الصفحات المخصصة إما في مجال مُصدّق عليه أو في مدخل Dynamics 365، ويجب أن تستخدم HTTPS.

-   تم تقييد الوصول إلى البيانات صراحةً لحقول قائمة السماح من كيان جهة الاتصال.

-   يجب أن تقبل جهات الاتصال تعبئة النموذج السابقة لرؤية محتوى صفحة التسويق المخصص.

-   استخدم كيان الصفحة المخصصة لإنشاء قائمة السماح وإنشاء JavaScript.

لتمكين هذه الميزة، ستحتاج أولاً إلى الانتقال إلى **التسويق الصادر> محتوى التسويق> الصفحات المخصصة** لتحديد حقول جهات الاتصال المراد إتاحتها ثم إنشاء الرمز لجلب هذه القيم إلى الصفحة.

لإعداد ميزة تخصيص الصفحة، عليك أيضاً إنشاء قائمة السماح بحقول جهات الاتصال وإنشاء كود JavaScript الذي ستحتاجه لاستيراد قيم الحقول إلى صفحتك. يُمكنك إكمال هذه المهام من خلال العمل مع سجلات الصفحة الشخصية. لمزيد من المعلومات، راجع [إعداد تخصيص الصفحة](/dynamics365/marketing/personalized-page-content?azure-portal=true#set-up-page-personalization).

**الوصول إلى معلومات أكثر قابلة للتطبيق**

-   [مصادقة المجالات الخارجية](/dynamics365/marketing/personalized-page-content?azure-portal=true#authenticate-your-external-domains)

-   [إضافة تخصيص إلى صفحة منتقل إليها أو صفحه ويب](/dynamics365/marketing/personalized-page-content?azure-portal=true#add-personalization-to-a-landing-page-or-web-page)

-   [اختبار تخصيص الصفحة](/dynamics365/marketing/personalized-page-content?azure-portal=true#test-your-page-personalization)
