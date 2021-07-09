---
ms.openlocfilehash: 949c4b6f93b03b7b068ae57365cc5df91a38f3aa
ms.sourcegitcommit: 22cf3947ad672b7b54cfc646440e4e93cc1dd9d4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/12/2021
ms.locfileid: "6071006"
---
<span data-ttu-id="173b0-101">سيركز هذا التمرين بشكل خاص على العمليات أو مهام الأعمال التالية.</span><span class="sxs-lookup"><span data-stu-id="173b0-101">This exercise will focus specifically on the following business processes or tasks.</span></span>

- <span data-ttu-id="173b0-102">إنشاء تدرج هرمي تنظيمي لتخطيط الموازنة وتكوين أمان المستخدم</span><span class="sxs-lookup"><span data-stu-id="173b0-102">Creating an organizational hierarchy for budget planning and configuring user security</span></span>

- <span data-ttu-id="173b0-103">تحديد سيناريوهات خطه الموازنة وأعمدة خطة الموازنة والتخطيطات وقوالب Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="173b0-103">Defining budget plan scenarios, budget plan columns, layouts, and Microsoft Excel templates</span></span>
 
- <span data-ttu-id="173b0-104">إنشاء وتنشيط عملية تخطيط الموازنة</span><span class="sxs-lookup"><span data-stu-id="173b0-104">Creating and activating the budget planning process</span></span>
 
- <span data-ttu-id="173b0-105">إنشاء مستند خطة الموازنة عن طريق سحب القيم الفعلية من دفتر الأستاذ العام</span><span class="sxs-lookup"><span data-stu-id="173b0-105">Creating a budget plan document by pulling in actuals from General ledger</span></span>
 
- <span data-ttu-id="173b0-106">استخدام التخصيصات لضبط بيانات وثيقة خطة الموازنة</span><span class="sxs-lookup"><span data-stu-id="173b0-106">Using allocations to adjust budget plan document data</span></span>
 
- <span data-ttu-id="173b0-107">تحرير بيانات وثيقة خطة الموازنة في Excel</span><span class="sxs-lookup"><span data-stu-id="173b0-107">Editing budget plan document data in Excel</span></span>

## <a name="prerequisites"></a><span data-ttu-id="173b0-108">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="173b0-108">Prerequisites</span></span>

<span data-ttu-id="173b0-109">لتحقيق أقصى استفادة من هذا التمرين، نوصي بأن يكون لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Finance والتي تم تثبيتها باستخدام Lifecycle Services ‏(LCS)، وأن يتم توفيرها كمسؤول في المثيل.</span><span class="sxs-lookup"><span data-stu-id="173b0-109">To get the most benefit from this exercise we recommend that you have the standard sample data available in Dynamics 365 Finance that is installed by using Lifecycle Services (LCS), and be provisioned as an administrator on the instance.</span></span> 

<span data-ttu-id="173b0-110">لا تستخدم في وضع المستعرض الخاص لهذا التمرين ؛ قم بتسجيل الخروج من أي حساب آخر في المستعرض، إذا لزم الأمر، وقم بتسجيل الدخول باستخدام بيانات اعتماد مسؤول الشؤون المالية.</span><span class="sxs-lookup"><span data-stu-id="173b0-110">Do not use In Private browser mode for this exercise; sign out from any other account in the browser, if needed, and sign in with Finance administrator credentials.</span></span> <span data-ttu-id="173b0-111">عند تسجيل الدخول إلى Finance، يجب تحديد خانة الاختيار **ابقني مسجل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="173b0-111">When signing into Finance, you must select the **Keep me signed in** check box.</span></span>

<span data-ttu-id="173b0-112">يؤدي هذا إلى إنشاء ملف تعريف ارتباط دائم يحتاجه تطبيق Excel حالياً.</span><span class="sxs-lookup"><span data-stu-id="173b0-112">This creates a persistent cookie that the Excel app currently needs.</span></span> <span data-ttu-id="173b0-113">إذا قمت بتسجيل الدخول إلى Dynamics 365 Finance باستخدام مستعرض آخر بخلاف Internet Explorer، فستتم مطالبتك بتسجيل الدخول في تطبيق Excel.</span><span class="sxs-lookup"><span data-stu-id="173b0-113">If you sign in to Dynamics 365 Finance by using a browser other than Internet Explorer, then you'll be prompted to sign in within the Excel app.</span></span> <span data-ttu-id="173b0-114">عند تحديد **تسجيل الدخول** في تطبيق Excel، سيتم فتح نافذة IE المنبثقة.</span><span class="sxs-lookup"><span data-stu-id="173b0-114">When you select **Sign in** in the Excel app, an IE popup window will open.</span></span> <span data-ttu-id="173b0-115">عند تسجيل الدخول، يجب ليك تحديد خانة الاختيار **ابقني مسجل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="173b0-115">When signing in, you must select the **Keep me signed in** check box.</span></span> <span data-ttu-id="173b0-116">إذا لم يؤدي تحديد **تسجيل الدخول** في تطبيق Excel للقيام بأي شيء، فيجب عليك مسح ذاكره التخزين المؤقت لملفات تعريف الارتباط في IE.</span><span class="sxs-lookup"><span data-stu-id="173b0-116">If selecting **Sign in** in the Excel app doesn't appear to do anything, then you should clear the IE cookie cache.</span></span>

