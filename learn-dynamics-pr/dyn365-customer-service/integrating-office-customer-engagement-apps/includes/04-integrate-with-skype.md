---
ms.openlocfilehash: daa71e5c8f676b0f81ba1032fcfb2c18db607290
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7325611"
---
إذا كانت مؤسستك تستخدم Skype for Business أو Skype، فيمكنك الاستفادة من ميزات الاتصال مثل النقر للاتصال أو التحقق من توفر المستخدم من داخل تطبيقات Dynamics 365 Customer Engagement أو Microsoft Dynamics 365 for Outlook. 

### <a name="prerequisites"></a>المتطلبات الأساسية

يجب أن يكون لدى مؤسستك أحد المنتجات أو الاشتراكات التالية:

- Skype for Business

- Skype for Business Server 2015

- Lync Server 2013

- Lync Server 2010

### <a name="client-requirements-and-dynamics-365-configuration"></a>متطلبات العميل وتكوين Dynamics 365

- لاستخدام **انقر للاتصال**، يجب تحديد Skype for Business كموفر خدمة الهاتف في تطبيقات Dynamics 365 Customer Engagement. يمكنك تعيين هذا في **علامة التبويب عام** في **الإعدادات &gt; الإدارة &gt; إعدادات النظام**.

- بشكل افتراضي، يتم تمكين وجود Skype for Business في تطبيقات Dynamics 365 Customer Engagement. يمكن لمسؤولي النظام تمكين أو تعطيل التواجد في تطبيقات Dynamics 365 Customer Engagement. للقيام بذلك، انقر فوق **إعدادات &gt; الإدارة &gt; إعدادات النظام** وفي **علامة التبويب عام**، قم بتعيين IM خيار التواجد إلى "نعم" أو "لا".

- يجب أن يكون لدى كل مستخدم عميل Skype for Business مثبتاً وقيد التشغيل على أجهزة الكمبيوتر الخاصة به.

### <a name="click-to-call"></a>اضغط للاتصال

![لقطة شاشة تعرض رمز الهاتف بجوار رقم هاتف في Dynamics 365](../media/Skype_for_Business_and_Skype_image1.png)

عند استخدام "انقر للاتصال" لأول مرة، ستتم مطالبتك بما تريد حدوثه عند النقر فوق رمز رقم الهاتف. (ستختلف العناصر الموجودة في هذه القائمة بناءً على التطبيقات الموجودة على جهاز الكمبيوتر الخاص بك). حدد البرنامج المفضل لديك لإجراء المكالمات، وفي هذه الحالة سأحدد Skype for Business.

![لقطة شاشة تعرض الفتح مع الخيارات في نافذة منبثقة](../media/Skype_for_Business_and_Skype_image2.png)

بعد ذلك تفتح نافذة Skype for Business مما يسمح لك بالنقر للاتصال.

![لقطة شاشة تعرض نافذة Skype مفتوحة الآن للاتصال](../media/Skype_for_Business_and_Skype_image3.png)

### <a name="presence"></a>متواجد

يُشار إلى التحقق من توفر شخص ما على أنه حالة "متواجد" ويستخدم Skype for Business أيقونات ملونة لعرض ذلك.

![لقطة شاشة تعرض الحالات المختلفة لمستخدم Skype for Business](../media/Skype_for_Business_and_Skype_image4.png)

للحصول على معلومات إضافية، الرجاء مراجعة [تكامل Skype for Business وSkype](/dynamics365/customerengagement/on-premises/admin/skype-business-integration) و [إعداد تطبيقات (عبر الإنترنت) لاستخدام Skype أو Skype for Business](/dynamics365/customer-engagement/admin/set-up-skype-or-skype-for-business). 
