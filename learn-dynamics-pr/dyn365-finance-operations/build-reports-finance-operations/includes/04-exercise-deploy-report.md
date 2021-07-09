---
ms.openlocfilehash: 0e1c6a8cdf327a4dbe49444fdcbdc1b53c72bd11
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071752"
---
 
<span data-ttu-id="2004e-101">أولاً، يجب عليك إنشاء استعلام.</span><span class="sxs-lookup"><span data-stu-id="2004e-101">First, you need to create a query.</span></span>

1.  <span data-ttu-id="2004e-102">افتح Visual Studio كمسؤول.</span><span class="sxs-lookup"><span data-stu-id="2004e-102">Open Visual Studio as administrator.</span></span>
2.  <span data-ttu-id="2004e-103">من القائمة **ملف** حدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="2004e-103">From the **File** menu, select **New > Project**.</span></span> <span data-ttu-id="2004e-104">حدد    **Dynamics 365** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="2004e-104">Select    **Dynamics 365** on the left pane.</span></span> <span data-ttu-id="2004e-105">حدد **Finance Operations** في الجزء الأوسط.</span><span class="sxs-lookup"><span data-stu-id="2004e-105">select **Finance Operations** in the middle pane.</span></span> <span data-ttu-id="2004e-106">أدخل **ReportingProject** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="2004e-106">Enter **ReportingProject** in the **Name** field.</span></span> <span data-ttu-id="2004e-107">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2004e-107">Select **OK**.</span></span>
3.  <span data-ttu-id="2004e-108">في مستكشف الحلول، انقر بزر الماوس الأيمن فوق عقدة مشروعك، ثم حدد **إضافة > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="2004e-108">In the Solution Explorer, right-click your project node, and then    select **Add > New Item**.</span></span>
4.  <span data-ttu-id="2004e-109">حدد **نموذج البيانات** ثم حدد **استعلام**.</span><span class="sxs-lookup"><span data-stu-id="2004e-109">Select **Data Model** and then select **Query**.</span></span>
5.  <span data-ttu-id="2004e-110">بالنسبة لحقل **الاسم**، أدخل **FMVehicleModelQuery** ثم حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="2004e-110">For the **Name** field, enter **FMVehicleModelQuery** and then select **Add**.</span></span>
6.  <span data-ttu-id="2004e-111">افتح طريقة عرض مستكشف التطبيقات، إذا لم تكن مفتوحة بالفعل.</span><span class="sxs-lookup"><span data-stu-id="2004e-111">Open the Application Explorer view, if it is not already open.</span></span>
7.  <span data-ttu-id="2004e-112">في AOT، افتح **نموذج البيانات > الجداول**، ثم حدد واسحب جدول FMVehicleModel إلى مصدر بيانات الاستعلام.</span><span class="sxs-lookup"><span data-stu-id="2004e-112">In the AOT, open **Data Model > Tables**, and then select and drag FMVehicleModel table to the data source of your query.</span></span>
8.  <span data-ttu-id="2004e-113">في خصائص **QueryRootDataSource** **FMVehicleModel**، قم بتعيين خاصية **الحقول الديناميكية** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="2004e-113">In the properties of the **QueryRootDataSource** **FMVehicleModel**, set the **Dynamic Fields** property to **Yes**.</span></span>
9.  <span data-ttu-id="2004e-114">حدد **حفظ الكل**.</span><span class="sxs-lookup"><span data-stu-id="2004e-114">Select **Save all**.</span></span>
10. <span data-ttu-id="2004e-115">انقر بزر الماوس الأيمن فوق مشروع والبناء (Ctrl+Shift+B).</span><span class="sxs-lookup"><span data-stu-id="2004e-115">Right-click the Project and build (Ctrl+Shift+B).</span></span>

<span data-ttu-id="2004e-116">والآن، ستقوم بإنشاء التقرير.</span><span class="sxs-lookup"><span data-stu-id="2004e-116">Now, you will create the report.</span></span>