## <a name="scenario"></a><span data-ttu-id="173b0-117">السيناريو</span><span class="sxs-lookup"><span data-stu-id="173b0-117">Scenario</span></span>

<span data-ttu-id="173b0-118">تعمل Julia مدير تمويل في Contoso ‏Entertainment Systems في ألمانيا (DEMF).</span><span class="sxs-lookup"><span data-stu-id="173b0-118">Julia works as a finance manager in Contoso Entertainment Systems in Germany (DEMF).</span></span> <span data-ttu-id="173b0-119">مع اقتراب السنة المالية 2016، تحتاج إلى العمل على إعداد موازنة الشركة للعام المقبل.</span><span class="sxs-lookup"><span data-stu-id="173b0-119">As FY2016 approaches, she needs to work on setting up the company's budget for the upcoming year.</span></span> <span data-ttu-id="173b0-120">يبدو إعداد الموازنة على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="173b0-120">Budget preparation looks as follows:</span></span>

1.  <span data-ttu-id="173b0-121">تستخدم Julia المبالغ الفعلية للعام السابق كنقطة بداية لإنشاء الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-121">Julia uses previous year actuals amounts as a starting point to create the budget.</span></span>

2.  <span data-ttu-id="173b0-122">استناداً إلى القيم الفعلية للعام السابق، تقوم بإنشاء تقديرات لمدة 12 شهراً في العام المقبل.</span><span class="sxs-lookup"><span data-stu-id="173b0-122">Based on the previous year actuals, she creates estimates for 12 months in the upcoming year.</span></span>

3.  <span data-ttu-id="173b0-123">تستعرض Julia جوليا الموازنة مع المدير المالي.</span><span class="sxs-lookup"><span data-stu-id="173b0-123">Julia reviews the budget with the CFO.</span></span> <span data-ttu-id="173b0-124">بعد ذلك، تقوم بإجراء التعديلات اللازمة على خطة الميزانية وتنتهي من إعداد الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-124">Afterward, she makes necessary adjustments for the budget plan and finalizes budget preparation.</span></span> <span data-ttu-id="173b0-125">تستخدم Julia قالب Excel لإعداد الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-125">Julia uses an Excel template to prepare the budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="173b0-126">التكوين</span><span class="sxs-lookup"><span data-stu-id="173b0-126">Configuration</span></span>

### <a name="create-the-organizational-hierarchy"></a><span data-ttu-id="173b0-127">إنشاء التدرج الهرمي المؤسسي</span><span class="sxs-lookup"><span data-stu-id="173b0-127">Create the organizational hierarchy</span></span>

<span data-ttu-id="173b0-128">نظراً لأن عملية إعداد الميزانية بأكملها تحدث في قسم Finance، تحتاج Julia إلى إنشاء تدرج هرمي مؤسسي بسيط يتكون من قسم الشؤون المالية فقط.</span><span class="sxs-lookup"><span data-stu-id="173b0-128">Because the entire budgeting process happens in the Finance department, Julia needs to create a simple organizational hierarchy consisting of the Finance department only.</span></span>

1.  <span data-ttu-id="173b0-129">انتقل إلى **إدارة المؤسسة > المؤسسات > التدرجات الهرمية للمؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-129">Go to **Organization administration > Organizations > Organization hierarchies**.</span></span>

2.  <span data-ttu-id="173b0-130">حدد الزر **جديد**.</span><span class="sxs-lookup"><span data-stu-id="173b0-130">Select the **New** button.</span></span>

3.  <span data-ttu-id="173b0-131">اكتب اسم التدرج الهرمي المؤسسي وحدد ارتباط **تعيين الارتباط**.</span><span class="sxs-lookup"><span data-stu-id="173b0-131">Type the name for the organizational hierarchy and select the **Assign purpose** link.</span></span>

