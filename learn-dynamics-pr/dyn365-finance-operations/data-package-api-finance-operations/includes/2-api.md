---
ms.openlocfilehash: aeb5f7f5161541443e261edde11102f25ab8de43
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071399"
---
<span data-ttu-id="3d3f1-101">يمكن للمطورين استيراد وتصدير واجهات برمجة التطبيقات (API) بين تطبيقات Finance and Operations وعمليات التوزيع المحلية.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-101">Developers can import and export APIs between Finance and Operations apps and on-premises deployments.</span></span> <span data-ttu-id="3d3f1-102">ضع في اعتبارك أن هناك بعض الاختلافات الأساسية مع هذه العمليات لعمليات التوزيع المحلية وعلى السحابة:</span><span class="sxs-lookup"><span data-stu-id="3d3f1-102">Keep in mind that there are some key differences with these processes for on-premises and cloud deployments:</span></span> 

-   <span data-ttu-id="3d3f1-103">بالنسبة لعمليات التوزيع المحلية، تمت إضافة الدعم لواجهة برمجة تطبيقات (API) REST لحزمة إدارة البيانات على الرغم من عدم تغيير أسماء واجهة برمجة التطبيقات (API).</span><span class="sxs-lookup"><span data-stu-id="3d3f1-103">For on-premises deployments, support has been added for the Data  management package REST API even though API names have not been changed.</span></span> <span data-ttu-id="3d3f1-104">بهذه الطريقة، يمكن لـ Microsoft الاحتفاظ بمجموعة API واحدة لكل من عمليات التوزيع السحابية وعمليات التوزيع المحلية.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-104">This way, Microsoft can keep a single API set for both cloud deployments and on-premises deployments.</span></span>
-   <span data-ttu-id="3d3f1-105">تستخدم حزمة واجهة برمجة تطبيقات (API) إطار عمل إدارة البيانات OAuth 2.0 لتفويض الوصول.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-105">The Data management framework API package uses OAuth 2.0 to   authorize access.</span></span>
-   <span data-ttu-id="3d3f1-106">لعمليات التوزيع المحلية، تتم إدارة التفويض من خلال Active Directory Federation Services ‏(AD FS).</span><span class="sxs-lookup"><span data-stu-id="3d3f1-106">For on-premises deployments, authorization is managed with Active  Directory Federation Services (AD FS).</span></span>
-   <span data-ttu-id="3d3f1-107">لا يتم دعم واجهات برمجة التطبيقات (API) للتكامل المتكرر لعمليات التوزيع المحلية.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-107">Recurring integration APIs are not supported for on-premises   deployments.</span></span>

## <a name="importing-apis"></a><span data-ttu-id="3d3f1-108">استيراد واجهات برمجة التطبيقات (API)</span><span class="sxs-lookup"><span data-stu-id="3d3f1-108">Importing APIs</span></span>

<span data-ttu-id="3d3f1-109">لبدء عملية استيراد حزمة البيانات، يتم استخدام واجهة برمجة تطبيقات (API) **ImportFromPackage** لبدء الاستيراد من حزمة بيانات.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-109">To start the data package import process, the **ImportFromPackage** API is used to initiate an import from a data package.</span></span> <span data-ttu-id="3d3f1-110">يتم تحميل حزمة البيانات إلى وحدة تخزين Blob المرتبطة بتنفيذ تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-110">The data package is uploaded to the Blob storage that is associated with the Finance and Operations apps implementation.</span></span>

<span data-ttu-id="3d3f1-111">بالنسبة لعمليات التوزيع المحلية، سيتم بدء الاستيراد من ملف التخزين المحلي الذي تم تحميله مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-111">For on-premises deployments, the import will be initiated from the local storage file that was uploaded previously.</span></span>

<span data-ttu-id="3d3f1-112">فيما يلي مثال على الرمز المستخدم لبدء عملية الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-112">The following is an example of code that is used to initiate the import process.</span></span>
```csharp
POST /data/DataManagementDefinitionGroups/Microsoft.Dynamics.DataEntities.**ImportFromPackage**
BODY
{
    "packageUrl":"<string>",
    "definitionGroupId":"<string>",
    "executionId":"<string>",
    "execute":<bool>,
    "overwrite":<bool>,
    "legalEntityId":"<string>"
}
```
<span data-ttu-id="3d3f1-113">تصف القائمة التالية عناصر الرمز المختلفة:</span><span class="sxs-lookup"><span data-stu-id="3d3f1-113">The following list describes the various code elements:</span></span>

