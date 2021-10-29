---
ms.openlocfilehash: 6271d0ef7c5adc0627b11e2025e4047630928e33
ms.sourcegitcommit: 917d1f0968d01f74c095042b24ba5acfbe111f76
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/26/2021
ms.locfileid: "7582758"
---
ترشدك هذه الوحدة خلال إعداد إصدار تم شراؤه من Fraud Protection. 

## <a name="prerequisites"></a>المتطلبات الأساسية
لإعداد Fraud Protection والتحكم في وصول المستخدم إلى بياناتك، يجب أن يكون لديك مستأجر Azure Active Directory (Azure AD). إذا لم يكن لديك بالفعل مستأجر Azure AD، فيمكنك التسجيل للحصول على واحد.

## <a name="select-the-correct-azure-tenant"></a>تحديد مستأجر Azure الصحيح
سيناريوهات تسجيل الدخول التالية مخصصة للعملاء الذين اشتروا ترخيصاً لـ Fraud Protection.

- عند شراء ترخيص من خلال Microsoft Cloud Solution Provider ‏(CSP)، يحدد CSP مستأجر Azure AD الذي ستستخدمه. لتبدأ مع ذلك المستأجر، انتقل إلى [الوصول إلى حساب Dynamics 365 Fraud Protection الخاص بك](https://dynamics.microsoft.com/ai/fraud-protection/signin/?RU=https%3A%2F%2Fdfp.microsoft.com%2Fsignin/?azure-portal=true)، وقم بتسجيل الدخول باستخدام بيانات اعتماد المسؤول العام.
- إذا اشتريت ترخيصاً من خلال قناة ترخيص مجمع (VL)، فاتبع الإرشادات الواردة في البريد الإلكتروني الذي تلقيته لتنشيط اشتراكك في المستأجر المطلوب. بعد ذلك، للشروع في العمل، انتقل إلى [الوصول إلى حساب Dynamics 365 Fraud Protection الخاص بك](https://dynamics.microsoft.com/ai/fraud-protection/signin/?RU=https%3A%2F%2Fdfp.microsoft.com%2Fsignin/?azure-portal=true)، وقم بتسجيل الدخول باستخدام بيانات اعتماد المسؤول العام.

## <a name="complete-the-setup-process"></a>إكمال عملية الإعداد
لإكمال عملية الإعداد، اتبع الخطوات التالية.

1. انتقل إلى [الوصول إلى حساب Dynamics 365 Fraud Protection الخاص بك](https://dynamics.microsoft.com/ai/fraud-protection/signin/?RU=https%3A%2F%2Fdfp.microsoft.com%2Fsignin/?azure-portal=true)، وقم بتسجيل الدخول كمسؤول عام لمستأجر Azure AD.
1. في الشاشة **التالي** ضمن حقل **جغرافيا تخزين البيانات**، حدد المنطقة الجغرافية حيث تريد تخزين بياناتك، ثم حدد **بدء الإعداد**.
    > [!NOTE]
    > لا يمكنك تغيير قيمة جغرافيا تخزين البيانات بعد تعيينها.

1. تبدأ عملية الإعداد وقد تستغرق بضع دقائق للتشغيل. إذا كنت تفضل ذلك، فيمكنك تسجيل الخروج ثم العودة بعد اكتمال التثبيت.
1. بعد اكتمال الإعداد، ستتم مطالبتك بمراجعة المعلومات المهمة حول قانون الإبلاغ عن الائتمان العادل (FCRA). بعد إكمال المراجعة، حدد **أوافق**.
1. يتم فتح **مدخل Fraud Protection**.

## <a name="configure-access-for-other-users-optional"></a>تكوين الوصول للمستخدمين الآخرين (اختياري)
يوفر Fraud protection التحكم في الوصول المستند إلى الأدوار (RBAC) لتحسين الأمان وإدارة الأدوار. يجب إجراء التكوين الأولي للمستخدمين والأدوار بواسطة المسؤول العام لمستأجر Azure AD. بعد إعداد حساب **AllAreas_Admin**، يمكنك استخدامه لإضافة المزيد من المستخدمين. 

لمزيد من المعلومات حول كيفية تكوين وصول المستخدم، راجع الوحدة التالية.