4.  <span data-ttu-id="173b0-132">حدد **تخطيط الموازنة**، وحدد الزر **إضافة**، ثم قم بتعيين التدرج الهرمي المؤسسي الذي تم إنشاؤه حديثاً.</span><span class="sxs-lookup"><span data-stu-id="173b0-132">Select **Budget planning**, select the **Add** button, and then assign the newly created organizational hierarchy.</span></span>

5.  <span data-ttu-id="173b0-133">كرر الخطوة أعلاه لغرض تنظيمي للأمان.</span><span class="sxs-lookup"><span data-stu-id="173b0-133">Repeat the step above for Security organizational purpose.</span></span>

6.  <span data-ttu-id="173b0-134">أغلق الصفحة عند إتمام العملية.</span><span class="sxs-lookup"><span data-stu-id="173b0-134">Close the page when done.</span></span>

7.  <span data-ttu-id="173b0-135">في صفحة **التدرجات الهرمية للمؤسسة**، حدد الزر **عرض**.</span><span class="sxs-lookup"><span data-stu-id="173b0-135">In the **Organization hierarchies** page, select the **View** button.</span></span> <span data-ttu-id="173b0-136">حدد **تحرير** في مصمم التدرج الهرمي وقم بإنشاء تدرج هرمي بتحديد الزر **إدراج**.</span><span class="sxs-lookup"><span data-stu-id="173b0-136">Select **Edit** in the Hierarchy designer and create a hierarchy by selecting the **Insert** button.</span></span>

8.  <span data-ttu-id="173b0-137">حدد **قسم Finance** للتدرج الهرمي لإعداد الموازنات.</span><span class="sxs-lookup"><span data-stu-id="173b0-137">Select **Finance department** for the budgeting hierarchy.</span></span>

9.  <span data-ttu-id="173b0-138">عند الانتهاء، حدد **نشر وإغلاق**.</span><span class="sxs-lookup"><span data-stu-id="173b0-138">When done, select **Publish and Close**.</span></span> <span data-ttu-id="173b0-139">حدد **1/1/2019** كتاريخ سريان للنشر الخاص بالتدرج الهرمي.</span><span class="sxs-lookup"><span data-stu-id="173b0-139">Select **1/1/2019** as the effective date for hierarchy publishing.</span></span>

### <a name="configure-user-security"></a><span data-ttu-id="173b0-140">تكوين أمان المستخدم</span><span class="sxs-lookup"><span data-stu-id="173b0-140">Configure user security</span></span>

<span data-ttu-id="173b0-141">يستخدم تخطيط الميزانية سياسات أمان خاصة لتكوين الوصول إلى بيانات خطة الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-141">Budget planning uses special security policies to configure access to budget plan data.</span></span> <span data-ttu-id="173b0-142">تحتاج Julia إلى منح نفسها حق الوصول إلى خطط موازنة Finance.</span><span class="sxs-lookup"><span data-stu-id="173b0-142">Julia needs to give herself access to Finance budget plans.</span></span>

1. <span data-ttu-id="173b0-143">في DEMF، انتقل إلى **إعداد الموازنة > الإعداد > تخطيط الموازنة > تكوين تخطيط الموازنة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-143">In DEMF, go to **Budgeting > Setup > Budget planning > Budget planning configuration**.</span></span>

2. <span data-ttu-id="173b0-144">في علامة التبويب **المعلمات**، قم بتعيين قيمة **نموذج الأمان** إلى **استناداً إلى مؤسسات الأمان**.</span><span class="sxs-lookup"><span data-stu-id="173b0-144">In the **Parameters** tab, set the **Security model** value to  **Based on security organizations**.</span></span>

3. <span data-ttu-id="173b0-145">انقر على **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="173b0-145">Click **Save**.</span></span> 

3. <span data-ttu-id="173b0-146">انتقل إلى **إدارة النظام > المستخدمون > المستخدمون**.</span><span class="sxs-lookup"><span data-stu-id="173b0-146">Go to **System administration > Users > Users**.</span></span>

4. <span data-ttu-id="173b0-147">للمستخدم **المسؤول** (‏Julia Funderburk) قم بتعيين **دور مدير الموازنة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-147">Assign the user **Admin** (Julia Funderburk) the **Budget manager role**.</span></span>

5. <span data-ttu-id="173b0-148">قم بانتقاء دور المستخدم وحدد **تعيين المؤسسات**.</span><span class="sxs-lookup"><span data-stu-id="173b0-148">Pick the user role and select **Assign organizations**.</span></span>

6. <span data-ttu-id="173b0-149">حدد **منح حق الوصول إلى مؤسسات محددة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-149">Select **Grant access to specific organizations**.</span></span>

