---
ms.openlocfilehash: 84edabffcb1233c12298f357ea9236147a0b831e
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072605"
---
## <a name="scenario"></a><span data-ttu-id="2dc46-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="2dc46-101">Scenario</span></span>

<span data-ttu-id="2dc46-102">كُلف مطور تطبيقات Finance and Operations بإنشاء تعداد أساسي جديد لشركة Fleet Management.</span><span class="sxs-lookup"><span data-stu-id="2dc46-102">The Finance and Operations apps developer has been tasked with creating a new base enumeration for the Fleet Management company.</span></span> <span data-ttu-id="2dc46-103">إذ تحتاج الشركة إلى جمع معلومات حول نوع المركبة عند تسجيل مركبة جديدة من أجل الصيانة.</span><span class="sxs-lookup"><span data-stu-id="2dc46-103">The company needs to collect information about the vehicle type when a new vehicle is checked in for service.</span></span> <span data-ttu-id="2dc46-104">وترغب في استخدام قائمة منسدلة في واجهة المستخدم مع خيارات للسيارة والشاحنة وسيارات الدفع الرباعي الرياضية والشاحنة المغلقة.</span><span class="sxs-lookup"><span data-stu-id="2dc46-104">They would like a drop-down list to use in the user interface with the options for car, truck, SUV, and van.</span></span>


## <a name="create-a-new-project"></a><span data-ttu-id="2dc46-105">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="2dc46-105">Create a new project</span></span>

1.  <span data-ttu-id="2dc46-106">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2dc46-106">Minimize the Internet Explorer window.</span></span> 
2.  <span data-ttu-id="2dc46-107">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="2dc46-107">Open Visual Studio.</span></span>
3.  <span data-ttu-id="2dc46-108">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-108">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
2.  <span data-ttu-id="2dc46-109">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-109">Open the **File** menu and select **New > Project**.</span></span>
2.  <span data-ttu-id="2dc46-110">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-110">In the **New Project** dialog box, ensure that **Dynamics 365** is    selected on the left pane under **Installed**.</span></span>
3.  <span data-ttu-id="2dc46-111">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-111">On the middle pane, select **Finance Operations**.</span></span>
4.  <span data-ttu-id="2dc46-112">قم بتسمية المشروع **FleetManagementProject**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-112">Name the project **FleetManagementProject**.</span></span>
5.  <span data-ttu-id="2dc46-113">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-113">Select **OK**.</span></span>
6.  <span data-ttu-id="2dc46-114">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="2dc46-114">Open the **Dynamics 365** menu in the ribbon.</span></span>
7.  <span data-ttu-id="2dc46-115">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-115">Select **Options**.</span></span>
8.  <span data-ttu-id="2dc46-116">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-116">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
9. <span data-ttu-id="2dc46-117">تأكد من تحديد خانتي الاختيار لكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-117">Ensure the check boxes are selected for **Organize projects by element type** and   **Synchronize database on build for newly created project**.</span></span>
10. <span data-ttu-id="2dc46-118">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-118">Select **OK**.</span></span>

## <a name="create-a-base-enumeration-for-vehicle-type"></a><span data-ttu-id="2dc46-119">إنشاء تعداد أساسي لنوع المركبة</span><span class="sxs-lookup"><span data-stu-id="2dc46-119">Create a base enumeration for vehicle type</span></span>

1. <span data-ttu-id="2dc46-120">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementProject (ISV) [Fleet Management]**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-120">In the **Solution Explorer** window, right-click the project     **FleetManagementProject (ISV) [Fleet Management]**.</span></span> <span data-ttu-id="2dc46-121">(في هذا المعمل، يشير (ISV) و[Fleet Management] إلى معلمات المشروع أو الكائن)</span><span class="sxs-lookup"><span data-stu-id="2dc46-121">(In this lab, (ISV) and [Fleet Management] denote parameters of the project or object)</span></span>
2. <span data-ttu-id="2dc46-122">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-122">Select **Add > New Item**.</span></span>
3. <span data-ttu-id="2dc46-123">في الجزء الأيمن، حدد **عناصر Dynamics 365** ثم حدد **أنواع البيانات**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-123">On the left pane, select **Dynamics 365 Items** and then select    **Data Types**.</span></span>
4. <span data-ttu-id="2dc46-124">في الجزء الأوسط، حدد **تعداد أساسي**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-124">On the middle pane, select **Base enum**.</span></span>
5. <span data-ttu-id="2dc46-125">أدخل **VehicleType** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-125">Enter  **VehicleType** in the **Name** field.</span></span>
6. <span data-ttu-id="2dc46-126">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-126">Select **Add**.</span></span> <span data-ttu-id="2dc46-127">سيتم فتح التعداد الأساسي لـVehicleType الآن في نافذة مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-127">The VehicleType base enumeration will now be open in    the element designer window.</span></span>
7. <span data-ttu-id="2dc46-128">انقر بزر الماوس الأيمن فوق العنوان **VehicleType (ISV) [Fleet Management]** في مصمم العناصر وحدد **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-128">Right-click the **VehicleType (ISV) [Fleet Management]** heading in the element designer and    select **Properties**.</span></span>
8. <span data-ttu-id="2dc46-129">في نافذة **الخصائص**، في حقل **التسمية**، أدخل **نوع المركبة**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-129">In the **Properties** window, in the **Label** field, enter  **Vehicle type**.</span></span>

