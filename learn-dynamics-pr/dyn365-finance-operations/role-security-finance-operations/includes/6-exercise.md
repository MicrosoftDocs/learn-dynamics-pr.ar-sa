---
ms.openlocfilehash: 57aff281aae51d008fc6bf5332b59e8c2a5593ab
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072596"
---
## <a name="scenario"></a><span data-ttu-id="52bb0-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="52bb0-101">Scenario</span></span>

<span data-ttu-id="52bb0-102">طالبت شركة Fleet Management مطور تطبيقات Finance and Operations بإنشاء دور جديد استنادً إلى منصب جديد يتم تعبئته ليشغله مدير Fleet Service Manager.</span><span class="sxs-lookup"><span data-stu-id="52bb0-102">The Finance and Operations apps developer has been asked by the Fleet Management company to create a new role based on a new position that they are filling for a Fleet Service Manager.</span></span> <span data-ttu-id="52bb0-103">يحتاج المدير إلى رسوم جمركية لإدارة السيارات والعملاء، بالإضافة إلى الرسوم الجمركية الأساسية المرتبطة بإدارة الأسطول.</span><span class="sxs-lookup"><span data-stu-id="52bb0-103">The manager needs duties to manage cars and customers, as well as the basic duties that are associated with Fleet Management.</span></span>


## <a name="create-a-new-project"></a><span data-ttu-id="52bb0-104">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="52bb0-104">Create a new project</span></span>

1. <span data-ttu-id="52bb0-105">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="52bb0-105">Minimize the Internet Explorer window.</span></span> 
2.  <span data-ttu-id="52bb0-106">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="52bb0-106">Open Visual Studio.</span></span>
3.  <span data-ttu-id="52bb0-107">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-107">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
2.  <span data-ttu-id="52bb0-108">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-108">Open the **File** menu and select **New > Project**.</span></span>
3.  <span data-ttu-id="52bb0-109">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-109">In the **New Project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Installed**.</span></span>
4.  <span data-ttu-id="52bb0-110">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-110">On the middle pane, select **Finance Operations**.</span></span>
5.  <span data-ttu-id="52bb0-111">قم بتسمية المشروع **FleetManagementSecurityProject**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-111">Name the project **FleetManagementSecurityProject**.</span></span>
6.  <span data-ttu-id="52bb0-112">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-112">Select **OK**.</span></span>
7.  <span data-ttu-id="52bb0-113">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="52bb0-113">Open the **Dynamics 365** menu in the ribbon.</span></span>
8.  <span data-ttu-id="52bb0-114">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-114">Select **Options**.</span></span>
9. <span data-ttu-id="52bb0-115">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-115">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
10. <span data-ttu-id="52bb0-116">تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **ومزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-116">Ensure the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project** are selected.</span></span>
11. <span data-ttu-id="52bb0-117">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-117">Select **OK**.</span></span>


## <a name="create-the-fmservicemanager-role"></a><span data-ttu-id="52bb0-118">إنشاء دور FMServiceManager</span><span class="sxs-lookup"><span data-stu-id="52bb0-118">Create the FMServiceManager role</span></span> 


1. <span data-ttu-id="52bb0-119">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق **FleetManagementSecurityProject**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-119">In the **Solution Explorer** window, right-click  **FleetManagementSecurityProject**.</span></span>
13. <span data-ttu-id="52bb0-120">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-120">Select **Add > New Item**.</span></span>
14. <span data-ttu-id="52bb0-121">في العمود الأيمن، ضمن عُقدة **أصناف Dynamics 365**، حدد    **الأمان**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-121">In the left column, under the **Dynamics 365 Items** node, select    **Security**.</span></span>
15. <span data-ttu-id="52bb0-122">في العمود الأوسط، حدد **دور الأمان**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-122">In the middle column, select **Security Role**.</span></span>
16. <span data-ttu-id="52bb0-123">تسمية دور **FMServiceManager**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-123">Name the role **FMServiceManager**.</span></span>
17. <span data-ttu-id="52bb0-124">حدد **إضافة** لإضافة دور الأمان الجديد إلى المشروع.</span><span class="sxs-lookup"><span data-stu-id="52bb0-124">Select **Add** to add the new security role to your project.</span></span> <span data-ttu-id="52bb0-125">سيتم فتح الدور **FMServiceManager** الآن في نافذة مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="52bb0-125">The **FMServiceManager** role will now be open in the element designer window.</span></span>

## <a name="add-duties-to-the-fmservicemanager-role"></a><span data-ttu-id="52bb0-126">إضافة الرسوم الجمركية إلى دور FMServiceManager</span><span class="sxs-lookup"><span data-stu-id="52bb0-126">Add duties to the FMServiceManager role</span></span> 



1.  <span data-ttu-id="52bb0-127">في نافذة **مستكشف التطبيقات**، في **AOT**، قم بتوسيع عقدة **الأمان**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-127">In the **Application Explorer** window, in the **AOT**, expand the    **Security** node.</span></span>
2.  <span data-ttu-id="52bb0-128">قم بتوسيع عقدة **رسوم الأمان الجمركية**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-128">Expand the **Security Duties** node.</span></span>
3.  <span data-ttu-id="52bb0-129">حدد الرسم الجمركي **FMBasicDuties** واسحبه من **AOT** في نافذة **مستكشف التطبيقات** إلى نافذة مصمم العناصر في العقدة **رسوم الجمارك** أسفل الدور **FMServiceManager**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-129">Select and drag the **FMBasicDuties** duty from the **AOT** in the    **Application Explorer** window to the element designer window in the **Duties** node beneath the **FMServiceManager** role.</span></span>
4.  <span data-ttu-id="52bb0-130">حدد الرسم الجمركي **FMManageCars** من **AOT** في نافذة **مستكشف التطبيقات** إلى نافذة مصمم العناصر في عقدة **الرسوم الجمركية** أسفل الدور **FMServiceManager**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-130">Select and drag the **FMManageCars** duty from the **AOT** in the    **Application Explorer** window to the element designer window in the    **Duties** node beneath the **FMServiceManager** role.</span></span>
5.  <span data-ttu-id="52bb0-131">حدد الرسم الجمركي **FMManageCustomers** واسحبه من **AOT** في نافذة **مستكشف التطبيقات** إلى نافذة مصمم العناصر في عقدة **الرسوم الجمركية** أسفل الدور **FMServiceManager**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-131">Select and drag the **FMManageCustomers** duty from the **AOT** in the **Application Explorer** window to the element designer window in the **Duties** node beneath the **FMServiceManager** role.</span></span>
6.  <span data-ttu-id="52bb0-132">قم بتنفيذ بنية بواسطة النقر بزر الماوس الأيمن فوق **FleetManagementSecurityProject** في نافذة **مستكشف الحلول** وحدد **البناء**.</span><span class="sxs-lookup"><span data-stu-id="52bb0-132">Perform a build by right-clicking the project **FleetManagementSecurityProject** in the **Solution Explorer**    window and selecting **Build**.</span></span>

<span data-ttu-id="52bb0-133">*قد يظهر لك خطأ نظراً لأنه يجب إيقاف تشغيل خادم المجموعة في البيئة. ومع ذلك، لا يؤثر هذا على البناء*.</span><span class="sxs-lookup"><span data-stu-id="52bb0-133">*You may see an error because the batch server needs to be turned off in the environment. However, this does not affect the build*.</span></span>