7. <span data-ttu-id="173b0-150">قم بانتقاء التدرج الهرمي التنظيمي الذي تم إنشاؤه في الخطوة الأولى.</span><span class="sxs-lookup"><span data-stu-id="173b0-150">Pick the Organizational hierarchy that was created in the first  step.</span></span>

8. <span data-ttu-id="173b0-151">قم بانتقاء عقدة **Finance** وحدد زر **منح مع الفروع**.</span><span class="sxs-lookup"><span data-stu-id="173b0-151">Pick the **Finance** node and select the **Grant with children** button.</span></span>

<span data-ttu-id="173b0-152">لاحظ أنك قد تحتاج إلى تحديث المستعرض الخاص بك لتفعيل سياسة **أمان البيانات القابلة للتوسعة‬ (XDS)** في المرة التالية التي تقوم فيها بتسجيل الدخول إلى Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="173b0-152">Note that you might need to refresh your browser to have the **eXtensible Data Security (XDS)** policy take effect the next time you log in to Dynamics 365 Finance.</span></span>

### <a name="create-scenarios"></a><span data-ttu-id="173b0-153">إنشاء السيناريوهات</span><span class="sxs-lookup"><span data-stu-id="173b0-153">Create scenarios</span></span>

1.  <span data-ttu-id="173b0-154">في DEMF، انتقل إلى **إعداد الموازنة > الإعداد > تخطيط الموازنة > تكوين تخطيط الموازنة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-154">In DEMF, go to **Budgeting > Setup > Budget planning > Budget planning configuration**.</span></span>

2.  <span data-ttu-id="173b0-155">في صفحة **السيناريوهات**، ستستخدم **القيم الفعلية والموازنة للعام السابق**.</span><span class="sxs-lookup"><span data-stu-id="173b0-155">In the **Scenarios** page, you will use **Previous year actuals and Budgeted**.</span></span>

### <a name="create-budget-plan-columns"></a><span data-ttu-id="173b0-156">إنشاء أعمدة خطة موازنة</span><span class="sxs-lookup"><span data-stu-id="173b0-156">Create budget plan columns</span></span>

<span data-ttu-id="173b0-157">أعمدة خطة الموازنة هي أعمدة نقدية أو أعمدة قائمة على الكمية يمكن استخدامها في تخطيط مستند خطة الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-157">Budget plan columns are either Monetary or quantity-based columns that can be used in budget plan document layout.</span></span> <span data-ttu-id="173b0-158">في هذا المثال، تحتاج إلى إنشاء عمود للقيم الفعلية للسنة السابقة و12 عموداً لتمثيل كل شهر في سنة الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-158">In this example, you need to create a column for Previous year actuals and 12 columns to represent each month in a budgeted year.</span></span>

<span data-ttu-id="173b0-159">يمكن إنشاء الأعمدة إما ببساطة عن طريق تحديد الزر **إضافة** وملء القيم، أو بمساعدة كيان البيانات.</span><span class="sxs-lookup"><span data-stu-id="173b0-159">Columns can be created either by simply selecting the **Add** button and filling in the values, or with the help of Data entity.</span></span> <span data-ttu-id="173b0-160">في هذا التمرين، ستستخدم كيان البيانات لملء القيم.</span><span class="sxs-lookup"><span data-stu-id="173b0-160">In this exercise, you will use Data entity to fill in the values.</span></span>
<span data-ttu-id="173b0-161">مهم - يجب عليك استخدام Microsoft Excel ‏2016 لإكمال هذا التمرين.</span><span class="sxs-lookup"><span data-stu-id="173b0-161">Important - You must use Microsoft Excel 2016 to complete this exercise.</span></span> 

1.  <span data-ttu-id="173b0-162">في DEMF، انتقل إلى **إعداد الموازنة > الإعداد > تخطيط الموازنة > تكوين تخطيط الموازنة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-162">In DEMF, go to **Budgeting > Setup > Budget planning > Budget planning configuration**.</span></span>

2.  <span data-ttu-id="173b0-163">حدد صفحة **الأعمدة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-163">Select the **Columns** page.</span></span>

3.  <span data-ttu-id="173b0-164">حدد زر **Office** في الزاوية العلوية اليمنى من الصفحة واختر **الأعمدة (غير مصفاة)**.</span><span class="sxs-lookup"><span data-stu-id="173b0-164">Select the **Office** button on the top right corner of the page and pick **Columns (unfiltered)**.</span></span>

