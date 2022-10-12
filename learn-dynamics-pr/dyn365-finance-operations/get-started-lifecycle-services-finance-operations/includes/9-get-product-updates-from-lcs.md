---
ms.openlocfilehash: 35f5401b4bbcc89b3b9e2ac04e438f775813f4cd
ms.sourcegitcommit: c1858cd3b2bd6663edff36e214795d4934ad3ddf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2022
ms.locfileid: "9580978"
---
بدلاً من تطبيق تحديثات منفصلة لإصدار التطبيق وتحديث آخر لإصدار النظام الأساسي، سيتم تحديثهما في نفس الوقت لتحديثات عمليات التوزيع السحابية في Dynamics 365. تسمى هذه الميزة تحديث خدمة الإصدار الواحد.

في Lifecycle Services، يمكنك إدارة التحديثات المستمرة لمثيل تطبيقات التمويل والعمليات. يوجد [وتيره إصدار](/dynamics365/fin-ops-core/fin-ops/get-started/public-preview-releases?azure-portal=true#release-cadence) لهذه التحديثات يتم توفيرها بواسطة Microsoft.

يمكن تطبيق التحديثات تلقائياً بواسطة Microsoft، أو تحديثها يدوياً بواسطة العميل، طالما أن الجدول يتوافق مع الإطار الزمني حيث تصدر Microsoft هذا الإصدار المحدد من [تحديث الخدمة](/dynamics365/fin-ops-core/fin-ops/get-started/public-preview-releases/?azure-portal=true).

يمكنك اختبار الميزات الجديدة مقدماً، باستخدام برنامج المعاينة للوصول المبكر (PEAP)، حيث يمكنك الحصول على آخر تحديث شهري متاح قبل حالة التثبيت مباشرة. يمكنك التسجيل في برنامج PEAP بالانضمام إلى برنامج Insider المتاح على [تجربة Dynamics 365](https://experience.dynamics.com/?azure-portal=true). بعد قبول طلبك، ستنضم إلى البرنامج وستتمكن من تمكين الميزات في الإصدار الأولي، قبل أن تصبح متاحة بشكل عام.

يمكنك إدارة الميزات الجديدة من مساحة العمل **إدارة الميزات** في تطبيقات التمويل والعمليات. لمزيد من المعلومات حول كيفية استخدام مساحة عمل **إدارة الميزات**، راجع [نظرة عامة على إدارة الميزات](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview/?azure-portal=true).

## <a name="continuous-update-settings"></a>إعدادات التحديث المستمر

يمكن للعملاء تحديد نافذة الصيانة، بناءً على قيود أعمالهم. في Lifecycle Services، استخدم الحقول الموجودة في قسم **وتيرة تحديث بيئة الإنتاج** في علامة التبويب **إعدادات التحديث** في صفحة **إعدادات المشروع**، كما هو موضح في الصورة التالية. يتوفر تقويم للتحديثات القادمة لمساعدتك في التخطيط.

[![لقطة شاشة لعلامة التبويب "إعداد التحديث" في صفحة إعدادات المشروع.](../media/update-settings.jpg)](../media/update-settings.jpg#lightbox)

ويمكن للعملاء إيقاف التحديث مؤقتًا أو تأخيره أو إلغاء الاشتراك فيه باستخدام **إعدادات التحديث** في مشروعات Lifecycle Services، لما يصل إلى ثلاثة تحديثات متتالية.

وسيتلقون إعلامات بالتحديثات القادمة في Lifecycle Services، قبل خمسة أيام، وفقًا لإعداداتهم. وإذا أرادوا التحديث يدوياً، فعليهم الانتقال إلى **تفاصيل البيئة**، ثم في القائمة **صيانة**، حدد **تطبيق التحديثات**.

يمكن للعملاء التحقق من صحة التحديثات في بيئة الاختبار المعزولة، قبل تحديث الإنتاج، باستخدام [Regression Suite Automation Tool (RSAT)](/dynamics365/fin-ops-core/dev-itpro/perf-test/rsat/rsat-overview/?azure-portal=true)، حيث يمكنك إنشاء حالات اختبار متعددة وتشغيلها تلقائياً للتحقق من تطبيق التحديثات بنجاح.

لمزيد من المعلومات، راجع [نظرة عامة على تحديثات خدمة الإصدار الواحد](/dynamics365/fin-ops-core/dev-itpro/lifecycle-services/oneversion-overview?azure-portal=true&toc=/dynamics365/commerce/toc.json).