1.  <span data-ttu-id="2004e-117">في مستكشف الحلول، انقر بزر الماوس الأيمن فوق عقدة مشروعك، ثم حدد **إضافة > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="2004e-117">In the Solution Explorer, right-click your project node and then select **Add > New Item**.</span></span>
2.  <span data-ttu-id="2004e-118">حدد عقدة **التقارير** في الجزء الأيمن، ثم حدد **تقرير** في الجزء الأوسط.</span><span class="sxs-lookup"><span data-stu-id="2004e-118">Select the **Reports** node on the left pane and then select **Report** on the middle pane.</span></span>
3.  <span data-ttu-id="2004e-119">في حقل **الاسم**، اكتب **FMVehicleModelReport** ثم حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="2004e-119">In the **Name** field, type **FMVehicleModelReport** and then select    **Add**.</span></span>
4.  <span data-ttu-id="2004e-120">انقر بزر الماوس الأيمن فوق عقدة **مجموعات البيانات** ثم حدد **مجموعات بيانات جديدة**.</span><span class="sxs-lookup"><span data-stu-id="2004e-120">Right-click the **Datasets** node and then select **New Data Set**.</span></span>
5.  <span data-ttu-id="2004e-121">في **الخصائص**، قم بتعيين خاصية **عوامل التصفية الديناميكية** إلى **صواب**.</span><span class="sxs-lookup"><span data-stu-id="2004e-121">In **Properties**, set the **Dynamic Filters** property to **True**.</span></span>
6.  <span data-ttu-id="2004e-122">أدخل **FMVehicleModelDS** في الخاصية **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="2004e-122">Enter **FMVehicleModelDS** in the **Name** property.</span></span>
7.  <span data-ttu-id="2004e-123">حدد الخاصية **استعلام** ثم حدد علامة الحذف (...) لعرض قائمة بالاستعلامات.</span><span class="sxs-lookup"><span data-stu-id="2004e-123">Select the **Query** property and then select the ellipsis (...) to view a list of Queries.</span></span>
8.  <span data-ttu-id="2004e-124">في الصفحة **تحديد استعلام**، حدد **FMVehicleModelQuery** ثم حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="2004e-124">On the **Select a Query** page, select **FMVehicleModelQuery** and    then select **Next**.</span></span>
9.  <span data-ttu-id="2004e-125">حدد خانة الاختيار **كل الحقول** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2004e-125">Select the **All Fields** check box and then select **OK**.</span></span>
10. <span data-ttu-id="2004e-126">اسحب **FMVehicleModelDS** وقم بإفلاتها من عقدة **مجموعات البيانات** إلى عقدة **التصميمات**.</span><span class="sxs-lookup"><span data-stu-id="2004e-126">Drag and drop **FMVehicleModelDS** from the **Datasets** node to the **Designs** node.</span></span>
11. <span data-ttu-id="2004e-127">في العقدة **التصميمات**، قم بتوسيع **AutoDesign1** التي تم إنشاؤها مؤخراً.</span><span class="sxs-lookup"><span data-stu-id="2004e-127">On the **Designs** node, expand the newly created **AutoDesign1**.</span></span>
12. <span data-ttu-id="2004e-128">قم بتوسيع **FMVehicleModelDSTable1**.</span><span class="sxs-lookup"><span data-stu-id="2004e-128">Expand the **FMVehicleModelDSTable1**.</span></span>
13. <span data-ttu-id="2004e-129">في عقدة **مجموعات البيانات**، قم بتوسيع **FMVehicleModelDS**.</span><span class="sxs-lookup"><span data-stu-id="2004e-129">On the **Datasets** node, expand the **FMVehicleModelDS**.</span></span>
14. <span data-ttu-id="2004e-130">قم بتوسيع عقدة **الحقول** إذا لم تكن قد تم توسيعها بالفعل.</span><span class="sxs-lookup"><span data-stu-id="2004e-130">Expand the **Fields** node if it is not already expanded.</span></span>
15. <span data-ttu-id="2004e-131">قم بسحب وإفلات **Make_Make** من عقدة **الحقول** إلى **التصميمات > AutoDesign1 > FMVehicleModelDSTable1 > التجميعات**.</span><span class="sxs-lookup"><span data-stu-id="2004e-131">Drag and drop **Make_Make** from the **Fields** node to **Designs > AutoDesign1 > FMVehicleModelDSTable1 > Groupings**.</span></span>
16. <span data-ttu-id="2004e-132">احفظ الكل.</span><span class="sxs-lookup"><span data-stu-id="2004e-132">Save all.</span></span>
17. <span data-ttu-id="2004e-133">انقر بزر الماوس الأيمن فوق الحل والبناء (Ctrl+Shift+B).</span><span class="sxs-lookup"><span data-stu-id="2004e-133">Right-click Solution and build (Ctrl+Shift+B).</span></span>
18. <span data-ttu-id="2004e-134">في مستكشف الحلول، انقر بزر الماوس الأيمن فوق **FMVehicleModelReport** ثم حدد **نشر التقارير**.</span><span class="sxs-lookup"><span data-stu-id="2004e-134">In the Solution Explorer, right-click **FMVehicleModelReport** and then select **Deploy Reports**.</span></span>