4.  <span data-ttu-id="173b0-165">سيقوم النظام بفتح مصنف Excel يمكنك استخدامه لتعبئة القيم.</span><span class="sxs-lookup"><span data-stu-id="173b0-165">The system will open an Excel workbook that you can use to fill in the values.</span></span> <span data-ttu-id="173b0-166">إذا طُلب منك، حدد **تمكين لتحرير** و **الوثوق بهذا التطبيق**.</span><span class="sxs-lookup"><span data-stu-id="173b0-166">If prompted, select **Enable editing** and **Trust this app**.</span></span>

5.  <span data-ttu-id="173b0-167">ستحتاج إلى المزيد من الأعمدة لملء القيم.</span><span class="sxs-lookup"><span data-stu-id="173b0-167">You will need more columns in which to fill the values.</span></span> <span data-ttu-id="173b0-168">حدد **تصميم** في الجزء الموجود على الجانب الأيمن لإضافة الأعمدة إلى الشبكة.</span><span class="sxs-lookup"><span data-stu-id="173b0-168">Select **Design** on the right-side pane to add the columns to the grid.</span></span>

6.  <span data-ttu-id="173b0-169">حدد زر قلم الرصاص الصغير الموجود بجوار **PlanColumns** لعرض الأعمدة المتوفرة لإضافتها إلى الشبكة.</span><span class="sxs-lookup"><span data-stu-id="173b0-169">Select the little pencil button next to **PlanColumns** to view available columns to add to the grid.</span></span>

7.  <span data-ttu-id="173b0-170">انقر نقراً مزدوجاً فوق كل حقل متوفر لإضافته إلى الحقول المحددة، ثم حدد **تحديث**</span><span class="sxs-lookup"><span data-stu-id="173b0-170">Double-click each available field to add them to Selected fields, and then select **Update**.</span></span>

8.  <span data-ttu-id="173b0-171">في جدول Excel، أضف جميع الأعمدة التي يلزم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="173b0-171">In the Excel table, add all the columns that need to be created.</span></span> <span data-ttu-id="173b0-172">استخدم ميزة **التعبئة التلقائية** في Excel لإضافة البنود بسرعة.</span><span class="sxs-lookup"><span data-stu-id="173b0-172">Use the **AutoFill** feature in Excel to add the lines quickly.</span></span> <span data-ttu-id="173b0-173">تأكد من إضافة الخطوط كجزء من الجدول (عند استخدام التمرير العمودي، يجب أن تكون قادراً على رؤية رؤوس الأعمدة أعلى الشبكة).</span><span class="sxs-lookup"><span data-stu-id="173b0-173">Make sure the lines are added as a part of the table (when using vertical scroll, you should be able to see column headers on the top of the grid).</span></span>

9.  <span data-ttu-id="173b0-174">ارجع إلى Finance وقم بتحديث الصفحة.</span><span class="sxs-lookup"><span data-stu-id="173b0-174">Return to Finance and refresh the page.</span></span> <span data-ttu-id="173b0-175">ستظهر القيم المنشورة في Finance.</span><span class="sxs-lookup"><span data-stu-id="173b0-175">Published values will appear in Finance.</span></span>

### <a name="create-budget-plan-document-layouts-and-templates"></a><span data-ttu-id="173b0-176">إنشاء تخطيطات وقوالب وثيقة خطة الموازنة</span><span class="sxs-lookup"><span data-stu-id="173b0-176">Create budget plan document layouts and templates</span></span>

<span data-ttu-id="173b0-177">يحدد التخطيط كيف ستبدو شبكة خطوط وثيقة خطة الموازنة عندما يفتح المستخدم مستند خطة الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-177">Layout defines how the budget plan document lines grid is going to look like when the user opens the budget plan document.</span></span> <span data-ttu-id="173b0-178">من الممكن أيضاً تبديل تخطيط مستند خطة الموازنة لعرض نفس البيانات بزوايا مختلفة.</span><span class="sxs-lookup"><span data-stu-id="173b0-178">It is also possible to switch the layout for the budget plan document to view the same data in different angles.</span></span>

<span data-ttu-id="173b0-179">الآن بعد أن حددت أعمدة يمكن استخدامها مع مستند خطة الموازنة، تحتاج Julia إلى إنشاء تخطيط مستند لخطة الموازنة، والذي سيبدو مشابهاً لجدول Excel الذي تستخدمه لإنشاء بيانات الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-179">Now that you have defined columns that can be used with the budget plan document, Julia needs to create a budget plan document layout, which would look similar to the Excel table that she uses to create budget data.</span></span>

1. <span data-ttu-id="173b0-180">في DEMF، انتقل إلى **إعداد الموازنة > الإعداد > تخطيط الموازنة > تكوين تخطيط الموازنة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-180">In DEMF, go to **Budgeting > Setup > Budget planning > Budget planning configuration**.</span></span>

