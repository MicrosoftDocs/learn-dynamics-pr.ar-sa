---
ms.openlocfilehash: 3ccf73216d1ce79410e919889141ab493065a499
ms.sourcegitcommit: 1619b2f0d1c8648728fda1c09721aa0c87e2546d
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/24/2022
ms.locfileid: "9047209"
---
إذا كانت مؤسستك لديها مشاريع ذات سمات مماثلة وهيكل تقسيم العمل، فيمكنك تسريع عملية إنشاء المشروع باستخدام قوالب المشاريع.

يمكنك إعداد قالب مشروع واحد أو أكثر باستخدام خصائص المشاريع الشائعة ومعلومات أخرى، مثل أعضاء الفريق، ومهام المشاريع، والتقديرات وما إلى ذلك. لمزيد من المعلومات، راجع [قوالب المشاريع](/dynamics365/project-operations/psa/project-templates/?azure-portal=true).

عندما يتم إعداد قالب المشروع في Project Operations، يمكنك إنشاء مشروع جديد بنسخه من قالب المشروع. سيتم نسخ الكيانات التالية من قالب المشروع:

- المشروع

- قوائم اختيار المشاريع

- مستودعات المشاريع

- أعضاء فريق المشروع

- مهمة المشروع

- تبعية مهمة المشروع

- تعيين المورد

- تقديرات المشاريع (بما في ذلك العمالة، والمصروفات، وتقديرات المواد)

يمكنك استخدام قالب المشروع جنباً إلى جنب مع "نسخ واجهة برمجة تطبيقات المشروع". قد تفكر في استخدام هذه الميزة أثناء ترحيل البيانات لترحيل المشاريع ونسخ البيانات من مشروع قالب، كما تمت مناقشة ذلك سابقاً.

## <a name="code-example"></a>مثال على الرمز

يوضح المثال التالي كيفية استدعاء الإجراء المخصص CopyProjectV3 مع مجموعة معلمات removeNamedResources.

```csharp
using System;
using Microsoft.Xrm.Sdk;

public class CopyProjectSample
{
    private IOrganizationService organizationService;

    public CopyProjectSample(IOrganizationService organizationService)
    {
        this.organizationService = organizationService;
    }

    public void SampleRun()
    {
        // Example source project GUID
        Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
        var sourceProject = new Entity("msdyn_project", sourceProjectId);

        Entity targetProject = new Entity("msdyn_project");
        targetProject["msdyn_subject"] = "Example Project - Copy";
        targetProject.Id = organizationService.Create(targetProject);

        CallCopyProjectAPI(sourceProject.ToEntityReference(),
            targetProject.ToEntityReference(),
            true,
            false);
        Console.WriteLine("Done ...");
    }

    private void CallCopyProjectAPI(
        EntityReference sourceProject,
        EntityReference TargetProject,
        bool replaceNamedResources = true,
        bool clearTeamsAndAssignments = false)
    {
        OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
        req["SourceProject"] = sourceProject;
        req["Target"] = TargetProject;

        if (replaceNamedResources)
        {
            req["ReplaceNamedResources"] = true;
        }
        else
        {
            req["ClearTeamsAndAssignments"] = true;
        }

        OrganizationResponse response = organizationService.Execute(req);
    }
}
```

لمزيد من المعلومات، راجع [تطوير قوالب المشاريع باستخدام "نسخ المشروع"](/dynamics365/project-operations/project-management/dev-copy-project/?azure-portal=true).
