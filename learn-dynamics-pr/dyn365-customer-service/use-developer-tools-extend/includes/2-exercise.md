---
ms.openlocfilehash: 0e4672624248f0aad80e1630a89cb458659227fd
ms.sourcegitcommit: 52cf5c51cdbfce3ce4662656a5d311e3ca98cade
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2021
ms.locfileid: "7605447"
---
في هذا التمرين، ستقوم بتثبيت بعض أدوات المطور من NuGet.

> [!IMPORTANT]
> استخدام بيئة اختبار مع توفير Microsoft Dataverse. وإذا لم يتوفر لديك، يمكنك الاشتراك في [خطة المجتمع](https://powerapps.microsoft.com/communityplan/?azure-portal=true).

## <a name="task-1-install-developer-tools"></a>المهمة 1: تثبيت أدوات المطور

في هذه المهمة، ستستخدم برنامج PowerShell نصي لتثبيت أدوات من NuGet.

1.  وفي قائمة "بدء تشغيل Windows، اكتب **Windows PowerShell** وافتحه.

1.  انتقل إلى المجلد الذي تريد تثبيت الأدوات إليه. على سبيل المثال، إذا كنت تريد تثبيتها في المجلد devtools على محرك الأقراص C لديك، فاكتب **md C:\devtools** لإنشاء هذا المجلد إذا لم يكن موجودًا.

1.  غيّر إلى المجلد الجديد عن طريق كتابة **cd C:\devtools** والضغط على Enter.

1.  انسخ البرنامج النصي PowerShell الآتي والصقه في نافذة PowerShell واضغط على Enter.

    ```powershell
    [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
    $sourceNugetExe = "https://dist.nuget.org/win-x86-commandline/latest/nuget.exe"
    $targetNugetExe = ".\nuget.exe"
    Remove-Item .\Tools -Force -Recurse -ErrorAction Ignore
    Invoke-WebRequest $sourceNugetExe -OutFile $targetNugetExe
    Set-Alias nuget $targetNugetExe -Scope Global -Verbose

    ##
    ##Download Plugin Registration Tool
    ##
    ./nuget install Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool -O .\Tools
    md .\Tools\PluginRegistration
    $prtFolder = Get-ChildItem ./Tools | Where-Object {$_.Name -match 'Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool.'}
    move .\Tools\$prtFolder\tools\*.* .\Tools\PluginRegistration
    Remove-Item .\Tools\$prtFolder -Force -Recurse

    ##
    ##Download CoreTools
    ##
    ./nuget install  Microsoft.CrmSdk.CoreTools -O .\Tools
    md .\Tools\CoreTools
    $coreToolsFolder = Get-ChildItem ./Tools | Where-Object {$_.Name -match 'Microsoft.CrmSdk.CoreTools.'}
    move .\Tools\$coreToolsFolder\content\bin\coretools\*.* .\Tools\CoreTools
    Remove-Item .\Tools\$coreToolsFolder -Force -Recurse

    ##
    ##Download Configuration Migration
    ##
    ./nuget install  Microsoft.CrmSdk.XrmTooling.ConfigurationMigration.Wpf -O .\Tools
    md .\Tools\ConfigurationMigration
    $configMigFolder = Get-ChildItem ./Tools | Where-Object {$_.Name -match 'Microsoft.CrmSdk.XrmTooling.ConfigurationMigration.Wpf.'}
    move .\Tools\$configMigFolder\tools\*.* .\Tools\ConfigurationMigration
    Remove-Item .\Tools\$configMigFolder -Force -Recurse

    ##
    ##Download Package Deployer 
    ##
    ./nuget install  Microsoft.CrmSdk.XrmTooling.PackageDeployment.WPF -O .\Tools
    md .\Tools\PackageDeployment
    $pdFolder = Get-ChildItem ./Tools | Where-Object {$_.Name -match 'Microsoft.CrmSdk.XrmTooling.PackageDeployment.Wpf.'}
    move .\Tools\$pdFolder\tools\*.* .\Tools\PackageDeployment
    Remove-Item .\Tools\$pdFolder -Force -Recurse

    ##
    ##Remove NuGet.exe
    ##
    Remove-Item nuget.exe
    ```
1.  بعد انتهاء البرنامج النصي من التنفيذ، اكتب **Explorer**، كلمة **Explorer** متبوعة بمسافة ونقطة، واضغط على Enter.

1.  من المفترض أن يظهر مجلدًا واحدًا بالاسم **Tools**، فانقر نقرًا مزدوجًا فوق **Tools**.

1.  ويجب أن ترى الآن المجلدات الخمسة الآتية للأدوات المثبتة:

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لمجلدات الأدوات في Explorer.](../media/exercise-1-1.png)](../media/exercise-1-1.png#lightbox)

## <a name="task-2-explore-a-registered-plug-in-with-the-plug-in-registration-tool"></a>المهمة 2: استكشاف مكون إضافي مسجل باستخدام أداة تسجيل المكونات الإضافية

1.  انتقل إلى المجلد **PluginRegistration**.

1.  حدد موقع PluginRegistration.exe في القائمة وانقر نقرًا مزدوجًا فوقها للبدء.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لتحديد موقع تطبيق تسجيل المكون الإضافي في قائمة الملفات.](../media/exercise-1-2.png)](../media/exercise-1-2.png#lightbox)

1.  حدد **إنشاء اتصال جديد**.

1.  تحقق من **عرض قائمة بالمؤسسات المتاحة**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تُظهر إنشاء اتصال جديد والتأكد من عرض قائمة بالمؤسسات المتاحة.](../media/exercise-1-3.png)](../media/exercise-1-3.png#lightbox)

1.  حدد **تسجيل الدخول** وسجِّل الدخول باستخدام بيانات اعتماد بيئة Dataverse عند المطالبة بذلك.

1.  في قائمة المؤسسات (البيئات)، اختر بيئة الاختبار الخاصة بك.

1.  سترى قائمة من المكونات الإضافية للنظام، وإذا قمت بذلك في بيئة باستخدام المكونات الإضافية المخصصة، فستراها في القائمة كذلك. (التجميع) هو ‎.NET DLLs التي تقوم بتطبيق المكونات الإضافية.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تُظهر قائمة المكونات الإضافات في الأداة.](../media/exercise-1-4.png)](../media/exercise-1-4.png#lightbox)

1.  حدد موقع **Microsoft.CDS.ApplicationUser.Plugins** وقم بتوسيعه.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة توضح تحديد موقع مكون إضافي محدد.](../media/exercise-1-5.png)](../media/exercise-1-5.png#lightbox)

1.  يتم تنفيذ كل عنصر من العناصر الفرعية في التجميع. يمكنك توسيع أحد العناصر لرؤية تسجيلات الخطوة لهذا المكون الإضافي الفردي.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تسلط الضوء على خطوة من مكون إضافي.](../media/exercise-1-6.png)](../media/exercise-1-6.png#lightbox)

1. يقوم تسجيل الخطوة بتوصيل المكون الإضافي بوصفه معالج حدث للحدث. في المثال أعلاه، تُعد هذه طريقة معالجة إنشاء على جدول مستخدم التطبيق.

1. انقر نقرًا مزدوجًا فوق الخطوة لرؤية تفاصيل تكوين الخطوة بما في ذلك تعريف الرسالة والكيان ومكان تسجيلها ومرحلة البنية الأساسية التي سيتم فيها استدعاء المكون الإضافي وما إذا كان التنفيذ متزامنًا أو غير متزامن وما إلى ذلك.
    
    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة تعرض خصائص الخطوة.](../media/exercise-1-7.png)](../media/exercise-1-7.png#lightbox)

1. عند إنشاء المكون الإضافي المخصص الخاص بك، ستستخدم هذه الأداة لتحميل التجميع وتسجيل الخطوات للأحداث التي تريد معالجتها.