2. <span data-ttu-id="173b0-181">حدد صفحة **التخطيطات**.</span><span class="sxs-lookup"><span data-stu-id="173b0-181">Select the **Layouts** page.</span></span>

3. <span data-ttu-id="173b0-182">أنشئ تخطيطاً جديداً لإدخال الموازنة الشهرية.</span><span class="sxs-lookup"><span data-stu-id="173b0-182">Create a new layout for the Monthly budget entry.</span></span> <span data-ttu-id="173b0-183">حدد مجموعة أبعاد **MA+BU** لتضمين الحسابات الرئيسية ووحدات الأعمال في التخطيط.</span><span class="sxs-lookup"><span data-stu-id="173b0-183">Select the **MA+BU** dimension set to include Main accounts and Business units to the layout.</span></span>
<span data-ttu-id="173b0-184">بعد ذلك، قم بإدراج جميع أعمدة خطة الموازنة، التي تم إنشاؤها في الخطوة السابقة، في قسم **العناصر**.</span><span class="sxs-lookup"><span data-stu-id="173b0-184">Then, list all budget plan columns, which were created in the previous step, in the **Elements** section.</span></span> <span data-ttu-id="173b0-185">اجعل جميع القيم الفعلية باستثناء قيم العام السابق قابلة للتعديل.</span><span class="sxs-lookup"><span data-stu-id="173b0-185">Make all but Previous year actuals editable.</span></span>

4. <span data-ttu-id="173b0-186">حدد الزر **أوصاف** لتحديد الأبعاد المالية التي يجب أن تعرض الأوصاف في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="173b0-186">Select the **Descriptions** button to select which financial dimensions should display Descriptions in the grid.</span></span>

    <span data-ttu-id="173b0-187">استناداً إلى تعريف تخطيط خطة الموازنة، يمكنك إنشاء قالب Excel لاستخدامه كطريقة بديلة لتحرير بيانات الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-187">Based on the budget plan layout definition, you can create an Excel template to be used as an alternative way to edit Budget data.</span></span> <span data-ttu-id="173b0-188">نظراً لأن قالب Excel يحتاج إلى أن يتطابق مع تعريف تخطيط خطة الموازنة، فلن تتمكن من تحرير تخطيط خطة الموازنة بعد إنشاء قالب Excel.</span><span class="sxs-lookup"><span data-stu-id="173b0-188">Because the Excel template needs to match the budget plan layout definition, you won't be able to edit the budget plan layout after generating the Excel template.</span></span> <span data-ttu-id="173b0-189">لذلك، يجب تنفيذ هذه المهمة بعد تحديد جميع مكونات التخطيط.</span><span class="sxs-lookup"><span data-stu-id="173b0-189">Therefore, this task should be done after all layout components are defined.</span></span>

5. <span data-ttu-id="173b0-190">بالنسبة للتخطيط الذي تم إنشاؤه، حدد الزر **القالب > إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="173b0-190">For the layout that was created, select the **Template > Generate** button.</span></span>

6. <span data-ttu-id="173b0-191">قم بتأكيد رسالة التحذير.</span><span class="sxs-lookup"><span data-stu-id="173b0-191">Confirm the warning message.</span></span>

7. <span data-ttu-id="173b0-192">لعرض القالب، حدد **القالب > طريقة العرض**.</span><span class="sxs-lookup"><span data-stu-id="173b0-192">To view the template, select **Template > View**.</span></span>

<span data-ttu-id="173b0-193">تأكد من تحديد **حفظ باسم** وحدد المكان الذي يجب تخزين القالب فيه بحيث يمكنك تحريره.</span><span class="sxs-lookup"><span data-stu-id="173b0-193">Make sure to select **Save as** and select the place where the template should be stored so you are able to edit it.</span></span> <span data-ttu-id="173b0-194">في حاله تحديد المستخدم **فتح** في مربع الحوار دون الحفظ، لن يتم الاحتفاظ بالتغييرات التي تم اجراؤها على الملف عند إغلاقه.</span><span class="sxs-lookup"><span data-stu-id="173b0-194">If the user selects **Open** in the dialog without saving, the changes done to the file will not be retained when the file is closed.</span></span>

## <a name="create-a-budget-planning-process"></a><span data-ttu-id="173b0-195">إنشاء عملية تخطيط موازنة</span><span class="sxs-lookup"><span data-stu-id="173b0-195">Create a budget planning process</span></span>

