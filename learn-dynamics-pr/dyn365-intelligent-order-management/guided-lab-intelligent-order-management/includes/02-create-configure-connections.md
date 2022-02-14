---
ms.openlocfilehash: ea1f678c7019842c4e52405a7a92ca7045b93120
ms.sourcegitcommit: 28b5b81155de28693455114a5fc5941cb314c9ef
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/31/2022
ms.locfileid: "8075790"
---
تصف هذه الوحدة الخطوات المطلوبة لإنشاء الاتصالات وتكوينها في Dynamics 365 Intelligent Order Management.

## <a name="create-platform-power-automate-connections"></a>إنشاء اتصالات النظام الأساسي Power Automate

انتقل إلى https://flow.microsoft.com/ وسجل دخولك. تأكد من وجودك في بيئة Intelligent Order Management التجريبية الصحيحة. للتأكد من البيئة التي أنت موجود فيها، حدد أيقونة **البيئة** على الزاوية العلوية اليسرى من مدخل Power Automate، وحدد اسم البيئة التي تم تعيينها لك أثناء التسجيل.

### <a name="create-dataverse-connection"></a>إنشاء اتصال Dataverse

لإنشاء اتصال Dataverse، اتبع هذه الخطوات.

1. انتقل إلى **البيانات \> الاتصالات‏‎**.
1. حدد **اتصال جديد**.
1. في مربع البحث في الزاوية العلوية اليسرى، أدخل "Dataverse".
1. حدد رمز علامة الجمع "**+**" لإنشاء اتصال Dataverse. عند مطالبتك بتسجيل الدخول، تأكد من استخدام بيانات الاعتماد نفسها التي استخدمتها لتسجيل الدخول إلى Intelligent Order Management.

### <a name="create-power-automate-connection"></a>إنشاء اتصال Power Automate

لإنشاء اتصال Power Automate، اتبع هذه الخطوات.

1. انتقل إلى **البيانات \> الاتصالات‏‎**.
1. حدد **اتصال جديد**.
1. في مربع البحث في الزاوية العلوية اليسرى، أدخل " إدارة Power Automate".
1. حدد رمز علامة الجمع "**+**" لإنشاء اتصال Power Automate. عند مطالبتك بتسجيل الدخول، تأكد من استخدام بيانات الاعتماد نفسها التي استخدمتها لتسجيل الدخول إلى Intelligent Order Management.

### <a name="create-intelligent-order-management-data-transformer-connection"></a>إنشاء اتصال محول بيانات Intelligent Order Management

لإنشاء اتصال محول بيانات Intelligent Order Management، اتبع هذه الخطوات.

1. انتقل إلى **البيانات \> الاتصالات‏‎**.
1. حدد **اتصال جديد**.
1. في مربع البحث في الزاوية العلوية اليسرى، أدخل "محول بيانات IOM".
    > [!NOTE]
    > إذا لم تتمكن من رؤية الموصل، فيمكنك إلحاق ``?addConnectorHideKey=iomtransforme`` بعنوان URL.
1. حدد رمز علامة الجمع "**+**" لإنشاء اتصال محول بيانات Intelligent Order Management. عند مطالبتك بتسجيل الدخول، تأكد من استخدام بيانات الاعتماد نفسها التي استخدمتها لتسجيل الدخول إلى Intelligent Order Management.

## <a name="configure-platform-connection-references"></a>تكوين مراجع اتصال النظام الأساسي

> [!NOTE]
> ستحتاج إلى تكوين ثلاثة مراجع لاتصال النظام الأساسي Dataverse، ولكن يمكنك استخدام اتصال Dataverse نفسه الذي تم إنشاؤه في وقت سابق لمراجع الاتصال الثلاثة كلها.

لتكوين مراجع اتصال النظام الأساسي‬ اتبع هذه الخطوات.

1.  في شاشة **الترحيب والشروع في العمل** في Intelligent Order Management، حدد **تكوين الإعدادات \> إدارة**.
1.  لكل مرجع اتصال، قم بما يلي:
    1. حدد مرجع الاتصال.
    1. انتقل إلى [مدخل Power Automate](https://powerautomate.microsoft.com/). 
    1. لاسترداد عنوان URL للاتصال، حدد الاتصال المناظر للانتقال إلى صفحة الاتصال المحدد هذا، ثم انسخ عنوان URL. على سبيل المثال، إذا كنت تعمل على إعداد محول بيانات Intelligent Order Management، فستحتاج إلى تحديد اتصال **محول بيانات IOM** على صفحة اتصال Power Automate ثم نسخ عنوان URL لصفحة اتصال محول بيانات Intelligent Order Management من شريط العناوين في المستعرض.
    1. عد إلى صفحه مرجع اتصال النظام الأساسي Intelligent Order Management المقابل والصق عنوان URL المنسوخ في حقل **عنوان URL للاتصال**.
1. حدد **تنشيط النظام**. 