## <a name="add-elements-to-the-new-base-enumeration"></a><span data-ttu-id="2dc46-130">إضافة عناصر إلى التعداد الأساسي الجديد</span><span class="sxs-lookup"><span data-stu-id="2dc46-130">Add elements to the new base enumeration</span></span>

1.  <span data-ttu-id="2dc46-131">انقر بزر الماوس الأيمن فوق التعداد الأساسي **VehicleType (ISV) [Fleet Management]** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-131">Right-click the **VehicleType (ISV) [Fleet Management]**  base enum in the element designer.</span></span>
2.  <span data-ttu-id="2dc46-132">حدد **عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-132">Select **New Element**.</span></span>
3.  <span data-ttu-id="2dc46-133">حدد **BaseEnumValue1** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-133">Select **BaseEnumValue1** in the element designer.</span></span>
4.  <span data-ttu-id="2dc46-134">في نافذة **الخصائص**، أدخل **سيارة** في حقل **الاسم** وفي حقل **التسمية**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-134">In the **Properties** window, enter **Car** in the **Name** field and in the **Label** field.</span></span>
5.  <span data-ttu-id="2dc46-135">انقر بزر الماوس الأيمن فوق التعداد الأساسي **VehicleType (ISV) [Fleet Management]** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-135">Right-click the **VehicleType (ISV) [Fleet Management]** base enum in the element designer.</span></span>
6.  <span data-ttu-id="2dc46-136">حدد **عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-136">Select **New Element**.</span></span>
7.  <span data-ttu-id="2dc46-137">حدد **BaseEnumValue1** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-137">Select **BaseEnumValue1** in the element designer.</span></span>
8.  <span data-ttu-id="2dc46-138">في نافذة **الخصائص**، أدخل **شاحنة** في حقل **الاسم** وفي حقل **التسمية**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-138">In the **Properties** window, enter **Truck** in the **Name** field and in the **Label** field.</span></span>
9.  <span data-ttu-id="2dc46-139">انقر بزر الماوس الأيمن فوق التعداد الأساسي **VehicleType (ISV) [Fleet Management]** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-139">Right-click the **VehicleType (ISV) [Fleet Management]** base enum in the element designer.</span></span>
10. <span data-ttu-id="2dc46-140">حدد **عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-140">Select **New Element**.</span></span>
11. <span data-ttu-id="2dc46-141">حدد **BaseEnumValue1** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-141">Select **BaseEnumValue1** in the element designer.</span></span>
12. <span data-ttu-id="2dc46-142">في نافذة **الخصائص**، أدخل **سيارة دفع رباعي رياضية** في حقل **الاسم** وفي حقل **التسمية**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-142">In the **Properties** window, enter **SUV** in the **Name** field  and in the **Label** field.</span></span>
13. <span data-ttu-id="2dc46-143">انقر بزر الماوس الأيمن فوق التعداد الأساسي **VehicleType (ISV) [Fleet Management]** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-143">Right-click the **VehicleType (ISV) [Fleet Management]** base enum in the element designer.</span></span>
14. <span data-ttu-id="2dc46-144">حدد **عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-144">Select **New Element**.</span></span>
15. <span data-ttu-id="2dc46-145">حدد **BaseEnumValue1** في مصمم العناصر.</span><span class="sxs-lookup"><span data-stu-id="2dc46-145">Select **BaseEnumValue1** in the element designer.</span></span>
16. <span data-ttu-id="2dc46-146">في نافذة **الخصائص**، أدخل **شاحنة مغلقة** في حقل **الاسم** وفي حقل **التسمية**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-146">In the **Properties** window, enter **Van** in the **Name** field  and in the **Label** field.</span></span>
17. <span data-ttu-id="2dc46-147">قم بتنفيذ بناء بالنقر بزر الماوس الأيمن فوق مشروع **FleetManagementProject (ISV) [Fleet Management]** في نافذة **مستكشف الحلول** ثم حدد **بناء**.</span><span class="sxs-lookup"><span data-stu-id="2dc46-147">Perform a build by right-clicking the project **FleetManagementProject (ISV) [Fleet Management]** in the **Solution Explorer** window and then selecting **Build**.</span></span>