<span data-ttu-id="173b0-196">تحتاج Julia إلى إنشاء وتنشيط عملية تخطيط موازنة جديدة، تجمع بين جميع مهام الإعداد التي تم إجراؤها مسبقاً، لبدء إدخال خطط الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-196">Julia needs to create and activate a new budget planning process, that combines all setup tasks previously performed, to start entering budget plans.</span></span> <span data-ttu-id="173b0-197">تحدد عملية تخطيط الموازنة مؤسسات الموازنة وسير العمل والتخطيطات والقوالب التي سيتم استخدامها لإنشاء خطط الموازنة.</span><span class="sxs-lookup"><span data-stu-id="173b0-197">The budget planning process defines which budgeting organizations, workflow, layouts, and templates will be used for creating budget plans.</span></span>

<span data-ttu-id="173b0-198">انتقل إلى **إعداد الموازنة > الإعداد > تخطيط الموازنة > عملية تخطيط الموازنة** وأنشئ سجلاً جديداً باستخدام المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="173b0-198">Go to **Budgeting > Setup > Budget planning > Budget planning process** and create a new record by using the following information:</span></span>

-   <span data-ttu-id="173b0-199">عملية تخطيط موازنة - إعداد موازنة العام المالي 2016 في DEMF</span><span class="sxs-lookup"><span data-stu-id="173b0-199">Budget planning process - DEMF budgeting FY2016</span></span>

-   <span data-ttu-id="173b0-200">دورة الموازنة - العام المالي 2016</span><span class="sxs-lookup"><span data-stu-id="173b0-200">Budget cycle - FY2016</span></span>

-   <span data-ttu-id="173b0-201">دفتر الأستاذ - DEMF</span><span class="sxs-lookup"><span data-stu-id="173b0-201">Ledger - DEMF</span></span>

-   <span data-ttu-id="173b0-202">بنيه الحساب الافتراضية - أرباح وخسائر التصنيع</span><span class="sxs-lookup"><span data-stu-id="173b0-202">Default account structure - Manufacturing P&L</span></span>

-   <span data-ttu-id="173b0-203">التدرج الهرمي للمؤسسات - اختر التدرج الهرمي الذي تم إنشاؤه في بداية التمرين</span><span class="sxs-lookup"><span data-stu-id="173b0-203">Organization hierarchy - pick the hierarchy that was created in the beginning of the exercise</span></span>

-   <span data-ttu-id="173b0-204">سير عمل تخطيط الموازنة - تعيين تلقائي - الموافقة على سير العمل لقسم Finance</span><span class="sxs-lookup"><span data-stu-id="173b0-204">Budget planning workflow - assign the Auto - Approve workflow for the Finance department</span></span>

-   <span data-ttu-id="173b0-205">في قواعد وتخطيطات مرحلة تخطيط الموازنة، لكل مرحلة من مراحل تخطيط ميزانية سير العمل، حدد ما إذا كانت إضافة البنود وتعديل البنود مسموحاً بها وما هو التخطيط الذي يجب استخدامه بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="173b0-205">In budget planning stage rules and layouts, for each workflow Budget planning stage, select whether adding lines and modifying lines is allowed and what layout should be used by default.</span></span>

-   <span data-ttu-id="173b0-206">في جزء الإجراء، حدد **الإجراءات**، ثم في **حالة العملية**، حدد **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="173b0-206">In the Action Pane, select **Actions**, and then in the **Process state**, select **Activate**.</span></span>

## <a name="generate-initial-data-for-the-budget-plan-from-general-ledger"></a><span data-ttu-id="173b0-207">إنشاء بيانات أولية لخطة الموازنة من دفتر الأستاذ العام</span><span class="sxs-lookup"><span data-stu-id="173b0-207">Generate initial data for the budget plan from General ledger</span></span>

1.  <span data-ttu-id="173b0-208">انتقل إلى **إعداد الموازنة > دورية > إنشاء خطة موازنة من دفتر الأستاذ العام**.</span><span class="sxs-lookup"><span data-stu-id="173b0-208">Go to **Budgeting > Periodic > Generate budget plan from General ledger**.</span></span>

2.  <span data-ttu-id="173b0-209">املأ معلمات العملية الدورية وحدد الزر **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="173b0-209">Fill in the periodic process parameters and select the **Generate** button.</span></span>

3.  <span data-ttu-id="173b0-210">انتقل إلى **إعداد الموازنة > خطط الموازنة للبحث عن خطه موازنة تم إنشاؤها بواسطة عملية الإنشاء**.</span><span class="sxs-lookup"><span data-stu-id="173b0-210">Go to **Budgeting > Budget plans to find a budget plan created by Generate process**.</span></span>