-    <span data-ttu-id="3d3f1-114">يبدأ `ImportPackageFrom` الاستيراد.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-114">`ImportPackageFrom` is initiating the import.</span></span>
-    <span data-ttu-id="3d3f1-115">`packageurl` هو اسم ملف فريد يُستخدم لتعقب معرفات الكائنات الثنائية كبيرة الحجم.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-115">`packageurl` is a unique file name that is used to track Blob IDs.</span></span> <span data-ttu-id="3d3f1-116">يمكنك تضمين معرف فريد عمومي (GUID) للمساعدة في ضمان اسم ملف فريد.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-116">You can include a globally unique identifier (GUID) to help guarantee a unique file name.</span></span>
-    <span data-ttu-id="3d3f1-117">`definitionGroupID` عبارة عن سلسلة تمثل اسم مشروع البيانات للاستيراد.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-117">`definitionGroupID` is a string that represents the name of the data project for the import.</span></span>
-    <span data-ttu-id="3d3f1-118">`executionId` هو المعرف الذي يجب استخدامه للوظيفة.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-118">`executionId` is the ID to use for the job.</span></span> <span data-ttu-id="3d3f1-119">إذا تم تعيين معرف فارغ، فسيتم إنشاء معرف تنفيذ جديد تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-119">If an empty ID is assigned, a new execution ID will be created automatically.</span></span>
-    <span data-ttu-id="3d3f1-120">`execute` هو قيمة منطقية.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-120">`execute` is a Boolean.</span></span> <span data-ttu-id="3d3f1-121">إذا تم تعيين المعلمة إلى **صواب**، فسيتم تشغيل الخطوة الهدف.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-121">If the parameter is set to **True**, the target step will run.</span></span>
-    <span data-ttu-id="3d3f1-122">`overwrite` هي أيضاً قيمة منطقية يجب تعيينها إلى **خطأ** عند استخدام كيان مركب في حزمة، إذا لم يكن الأمر كذلك، فيجب تعيين هذا إلى **صواب**.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-122">`overwrite` is also a Boolean that must be set to **False** when a composite entity is used in a package, if not, then this should be set to **True**.</span></span>
-    <span data-ttu-id="3d3f1-123">`legalentityId` هو الكيان القانوني للاستيراد.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-123">`legalentityId` is the legal entity for the import.</span></span>

<span data-ttu-id="3d3f1-124">إذا اكتمل الاستيراد بنجاح، فستتلقى استجابة نجاح JSON.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-124">If the import is successfully finished, you will receive a JSON success response.</span></span>

## <a name="exporting-apis"></a><span data-ttu-id="3d3f1-125">تصدير واجهات برمجة التطبيقات (API)</span><span class="sxs-lookup"><span data-stu-id="3d3f1-125">Exporting APIs</span></span>

<span data-ttu-id="3d3f1-126">تصدير واجهات برمجة التطبيقات (API) مشابه للاستيراد.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-126">The export for APIs is similar to the import.</span></span> <span data-ttu-id="3d3f1-127">الفرق هو أن واجهة برمجة تطبيقات (API) **ExportToPackage** تُستخدم لبدء التصدير.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-127">The difference is that the **ExportToPackage** API is used to initiate the export.</span></span> <span data-ttu-id="3d3f1-128">ينطبق هذا على عمليات التوزيع السحابية والمحلية.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-128">This is applicable for both cloud and on-premises deployments.</span></span>

<span data-ttu-id="3d3f1-129">فيما يلي مثال على الرمز المستخدم لبدء عملية التصدير.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-129">The following is an example of code that is used to initiate the export process.</span></span>
```csharp
POST
/data/DataManagementDefinitionGroups/Microsoft.Dynamics.DataEntities.**ExportToPackage**
BODY
{
    "definitionGroupId":"<Data project Id>",
    "packageName":"<Name to use for downloaded file.>",
    "executionId":"<Execution Id if it is a rerun>",
    "reExecute":<bool>,
    "legalEntityId":"<Legal entity Id>"
}
```
<span data-ttu-id="3d3f1-130">إذا تم الانتهاء من التصدير بنجاح، فستتلقى استجابة نجاح JSON.</span><span class="sxs-lookup"><span data-stu-id="3d3f1-130">If the export is finished successfully, you will receive a JSON success response.</span></span>
