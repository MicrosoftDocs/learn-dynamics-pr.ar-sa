---
ms.openlocfilehash: 3bd8c1b1506b466f2611a60aefd2102e24e86d46
ms.sourcegitcommit: c1858cd3b2bd6663edff36e214795d4934ad3ddf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2022
ms.locfileid: "9580178"
---
بعد إنشاء تقرير SSRS، يجب توزيعه قبل أن تتمكن من الوصول إليه في تطبيقات التمويل والعمليات. ويمكنك توزيع التقارير من PowerShell أو من Visual Studio. يمكن أن يكون توزيع التقارير من PowerShell مفيداً إذا كنت بحاجة إلى توزيع تقرير في بيئة لا يتوفر لديها حق الوصول إلى Visual Studio. ومع ذلك، يجب عدم القيام بذلك في بيئة تشغيل. 

يمكنك توزيع كل التقارير أو تقرير معين من PowerShell. لتوزيع كافة التقارير، افتح PowerShell كمسؤول، وشغِّل الأمر التالي:
```powershell
*C:\AosService\PackagesLocalDirectory\Plugins\AxReportVmRoleStartupTask\DeployAllReportsToSSRS.ps1 -PackageInstallLocation \"C:\AosService\PackagesLocalDirectory\" *
```
ووفقاً للبيئة التي تستخدمها، قد يختلف محرك الأقراص. بشكل عام، يكون محرك الأقراص هو C:\\ أو L:\\ أو K:\\.

لتشغيل تقرير محدد، ستحتاج إلى اسم التقرير. على الرغم من أنك ستفتح PowerShell كمسؤول، فستقوم بتشغيل سطر الأوامر التالي بدلاً من ذلك:
```powershell
*C:\AosService\PackagesLocalDirectory\Plugins\AxReportVmRoleStartupTask\DeployAllReportsToSSRS.ps1 -Module ApplicationSuite -ReportName TaxVatRegister.Report*
```
لنشر تقرير من Visual Studio، ستحتاج إلى إضافة التقرير إلى مشروعك. انقر بزر الماوس الأيمن فوق التقرير، وحدد خيار **التوزيع**.

[![لقطة شاشة لصفحة Visual Studio Solution Explorerتعرض خيار توزيع التقارير.](../media/deploy-report.png)](../media/deploy-report.png#lightbox)


