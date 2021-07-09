---
ms.openlocfilehash: 261ae81f6c9181b89cd4fb70e08c9d64d11d94d2
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072617"
---
## <a name="scenario"></a><span data-ttu-id="d2ff0-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="d2ff0-101">Scenario</span></span>
<span data-ttu-id="d2ff0-102">يُعد مطور تطبيقات Finance and Operations موظفاً جديداً في شركة Fleet Management.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-102">The Finance and Operations apps developer is a new employee at the Fleet Management company.</span></span> <span data-ttu-id="d2ff0-103">يحتاج المطور إلى إنشاء المشروع الخاص به في Visual Studio لبدء تطوير عناصر جديدة.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-103">The developer needs to create their own project in Visual Studio to begin developing new elements.</span></span> <span data-ttu-id="d2ff0-104">تم تكليف المطور بإنشاء نوع البيانات الملحقة (EDT) للون السيارة.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-104">The developer has been tasked with creating a new Extended Data Type (EDT) for vehicle color.</span></span>

## <a name="create-a-new-project"></a><span data-ttu-id="d2ff0-105">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="d2ff0-105">Create a new project</span></span>

1.  <span data-ttu-id="d2ff0-106">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-106">Minimize the Internet Explorer window.</span></span> 
2.  <span data-ttu-id="d2ff0-107">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-107">Open Visual Studio.</span></span>
3.  <span data-ttu-id="d2ff0-108">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-108">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
2.  <span data-ttu-id="d2ff0-109">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-109">Open the **File** menu and select **New > Project**.</span></span>
3.  <span data-ttu-id="d2ff0-110">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-110">In the **New project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Installed**.</span></span>
4.  <span data-ttu-id="d2ff0-111">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-111">On the middle pane, select **Finance Operations**.</span></span>
5.  <span data-ttu-id="d2ff0-112">قم بتسمية المشروع **FleetManagementProject**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-112">Name the project **FleetManagementProject**.</span></span>
6.  <span data-ttu-id="d2ff0-113">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-113">Select **OK**.</span></span>
7.  <span data-ttu-id="d2ff0-114">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-114">Open the **Dynamics 365** menu in the ribbon.</span></span>
8.  <span data-ttu-id="d2ff0-115">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-115">Select **Options**.</span></span>
9.  <span data-ttu-id="d2ff0-116">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-116">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
10. <span data-ttu-id="d2ff0-117">تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-117">Ensure that the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project** are selected.</span></span>
11. <span data-ttu-id="d2ff0-118">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-118">Select **OK**.</span></span>


## <a name="create-a-new-vehicle-color-edt"></a><span data-ttu-id="d2ff0-119">إنشاء نوع EDT جديد للون السيارة</span><span class="sxs-lookup"><span data-stu-id="d2ff0-119">Create a new vehicle color EDT</span></span> 

1.  <span data-ttu-id="d2ff0-120">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementProject (ISV) [Fleet Management]**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-120">In the **Solution Explorer** window, right-click the project **FleetManagementProject (ISV) [Fleet Management]**.</span></span> <span data-ttu-id="d2ff0-121">(في هذا المعمل، يشير (ISV) و[Fleet Management] إلى معلمات المشروع أو الكائن)</span><span class="sxs-lookup"><span data-stu-id="d2ff0-121">(In this lab, (ISV) and [Fleet Management] denote parameters of the project or object)</span></span> 
2.  <span data-ttu-id="d2ff0-122">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-122">Select **Add > New Item**.</span></span>
3.  <span data-ttu-id="d2ff0-123">في الجزء الأيمن، حدد **عناصر Dynamics 365** ثم حدد **أنواع البيانات**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-123">On the left pane, select **Dynamics 365 Items** and then select **Data Types**.</span></span>
4.  <span data-ttu-id="d2ff0-124">في الجزء الأوسط، حدد **سلسلة EDT**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-124">On the middle pane, select **EDT String**.</span></span>
5.  <span data-ttu-id="d2ff0-125">أدخل **FMVehicleColor** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-125">Enter **FMVehicleColor** in the **Name** field.</span></span>
6.  <span data-ttu-id="d2ff0-126">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-126">Select **Add**.</span></span>
7.  <span data-ttu-id="d2ff0-127">سيتم فتح نوع EDT لـ **FMVehicleColor** الآن في نافذة مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-127">The **FMVehicleColor** EDT will now be open in the element designer window.</span></span>
8.  <span data-ttu-id="d2ff0-128">انقر بزر الماوس الأيمن فوق العنوان **FMVehicleColor (ISV) [Fleet Management]** في مصمم العنصر وحدد **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-128">Right-click the **FMVehicleColor (ISV) [Fleet Management]** heading in the element designer and select **Properties**.</span></span>
9.  <span data-ttu-id="d2ff0-129">في خاصية **التسمية**، أدخل **لون السيارة**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-129">In the **Label** property, enter **Vehicle color**.</span></span>
10. <span data-ttu-id="d2ff0-130">في خاصية **حجم السلسلة**، أدخل **20** للسماح بإدخال 20 حرفاً للون.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-130">In the **String Size** property, enter **20** to allow 20 characters to be entered for a color.</span></span>
11. <span data-ttu-id="d2ff0-131">قم بتنفيذ بناء بالنقر بزر الماوس الأيمن فوق **FleetManagementProject (ISV) [Fleet Management]** في نافذة **مستكشف الحلول** ثم حدد **البناء**.</span><span class="sxs-lookup"><span data-stu-id="d2ff0-131">Perform a build by right-clicking the **FleetManagementProject (ISV) [Fleet Management]** project in the **Solution Explorer** window and then selecting **Build**.</span></span>

