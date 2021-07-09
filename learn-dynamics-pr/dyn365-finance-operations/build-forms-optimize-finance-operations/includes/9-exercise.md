---
ms.openlocfilehash: a1182ad59b8a5b682e5a1a0af29b94cb8d07e581
ms.sourcegitcommit: 977539219691830a564399fa637ced040d24475e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "6072563"
---
## <a name="scenario"></a><span data-ttu-id="abffa-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="abffa-101">Scenario</span></span>

<span data-ttu-id="abffa-102">طُلب من مطور تطبيقات Finance and Operations إنشاء نموذج جديد لشركة Fleet Management.</span><span class="sxs-lookup"><span data-stu-id="abffa-102">The Finance and Operations apps developer has been asked to create a new form for the Fleet Management company.</span></span> <span data-ttu-id="abffa-103">وترغب الشركة في عمل صفحة بسيطة لإدخال معلومات العميل.</span><span class="sxs-lookup"><span data-stu-id="abffa-103">The company wants a simple page to enter customer information.</span></span> <span data-ttu-id="abffa-104">يريدون أن يسحب النموذج الحقول من عنصر `CustTable`.</span><span class="sxs-lookup"><span data-stu-id="abffa-104">They want the form to pull fields from the `CustTable` element.</span></span>


## <a name="create-a-new-project"></a><span data-ttu-id="abffa-105">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="abffa-105">Create a new project</span></span> 

1.  <span data-ttu-id="abffa-106">أغلق نافذة مستعرض الإنترنت في بيئة المعمل.</span><span class="sxs-lookup"><span data-stu-id="abffa-106">Close the Internet browser window in the Lab environment.</span></span>
2.  <span data-ttu-id="abffa-107">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="abffa-107">Open Visual Studio.</span></span>
3.  <span data-ttu-id="abffa-108">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="abffa-108">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
2.  <span data-ttu-id="abffa-109">انتقل إلى قائمة **Dynamics 365** في الشريط في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="abffa-109">Go to the **Dynamics 365** menu in the ribbon in Visual Studio.</span></span>
3.  <span data-ttu-id="abffa-110">حدد **إدارة النماذج > تحديث معلمات النموذج**.</span><span class="sxs-lookup"><span data-stu-id="abffa-110">Select **Model management > Update model parameters**.</span></span>
4.  <span data-ttu-id="abffa-111">في الحقل **اسم النموذج** حدد **إدارة الأسطول**.</span><span class="sxs-lookup"><span data-stu-id="abffa-111">In the **Model name** field select **Fleet Management**.</span></span>
5.  <span data-ttu-id="abffa-112">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="abffa-112">Select **Next**.</span></span>
6.  <span data-ttu-id="abffa-113">حدد النماذج التالية عن طريق تحديد علامة الاختيار بجوار النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-113">Select the following models, by selecting the checkmark next to the model.</span></span> <span data-ttu-id="abffa-114">يجب أن تظل أي نماذج تم تحديدها بالفعل محددة.</span><span class="sxs-lookup"><span data-stu-id="abffa-114">Any models that are already selected should remain selected.</span></span>
    - <span data-ttu-id="abffa-115">ApplicationCommon</span><span class="sxs-lookup"><span data-stu-id="abffa-115">ApplicationCommon</span></span>
    - <span data-ttu-id="abffa-116">ApplicationFoundation</span><span class="sxs-lookup"><span data-stu-id="abffa-116">ApplicationFoundation</span></span>
    - <span data-ttu-id="abffa-117">ApplicationPlatform</span><span class="sxs-lookup"><span data-stu-id="abffa-117">ApplicationPlatform</span></span>
    - <span data-ttu-id="abffa-118">ApplicationSuite</span><span class="sxs-lookup"><span data-stu-id="abffa-118">ApplicationSuite</span></span>
    - <span data-ttu-id="abffa-119">ContactPerson</span><span class="sxs-lookup"><span data-stu-id="abffa-119">ContactPerson</span></span>
    - <span data-ttu-id="abffa-120">العملة</span><span class="sxs-lookup"><span data-stu-id="abffa-120">Currency</span></span>
    - <span data-ttu-id="abffa-121">GeneralLedger</span><span class="sxs-lookup"><span data-stu-id="abffa-121">GeneralLedger</span></span>
    - <span data-ttu-id="abffa-122">دفتر الأستاذ</span><span class="sxs-lookup"><span data-stu-id="abffa-122">Ledger</span></span>
    - <span data-ttu-id="abffa-123">العاملون</span><span class="sxs-lookup"><span data-stu-id="abffa-123">Personnel</span></span>
    - <span data-ttu-id="abffa-124">البيع بالتجزئة</span><span class="sxs-lookup"><span data-stu-id="abffa-124">Retail</span></span>
    - <span data-ttu-id="abffa-125">الضريبة</span><span class="sxs-lookup"><span data-stu-id="abffa-125">Tax</span></span>
