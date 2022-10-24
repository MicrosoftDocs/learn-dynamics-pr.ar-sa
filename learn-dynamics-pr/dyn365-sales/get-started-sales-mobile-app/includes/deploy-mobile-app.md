---
ms.openlocfilehash: 2f5d82b68ba3232c9c808711663d35d63ca7a718
ms.sourcegitcommit: c7da060c6aba7e8815ae515d2291e8a818cbba20
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/07/2022
ms.locfileid: "9639399"
---
قبل أن تتمكن من استخدام تطبيق Dynamics 365 Sales للأجهزة المحمولة، ستحتاج إلى إعداد Dynamics 365 Sales وتلبية المتطلبات الأساسية التالية:

-   **ضمان تجربة مثالية للهاتف المحمول:**

    -   تمكين البحث عن الصلة في البيئة. لمزيد من المعلومات، راجع [تكوين بحث Dataverse لبيئتك](/power-platform/admin/configure-relevance-search-organization/?azure-portal=true).

    -   نوصي بأن يكون لديك Exchange Online.

-   **تعيين سجل بخصوص اجتماع:**

    -   تمكين المزامنة من جانب الخادم في بيئتك.
        للحصول على المزيد من المعلومات، راجع [المزامنة على جانب الخادم](/power-platform/admin/server-side-synchronization/?azure-portal=true).

    -   وافق على عنوان البريد الإلكتروني. لمزيد من المعلومات، راجع [الموافقة على صندوق بريد المستخدم](/power-platform/admin/connect-exchange-online?azure-portal=true#approve-mailboxes).

-   **احصل على الأذونات التالية:**

    -   إذن القراءة [لجدول المؤسسة](/dynamics365/customerengagement/on-premises/developer/entities/organization/?azure-portal=true)

    -   إذن القراءة [لجدول صندوق البريد](/dynamics365/customer-engagement/web-api/mailbox?view=dynamics-ce-odata-9&preserve-view=true)

    -   امتياز [Dynamics 365 for Mobile](/dynamics365/mobile-app/set-up-dynamics-365-for-phones-and-dynamics-365-for-tablets?azure-portal=true#required-privileges) 

## <a name="download-and-install-the-application"></a>تنزيل التطبيق وتثبيته

بعد استيفاء جميع المتطلبات الأساسية، ستحتاج إلى تنزيل التطبيق وتثبيته على جهازك المفضل من متجر تطبيقات هذا الجهاز. كما ذكرنا سابقاً، يتم دعم التطبيق حالياً على أجهزة iOS وAndroid. لمزيد من المعلومات، راجع [تثبيت التطبيق على iOS وAndroid](/dynamics365/sales/sales-mobile/install-mobile-app/?azure-portal=true).


> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتطبيق Dynamics 365 Sales في متجر تطبيقات IOS ومتجر تطبيقات Android.](../media/sales-app-home-screen.png)](../media/sales-app-home-screen.png#lightbox)

بعد تثبيت التطبيق على جهازك، وعندما يكون لديك امتيازات الأمان الضرورية المعينة، يمكنك تسجيل الدخول إلى التطبيق. بعد تسجيل الدخول، سيطلب منك تحديد التطبيق الذي تريد تحميله في تطبيق الأجهزة المحمولة. بشكل افتراضي، ستحتوي القائمة على تطبيقات الإنتاج فقط. إذا لم يتم عرض التطبيق الذي تريد تحميله، فمن المحتمل أن يكون تطبيقاً غير إنتاجي.
حدد أيقونة **شريط التمرير** في الزاوية العلوية اليسرى من التطبيق، ثم حدد **إظهار التطبيقات غير الإنتاجية**.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة للخيار إظهار التطبيقات غير المنتجة في عامل التصفية.](../media/nonproduction.png)](../media/nonproduction.png#lightbox)

بعد تحميل التطبيق، سيتم نقلك إلى **تجربة التشغيل الأول**. توفر لك هذه التجربة بعض المعلومات الأساسية حول التطبيق. عندما تصل إلى نهاية **تجربة التشغيل الأولى** حدد **لننطلق** ليتم نقلك إلى الصفحة الرئيسية للتطبيق، كما هو موضح في لقطة الشاشة التالية.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتطبيق Dynamics 365 Sales على واجهة مستخدم هاتف محمول.](../media/operating-systems.png)](../media/operating-systems.png#lightbox)

الآن بعد أن تعرفت على كيفية نشر تطبيق الأجهزة المحمولة، ستتعلم كيفية استخدامه. 
