---
ms.openlocfilehash: f5823c557021deba339dba5902d40b02f873109e
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072330"
---
<span data-ttu-id="e39bc-101">بعد إنشاء تقرير SSRS، يجب توزيعه قبل أن تتمكن من الوصول إليه في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="e39bc-101">After an SSRS report is created, it must be deployed before you can access it in Finance and Operations apps.</span></span> <span data-ttu-id="e39bc-102">ويمكنك توزيع التقارير من PowerShell أو من Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="e39bc-102">You can deploy reports from the PowerShell or from Visual Studio.</span></span> <span data-ttu-id="e39bc-103">يمكن أن يكون توزيع التقارير من PowerShell مفيداً إذا كنت بحاجة إلى توزيع تقرير في بيئة لا يتوفر لديها حق الوصول إلى Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="e39bc-103">Deploying reports from PowerShell can be useful if you need to deploy a report in an environment that does not have access to Visual Studio.</span></span> <span data-ttu-id="e39bc-104">ومع ذلك، يجب عدم القيام بذلك في بيئة تشغيل.</span><span class="sxs-lookup"><span data-stu-id="e39bc-104">However, you should not do this in a Production environment.</span></span> 

<span data-ttu-id="e39bc-105">يمكنك توزيع كل التقارير أو تقرير معين من PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e39bc-105">You can deploy either all reports or a specific report from the PowerShell.</span></span> <span data-ttu-id="e39bc-106">لتوزيع كافة التقارير، افتح PowerShell كمسؤول، وشغِّل الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="e39bc-106">To deploy all reports, open the PowerShell as an administrator and run the following command:</span></span>
```powershell
*C:\AosService\PackagesLocalDirectory\Plugins\AxReportVmRoleStartupTask\DeployAllReportsToSSRS.ps1 -PackageInstallLocation \"C:\AosService\PackagesLocalDirectory\" *
```
<span data-ttu-id="e39bc-107">ووفقاً للبيئة التي تستخدمها، قد يختلف محرك الأقراص.</span><span class="sxs-lookup"><span data-stu-id="e39bc-107">Depending on the environment that you are using, the drive might vary.</span></span> <span data-ttu-id="e39bc-108">بشكل عام، يكون محرك الأقراص هو C:\\ أو L:\\ أو K:\\.</span><span class="sxs-lookup"><span data-stu-id="e39bc-108">Generally, the drive is C:\\, L:\\, or K:\\.</span></span>

<span data-ttu-id="e39bc-109">لتشغيل تقرير محدد، ستحتاج إلى اسم التقرير.</span><span class="sxs-lookup"><span data-stu-id="e39bc-109">To run a specific report, you need the report name.</span></span> <span data-ttu-id="e39bc-110">على الرغم من أنك ستفتح PowerShell كمسؤول، فستقوم بتشغيل سطر الأوامر التالي بدلاً من ذلك:</span><span class="sxs-lookup"><span data-stu-id="e39bc-110">Though you will open the PowerShell as an administrator, you will run the following command line instead:</span></span>
```powershell
*C:\AosService\PackagesLocalDirectory\Plugins\AxReportVmRoleStartupTask\DeployAllReportsToSSRS.ps1 -Module ApplicationSuite -ReportName TaxVatRegister.Report*
```
<span data-ttu-id="e39bc-111">لنشر تقرير من Visual Studio، ستحتاج إلى إضافة التقرير إلى مشروعك.</span><span class="sxs-lookup"><span data-stu-id="e39bc-111">To deploy a report from Visual Studio, you will need to add the report to your project.</span></span> <span data-ttu-id="e39bc-112">انقر بزر الماوس الأيمن فوق التقرير، وحدد خيار **التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="e39bc-112">Right-click the report and select the **Deploy** option.</span></span>

<span data-ttu-id="e39bc-113">[![لقطة شاشة لصفحة Visual Studio Solution Explorerتعرض خيار توزيع التقارير.](../media/deploy-report.png)](../media/deploy-report.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="e39bc-113">[![Screenshot of the Visual Studio Solution Explorer page showing the Deploy Reports option.](../media/deploy-report.png)](../media/deploy-report.png#lightbox)</span></span>


