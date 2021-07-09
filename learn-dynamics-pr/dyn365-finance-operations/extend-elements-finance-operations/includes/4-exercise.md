---
ms.openlocfilehash: 1d85c7c312bd9997a0914da1ba7c9038b931897a
ms.sourcegitcommit: 53504b2fc81adbe92e066d0fe8d4c87fd533fe31
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/26/2021
ms.locfileid: "6072566"
---

## <a name="scenario"></a><span data-ttu-id="041e9-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="041e9-101">Scenario</span></span>

<span data-ttu-id="041e9-102">طلبت شركة Fleet Management من مطور تطبيقات Finance and Operations تعديل المظهر والوظيفة لصفحة **العملاء** في الوحدة النمطية **إدارة الأسطول**.</span><span class="sxs-lookup"><span data-stu-id="041e9-102">The Finance and Operations apps developer has been asked by the Fleet Management company to adjust the appearance and functionality of the **Customers** page in the **Fleet management** module.</span></span> <span data-ttu-id="041e9-103">لتسريع العمليات الداخلية، تريد الشركة إضافة علامة تبويب إلى جزء الإجراءات مع زر يرتبط بالصفحة حتى يتمكنوا من إدخال فاتورة ذات نص حر.</span><span class="sxs-lookup"><span data-stu-id="041e9-103">To speed up internal processes, the company wants a tab added to the Action Pane with a button that links to the page so they can enter a free text invoice.</span></span> 

## <a name="create-a-new-project"></a><span data-ttu-id="041e9-104">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="041e9-104">Create a new project</span></span>

1.  <span data-ttu-id="041e9-105">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="041e9-105">Minimize the Internet Explorer window.</span></span> 
2.  <span data-ttu-id="041e9-106">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="041e9-106">Open Visual Studio.</span></span>
3.  <span data-ttu-id="041e9-107">حدد **نعم** في نافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**</span><span class="sxs-lookup"><span data-stu-id="041e9-107">Select **Yes** in the **Do you want to allow this app to make changes to your device?**</span></span> <span data-ttu-id="041e9-108">النافذة</span><span class="sxs-lookup"><span data-stu-id="041e9-108">Window</span></span>
4.  <span data-ttu-id="041e9-109">انتقل إلى قائمة **Dynamics 365** في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="041e9-109">Go to the **Dynamics 365** menu in Visual Studio.</span></span>
3.    <span data-ttu-id="041e9-110">حدد **إدارة النماذج > تحديث معلمات النموذج**.</span><span class="sxs-lookup"><span data-stu-id="041e9-110">Select **Model management > Update model parameters**.</span></span>
4.    <span data-ttu-id="041e9-111">حدد اسم نموذج **Fleet Management** من القائمة المنسدلة للنموذج.</span><span class="sxs-lookup"><span data-stu-id="041e9-111">Select the **Fleet Management** Model name from the model drop-down list.</span></span>
5.    <span data-ttu-id="041e9-112">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="041e9-112">Select **Next**.</span></span>
6.    <span data-ttu-id="041e9-113">تأكد من الإشارة إلى النماذج التالية عن طريق تحديد علامة الاختيار بجوار النموذج:</span><span class="sxs-lookup"><span data-stu-id="041e9-113">Ensure the following models are referenced by selecting the checkmark next to the model:</span></span>
        - <span data-ttu-id="041e9-114">مجموعة التطبيق</span><span class="sxs-lookup"><span data-stu-id="041e9-114">Application Suite</span></span>
        - <span data-ttu-id="041e9-115">أساس التطبيق</span><span class="sxs-lookup"><span data-stu-id="041e9-115">Application Foundation</span></span>
        - <span data-ttu-id="041e9-116">Application Common</span><span class="sxs-lookup"><span data-stu-id="041e9-116">Application Common</span></span>
        - <span data-ttu-id="041e9-117">النظام الأساسي للتطبيق</span><span class="sxs-lookup"><span data-stu-id="041e9-117">Application Platform</span></span>
        - <span data-ttu-id="041e9-118">مسؤول جهة الاتصال</span><span class="sxs-lookup"><span data-stu-id="041e9-118">Contact Person</span></span>
        - <span data-ttu-id="041e9-119">العملة</span><span class="sxs-lookup"><span data-stu-id="041e9-119">Currency</span></span>
        - <span data-ttu-id="041e9-120">دفتر الأستاذ العام</span><span class="sxs-lookup"><span data-stu-id="041e9-120">General Ledger</span></span>
        - <span data-ttu-id="041e9-121">دفتر الأستاذ</span><span class="sxs-lookup"><span data-stu-id="041e9-121">Ledger</span></span>
        - <span data-ttu-id="041e9-122">العاملون</span><span class="sxs-lookup"><span data-stu-id="041e9-122">Personnel</span></span>
        - <span data-ttu-id="041e9-123">البيع بالتجزئة</span><span class="sxs-lookup"><span data-stu-id="041e9-123">Retail</span></span>
        - <span data-ttu-id="041e9-124">الضريبة</span><span class="sxs-lookup"><span data-stu-id="041e9-124">Tax</span></span>
