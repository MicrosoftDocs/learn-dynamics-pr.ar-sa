---
ms.openlocfilehash: be97b18412309974f8299424c23c6ed6013b8cb91070e5ece563ad3e88d830b0
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7130829"
---
بعد إنشاء تقرير SSRS، يجب توزيعه قبل أن تتمكن من الوصول إليه في تطبيقات Finance and Operations. ويمكنك توزيع التقارير من PowerShell أو من Visual Studio. يمكن أن يكون توزيع التقارير من PowerShell مفيداً إذا كنت بحاجة إلى توزيع تقرير في بيئة لا يتوفر لديها حق الوصول إلى Visual Studio. ومع ذلك، يجب عدم القيام بذلك في بيئة تشغيل. 

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


