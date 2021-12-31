---
ms.openlocfilehash: 23c9e4c794344659afe497229c0f1736b32075f7
ms.sourcegitcommit: 1d9dbd81b128041197540f8687181cc789626fc2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2021
ms.locfileid: "7900531"
---
تصف هذه الوحدة النمطية كيفية تمكين المجموعة الكاملة من ميزات Microsoft Dynamics 365 Fraud Protection عن طريق إرسال بيانات الحركات إلى واجهات برمجة التطبيقات (API) في الوقت الحقيقي. تعمل إمكانيات حماية الحساب وحماية المشتريات‬ في Dynamics 365 Fraud Protection في الوقت الحقيقي. 

وبحسب الطريقة التي تختارها لاستخدام Fraud Protection، يمكنك استخدام مجموعات مختلفة من واجهات API:

- **واجهات API لحماية المشتريات** - ‏Purchase وPurchaseStatus وBankEvent وChargeback وRefund وUpdateAccount وLabel
- **واجهات API لحماية الحساب** - ‏AccountCreate وAccountCreateStatus وAccountLogin وAccountLoginStatus وAccountUpdate وLabel

تستخدم ميزة Dynamics 365 Fraud Protection وضعي تشغيل:

- تجربة *التقييم‏‎*، التي تمكّنك من تحليل نتائج استخدام Dynamics 365 Fraud Protection في تكوين اختبار. 
- تجربة *الحماية*، التي تمكّنك من مراعاة القرارات بالاستناد إلى القواعد التي قمت بإعدادها. استخدم وضع *الحماية* فقط إذا كان لديك ترخيص مدفوع. 

> [!NOTE]
> لاختبار المنتج، استخدم البيئة في وضع *التقييم* فقط. 

تعاون مع مسؤول مستأجر Microsoft Azure لإعداد تطبيق Microsoft Azure Active Directory (Azure AD) بواسطة الأدوار التي يمكنك استخدامها للحصول على رمز مميز وإرسال الطلبات إلى Dynamics 365 Fraud Protection. لمزيد من المعلومات، راجع الوحدة **الحصول على رمز مميز لـ Azure AD** لاحقاً في هذه الوحدة النمطية.

لمزيد من المعلومات حول جميع الأحداث المدعومة، راجع واجهة API في [Dynamics 365 Fraud Protection](/fraud-protection-rest/api/fraud-protection-rest/?azure-portal=true). 
 
## <a name="prerequisites"></a>المتطلبات الأساسية

المتطلبات الأساسية التي تحتاج إليها لإكمال هذه الوحدة النمطية هي:

- **الوصول إلى مدخل Dynamics 365 Fraud Protection** - تنشئ ميزة Fraud Protection جميع التفاصيل المطلوبة لإنشاء رمز مميز واستدعاء بيئتك في Dynamics 365 Fraud Protection. وبالتالي، ستحتاج إلى الوصول إلى لوحة معلومات مدخل Dynamics 365 Fraud Protection. ستستخدم المعلومات من لوحة المعلومات لإعداد استدعاءات واجهة API وعينة تطبيق، كما هو موضح في الأقسام التالية من هذا المستند. 

- **تنزيل عميل Postman (أو أي عميل آخر من اختيارك)** - ستحتاج إلى عميل Postman (أو أي عميل آخر من اختيارك)، على جهازك الذي ستستخدمه لورشة العمل هذه. ستستخدم Postman (أو أي عميل آخر من اختيارك) للحصول على الرموز المميزة لاستدعاء واجهات API. بعد إنشاء الرمز المميز، ستستخدم العميل لاستدعاء واجهات API لـ Dynamics 365 Fraud Protection. 
 
في حال عدم وجود عميل مثبت على جهازك، يمكنك تنزيل تطبيق Postman من [تنزيل Postman](https://www.postman.com/downloads/?azure-portal=true).