7.  <span data-ttu-id="041e9-125">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="041e9-125">Select **Next**.</span></span>
8.  <span data-ttu-id="041e9-126">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="041e9-126">Select **Finish**.</span></span>
2.  <span data-ttu-id="041e9-127">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="041e9-127">Open the **File** menu and select **New > Project**.</span></span>
3.  <span data-ttu-id="041e9-128">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="041e9-128">In the **New project** dialog box, ensure that **Dynamics 365** is  selected in the left pane under **Installed**.</span></span>
4.  <span data-ttu-id="041e9-129">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="041e9-129">In the middle pane, select **Finance Operations**.</span></span>
5.  <span data-ttu-id="041e9-130">قُم بتسمية المشروع **FleetManagementFormProject**.</span><span class="sxs-lookup"><span data-stu-id="041e9-130">Name the project **FleetManagementFormProject**.</span></span>
6.  <span data-ttu-id="041e9-131">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="041e9-131">Select **OK**.</span></span>
7.  <span data-ttu-id="041e9-132">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="041e9-132">Open the **Dynamics 365** menu in the ribbon.</span></span>
8.  <span data-ttu-id="041e9-133">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="041e9-133">Select **Options**.</span></span>
9.  <span data-ttu-id="041e9-134">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="041e9-134">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
10. <span data-ttu-id="041e9-135">حدد خانتي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً‏**.</span><span class="sxs-lookup"><span data-stu-id="041e9-135">Select the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project**.</span></span>
11. <span data-ttu-id="041e9-136">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="041e9-136">Select **OK**.</span></span>

## <a name="extend-the-fmcustomer-form"></a><span data-ttu-id="041e9-137">توسيع نموذج FMCustomer</span><span class="sxs-lookup"><span data-stu-id="041e9-137">Extend the FMCustomer form</span></span> 

