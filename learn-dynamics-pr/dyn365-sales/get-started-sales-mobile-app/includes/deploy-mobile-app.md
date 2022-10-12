---
ms.openlocfilehash: 31a7c485396b9c42b12b6bab9df00a31650b05c8
ms.sourcegitcommit: b553b85e16cc744acb7223ab5348070f6e26a4fe
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/21/2022
ms.locfileid: "9567438"
---
قبل ان تتمكن من استخدام تطبيق Sales للأجهزة المحمولة، يجب إعداد Dynamics 365 Sales وتلبية المتطلبات الأساسية التالية:

-   **للحصول على التجربة المثلى على الأجهزة المحمولة:**

    -   يجب تمكين بحث الصلة في البيئة. للحصول على المزيد من المعلومات، راجع [تكوين بحث الصلة لتحسين نتائج البحث والأداء](/power-platform/admin/configure-relevance-search-organization/?azure-portal=true).

    -   من المستحسن أن يكون لديك Exchange Online.

-   **لتعيين سجل "بخصوص" لاجتماع:**

    -   يجب عليك تمكين المزامنة على جانب الخادم في بيئتك. 
        للحصول على المزيد من المعلومات، راجع [المزامنة على جانب الخادم](/power-platform/admin/server-side-synchronization/?azure-portal=true).

    -   وافق على عنوان البريد الإلكتروني. للحصول على المزيد من المعلومات، راجع 
        [الموافقة على صناديق البريد](/power-platform/admin/connect-exchange-online?azure-portal=true#approve-mailboxes).

-   **يجب أن تتوفر الأذونات التالية لدى مستخدمي تطبيق الأجهزة المحمولة:**

    -   إذن القراءة في [جدول المؤسسة](/dynamics365/customerengagement/on-premises/developer/entities/organization/?azure-portal=true).

    -   إذن القراءة في[جدول صندوق البريد](/dynamics365/customer-engagement/web-api/mailbox?view=dynamics-ce-odata-9&preserve-view=true).

    -   [امتياز Dynamics 365 for mobile](/dynamics365/mobile-app/set-up-dynamics-365-for-phones-and-dynamics-365-for-tablets?azure-portal=true#required-privileges) .

## <a name="download-and-install-the-application"></a>تنزيل التطبيق وتثبيته

بعد تلبية جميع المتطلبات الأساسية، سيحتاج البائعون الميدانيون إلى تنزيل التطبيق وتثبيته على جهازهم المفضل من متجر تطبيقات ذلك الجهاز. كما ذكرنا سابقاً، التطبيق مدعوم حالياً على أجهزة IOS وAndroid على حدٍ سواء. للحصول على المزيد من المعلومات حول الحد الأدنى من متطلبات الجهاز ومتطلبات الجهاز الموصى بها، راجع [تثبيت التطبيق على iOS وAndroid](/dynamics365/sales/sales-mobile/install-mobile-app/?azure-portal=true).


> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتطبيق Dynamics 365 Sales في متجر تطبيقات IOS ومتجر تطبيقات Android.](../media/sales-app-home-screen.png)](../media/sales-app-home-screen.png#lightbox)

بعد تثبيت التطبيق على جهاز المندوب وبعد حصول المندوب على امتيازات الأمان اللازمة المعينة له، بإمكان البائع الميداني تسجيل الدخول إلى التطبيق. بعد أن تسجل دخولك، سيُطلب منك تحديد التطبيق الذي تريد تحميله في تطبيق الأجهزة المحمولة. ستحتوي القائمة على تطبيقات إنتاجية فقط، بشكل افتراضي. إذا لم تتمكن من رؤية التطبيق الذي تريد تحميله، فمن المحتمل أن يكون تطبيقاً غير إنتاجي.
حدد أيقونة **شريط التمرير** في الزاوية العليا اليسرى من التطبيق، ثم اختر **إظهار التطبيقات غير الإنتاجية‬‏‫**.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة للتطبيقات غير الإنتاجية في عامل التصفية.](../media/nonproduction.png)](../media/nonproduction.png#lightbox)

بعد تحميل التطبيق، سيتم نقلك إلى **تجربة التشغيل الأول**. سيؤدي ذلك إلى تزويدك ببعض المعلومات الأساسية حول التطبيق. عندما تصل إلى نهاية **تجربة التشغيل الأول**، حدد **هيا بنا** كي يتم نقلك إلى الصفحة الرئيسية للتطبيقات كما يظهر أدناه.

> [!div class="mx-imgBorder"]
> [![لقطة شاشة لتطبيق Dynamics 365 Sales على واجهة مستخدم هاتف خلوي.](../media/operating-systems.png)](../media/operating-systems.png#lightbox)

الآن بعد أن تعرفنا على كيفية نشر تطبيق الأجهزة المحمولة، دعنا نراجع كيفية استخدامه. 