7.  <span data-ttu-id="abffa-126">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="abffa-126">Select **Next**.</span></span>
8.  <span data-ttu-id="abffa-127">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="abffa-127">Select **Finish**.</span></span>
2.  <span data-ttu-id="abffa-128">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="abffa-128">Open the **File** menu and select **New > Project**.</span></span>
3.  <span data-ttu-id="abffa-129">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="abffa-129">In the **New project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Installed**.</span></span>
4.  <span data-ttu-id="abffa-130">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="abffa-130">On the middle pane, select **Finance Operations**.</span></span>
5.  <span data-ttu-id="abffa-131">قُم بتسمية المشروع **FleetManagementFormProject**.</span><span class="sxs-lookup"><span data-stu-id="abffa-131">Name the project **FleetManagementFormProject**.</span></span>
6.  <span data-ttu-id="abffa-132">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="abffa-132">Select **OK**.</span></span>
7.  <span data-ttu-id="abffa-133">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="abffa-133">Open the **Dynamics 365** menu in the ribbon.</span></span>
8.  <span data-ttu-id="abffa-134">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="abffa-134">Select **Options**.</span></span>
9.  <span data-ttu-id="abffa-135">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="abffa-135">Under the **Dynamics 365** node on the left pane, select  **Projects**.</span></span>
10. <span data-ttu-id="abffa-136">تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **ومزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="abffa-136">Ensure that the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project** are selected already.</span></span> <span data-ttu-id="abffa-137">إذا لم تكن كذلك، فقم بذلك.</span><span class="sxs-lookup"><span data-stu-id="abffa-137">If they are not, then do so.</span></span>
11. <span data-ttu-id="abffa-138">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="abffa-138">Select **OK**.</span></span>

## <a name="create-a-form"></a><span data-ttu-id="abffa-139">إنشاء نموذج</span><span class="sxs-lookup"><span data-stu-id="abffa-139">Create a form</span></span> 

1.  <span data-ttu-id="abffa-140">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementFormProject (ISV)**.</span><span class="sxs-lookup"><span data-stu-id="abffa-140">In the **Solution Explorer** window, right-click the project     **FleetManagementFormProject (ISV)**.</span></span>
2.  <span data-ttu-id="abffa-141">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="abffa-141">Select **Add > New Item**.</span></span>
3.  <span data-ttu-id="abffa-142">ضمن **عناصر Dynamics 365** حدد **واجهة المستخدم**.</span><span class="sxs-lookup"><span data-stu-id="abffa-142">Under **Dynamics 365 Items** select **User Interface**.</span></span>
4.  <span data-ttu-id="abffa-143">في الجزء الأوسط، حدد **نموذج**.</span><span class="sxs-lookup"><span data-stu-id="abffa-143">On the middle pane, select **Form**.</span></span>
5.  <span data-ttu-id="abffa-144">في حقل **الاسم** أدخل **FleetCustomersForm**.</span><span class="sxs-lookup"><span data-stu-id="abffa-144">Enter **FleetCustomersForm** in the **Name** field.</span></span>
6.  <span data-ttu-id="abffa-145">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="abffa-145">Select **Add**.</span></span> <span data-ttu-id="abffa-146">سيتم الآن فتح نموذج **FleetCustomersForm** في نافذة مصمم النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-146">The **FleetCustomersForm** form will now open in the form designer window.</span></span>

