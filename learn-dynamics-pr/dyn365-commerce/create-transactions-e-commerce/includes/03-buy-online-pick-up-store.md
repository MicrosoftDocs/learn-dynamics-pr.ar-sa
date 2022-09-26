---
ms.openlocfilehash: 91d69d4aeb26330aeca2265ca4efe9da42661275
ms.sourcegitcommit: 25d64783ca6b8521eb4960df6ceee686e1d8a2b2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/02/2022
ms.locfileid: "9404137"
---
يجب تطبيق بعض المتطلبات الأساسية لتتمكن من الشراء عبر الإنترنت والاستلام في المتجر (BOPIS):

- تتطلب سيناريوهات BOPIS التي تتضمن الدفع بالبطاقة المدينة محطة أجهزة. تم تضمين محطة الأجهزة في Store Commerce لعملاء Windows وAndroid. إذا كنت تستخدم Store Commerce للمتصفحات أو نقطة البيع لنظام iOS، فيجب إقران عميل Store Commerce بمحطة أجهزة مشتركة. 
- قم بتمكين الخيار **استخدام محطة الأجهزة** في Store Commerce لـ Windows.
- قبل تسجيل الدخول إلى Store Commerce، تأكد من أن حساب Microsoft Azure Active Directory (Azure AD) الذي تستخدمه مرتبط بالعامل الذي قام بتسجيل الدخول.‬

لقد تعلمت سابقاً كيفية إنشاء أمر الاستلام ومزامنته مع المركز الرئيسي لـ Commerce.

للتعامل مع هذا الأمر الذي سيتم استلامه في المتجر، اتبع هذا الإجراء:
 
1. سجّل الدخول إلى Store Commerce (متجر التجارة لنظام Windows أو متجر التجارة للمتصفحات) وحدد **أوامر الالتقاط**.

    [ ![لقطة شاشة للإجراء "الأوامر المطلوب استلامها" في Dynamics 365 Commerce.](../media/orders-pick-up-ss.jpg) ](../media/orders-pick-up-ss.jpg#lightbox)
    
2. حدد الأمر المطلوب استلامه (1)، ثم حدد **استلام** (2)، كما هو موضح في لقطة الشاشة التالية.

    [ ![لقطة شاشة لإجراء الاستلام في Dynamics 365 Commerce.](../media/pick-up-ss.jpg) ](../media/pick-up-ss.jpg#lightbox)
    
3. حدد الصنف المراد استلامه، ثم حدد **طرق الدفع** لإكمال الحركة.

    [ ![لقطة شاشة للإجراء "طرق الدفع" في Dynamics 365 Commerce.](../media/payment-methods-ss.jpg) ](../media/payment-methods-ss.jpg#lightbox) 

