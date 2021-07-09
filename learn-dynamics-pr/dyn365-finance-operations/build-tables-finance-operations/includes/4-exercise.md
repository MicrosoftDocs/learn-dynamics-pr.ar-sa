---
ms.openlocfilehash: 8de726622b4c8e7d2ac0d9c64562a7217fa086a5
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072621"
---
## <a name="before-you-begin"></a><span data-ttu-id="f16b0-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="f16b0-101">Before you begin</span></span>
<span data-ttu-id="f16b0-102">يجب إيقاف تشغيل خدمة الدُفعة.</span><span class="sxs-lookup"><span data-stu-id="f16b0-102">You need to turn off the batch service.</span></span> <span data-ttu-id="f16b0-103">فيما يلي الخطوات الخاصة بإيقاف تشغيل خدمة الدُفعة:</span><span class="sxs-lookup"><span data-stu-id="f16b0-103">Here are the steps to shut off the batch service:</span></span>
 
1. <span data-ttu-id="f16b0-104">افتح موجه الأوامر في البيئة وقمّ بتشغيله كمسؤول</span><span class="sxs-lookup"><span data-stu-id="f16b0-104">Open command prompt in the environment and run as administrator</span></span>
2. <span data-ttu-id="f16b0-105">النوع: sc queryex DynamicsAxBatch</span><span class="sxs-lookup"><span data-stu-id="f16b0-105">Type: sc queryex DynamicsAxBatch</span></span>
3. <span data-ttu-id="f16b0-106">ابحث عن PID</span><span class="sxs-lookup"><span data-stu-id="f16b0-106">Find the PID</span></span>
4. <span data-ttu-id="f16b0-107">ثمّ أدخل: taskkill / f /pid ***رقم PID***</span><span class="sxs-lookup"><span data-stu-id="f16b0-107">Then enter:  taskkill / f /pid ***PID number***</span></span>


## <a name="scenario"></a><span data-ttu-id="f16b0-108">السيناريو</span><span class="sxs-lookup"><span data-stu-id="f16b0-108">Scenario</span></span>
<span data-ttu-id="f16b0-109">طُلب من مطور تطبيقات Finance and Operations إنشاء جدول جديد لشركة Fleet Management.</span><span class="sxs-lookup"><span data-stu-id="f16b0-109">The Finance and Operations apps developer has been asked to create a new table for the Fleet Management company.</span></span> <span data-ttu-id="f16b0-110">تحتاج شركة Fleet Management إلى جمع معلومات العملاء بطريقة مختلفة عن صفحة **كافة العملاء** الجاهزة.</span><span class="sxs-lookup"><span data-stu-id="f16b0-110">The Fleet Management company needs to collect customer information in a different way than the out-of-the-box **All Customers** page.</span></span> <span data-ttu-id="f16b0-111">وترغب في أن يحتوي الجدول على كل من البيانات الشخصية وبيانات الموقع باستخدام العناصر الموجودة في AOT.</span><span class="sxs-lookup"><span data-stu-id="f16b0-111">They want the table to contain both personal and location data by using existing elements in the AOT.</span></span>

## <a name="create-a-new-project"></a><span data-ttu-id="f16b0-112">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="f16b0-112">Create a new project</span></span>
1.  <span data-ttu-id="f16b0-113">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f16b0-113">Minimize the Internet Explorer window.</span></span> 
2.  <span data-ttu-id="f16b0-114">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="f16b0-114">Open Visual Studio.</span></span>
3.  <span data-ttu-id="f16b0-115">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-115">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
2.  <span data-ttu-id="f16b0-116">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-116">Open the **File** menu and select **New > Project**.</span></span>
2.  <span data-ttu-id="f16b0-117">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-117">In the **New Project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Installed**.</span></span>
3.  <span data-ttu-id="f16b0-118">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-118">On the middle pane, select **Finance Operations**.</span></span>
4.  <span data-ttu-id="f16b0-119">قُم بتسمية المشروع **FleetManagementTableProject**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-119">Name the project **FleetManagementTableProject**.</span></span>
5.  <span data-ttu-id="f16b0-120">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-120">Select **OK**.</span></span>
6.  <span data-ttu-id="f16b0-121">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="f16b0-121">Open the **Dynamics 365** menu in the ribbon.</span></span>
7.  <span data-ttu-id="f16b0-122">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-122">Select **Options**.</span></span>
8.  <span data-ttu-id="f16b0-123">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-123">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
9.  <span data-ttu-id="f16b0-124">تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً‏**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-124">Ensure that the checkboxes for **Organize projects by element type** and **Synchronize database on build for newly created project** are selected.</span></span>
10. <span data-ttu-id="f16b0-125">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-125">Select **OK**.</span></span>