## <a name="add-a-pattern-and-data-source-to-the-form"></a><span data-ttu-id="abffa-147">إضافة نمط ومصدر بيانات إلى النموذج</span><span class="sxs-lookup"><span data-stu-id="abffa-147">Add a pattern and data source to the form</span></span> 

1.  <span data-ttu-id="abffa-148">في نافذة مصمم النموذج، انقر بزر الماوس الأيمن فوق عقدة **تصميم** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="abffa-148">In the form designer window, right-click the **Design** node on the right pane.</span></span>
2.  <span data-ttu-id="abffa-149">حدد **تطبيق النمط > قائمة بسيطة**.</span><span class="sxs-lookup"><span data-stu-id="abffa-149">Select **Apply pattern > Simple List**.</span></span>
3.  <span data-ttu-id="abffa-150">في الجزء الأيمن من نافذة مصمم النماذج، انقر بزر الماوس الأيمن فوق العقدة **مصادر البيانات**.</span><span class="sxs-lookup"><span data-stu-id="abffa-150">On the left pane of the form designer window, right-click the **Data Sources** node.</span></span>
4.  <span data-ttu-id="abffa-151">حدد **مصدر بيانات جديد**.</span><span class="sxs-lookup"><span data-stu-id="abffa-151">Select **New Data Source**.</span></span>
5.  <span data-ttu-id="abffa-152">باستخدام العنصر الجديد **DataSource1** المُحدد، انتقل إلى نافذة **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="abffa-152">With the new item **DataSource1** selected, go to the **Properties** window.</span></span>
6.  <span data-ttu-id="abffa-153">بالنسبة إلى خاصية **الجدول**، حدد **CustTable** من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="abffa-153">For the **Table** property, select **CustTable** from the drop-down menu.</span></span>
7.  <span data-ttu-id="abffa-154">حدد **حفظ** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="abffa-154">Select **Save** in the ribbon.</span></span>

## <a name="build-the-simple-list-form-pattern"></a><span data-ttu-id="abffa-155">قم بإنشاء نمط نموذج قائمة بسيط</span><span class="sxs-lookup"><span data-stu-id="abffa-155">Build the simple list form pattern</span></span>  

