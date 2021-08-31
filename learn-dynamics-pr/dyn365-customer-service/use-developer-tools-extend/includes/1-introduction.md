---
ms.openlocfilehash: 05eb84780ec1ffaf099af83f7d042c415fb073d0
ms.sourcegitcommit: a3960642d20383fe20430aacf4036514baac8c9f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2021
ms.locfileid: "6659318"
---
يستطيع المطورون استخدام العديد من أدوات التطوير التقليدية عند إنشاء حلول من أجل Microsoft Power Platform. ولكن هناك أدوات متميزة متنوعة تستهدف تطوير Microsoft Power Platform بشكلٍ حصري. توفر Microsoft الأدوات الرسمية عبر [NuGet مدير الحزمة](https://nuget.org/?azure-portal=true) وغيرها من مثبتات الأدوات المنشورة. وهناك أيضاً مجتمع متألق من الأدوات والمكتبات تُكمل منشورات Microsoft. في هذه الوحدة، سنستكشف الأدوات التي ينبغي أن يكون مطور Microsoft Power Platform على دراية بها.

## <a name="microsoft-power-apps-cli"></a>واجهة سطر الأوامر (CLI) لـ Microsoft Power Apps

Power Apps CLI هي واجهة سطر أوامر لإنشاء مكونات الأكواد. على سبيل المثال، هذه هي الطريقة التي تقوم من خلالها بتهيئة وإدارة دورة حياة مكون Power Apps Component Framework. يمكن كذلك أن تساعد الأداة على تطوير المكونات الإضافية أيضاً. الأداة على دراية بالحل ويمكن أن تساعدك على توزيع ملحقات النظام الأساسي المعتمدة إلى بيئة تطوير للاختبار.

## <a name="microsoft-power-platform-connectors-cli"></a>واجهة سطر أوامر موصلات Microsoft Power Platform

يوفر موصل CLI أداة سطر الأوامر لإنشاء وتحميل وتحديث والتحقق من صحة الروابط المخصصة. الأداة ضرورية للتحرير المتقدم لتعريف موصل مخصص. يجب كذلك استخدام الأداة إذا كنت تقوم بإعداد موصل مخصص للمصادر المفتوحة أو الشهادات.

## <a name="application-lifecycle-management-alm-tools"></a>أدوات إدارة دورة حياة التطبيقات (ALM)

هناك جزء مهم من تنفيذ إدارة دورة حياة التطبيقات لمشاريعك وهو وجود عملية قابلة للتكرار تسمح لك بتعديل مكونات الحل وتسجيل هذه التغييرات في نظام تحكم بالمصادر. في حين أن خطوات إنجاز هذه المهام يمكن تنفيذها بطريقة يدوية، إلا أن وجود عملية آلية خيار أفضل لضمان الاتساق والتكرار. لدعم إنشاء هذه الأتمتة، توفر Microsoft مهام إنشاء من أجل Azure DevOps وإجراءات من أجل GitHub.

راجع [القائمة](https://docs.microsoft.com/power-platform/alm/devops-build-tool-tasks/?azure-portal=true) الكاملة Azure DevOps لمهام الإنشاء للحصول على مزيد من التفاصيل حول كل مهمة.

راجع [القائمة الكاملة](https://docs.microsoft.com/power-platform/alm/devops-github-available-actions/?azure-portal=true) لإجراءات GitHub للحصول على مزيد من التفاصيل حول كل إجراء.

## <a name="microsoft-nuget-tools-for-dataverse"></a>أدوات Microsoft NuGet من أجل Dataverse

فيما يأتي أدوات Microsoft المتوفرة التي تساعد على مختلف جوانب التطوير عند استخدام Microsoft Dataverse.

  |     حزمة NuGet                                                                                |     الوصف                                                                                                                                                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|     أداة إنشاء الأكواد [Microsoft.CrmSdk.CoreTools](https://www.nuget.org/packages/Microsoft.CrmSdk.CoreTools/?azure-portal=true)                                           |     إنشاء فئات .NET Framework ذات الحد المبكر التي تمثل نموذج بيانات الجدول المستخدم من جانب التطبيقات المستندة إلى النموذج.                                                                                                                                                                                                           |
|     أداة ترحيل التكوين [Microsoft.CrmSdk.XrmTooling.ConfigurationMigration.Wpf](https://www.nuget.org/packages/Microsoft.CrmSdk.XrmTooling.ConfigurationMigration.Wpf/?azure-portal=true)       |     الأداة المستخدمة لنقل بيانات التكوين عبر بيئات Dataverse.                                                                                                                                                                                                                                                   |
|     Package Deployer [Microsoft.CrmSdk.XrmTooling.PackageDeployment.WPF](https://www.nuget.org/packages/Microsoft.CrmSdk.XrmTooling.PackageDeployment.Wpf/?azure-portal=true)                        |     أداة تمكن المسؤولين من توزيع الحزم في بيئة Dataverse. يجمع المطورون بين أصول الحلول والأكواد المخصصة في حزمة لتوزيعها بواسطة Package Deployer. يجب على موردي البرامج المستقلين (ISV) استخدام تنسيق الحزمة نفسه عند إعداد حلولهم لنشرها في AppSource.    |
|     أداة تسجيل المكونات الإضافية [Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool](https://www.nuget.org/packages/Microsoft.CrmSdk.XrmTooling.PluginRegistrationTool/?azure-portal=true)                 |     أداة مستخدمة لتسجيل تجميعات المكونات الإضافية للأكواد المخصصة والخطوات في بيئة Dataverse.                                                                                                                                                                                                                            |
|     أداة إنشاء حزم الحلول [Microsoft.CrmSdk.CoreTools](https://www.nuget.org/packages/Microsoft.CrmSdk.CoreTools/?azure-portal=true)                                         |     أداة يمكنها تفكيك حلول Dataverse إلى ملفات XML متعددة لإدارتها بواسطة نظام تحكم بالمصادر.   كما يمكن استخدامه لإعادة إنشاء حل Dataverse من ملفات XML المصدر.                                                                                                                              |

## <a name="community-tools"></a>أدوات Community

هناك العديد من أدوات community والمكتبات والحلول، ومعظمها مفتوحة المصدر، متاحة لتحسين تجربة مطور Microsoft Power Platform لسد الثغرات في أدوات التطوير والمكتبات الرسمية من Microsoft. يتم ذكر بعض الأدوات في [أدوات Community لصفحة Microsoft Dataverse](https://docs.microsoft.com/powerapps/developer/data-platform/community-tools/?azure-portal=true).

الأدوات التي تم إنشاؤها بواسطة community غير مدعومة من Microsoft. إذا كانت لديك أسئلة أو مشكلات تتعلق بأدوات community، فاتصل بناشر الأداة.