## <a name="create-a-table"></a><span data-ttu-id="f16b0-126">أنشئ جدولاً</span><span class="sxs-lookup"><span data-stu-id="f16b0-126">Create a table</span></span>

1. <span data-ttu-id="f16b0-127">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementTableProject**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-127">In the **Solution Explorer** window, right-click the project  **FleetManagementTableProject**.</span></span>
12. <span data-ttu-id="f16b0-128">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-128">Select **Add > New Item**.</span></span>
13. <span data-ttu-id="f16b0-129">في الجزء الأيسر، حدد **عناصر Dynamics 365** ثم حدد **نموذج البيانات**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-129">On the left pane, select **Dynamics 365 Items** and then select **Data Model**.</span></span>
14. <span data-ttu-id="f16b0-130">في الجزء الأوسط، حدد **جدول**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-130">On the middle pane, select **Table**.</span></span>
15. <span data-ttu-id="f16b0-131">في حقل **الاسم** أدخل **FleetCustomersTable**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-131">Enter **FleetCustomersTable** in the **Name** field.</span></span>
16. <span data-ttu-id="f16b0-132">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-132">Select **Add**.</span></span>
17. <span data-ttu-id="f16b0-133">سيتم فتح **FleetCustomersTable** الآن في نافذة **مصمم العناصر**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-133">The **FleetCustomersTable** will now be open in the **Element Designer** window.</span></span>
18. <span data-ttu-id="f16b0-134">انقر بزر الماوس الأيمن فوق العنوان **FleetCustomersTable** في مصمم العناصر وحدد **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-134">Right-click the **FleetCustomersTable** heading in the element designer and select **Properties**.</span></span>
19. <span data-ttu-id="f16b0-135">في النافذة **خصائص**، في حقل **التسمية**، أدخل **عملاء الأسطول**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-135">In the **Properties** window, in the **Label** field, enter **Fleet customers**.</span></span>

## <a name="add-fields-to-the-table"></a><span data-ttu-id="f16b0-136">إضافة حقول إلى الجدول</span><span class="sxs-lookup"><span data-stu-id="f16b0-136">Add fields to the table</span></span>


1.  <span data-ttu-id="f16b0-137">في شجرة مكونات البرنامج (AOT) في نافذة **مستكشف التطبيقات**، قمّ بتوسيع عقدة **أنواع البيانات**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-137">In the Application object tree (AOT) in the **Application Explorer** window, expand the **Data types** node.</span></span>
2.  <span data-ttu-id="f16b0-138">قمّ بتوسيع عقدة **أنواع البيانات الموسعة**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-138">Expand the **Extended Data Types** node.</span></span>
3.  <span data-ttu-id="f16b0-139">حدد واسحب أنواع EDT التالية إلى عقدة **الحقول** في جدول **FleetCustomersTable**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-139">Select and drag the following EDTs onto the **Fields** node of the table **FleetCustomersTable**.</span></span>
    -   <span data-ttu-id="f16b0-140">FirstName</span><span class="sxs-lookup"><span data-stu-id="f16b0-140">FirstName</span></span>
    -   <span data-ttu-id="f16b0-141">LastName</span><span class="sxs-lookup"><span data-stu-id="f16b0-141">LastName</span></span>
    -   <span data-ttu-id="f16b0-142">Email</span><span class="sxs-lookup"><span data-stu-id="f16b0-142">Email</span></span>
    -   <span data-ttu-id="f16b0-143">Phone</span><span class="sxs-lookup"><span data-stu-id="f16b0-143">Phone</span></span>
    -   <span data-ttu-id="f16b0-144">AddressStreet</span><span class="sxs-lookup"><span data-stu-id="f16b0-144">AddressStreet</span></span>
    -   <span data-ttu-id="f16b0-145">AddressCity</span><span class="sxs-lookup"><span data-stu-id="f16b0-145">AddressCity</span></span>
    -   <span data-ttu-id="f16b0-146">AddressStateId</span><span class="sxs-lookup"><span data-stu-id="f16b0-146">AddressStateId</span></span>
    -   <span data-ttu-id="f16b0-147">AddressZipCodeId</span><span class="sxs-lookup"><span data-stu-id="f16b0-147">AddressZipCodeId</span></span>
