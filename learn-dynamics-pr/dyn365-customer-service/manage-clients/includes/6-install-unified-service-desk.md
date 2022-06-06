---
ms.openlocfilehash: 382d574fad19f3e8936c768c4a59c452de976115
ms.sourcegitcommit: 30fe1e3724fe666c25c4096a05197776b33ae54e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/12/2022
ms.locfileid: "8743378"
---
قبل أن تتمكن من تثبيت Unified Service Desk ونشره لـ Dynamics 365، يجب عليك تحديد مثيل تطبيقات Dynamics 365إشراك العملاء الذي تريد إنشاء التكوين ونشره عليه. في حين أنه يمكنك استخدام مثيل جديد، يعمل Unified Service Desk بشكل أفضل عندما يكتمل التخصيص في الغالب. يتحكم Unified Service Desk في طريقة العرض لمندوب مركز الاتصال من خلال معالجة النوافذ وإدخال JavaScript وما إلى ذلك. إذا حدثت تغييرات كبيرة في البيئة بعد نشر Unified Service Desk، فقد يتسبب ذلك في عدم عمل تكوين Unified Service Desk الخاص بك كما هو مطلوب. في حين أن تكوين Unified Service Desk غالباً ما يأتي لاحقاً في عملية التنفيذ، فإن وضع Unified Service Desk في الاعتبار عند تصميم بيئتك أمر مفيد.

يتم تثبيت ونشر Unified Service Desk على مراحل حيث تقوم في البداية بإعداد بيئة تطوير لتكوين تطبيقات المندوب باستخدام أحد نماذج تطبيقات Unified Service Desk كأساس. بعد ذلك، يمكنك اختبار كيفية ظهور التكوينات الخاصة بك والعمل باستخدام تطبيق عميل Unified Service Desk من خلال الاتصال بالمثيل الذي قمت بتكوين Unified Service Desk داخله.

بعد ذلك، يمكنك استخدام تكوين Unified Service Desk المخصص في مثيل إنتاج وتطبيق العميل. يتضمن التكوين حزمة ملفات التخصيص المستخدمة لتوزيع أي ملفات وعمليات تجميع مطلوبة على أجهزة كمبيوتر مندوبك.

### <a name="installation-process"></a>عملية التثبيت

تأكد من أن جهاز الكمبيوتر لديك يلبي جميع المتطلبات قبل تثبيت تطبيق عميل Unified Service Desk. مزيد من المعلومات: [متطلبات نظام Unified Service Desk](/dynamics365/unified-service-desk/admin/unified-service-desk-system-requirements/?azure-portal=true)

قُم [بتنزيل](/dynamics365/unified-service-desk/download-unified-service-desk/?azure-portal=true) ملف إعداد عميل Unified Service Desk المناسب (.exe) واحفظه على جهاز الكمبيوتر:

- لإصدار 32 بت من Windows، قُم بتنزيل ملف Dynamics 365-USD-3.xxxxx-i386.exe.

- لإصدار 64 بت من Windows، قُم بتنزيل ملف Dynamics 365-USD-3.x.x.xxx-amd64.exe file.

### <a name="install-the-unified-service-desk-client-using-the-setup-wizard"></a>تثبيت عميل Unified Service Desk باستخدام معالج الإعداد

1. قُم بتسجيل الدخول كمستخدم لديه عضوية مجموعة المسؤولين المحليين، ثم انقر نقراً مزدوجاً فوق الملف الذي تم تنزيله لبدء الإعداد.

2. يبدأ تشغيل مثبت عميل Unified Service Desk تلقائياً. إذا لم يحدث ذلك، فانتقل إلى المجلد حيث توجد ملفات التثبيت المستخرجة وقم بتشغيل ملف SetupUnifiedServiceDesk.exe لبدء التثبيت.

3. في شاشة **Microsoft Dynamics 365إشراك العملاء apps Unified Service Desk** ، احتفظ بالموقع الافتراضي أو أدخل المسار الكامل حيث سيتم تثبيت ملفات تطبيق عميل Unified Service Desk، ثم انقر فوق  **التالي**.

4. في شاشة **تثبيت Unified Service Desk لتطبيقات Microsoft Dynamics 365 Customer** ‎‏‎، اختر من بين الخيارات التالية:

    - Microsoft .NET Framework والمتطلبات الأساسية لـ Windows Identity Foundation. لا يمكنك إزالة هذه من التثبيت إذا لم تكن هذه المتطلبات الأساسية مثبتة بالفعل.
    - **Unified Service Desk**. نظراً لأن Unified Service Desk هو المكون الأساسي للإعداد، فلا يمكنك المتابعة ما لم يتم تحديده.
    - **إنشاء اختصار لـ Unified Service Desk على سطح المكتب**. بشكل افتراضي، سيتم إنشاء اختصار لسهولة تشغيل عميل Unified Service Desk من سطح المكتب.

1. انقر فوق **تثبيت**.

2. تُظهر الشاشة التالية حالة التثبيت لعميل Unified Service Desk. عندما يُطلب منك تخويل التثبيت (نتيجة التحكم في حساب المستخدم)، انقر فوق **نعم**.

3. تظهر رسالة تأكيد عند نجاح تثبيت عميل Unified Service Desk. انقر فوق **X** للخروج من المثبت أو انقر فوق **تشغيل** لبدء عميل Unified Service Desk.

### <a name="upgrade-the-unified-service-desk-client-using-the-setup-wizard"></a>ترقية عميل Unified Service Desk باستخدام معالج الإعداد