<span data-ttu-id="2004e-135">بعد ذلك، ستقوم بإنشاء عنصر قائمة لتشغيل التقرير.</span><span class="sxs-lookup"><span data-stu-id="2004e-135">Next, you will create a menu item to run the report.</span></span>

1.  <span data-ttu-id="2004e-136">في مستكشف الحلول، انقر بزر الماوس الأيمن فوق عقدة مشروعك، ثم حدد **إضافة > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="2004e-136">In the Solution Explorer, right-click your project node and then    select **Add > New Item**.</span></span>
2.  <span data-ttu-id="2004e-137">حدد **واجهة المستخدم** ثم حدد **عنصر قائمة المخرجات**.</span><span class="sxs-lookup"><span data-stu-id="2004e-137">Select **User Interface** and then select **Output Menu Item**.</span></span>
3.  <span data-ttu-id="2004e-138">قم بتسمية عنصر قائمة المخرجات **FMVehicleModelReport** ثم حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="2004e-138">Name the Output menu item **FMVehicleModelReport** and then select **Add**.</span></span>
4.  <span data-ttu-id="2004e-139">اسحب التقرير **FMVehicleModelReport** من مستكشف الحلول إلى عنصر القائمة الذي أنشأته للتو.</span><span class="sxs-lookup"><span data-stu-id="2004e-139">Drag the **FMVehicleModelReport** report from the Solution explorer onto the Menu Item that you just created.</span></span>
5.  <span data-ttu-id="2004e-140">احفظ الكل.</span><span class="sxs-lookup"><span data-stu-id="2004e-140">Save all.</span></span>
6.  <span data-ttu-id="2004e-141">انقر بزر الماوس الأيمن فوق **الحل والبناء** (Ctrl+Shift+B).</span><span class="sxs-lookup"><span data-stu-id="2004e-141">Right-click **Solution and build** (Ctrl+Shift+B).</span></span>

<span data-ttu-id="2004e-142">وأخيراً، ستقوم بتشغيل التقرير.</span><span class="sxs-lookup"><span data-stu-id="2004e-142">Finally, you will run the report.</span></span>

1.  <span data-ttu-id="2004e-143">في مستكشف الحلول، حدد عنصر قائمة المخرجات **FMVehicleModelReport** ثم انقر بزر الماوس الأيمن وحدد **تعيين ككائن بدء التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="2004e-143">In the Solution explorer, select the **FMVehicleModelReport** Output menu item, and then right-click and select **Set as Startup object**.</span></span>
2.  <span data-ttu-id="2004e-144">حدد **بدء** في شريط الأدوات القياسي في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="2004e-144">Select **Start** on the Standard Toolbar in Visual Studio.</span></span>
3.  <span data-ttu-id="2004e-145">حدد Ctrl+F5 لتشغيل عنصر القائمة.</span><span class="sxs-lookup"><span data-stu-id="2004e-145">Select Ctrl+F5 to run the menu item.</span></span>