4.  <span data-ttu-id="f16b0-148">حدد **حفظ** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="f16b0-148">Select **Save** in the ribbon.</span></span>
5.  <span data-ttu-id="f16b0-149">في نافذة مستكشف الحلول انقر بزر الماوس الأيمن وانقر فوق **مزامنة FleetManagementTableProject(ISV) [Fleet Management] مع قاعدة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-149">Right-click the project in the Solution Explorer and click **Synchronize FleetManagementTableProject(ISV) [Fleet Management]with Database**.</span></span>
6.  <span data-ttu-id="f16b0-150">قمّ بتنفيذ إنشاء بواسطة النقر بزر الماوس الأيمن فوق مشروع **FleetManagementTableProject** في نافذة **مستكشف الحلول** وحدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-150">Perform a build by right-clicking the project  **FleetManagementTableProject** in the **Solution Explorer** window and selecting **Build**.</span></span>

## <a name="create-field-groups-and-add-fields-to-the-field-groups"></a><span data-ttu-id="f16b0-151">إنشاء مجموعات الحقول وإضافة حقول إلى مجموعات الحقول</span><span class="sxs-lookup"><span data-stu-id="f16b0-151">Create field groups and add fields to the field groups</span></span>


1.  <span data-ttu-id="f16b0-152">في مصمم الجدول، انقر بزر الماوس الأيمن فوق عقدة **مجموعات الحقول** الخاصة بعنوان **FleetCustomersTable**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-152">In the Table designer, right-click the **Field groups** node of the  **FleetCustomersTable** heading.</span></span>
2.  <span data-ttu-id="f16b0-153">حدد **مجموعة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-153">Select **New group**.</span></span>
3.  <span data-ttu-id="f16b0-154">انقر بزر الماوس الأيمن فوق مجموعة الحقول الجديدة وأعد تسميتها **PersonalInfo**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-154">Right-click the new field group and rename it **PersonalInfo**.</span></span>
4.  <span data-ttu-id="f16b0-155">قمّ بتوسيع عقدة **الحقول** الخاصة بـ **FleetCustomersTable**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-155">Expand the **Fields** node of the **FleetCustomersTable**.</span></span>
5.  <span data-ttu-id="f16b0-156">حدد واسحب حقول **FirstName**، و **LastName**، و **Email‎**، و **Phone‎** من عقدة **الحقول** إلى مجموعة حقول **PersonalInfo**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-156">Select and drag the **FirstName**, **LastName**, **Email**, and **Phone** fields from the **Fields** node to the **PersonalInfo** Field group.</span></span>
6.  <span data-ttu-id="f16b0-157">في مصمم الجدول، انقر بزر الماوس الأيمن فوق عقدة **مجموعات الحقول** الخاصة بعنوان **FleetCustomersTable**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-157">In the table designer, right-click the **Field groups** node of the **FleetCustomersTable** heading.</span></span>
7.  <span data-ttu-id="f16b0-158">حدد **مجموعة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-158">Select **New group**.</span></span>
8.  <span data-ttu-id="f16b0-159">انقر بزر الماوس الأيمن فوق مجموعة الحقول الجديدة وأعد تسميتها **LocationInfo**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-159">Right-click the new field group and rename it **LocationInfo**.</span></span>
9.  <span data-ttu-id="f16b0-160">قمّ بتوسيع عقدة **الحقول** الخاصة بـ **FleetCustomersTable**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-160">Expand the **Fields** node of **FleetCustomersTable**.</span></span>
10. <span data-ttu-id="f16b0-161">حدد واسحب حقول **AddressStreet**، و **AddressCity**، و **AddressStateId**، و **‎AddressZipCodeId** من عقدة **الحقول** إلى مجموعة حقول **‎LocationInfo**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-161">Select and drag the **AddressStreet**, **AddressCity**, **AddressStateId**, and **AddressZipCodeId** fields from the **Fields** node to the **LocationInfo** field group.</span></span>
11. <span data-ttu-id="f16b0-162">في نافذة مستكشف الحلول انقر بزر الماوس الأيمن وانقر فوق **مزامنة FleetManagementTableProject(ISV) [Fleet Management] مع قاعدة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-162">Right-click the project in the Solution Explorer and click **Synchronize FleetManagementTableProject(ISV) [Fleet Management] with Database**.</span></span>
12. <span data-ttu-id="f16b0-163">قمّ بتنفيذ بناء بواسطة النقر بزر الماوس الأيمن فوق مشروع **FleetManagementTableProject** في نافذة **مستكشف الحلول** وحدد **البناء**.</span><span class="sxs-lookup"><span data-stu-id="f16b0-163">Perform a build by right-clicking the project **FleetManagementTableProject** in the **Solution Explorer** window and then selecting **Build**.</span></span>