1.  <span data-ttu-id="abffa-156">انقر في الجزء السفلي **نمط** من مصمم النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-156">Click in the bottom **Pattern** pane of the form designer.</span></span> <span data-ttu-id="abffa-157">تحتاج إلى **ActionPane** و **مجموعة** و **شبكة** لإكمال نمط النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-157">You need an **ActionPane**, **Group**, and **Grid** to complete the form pattern.</span></span>
2.  <span data-ttu-id="abffa-158">في الجزء الأيسر من مصمم النموذج، انقر بزر الماوس الأيمن فوق العقدة **تصميم**.</span><span class="sxs-lookup"><span data-stu-id="abffa-158">On the right pane of the form designer, right-click the **Design** node.</span></span>
3.  <span data-ttu-id="abffa-159">حدد **جديد> جزء الإجراءات**.</span><span class="sxs-lookup"><span data-stu-id="abffa-159">Select **New > Action Pane**.</span></span>
4.  <span data-ttu-id="abffa-160">مع تحديد عقدة جزء الإجراء الجديدة، انتقل إلى نافذة **الخصائص** وقم بتغيير خاصية **الاسم** إلى **ActionPane**.</span><span class="sxs-lookup"><span data-stu-id="abffa-160">With the new Action Pane node selected, go to the **Properties** window and change the **Name** property to **ActionPane**.</span></span>
5.  <span data-ttu-id="abffa-161">قم بطي عقدة **ActionPane** للحفاظ على تبسيط الجزء الأيمن من عقدة التصميم.</span><span class="sxs-lookup"><span data-stu-id="abffa-161">Collapse the **ActionPane** node to keep the right pane of the design node simplified.</span></span>
6.  <span data-ttu-id="abffa-162">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="abffa-162">Select **Save**.</span></span>
7.  <span data-ttu-id="abffa-163">انقر بزر الماوس الأيمن فوق عقدة **تصميم** في الجزء الأيمن من مصمم النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-163">Right-click the **Design** node on the right pane of the form designer.</span></span>
8.  <span data-ttu-id="abffa-164">حدد **جديد > مجموعة**.</span><span class="sxs-lookup"><span data-stu-id="abffa-164">Select **New > Group**.</span></span>
9.  <span data-ttu-id="abffa-165">بعد تحديد المجموعة الجديدة، انتقل إلى نافذة **الخصائص** وقم بتغيير خاصية **الاسم** إلى **عوامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="abffa-165">With the new group selected, go to the **Properties** window and change the **Name** property to **Filters**.</span></span>
10.  <span data-ttu-id="abffa-166">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="abffa-166">Select **Save**.</span></span>
10. <span data-ttu-id="abffa-167">انقر بزر الماوس الأيمن فوق عقدة **عوامل التصفية** في الجزء الأيمن من مصمم النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-167">Right-click the **Filters** node on the right pane of the form designer.</span></span>
11. <span data-ttu-id="abffa-168">حدد **تطبيق النمط > عوامل التصفية المخصصة والسريعة**.</span><span class="sxs-lookup"><span data-stu-id="abffa-168">Select **Apply pattern > Custom and Quick Filters**.</span></span>
12. <span data-ttu-id="abffa-169">انقر بزر الماوس الأيمن فوق عقدة **عوامل التصفية** في الجزء الأيمن من مصمم النموذج مرة أخرى..</span><span class="sxs-lookup"><span data-stu-id="abffa-169">Right-click the **Filters** node on the right pane of the form designer again.</span></span>
13. <span data-ttu-id="abffa-170">حدد **جديد > QuickFilter**.</span><span class="sxs-lookup"><span data-stu-id="abffa-170">Select **New > QuickFilter**.</span></span>
14. <span data-ttu-id="abffa-171">بعد تحديد عامل التصفية السريع الجديد، انتقل إلى نافذة **الخصائص** وقم بتغيير خاصية **الاسم** إلى **QuickFilter**.</span><span class="sxs-lookup"><span data-stu-id="abffa-171">With the new QuickFilter selected, go to the **Properties** window and change the **Name** property to **QuickFilter**.</span></span>
15. <span data-ttu-id="abffa-172">في الجزء الأيمن من مصمم النموذج، قم بطي عقدة **عوامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="abffa-172">On the right pane of the form designer, collapse the **Filters** node.</span></span>
16. <span data-ttu-id="abffa-173">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="abffa-173">Select **Save**.</span></span>
17. <span data-ttu-id="abffa-174">انقر بزر الماوس الأيمن فوق عقدة **تصميم** الرئيسية في الجزء الأيمن من مصمم النموذج.</span><span class="sxs-lookup"><span data-stu-id="abffa-174">Right-click the main **Design** node on the right pane of the form designer.</span></span>
18. <span data-ttu-id="abffa-175">حدد **جديد > شبكة**.</span><span class="sxs-lookup"><span data-stu-id="abffa-175">Select **New > Grid**.</span></span>
19. <span data-ttu-id="abffa-176">بعد تحديد المجموعة الجديدة، قم بتغيير خاصية **الاسم** نافذة **الخصائص** إلى **MainGrid**.</span><span class="sxs-lookup"><span data-stu-id="abffa-176">With the new Grid selected, change the **Name** property in the **Properties** window to **MainGrid**.</span></span>
20. <span data-ttu-id="abffa-177">في الجزء الأيسر من مصمم النموذج، ضمن عُقدة **مصادر البيانات**، وضمن عُقدة **CustTable**، قم بتوسيع عقدة **الحقول**.</span><span class="sxs-lookup"><span data-stu-id="abffa-177">On the left pane of the form designer, under the **Data Sources** node, and under the  **CustTable** node, expand the **Fields** node.</span></span>
22. <span data-ttu-id="abffa-178">حدد واسحب الحقول **Party** و **SalesGroup** و **CustGroup** و **AccountNum** من عقدة **الحقول** في عقدة **MainGrid** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="abffa-178">Select and drag the **Party**, **SalesGroup**, **CustGroup**, and **AccountNum** fields from the **Fields** node onto the **MainGrid** node on the right pane.</span></span>
23. <span data-ttu-id="abffa-179">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="abffa-179">Select **Save**.</span></span>
24. <span data-ttu-id="abffa-180">قم بتنفيذ إنشاء بالنقر بزر الماوس الأيمن فوق **FleetManagementFormProject (ISV)** في نافذة **مستكشف الحلول** ثم تحديد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="abffa-180">Perform a build by right-clicking the project **FleetManagementFormProject (ISV)** in the **Solution Explorer** window and then selecting **Build.**</span></span>

