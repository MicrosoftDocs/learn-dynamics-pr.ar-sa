---
ms.openlocfilehash: f5823c557021deba339dba5902d40b02f873109e
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072330"
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