1. <span data-ttu-id="041e9-138">في شريط البحث، في نافذة **مستكشف التطبيقات**، قمّ بتوسيع عُقد **AOT > واجهة المستخدم > النماذج**.</span><span class="sxs-lookup"><span data-stu-id="041e9-138">In the search bar, in the **Application Explorer** window, expand the    **AOT > User Interface > Forms** nodes.</span></span>
2. <span data-ttu-id="041e9-139">حدد نموذج **FMCustomer**.</span><span class="sxs-lookup"><span data-stu-id="041e9-139">Select the **FMCustomer** form.</span></span>
3. <span data-ttu-id="041e9-140">انقر بزر الماوس الأيمن فوق نموذج **FMCustomer** وحدد **إنشاء ملحق**.</span><span class="sxs-lookup"><span data-stu-id="041e9-140">Right-click the **FMCustomer** form and select **Create extension**.</span></span> <span data-ttu-id="041e9-141">ستتم إضافة عنصر يسمى **FMCustomer.FleetManagement** إلى **FleetManagementFormProject** في نافذة **مستكشف الحلول**.</span><span class="sxs-lookup"><span data-stu-id="041e9-141">An element named **FMCustomer.FleetManagement** will be added to your **FleetManagementFormProject** in the **Solution Explorer** window.</span></span> 
4. <span data-ttu-id="041e9-142">أعد تسمية الكائن **FMCustomer.Extension**.</span><span class="sxs-lookup"><span data-stu-id="041e9-142">Rename the object **FMCustomer.Extension**.</span></span> 
5. <span data-ttu-id="041e9-143">انقر نقراً مزدوجاً فوق نموذج **FMCustomer.Extension** في نافذة **مستكشف الحلول** لفتحه في نافذة مصمم النماذج.</span><span class="sxs-lookup"><span data-stu-id="041e9-143">Double-click the **FMCustomer.Extension** form in the **Solution Explorer** window to open it in the form designer window.</span></span>
6. <span data-ttu-id="041e9-144">حدد **حفظ** في الشريط لحفظ تقدمك.</span><span class="sxs-lookup"><span data-stu-id="041e9-144">Select **Save** in the ribbon to save your progress.</span></span>

## <a name="add-a-tab-button-group-and-button-to-the-action-pane-control"></a><span data-ttu-id="041e9-145">أضف علامة تبويب ومجموعة أزرار وزراً إلى عنصر التحكم في جزء الإجراءات</span><span class="sxs-lookup"><span data-stu-id="041e9-145">Add a tab, button group, and button to the Action Pane control</span></span> 

