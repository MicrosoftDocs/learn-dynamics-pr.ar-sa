---
ms.openlocfilehash: 667c643bf8ef573f9b1c09f5f12589dfd7fc5ddc
ms.sourcegitcommit: 8594c8c897c84afee64be07d76b49d8e1ed405e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2022
ms.locfileid: "8771682"
---
يستطيع المطورون استخدام العديد من أدوات التطوير التقليدية عند إنشاء حلول من أجل Microsoft Power Platform. ولكن هناك أدوات متميزة متنوعة تستهدف تطوير Microsoft Power Platform بشكلٍ حصري. توفر Microsoft الأدوات الرسمية عبر [مدير حزمة NuGet](https://nuget.org/?azure-portal=true) وغيرها من مثبتات الأدوات المنشورة. هناك أيضاً مجتمع متألق من الأدوات والمكتبات تُكمل ما تنشره Microsoft. في هذه الوحدة النمطية، سنستكشف الأدوات التي ينبغي أن يكون مطور Microsoft Power Platform على دراية بها.

## <a name="microsoft-power-platform-cli"></a>واجهة سطر الأوامر (CLI) لـ Microsoft Power Platform

Power Platform CLI هي واجهة سطر أوامر لإنشاء مكونات الأكواد. وتهدف CLI إلى أن تكون CLI أساسية بالنسبة للمطورين لتنفيذ عمليات مختلفة. على سبيل المثال، هذه هي الطريقة التي تقوم من خلالها بتهيئة وإدارة دورة حياة مكون Power Apps Component Framework. يمكن كذلك أن تساعد الأداة على تطوير المكونات الإضافية أيضاً. الأداة على دراية بالحل ويمكن أن تساعدك على توزيع ملحقات النظام الأساسي المدعومة في بيئة تطوير للاختبار. يمكن تثبيت CLI [بشكل مستقل](/power-apps/developer/data-platform/powerapps-cli?azure-portal=true#standalone-power-platform-cli) أو باعتبارها [ملحق Visual Studio Code](/power-apps/developer/data-platform/powerapps-cli?azure-portal=true#using-power-platform-tools-for-visual-studio-code). باستخدام الملحقات، يمكن تنفيذ الأوامر من نوافذ الوحدات الطرفية Visual Studio Code.

فيما يلي وصف لبعض المهام الشائعة التي يمكنك القيام بها باستخدام CLI:

|فئة الأمر|الوصف‏‎|
|---| ---|
|المسؤول|   أوامر لميزات دورة حياة البيئة.|
|المصادقة|أوامر مصادقة Dataverse.|
|التطبيق|تعمل أوامر تثبيت تطبيقات AppSource التي تعتبر متطلبات مسبقة للحل في البيئة المستهدفة.|
اللوحة| أوامر للعمل مع ملفات مصدر تطبيق اللوحة.|
المؤسسة|    أوامر للعمل مع بيئات Dataverse.|
الحزمة |أوامر للعمل مع حزم الحلول.|
المدخل|   أوامر للعمل مع مداخل Power Apps.|
PCF|    أوامر للعمل مع Power Apps component framework.|
المكون الإضافي| أمر لإنشاء مشروع مكون إضافي.|
الحل|   أوامر للعمل مع مشاريع حلول Dataverse.|
بيانات تتبع الاستخدام|  إدارة إعدادات بيانات تتبع الاستخدام.|

## <a name="microsoft-power-platform-connectors-cli"></a>واجهة سطر أوامر موصلات Microsoft Power Platform

يوفر موصل CLI أداة سطر الأوامر لإنشاء الروابط المخصصة وتحميلها وتحديثها والتحقق من صحتها. الأداة ضرورية للتحرير المتقدم لتعريف موصل مخصص. يجب أيضاً استخدام الأداة إذا كنت تقوم بإعداد موصل مخصص للمصادر المفتوحة أو الشهادات.

## <a name="application-lifecycle-management-alm-tools"></a>أدوات إدارة دورة حياة التطبيقات (ALM)

هناك جزء مهم من تنفيذ إدارة دورة حياة التطبيقات لمشاريعك وهو وجود عملية قابلة للتكرار تسمح لك بتعديل مكونات الحل وتسجيل هذه التغييرات في نظام تحكم بالمصادر. في حين أن خطوات إنجاز هذه المهام يمكن تنفيذها بطريقة يدوية، إلا أن وجود عملية آلية خيار أفضل لضمان الاتساق والتكرار. لدعم إنشاء هذه الأتمتة، توفر Microsoft مهام إنشاء من أجل Azure DevOps وإجراءات من أجل GitHub.

راجع [القائمة](/power-platform/alm/devops-build-tool-tasks/?azure-portal=true) الكاملة Azure DevOps لمهام الإنشاء للحصول على مزيد من التفاصيل حول كل مهمة.

راجع [القائمة الكاملة](/power-platform/alm/devops-github-available-actions/?azure-portal=true) لإجراءات GitHub للحصول على مزيد من التفاصيل حول كل إجراء.

## <a name="microsoft-nuget-tools-for-dataverse"></a>أدوات Microsoft NuGet من أجل Dataverse

فيما يأتي أدوات Microsoft المتوفرة التي تساعد على مختلف جوانب التطوير عند استخدام Microsoft Dataverse.

| حزمة NuGet                                                | الوصف                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| أداة إنشاء الأكواد [Microsoft.CrmSdk.CoreTools](https://www.nuget.org/packages/Microsoft.CrmSdk.CoreTools/?azure-portal=true) | إنشاء فئات .NET Framework ذات الحد المبكر التي تمثل نموذج بيانات الجدول المستخدم من جانب التطبيقات المستندة إلى النموذج. |
| أداة ترحيل التكوين [Microsoft.CrmSdk.XrmTooling.ConfigurationMigration.Wpf](https://www.nuget.org/packages/Microsoft.CrmSdk.XrmTooling.ConfigurationMigration.Wpf/?azure-portal=true) | الأداة المستخدمة لنقل بيانات التكوين عبر بيئات Dataverse. |
| Package Deployer [Microsoft.CrmSdk.XrmTooling.PackageDeployment.WPF](https://www.nuget.org/packages/Microsoft.CrmSdk.XrmTooling.PackageDeployment.Wpf/?azure-portal=true) | أداة تمكن المسؤولين من توزيع الحزم في بيئة Dataverse. يجمع المطورون بين أصول الحلول والأكواد المخصصة في حزمة لتوزيعها بواسطة Package Deployer. يجب على موردي البرامج المستقلين (ISV) استخدام تنسيق الحزمة نفسه عند إعداد حلولهم لنشرها في AppSource. |
| أداة تسجيل المكونات الإضافية [Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool](https://www.nuget.org/packages/Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool/?azure-portal=true) | أداة مستخدمة لتسجيل تجميعات المكونات الإضافية للأكواد المخصصة والخطوات في بيئة Dataverse. |
| أداة إنشاء حزم الحلول [Microsoft.CrmSdk.CoreTools](https://www.nuget.org/packages/Microsoft.CrmSdk.CoreTools/?azure-portal=true) | أداة يمكنها تفكيك حلول Dataverse إلى ملفات XML متعددة لإدارتها بواسطة نظام تحكم بالمصادر.   كما يمكن استخدامه لإعادة إنشاء حل Dataverse من ملفات XML المصدر. |

## <a name="community-tools"></a>أدوات Community

هناك العديد من أدوات community والمكتبات والحلول، ومعظمها مفتوحة المصدر، متاحة لتحسين تجربة مطور Microsoft Power Platform لسد الثغرات في أدوات التطوير والمكتبات الرسمية من Microsoft. يتم ذكر بعض الأدوات في [أدوات Community لصفحة Microsoft Dataverse](/power-apps/developer/data-platform/community-tools/?azure-portal=true).

الأدوات التي تم إنشاؤها بواسطة community غير مدعومة من Microsoft. إذا كانت لديك أي أسئلة أو مشكلات تتعلق بأدوات community، فاتصل بناشر الأداة.