1. على جهاز كمبيوتر مثبت عليه إصدار سابق من عميل Unified Service Desk، قُم بتسجيل الدخول إلى الكمبيوتر كمستخدم لديه عضوية مجموعة المسؤولين المحليين، ثم انقر نقراً مزدوجاً فوق ملف SetupUnifiedServiceDesk.exe لبدء الترقية.

2. عندما يكتشف الإعداد الإصدار السابق من عميل Unified Service Desk، سترى المعلومات التالية: **تم بالفعل تثبيت إصدار أقدم من Unified Service Desk على جهاز الكمبيوتر لديك. سيقوم برنامج الإعداد بترقية Unified Service Desk على جهاز الكمبيوتر لديك**.

3. انقر فوق **التالي**.

4. على شاشة ترقية Unified Service Desk، حدد ما إذا كنت تريد إنشاء اختصار لعميل Unified Service Desk.

5. تُظهر الشاشة التالية حالة التثبيت لعميل Unified Service Desk.

6. تظهر رسالة تأكيد عند نجاح ترقية عميل Unified Service Desk. انقر فوق **X** للخروج من المثبت أو انقر فوق **تشغيل** لبدء عميل Unified Service Desk.

### <a name="install-or-upgrade-the-unified-service-desk-client-in-silent-mode"></a>تثبيت أو ترقية عميل Unified Service Desk في وضع السكون

عند تشغيل إعداد Unified Service Desk في وضع السكون، لا يتم عرض أي واجهة مستخدم (UI). بدلاً من ذلك، تقوم بتوفير المعلومات المطلوبة في موجه الأوامر.

> [!Note]
> قد يُطلب منك تقديم المعلومات بسبب إعدادات التحكم في حساب المستخدم بالكمبيوتر. لمنع هذه الرسالة عند تشغيل الإعداد، اضبط إعدادات التحكم في حساب المستخدم على **عدم الإعلام**. بعد اكتمال الإعداد، نوصيك بإعادة تعيين إعدادات التحكم في حساب المستخدم إلى مستوى الإخطار الأصلي.

- عند تثبيت .NET Framework كجزء من إعداد عميل Unified Service Desk، قد يلزم إعادة التشغيل لمتابعة الإعداد.

### <a name="command-line-syntax"></a>بناء جملة سطر الأوامر

'SetupUnifiedServiceDesk.exe [الوجهة] [اختصار = [y | n] / S] [تثبيت/إزالة تثبيت/تعليمات]'

|  **المعلمة**            | **الوصف**                                           |
|  -------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|  تثبيت                  | يُثبت أو، في حالة وجود إصدار سابق، يرقي عميل Unified Service Desk.|
|  إزالة تثبيت                | إزالة تثبيت عميل Unified Service Desk. هذا هو خيار وضع الصيانة الذي يتوفر فقط عندما يكون التطبيق مثبتاً بالفعل.|
|  التعليمات                     | يعرض معلومات حول الإعداد، مثل المعلمات المعتمدة والاستخدام.|
|  /S                       | وضع السكون. لا يتم عرض واجهة مستخدم الإعداد.|
|  الوجهة              | المجلد حيث سيتم تثبيت ملفات عميل Unified Service Desk. بشكل افتراضي، يتم تثبيت USD في مجلد USD لتطبيقات Microsoft Dynamics 365إشراك العملاء في ملفات c:program.|
|  الاختصار = [y/n]         | =y تنشئ اختصارًا لتطبيق Unified Service Desk على سطح مكتب المستخدم. إذا لم تقم بتعيين هذه المعلمة، فسيتم تعيين الاختصار افتراضياً على y. عند تحديد اختصار =n، لا يتم إنشاء اختصار.|
|  التعليمات                     | تُظهر قائمة بالمعلمات الصالحة. |

### <a name="examples"></a>أمثلة

يقوم هذا المثال بتثبيت أو ترقية عميل Unified Service Desk في وضع السكون، وإنشاء اختصار على سطح المكتب.

*تثبيت SetupUnifiedServiceDesk.exe الاختصار=y /S*

يقوم هذا المثال بإزالة تثبيت عميل Unified Service Desk. لاحظ أنه لا يتم عرض أي واجهة مستخدم، حتى في حالة عدم استخدام المعلمة /S.

*إزالة تثبيت SetupUnifiedServiceDesk.exe*

### <a name="next-step"></a>الخطوة التالية

قُم بنشر حزم نماذج Unified Service Desk على Dynamics 365 Server. لمزيد من المعلومات، راجع  [نشر حزم Unified Service Desk على خادم تطبيقات Dynamics 365إشراك العملاء باستخدام Package Deployer](/dynamics365/unified-service-desk/admin/deploy-sample-unified-service-desk-applications-using-package-deployer/?azure-portal=true).

### <a name="troubleshooting--unified-service-desk-client-setup-setupunifiedservicedeskexe-hangs-after-you-click-install"></a>استكشاف الأخطاء وإصلاحها- يتوقف إعداد عميل Unified Service Desk ‏(SetupUnifiedServiceDesk.exe) بعد النقر فوق تثبيت

يمكن أن يحدث هذا عند تشغيل الإعداد كمستخدم ليس لديه عضوية مجموعة المسؤولين المحليين، باستخدام "تشغيل كمستخدم آخر"، وعندما يتم تغيير بعض إعدادات التحكم في حساب المستخدم (UAC) في Windows من الإعداد الافتراضي، على سبيل المثال، إذا تم تعيين إعداد التحكم في حساب المستخدم **وضع موافقة المسؤول لحساب المسؤول المضمّن** على **معطل** على الكمبيوتر المحلي حيث يتم تشغيل الإعداد. بشكل افتراضي، يتم تمكين وضع موافقة المسؤول لحساب المسؤول المضمّن، ولكن يمكن تعطيله من خلال تغيير نهج المجموعة.
