---
ms.openlocfilehash: dba0ccc32bdf29bd379d21231c5da34a88c15aca
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071893"
---
يمكنك استخدام العديد من الإجراءات لاستكشاف مشكلات مصادقة الخدمة وإصلاحها. ويتمثل الإجراء الشائع في فحص ‏‫رموز ويب JSON المميزة‬ (JWTs).

الخيار الأول هو التقاط رمز JWT من طلب HTTP. ويمكنك استخدام <a href="https://go.microsoft.com/fwlink/?linkid=2098190" target="_blank">Fiddler</a>. يمكنك إعداد التقاط HTTPS لمشاهدة النقل في بروتوكول HTTPS من العميل. وبعد ذلك، تحتاج إلى رمز JWT لـ Open Authorization ‏(OAuth)، وهو قيمة رأس مصادقة HTTP مع إزالة مقطع الحامل.

كما يمكنك استخدام أداة إلغاء تسلسل لفحص محتويات الرمز المميز. وللقيام بذلك، انتقل إلى <a href="https://go.microsoft.com/fwlink/?linkid=2098441" target="_blank">JWT.io</a> والصق رمز JWT الخاص بك في القسم "الإدخال". بعد ذلك، يمكنك عرض المحتويات كأزواج الاسم-القيمة، ثم تتحقق من صحة المعلومات المعروضة.

استخدم الدليل الآتي للتحقق من المعلومات الخاصة بك:

-   **aud** - يتوافق مع مفهوم الموارد Azure Active Directory (Azure AD). وهناك مشكلتان نموذجيتان تتمثلان في أن المقطع **aud** لرمز JWT يحتوي على معرف موارد موحد (URI) به شرطة مائلة لاحقة أو أن مقطع **aud** يستخدم أحرف كبيرة غير صحيحة.
-   **appid** - يتوافق مع معرف تطبيق Azure AD‏ Native Client، والذي يشار إليه أحياناً باسم "معرف تطبيق Service".
-   **upn** - يتوافق مع المستخدم الذي تتم المصادقة عليه من خلال تطبيق Native Client. 