1.  <span data-ttu-id="041e9-146">في جزء التصميم الأيمن في مصمم النماذج، انقر بزر الماوس الأيمن فوق عنصر التحكم **ApplicationBar (جزء الإجراءات)**.</span><span class="sxs-lookup"><span data-stu-id="041e9-146">On the right Design pane of the form designer, right-click the    **ApplicationBar (Action Pane)** control.</span></span>
2.  <span data-ttu-id="041e9-147">حدد **جديد > علامة تبويب جزء الإجراءات**. تمت إضافة عنصر تحكم جديد يسمي **FormActionPaneTabControl1 (علامة تبويب جزء الإجراءات)**.</span><span class="sxs-lookup"><span data-stu-id="041e9-147">Select **New > Action Pane Tab**. A new control has been added    named **FormActionPaneTabControl1 (Action Pane Tab)**.</span></span>
3.  <span data-ttu-id="041e9-148">حدد عنوان **FormActionPaneTabControl1 (علامة تبويب جزء الإجراءات)**.</span><span class="sxs-lookup"><span data-stu-id="041e9-148">Select the **FormActionPaneTabControl1 (Action Pane Tab)** heading.</span></span>
4.  <span data-ttu-id="041e9-149">في النافذة **خصائص**، أدخل **InvoicingTab‎** لخاصية **الاسم** و **الفوترة** لخاصية **التسمية التوضيحية**.</span><span class="sxs-lookup"><span data-stu-id="041e9-149">In the **Properties** window, enter **InvoicingTab** for the **Name** property and **Invoicing** for the **Caption** property.</span></span>
5.  <span data-ttu-id="041e9-150">في جزء التصميم، انقر بزر الماوس الأيمن فوق عنصر تحكم **InvoicingTab (علامة تبويب جزء الإجراءات)** ثم حدد **مجموعة زر جديدة**.</span><span class="sxs-lookup"><span data-stu-id="041e9-150">On the Design pane, right-click the **InvoicingTab (Action Pane    Tab)** control and select **New Button Group**.</span></span>
6.  <span data-ttu-id="041e9-151">حدد العنوان **FormButtonGroupControl1 (مجموعة الأزرار)**.</span><span class="sxs-lookup"><span data-stu-id="041e9-151">Select the **FormButtonGroupControl1 (Button Group)** heading.</span></span>
7.  <span data-ttu-id="041e9-152">في النافذة **خصائص**، أدخل **CustomersButtonGroup‎** لخاصية **الاسم** و **العملاء** لخاصية **التسمية التوضيحية**.</span><span class="sxs-lookup"><span data-stu-id="041e9-152">In the **Properties** window, enter **CustomersButtonGroup** for the    **Name** property and **Customers** for the **Caption** property.</span></span>
8.  <span data-ttu-id="041e9-153">في جزء التصميم، انقر بزر الماوس الأيمن فوق عنصر تحكم **CustomersButtonGroup (مجموعة الأزرار)** ثم حدد **جديد > زر عنصر القائمة**.</span><span class="sxs-lookup"><span data-stu-id="041e9-153">On the Design pane, right-click the **CustomersButtonGroup (Button Group)** control and select **New > Menu Item Button**.</span></span>
9.  <span data-ttu-id="041e9-154">في النافذة **خصائص**، لخاصية **اسم عنصر القائمة**، حدد **CustFreeInvoiceNew‎** من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="041e9-154">In the **Properties** window, for the **Menu Item Name** property,    select **CustFreeInvoiceNew** from the drop-down list.</span></span>
10. <span data-ttu-id="041e9-155">انقر بزر الماوس الأيمن فوق **FMCustomer.Extension**، من نافذة **مستكشف الحلول**.</span><span class="sxs-lookup"><span data-stu-id="041e9-155">Right-click the **FMCustomer.Extension** form in the **Solution    Explorer** window.</span></span>
11. <span data-ttu-id="041e9-156">حدد **تعيين ككائن بدء التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="041e9-156">Select **Set as Startup Object**.</span></span>
12. <span data-ttu-id="041e9-157">قُم بتنفيذ إنشاء بالنقر بزر الماوس الأيمن فوق **FleetManagementFormProject** في نافذة **مستكشف الحلول** ثم تحديد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="041e9-157">Perform a build by right-clicking **FleetManagementFormProject** in the **Solution Explorer** window and then selecting **Build**.</span></span>
13. <span data-ttu-id="041e9-158">قُم بتشغيل النموذج الخاص بك لعرضه في نافذة مستعرض بتحديد **تصحيح الأخطاء > البدء بدون تصحيح الأخطاء** من الشريط.</span><span class="sxs-lookup"><span data-stu-id="041e9-158">Run your form to view it in a browser window by selecting **Debug > Start Without Debugging** from the ribbon.</span></span> <span data-ttu-id="041e9-159">يمكنك أيضاً استخدام **Ctrl + F5**.</span><span class="sxs-lookup"><span data-stu-id="041e9-159">You can also use **Ctrl + F5**.</span></span>
14. <span data-ttu-id="041e9-160">في نافذة المستعرض، حدد علامة التبويب **فوترة** في جزء الإجراءات ثم حدد **الفاتورة ذات النص الحر**.</span><span class="sxs-lookup"><span data-stu-id="041e9-160">In the browser window, select the **INVOICING** tab on the Action    Pane and then select **Free text invoice**.</span></span> <span data-ttu-id="041e9-161">يجب أن يتم نقلك إلى الصفحة لإدخال فاتورة نص حر للعميل المحدد في صفحة **FMCustomer.Extension**.</span><span class="sxs-lookup"><span data-stu-id="041e9-161">You should be taken to the page to enter a free text invoice for the selected customer in the **FMCustomer.Extension** page.</span></span>


### <a name="now-close-the-lab-environment"></a><span data-ttu-id="041e9-162">أغلق بيئة التمرين العملي الآن</span><span class="sxs-lookup"><span data-stu-id="041e9-162">Now close the lab environment</span></span> 

1. <span data-ttu-id="041e9-163">حدد الزر **التالي** في الركن الأيسر السفلي من الشريط الجانبي.</span><span class="sxs-lookup"><span data-stu-id="041e9-163">Select the **Next** button in the bottom-right corner of the side bar.</span></span>
2. <span data-ttu-id="041e9-164">حدد **مغادرة** في النافذة المنبثقة التي تظهر.</span><span class="sxs-lookup"><span data-stu-id="041e9-164">Select **Leave** in the pop-up window that appears.</span></span>