## <a name="preview-the-form-in-a-browser"></a><span data-ttu-id="abffa-181">معاينه النموذج في مستعرض</span><span class="sxs-lookup"><span data-stu-id="abffa-181">Preview the form in a browser</span></span> 

1.  <span data-ttu-id="abffa-182">بعد اكتمال الإنشاء بدون أخطاء، انقر بزر الماوس الأيمن فوق النموذج **FleetCustomersForm** في نافذه **مستكشف الحلول**.</span><span class="sxs-lookup"><span data-stu-id="abffa-182">After the build is completed without errors, right-click the form **FleetCustomersForm** in the **Solution Explorer** window.</span></span>
2.  <span data-ttu-id="abffa-183">حدد **تعيين ككائن بدء التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="abffa-183">Select **Set as Startup Object**.</span></span>
3.  <span data-ttu-id="abffa-184">حدد **Ctrl + F5** أو حدد **أبدأ** في الشريط لبدء تشغيل المشروع.</span><span class="sxs-lookup"><span data-stu-id="abffa-184">Select **Ctrl + F5** or select **Start** in the ribbon to begin running the project.</span></span> <span data-ttu-id="abffa-185">ستفتح نافذة مستعرض الإنترنت لعرض النموذج الذي تم إنشاؤه حديثاً (قد يستغرق ذلك دقيقتين).</span><span class="sxs-lookup"><span data-stu-id="abffa-185">An Internet browser window will open to display the newly created form (this can take a couple of minutes).</span></span>
5.  <span data-ttu-id="abffa-186">قم بإضافة بعض السجلات إلى النموذج عن طريق تحديد الزر **جديد** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="abffa-186">Add a few records to the form by selecting the **New** button in the Action Pane.</span></span>

## <a name="close-the-lab-environment"></a><span data-ttu-id="abffa-187">أغلق بيئة التمرين العملي</span><span class="sxs-lookup"><span data-stu-id="abffa-187">Close the lab environment</span></span> 

1. <span data-ttu-id="abffa-188">حدد الزر **التالي** في الركن الأيسر السفلي من الشريط الجانبي.</span><span class="sxs-lookup"><span data-stu-id="abffa-188">Select the **Next** button in the bottom-right corner of the side bar.</span></span>
2. <span data-ttu-id="abffa-189">حدد **مغادرة** في النافذة المنبثقة التي تظهر.</span><span class="sxs-lookup"><span data-stu-id="abffa-189">Select **Leave** in the pop-up window that appears.</span></span>