4.  <span data-ttu-id="173b0-211">افتح تفاصيل المستند عن طريق تحديد الارتباط التشعبي لرقم المستند.</span><span class="sxs-lookup"><span data-stu-id="173b0-211">Open document details by selecting the Document number hyperlink.</span></span>
    <span data-ttu-id="173b0-212">يتم عرض خطة الموازنة على النحو المحدد في التخطيط الذي تم إنشاؤه أثناء هذا التمرين المعملي.</span><span class="sxs-lookup"><span data-stu-id="173b0-212">Budget plan is displayed as defined in the layout that was created during this lab.</span></span>

## <a name="create-a-current-year-budget-based-on-previous-year-actuals"></a><span data-ttu-id="173b0-213">إنشاء موازنة السنة الحالية بناءً على القيم الفعلية للسنة السابقة</span><span class="sxs-lookup"><span data-stu-id="173b0-213">Create a current year budget based on previous year actuals</span></span>

<span data-ttu-id="173b0-214">يمكن استخدام أساليب التوزيع في خطة الموازنة لنسخ معلومات خطط الموازنة بسهولة من سيناريو إلى آخر، وتوزيعها عبر الفترات، وتوزيعها للأبعاد.</span><span class="sxs-lookup"><span data-stu-id="173b0-214">Allocation methods can be used in the budget plan to easily copy information for budget plans from one scenario to another, spread them across periods, and allocate to dimensions.</span></span> <span data-ttu-id="173b0-215">في هذه المهمة، ستستخدم عمليات التوزيع لإنشاء موازنة السنة الحالية من القيم الفعلية للسنة السابقة.</span><span class="sxs-lookup"><span data-stu-id="173b0-215">In this task, you will use allocations to create current year budget from previous year actuals.</span></span>

1.  <span data-ttu-id="173b0-216">اختر جميع البنود في شبكة مستند خطة الموازنة وحدد زر **توزيع الموازنة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-216">Pick all lines in the budget plan document grid and select the **Allocate budget** button.</span></span>

2.  <span data-ttu-id="173b0-217">حدد **أسلوب التوزيع**، و **مفتاح الفترة**، و **السيناريوهات المصدر والوجهة**، ثم حدد **توزيع**.</span><span class="sxs-lookup"><span data-stu-id="173b0-217">Select **Allocation method**, **Period key**, **Source and destination scenarios**, and then select **Allocate**.</span></span>

3.  <span data-ttu-id="173b0-218">سيتم نسخ المبالغ الفعلية للعام السابق إلى موازنة العام الحالي.</span><span class="sxs-lookup"><span data-stu-id="173b0-218">The previous year actual amounts will be copied to the current year budget.</span></span> <span data-ttu-id="173b0-219">قم بتوزيع المبالغ عبر الفترات باستخدام مفتاح **فترة منحنى المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="173b0-219">Allocate the amounts across periods by using the **Sales curve period** key.</span></span>

## <a name="adjust-a-budget-plan-document-by-using-excel-and-finalize-the-document"></a><span data-ttu-id="173b0-220">تعديل مستند خطة الموازنة باستخدام Excel وإنهاء المستند</span><span class="sxs-lookup"><span data-stu-id="173b0-220">Adjust a budget plan document by using Excel and finalize the document</span></span>

1.  <span data-ttu-id="173b0-221">حدد الزر **ورقة العمل** لفتح محتويات المستند في Excel.</span><span class="sxs-lookup"><span data-stu-id="173b0-221">Select the **Worksheet** button to open document contents in Excel.</span></span>

2.  <span data-ttu-id="173b0-222">عند فتح مصنف Excel، قم بتعديل الأرقام الموجودة في مستند خطه الموازنة، ثم حدد الزر **نشر**.</span><span class="sxs-lookup"><span data-stu-id="173b0-222">When an Excel workbook opens, adjust the numbers in the budget plan document, and then select the **Publish** button.</span></span>

3.  <span data-ttu-id="173b0-223">ارجع إلى مستند خطة الموازنة في Finance.</span><span class="sxs-lookup"><span data-stu-id="173b0-223">Return to the budget plan document in Finance.</span></span> <span data-ttu-id="173b0-224">حدد **سير العمل > إرسال** للموافقة على المستند تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="173b0-224">Select **Workflow > Submit** to Auto-approve the document.</span></span>

4.  <span data-ttu-id="173b0-225">عند اكتمال سير العمل، تتغير مرحلة مستند خطة الموازنة إلى **تمت الموافقة**.</span><span class="sxs-lookup"><span data-stu-id="173b0-225">When the workflow completes, the budget plan document stage changes to **Approved**.</span></span>  
