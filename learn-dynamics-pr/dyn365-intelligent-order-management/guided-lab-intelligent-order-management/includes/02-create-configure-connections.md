---
ms.openlocfilehash: 3068979f45a91729f6e5640b8273415a57091ba2
ms.sourcegitcommit: 70e51e3ba609b4f9cf6b7a3b2770f4a0916c051a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2022
ms.locfileid: "8091163"
---
تصف هذه الوحدة الخطوات المطلوبة لإنشاء الاتصالات وإعدادها في Dynamics 365 Intelligent Order Management.

## <a name="create-platform-power-automate-connections"></a>إنشاء اتصالات النظام الأساسي Power Automate

انتقل إلى https://flow.microsoft.com/ وسجل دخولك. تأكد من وجودك في بيئة Intelligent Order Management التجريبية الصحيحة. للتأكد من البيئة، حدد أيقونة **البيئة** في الزاوية العلوية اليسرى من مدخل Microsoft Power Automate، وحدد اسم البيئة التي تم تعيينها لك أثناء التسجيل.

### <a name="create-a-dataverse-connection"></a>إنشاء اتصال Dataverse

لإنشاء اتصال Microsoft Dataverse، اتبع هذه الخطوات:

1. انتقل إلى **البيانات > الاتصالات**.
1. حدد **اتصال جديد**.
1. في مربع البحث في الزاوية العلوية اليسرى، أدخل **Dataverse**.
1. حدد رمز علامة الجمع (**+**) لإنشاء اتصال Dataverse. عند مطالبتك بتسجيل الدخول، تأكد من استخدام بيانات الاعتماد نفسها التي استخدمتها عند تسجيل الدخول إلى Intelligent Order Management.

### <a name="create-a-power-automate-connection"></a>إنشاء اتصال Power Automate

لإنشاء اتصال Power Automate، اتبع هذه الخطوات:

1. انتقل إلى **البيانات > الاتصالات**.
1. حدد **اتصال جديد**.
1. في مربع البحث في الزاوية العلوية اليسرى، أدخل **إدارة Power Automate**.
1. حدد رمز علامة الجمع (**+**) لإنشاء اتصال Power Automate. عند مطالبتك بتسجيل الدخول، تأكد من استخدام بيانات الاعتماد نفسها التي استخدمتها عند تسجيل الدخول إلى Intelligent Order Management.

### <a name="create-an-intelligent-order-management-data-transformer-connection"></a>إنشاء اتصال محول بيانات Intelligent Order Management

لإنشاء اتصال محول بيانات Intelligent Order Management، اتبع هذه الخطوات:

1. انتقل إلى **البيانات > الاتصالات**.
1. حدد **اتصال جديد**.
1. في مربع البحث في الزاوية العلوية اليسرى، أدخل **محول بيانات IOM**.
    > [!NOTE]
    > إذا لم يظهر الموصل، فيمكنك إلحاق **``?addConnectorHideKey=iomtransforme``** بعنوان URL.
1. حدد رمز علامة الجمع (**+**) لإنشاء اتصال محول بيانات Intelligent Order Management. عند مطالبتك بتسجيل الدخول، تأكد من استخدام بيانات الاعتماد نفسها التي استخدمتها عند تسجيل الدخول إلى Intelligent Order Management.

## <a name="set-up-platform-connection-references"></a>إعداد مراجع اتصال النظام الأساسي

> [!NOTE]
> ستحتاج إلى إعداد ثلاثة مراجع لاتصال النظام الأساسي Dataverse، ولكن يمكنك استخدام اتصال Dataverse نفسه الذي تم إنشاؤه في وقت سابق لمراجع الاتصال الثلاثة كلها.

لإعداد مراجع اتصال النظام الأساسي‬ اتبع هذه الخطوات:

1.  في شاشة **الترحيب والشروع في العمل** في Intelligent Order Management، حدد **تكوين الإعدادات > إدارة‏‎**.
1.  لكل مرجع اتصال، أكمل الخطوات التالية:
    1. حدد مرجع الاتصال.
    1. انتقل إلى [مدخل Power Automate](https://powerautomate.microsoft.com/). 
    1. لاسترداد عنوان URL للاتصال، حدد الاتصال المناظر للانتقال إلى صفحة الاتصال المحدد هذا، ثم انسخ عنوان URL. على سبيل المثال، إذا كنت تعمل على إعداد محول بيانات Intelligent Order Management، فستحتاج إلى تحديد اتصال **محول بيانات IOM** على صفحة اتصال Power Automate ثم نسخ عنوان URL لصفحة اتصال محول بيانات Intelligent Order Management من شريط العناوين في المستعرض.
    1. عد إلى صفحة مرجع اتصال النظام الأساسي Intelligent Order Management المناظر، ثم الصق عنوان URL المنسوخ في حقل **عنوان URL للاتصال**.
1. حدد **تنشيط النظام**. 
