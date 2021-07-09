---
ms.openlocfilehash: e2dbac2468e0c803359b3f5fdbd3d7efdcd7e48b
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6073863"
---

## <a name="scenario"></a><span data-ttu-id="e9a51-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="e9a51-101">Scenario</span></span>

<span data-ttu-id="e9a51-102">ستقوم في هذا التمرين بإجراء المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="e9a51-102">In this lab you will perform the following tasks:</span></span>

- <span data-ttu-id="e9a51-103">الإصدار التلقائي في العمليات</span><span class="sxs-lookup"><span data-stu-id="e9a51-103">Backflush on operations</span></span>
- <span data-ttu-id="e9a51-104">استهلاك المسار التلقائي في مهام الإعداد</span><span class="sxs-lookup"><span data-stu-id="e9a51-104">Automatic route consumption on setup jobs</span></span>
- <span data-ttu-id="e9a51-105">اختبر إعداد المعلمة</span><span class="sxs-lookup"><span data-stu-id="e9a51-105">Test the parameter setup</span></span>
- <span data-ttu-id="e9a51-106">استخدام تنفيذ التصنيع</span><span class="sxs-lookup"><span data-stu-id="e9a51-106">Use Manufacturing execution</span></span>



## <a name="backflush-on-operations"></a><span data-ttu-id="e9a51-107">الإصدار التلقائي في العمليات</span><span class="sxs-lookup"><span data-stu-id="e9a51-107">Backflush on operations</span></span>

<span data-ttu-id="e9a51-108">قرر مدير الإنتاج أن أفضل طريقة لنشر قوائم الانتقاء هي استخدام أسلوب **ملاحظات كمية العملية** (الإصدار التلقائي في العمليات) .</span><span class="sxs-lookup"><span data-stu-id="e9a51-108">The Production manager decided that the best way to post picking lists is to use the **Operation quantity feedback** (backflush on operations) method.</span></span> <span data-ttu-id="e9a51-109">إذا كان الاستهلاك الفعلي لأصناف قائمة مكونات الصنف يختلف عن الاستهلاك المقدر، يمكن للموظف إدخال استهلاك الصنف الفعلي عند تقديم ملاحظات الكمية.</span><span class="sxs-lookup"><span data-stu-id="e9a51-109">If the actual consumption on BOM items differs from the estimated consumption, the employee can enter the actual item consumption when providing quantity feedback.</span></span>

1.  <span data-ttu-id="e9a51-110">افتح **التحكم بالإنتاج > إعداد > تنفيذ التصنيع > الإعدادات الافتراضية لأمر الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-110">Open **Production control > Setup > Manufacturing execution > Production order defaults**.</span></span>

2.  <span data-ttu-id="e9a51-111">في علامة التبويب **بدء**، حدد **الحالة + الكمية** في حقل **تحديث بدء التشغيل على الإنترنت**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-111">On the **Start** tab, select **Status + quantity** in the **Update start on-line** field.</span></span>

3.  <span data-ttu-id="e9a51-112">في حقل **استهلاك قائمة مكونات الصنف التلقائي**، حدد **أبداً**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-112">In the **Automatic BOM consumption** field, select **Never**.</span></span>

4.  <span data-ttu-id="e9a51-113">حدد علامة التبويب **العمليات**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-113">Select the **Operations** tab.</span></span>

5.  <span data-ttu-id="e9a51-114">قم بتعيين خيار **الإعداد** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-114">Set the **Setup** option to **Yes**.</span></span>

6.  <span data-ttu-id="e9a51-115">في حقل **استهلاك قائمة مكونات الصنف التلقائي**، حدد **دائماً**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-115">In the **Automatic BOM consumption** field, select **Always**.</span></span>

7.  <span data-ttu-id="e9a51-116">حدد علامة التبويب **الإبلاغ كمنتهٍ**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-116">Select the **Report as finished** tab.</span></span>

8.  <span data-ttu-id="e9a51-117">في حقل **تحديث التقرير النهائي عبر الإنترنت**، حدد **الحالة + الكمية**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-117">In the **Update finished report on-line** field, select **Status + Quantity**.</span></span>

9.  <span data-ttu-id="e9a51-118">في حقل **استهلاك قائمة مكونات الصنف التلقائي**، حدد **أبداً**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-118">In the **Automatic BOM consumption** field, select **Never**.</span></span>

10. <span data-ttu-id="e9a51-119">احفظ وأغلق صفحة **الإعدادات الافتراضية لأمر الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-119">Save and close the **Production order defaults** page.</span></span>


## <a name="automatic-route-consumption-on-setup-jobs"></a><span data-ttu-id="e9a51-120">استهلاك المسار التلقائي في مهام الإعداد</span><span class="sxs-lookup"><span data-stu-id="e9a51-120">Automatic route consumption on setup jobs</span></span>


<span data-ttu-id="e9a51-121">تقدير إعداد العملية دقيق، لذا قرر مدير الإنتاج أنه ليس من الضروري أن يقوم الموظفون بالتسجيل في وظائف الإعداد.</span><span class="sxs-lookup"><span data-stu-id="e9a51-121">The estimation on operation setup is accurate, so the Production manager decides that it is not necessary for employees to register on setup jobs.</span></span> <span data-ttu-id="e9a51-122">يجب نشر استهلاك الوقت في وظائف الإعداد تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="e9a51-122">The time consumption on setup jobs must be posted automatically.</span></span>

1.  <span data-ttu-id="e9a51-123">افتح **التحكم بالإنتاج > الإعداد > المسارات > مجموعات المسارات**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-123">Open **Production control > Setup > Routes > Route groups**.</span></span>

2.  <span data-ttu-id="e9a51-124">من القائمة الموجودة في الجزء الأيمن، حدد **مجموعة توجيه التحكم في أرضية المتجر**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-124">From the list in the left pane, select **Shop Floor Control Routing Group**.</span></span>

3.  <span data-ttu-id="e9a51-125">حدد **تحرير** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e9a51-125">Select **Edit** in the Action Pane.</span></span>

1.  <span data-ttu-id="e9a51-126">في علامة التبويب السريعة **عام**، في مجموعة **استهلاك المسار التلقائي**، قم بتمكين حقل **إعداد الوقت**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-126">On the **General** FastTab, in the **Automatic route consumption** group, enable the **Setup time** field.</span></span>

4.  <span data-ttu-id="e9a51-127">حدد "حفظ" وأغلق صفحة **مجموعات المسارات**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-127">Select Save and close the **Route groups** page.</span></span>

2.  <span data-ttu-id="e9a51-128">افتح **التحكم بالإنتاج > إعداد > تنفيذ التصنيع > الإعدادات الافتراضية لأمر الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-128">Open **Production control > Setup > Manufacturing execution > Production order defaults**.</span></span>

3.  <span data-ttu-id="e9a51-129">في علامة التبويب **بدء** في الجزء الأيسر، في حقل **استهلاك المسار التلقائي**، حدد **مجموعة المسارات التابعة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-129">On the **Start** tab in the left pane, in the **Automatic route consumption** field, select **Route group dependent**.</span></span>

5.  <span data-ttu-id="e9a51-130">قم بتمكين حقل **ترحيل بطاقة المسار الآن**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-130">Enable the **Post route card now** field.</span></span>

6.  <span data-ttu-id="e9a51-131">احفظ وأغلق صفحة **الإعدادات الافتراضية لأمر الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-131">Save and close the **Production order defaults** page.</span></span>

## <a name="test-the-parameter-setup"></a><span data-ttu-id="e9a51-132">اختبر إعداد المعلمة</span><span class="sxs-lookup"><span data-stu-id="e9a51-132">Test the parameter setup</span></span>

<span data-ttu-id="e9a51-133">في الأقسام السابقة، قمت بتغيير ترحيل قائمة الانتقاء إلى الإصدار التلقائي في العمليات ثم ترتيب ترحيل وقت الإعداد على أمر الإنتاج ليتم إجراؤه تلقائياً عند بدء إنتاج جديد.</span><span class="sxs-lookup"><span data-stu-id="e9a51-133">In the previous sections, you changed the picking list posting to backflush on operations and then arranged the posting of setup time on a production order to be done automatically when you start a new production.</span></span> <span data-ttu-id="e9a51-134">الآن، تحتاج إلى اختبار الإعداد.</span><span class="sxs-lookup"><span data-stu-id="e9a51-134">Now, you need to test the setup.</span></span>

1.  <span data-ttu-id="e9a51-135">افتح **إدارة المؤسسة > التسلسلات الرقمية > التسلسلات الرقمية**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-135">Open **Organization administration > Number sequences > Number sequences**.</span></span>

2.  <span data-ttu-id="e9a51-136">حدد **رمز التسلسل الرقمي** ‏"Prod_128".</span><span class="sxs-lookup"><span data-stu-id="e9a51-136">Select **Number sequence code** 'Prod_128'.</span></span>

3.  <span data-ttu-id="e9a51-137">حدد **تحرير** في مجموعة **الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-137">Select **Edit** in the **Maintain** group.</span></span>

5.  <span data-ttu-id="e9a51-138">في حقل **الاسم**، أدخل "دفتر يومية الإنتاج"، وفي أسفل الصفحة في حقل **التالي**، أدخل "1900".</span><span class="sxs-lookup"><span data-stu-id="e9a51-138">In the **Name** field, enter  'Production Journal',  and at the bottom of the page in the **Next** field, enter '1900'.</span></span>

4.  <span data-ttu-id="e9a51-139">حدد لتوسيع علامة التبويب السريعة **معلمات النطاق** إذا لم تكن موسعة بالفعل.</span><span class="sxs-lookup"><span data-stu-id="e9a51-139">Select to expand the **Scope parameters** FastTab if it is not expanded already.</span></span>

5.  <span data-ttu-id="e9a51-140">تحقق من أن **الشركة** هي **USMF**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-140">Verify that **Company** is **USMF**.</span></span>

6.  <span data-ttu-id="e9a51-141">حدد لتوسيع علامة التبويب السريعة **عام** إذا لم تكن موسعة بالفعل.</span><span class="sxs-lookup"><span data-stu-id="e9a51-141">Select to expand the **General** FastTab if it is not expanded already.</span></span>

7.  <span data-ttu-id="e9a51-142">تحقق من تعيين حقل **مستمر** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-142">Verify that the **Continuous** field is set to **No**.</span></span>

8.  <span data-ttu-id="e9a51-143">حدد "حفظ" وأغلق صفحة **التسلسلات الرقمية**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-143">Select Save and close the **Number sequences** page.</span></span>

9. <span data-ttu-id="e9a51-144">في حالة ظهور الرسالة المنبثقة **قد يؤدي تغيير التسلسل الرقمي إلى عدم الاتساق - هل تقبل ذلك؟**، حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-144">If the pop-up message **Change of number sequence may create inconsistency - accept?** appears, select **Yes**.</span></span>

### <a name="to-run-the-synchronize-job-table-periodic-job-follow-these-steps"></a><span data-ttu-id="e9a51-145">لتشغيل مهمة "مزامنة جدول المهام" الدورية، اتبع هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="e9a51-145">To run the Synchronize job table periodic job, follow these steps.</span></span>

1.  <span data-ttu-id="e9a51-146">افتح **التحكم بالإنتاج > المهام الدورية > تحديث الكيانات > مزامنة جدول العمل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-146">Open **Production control > Periodic tasks > Update entities > Synchronize job table**.</span></span>

2.  <span data-ttu-id="e9a51-147">قم بتمكين جميع الخيارات الأربعة: **مزامنة الإنتاج**، و **مزامنة الوقت والحضور**، و **مزامنة المشروع**، و **مزامنة غياب مدير الموارد البشرية (HRM)**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-147">Enable all four options: **Synchronize production**, **Synchronize Time and attendance**, **Synchronize project**, and **Synchronize HRM absence**.</span></span>

3.  <span data-ttu-id="e9a51-148">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-148">Select **OK**.</span></span> <span data-ttu-id="e9a51-149">قد تستغرق هذه العملية عدة دقائق حتى تكتمل.</span><span class="sxs-lookup"><span data-stu-id="e9a51-149">This process might take several minutes to complete.</span></span>

## <a name="use-manufacturing-execution"></a><span data-ttu-id="e9a51-150">استخدام تنفيذ التصنيع</span><span class="sxs-lookup"><span data-stu-id="e9a51-150">Use Manufacturing execution</span></span>

<span data-ttu-id="e9a51-151">يمكنك تمكين تسجيل الوقت لشانون عامل تشغيل الجهاز في USMF.</span><span class="sxs-lookup"><span data-stu-id="e9a51-151">Enable time registration for Shannon the machine operator in USMF.</span></span> <span data-ttu-id="e9a51-152">يحتاج شانون إلى استخدام وحدة طرفية لبطاقة العمل للتحكم في تنفيذ أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="e9a51-152">Shannon needs to use the Job card terminal to control the execution of the production order.</span></span>

1. <span data-ttu-id="e9a51-153">انتقل إلى **الموارد البشرية > العمال > العمال**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-153">Go to **Human resources > Workers > Workers**.</span></span>

2. <span data-ttu-id="e9a51-154">استخدم **عامل التصفية السريع** للتصفية في حقل **الاسم** بقيمة **شانون**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-154">Use the **Quick Filter** to filter on the **Name** field with a value of **SHANNON**.</span></span>

3. <span data-ttu-id="e9a51-155">سيظهر سجل **شانون داشر**، فحدد السجل لفتح التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="e9a51-155">The record **Shannon Dascher** will appear, select the record to open the details.</span></span> 

4. <span data-ttu-id="e9a51-156">حدد **تحرير** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e9a51-156">Select **Edit** in the Action Pane.</span></span>

5. <span data-ttu-id="e9a51-157">حدد علامة التبويب **تسجيل الوقت** في سجل العامل.</span><span class="sxs-lookup"><span data-stu-id="e9a51-157">Select the **Time registration** tab on the worker record.</span></span>

4. <span data-ttu-id="e9a51-158">حدد **تنشيط في الوحدات الطرفية للتسجيل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-158">Select **Activate on registration terminals**.</span></span>

4. <span data-ttu-id="e9a51-159">في حقل **مجموعة الحساب**، أدخل أو حدد **رجل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-159">In the **Calculation group** field, enter or select **Man**.</span></span>

5. <span data-ttu-id="e9a51-160">في حقل **مجموعة الحساب الافتراضية**، أدخل أو حدد **رجل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-160">In the **Default calculation group** field, enter or select **Man**.</span></span>

6. <span data-ttu-id="e9a51-161">في حقل **مجموعة الموافقة**، أدخل أو حدد **AdmMan**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-161">In the **Approval group** field, enter or select **AdmMan**.</span></span>

7. <span data-ttu-id="e9a51-162">في حقل **ملف التعريف القياسي**، أدخل أو حدد **قياسي**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-162">In the **Standard profile** field, enter or select **Standard**.</span></span>

8. <span data-ttu-id="e9a51-163">في حقل **مجموعة ملف التعريف**، أدخل أو حدد **رجل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-163">In the **Profile group** field, enter or select **Man**.</span></span>

9. <span data-ttu-id="e9a51-164">حدد **نعم** في حقل **استخدام بطاقة الوقت**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-164">Select **Yes** in the **Use timecard** field.</span></span>

10. <span data-ttu-id="e9a51-165">في الحقل **تكوين**، أدخل أو حدد **إنتاج‎**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-165">In the **Configuration** field, enter or select **Production**.</span></span>

11. <span data-ttu-id="e9a51-166">حدد **نعم** في حقل **خيارات المشرفين**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-166">Select **Yes** in the **Supervisor options** field.</span></span>

12. <span data-ttu-id="e9a51-167">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-167">Select **OK**.</span></span>

16. <span data-ttu-id="e9a51-168">في حقل **الهوية**، أدخل **069**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-168">In the **Identification** field, enter **069**.</span></span>

17. <span data-ttu-id="e9a51-169">في حقل **معرف الشارة**، أدخل **069**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-169">In the **Badge ID** field, enter **069**.</span></span>

18. <span data-ttu-id="e9a51-170">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="e9a51-170">Select **Save** in the Action Pane.</span></span>

19. <span data-ttu-id="e9a51-171">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="e9a51-171">Close the page.</span></span>

> [!NOTE]
> <span data-ttu-id="e9a51-172">لإكمال الخطوات التالية، تأكد من تعيين المستخدم الخاص بك إلى دور **عامل الجهاز** في إدارة النظام.</span><span class="sxs-lookup"><span data-stu-id="e9a51-172">To complete the following steps, ensure your user is assigned to the **Machine operator** role in System administration.</span></span> <span data-ttu-id="e9a51-173">تأكد أيضاً من تعيين العمال لديك لجهاز من خلال الانتقال إلى **التحكم بالإنتاج > الإعداد > تنفيذ التصنيع > تكوين بطاقة الوظيفة للأجهزة**، وإذا لزم الأمر فحدد **إضافة** في علامة التبويب السريعة **المستخدمين المعينين**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-173">Also ensure that your worker is assigned to a device by going to **Production control > Setup > Manufacturing execution > Configure job card for devices** and if necessary select **Add** in the **Assigned users** FastTab.</span></span>

20. <span data-ttu-id="e9a51-174">انتقل إلى **التحكم في الإنتاج > تنفيذ التصنيع > جهاز بطاقة الوظيفة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-174">Go to **Production control > Manufacturing execution > Job card device**.</span></span>

21. <span data-ttu-id="e9a51-175">في الحقل **رقم الموظف**، أدخل **069**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-175">In the **Personnel number** field, enter **069**.</span></span>

22. <span data-ttu-id="e9a51-176">حدد **تسجيل الدخول**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-176">Select **Log in**.</span></span>

23. <span data-ttu-id="e9a51-177">حدد **بدء الوظيفة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-177">Select **Start job**.</span></span>

24. <span data-ttu-id="e9a51-178">قم بتعيين **الكمية المراد بدؤها** إلى **1.00**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-178">Set **Quantity to start** to **1.00**.</span></span>

25. <span data-ttu-id="e9a51-179">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-179">Select **OK**.</span></span>

26. <span data-ttu-id="e9a51-180">حدد **تقدم التقرير**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-180">Select **Report progress**.</span></span>

27. <span data-ttu-id="e9a51-181">قم بتعيين **كمية الخطأ** إلى **1.00**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-181">Set **Error quantity** to **1.00**.</span></span>

28. <span data-ttu-id="e9a51-182">في حقل **سبب الخطأ**، حدد **المادة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-182">In the **Error cause** field, select **Material**.</span></span>

29. <span data-ttu-id="e9a51-183">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-183">Select **Complete**.</span></span>

30. <span data-ttu-id="e9a51-184">حدد **وقت الراحة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-184">Select **Break**.</span></span>

31. <span data-ttu-id="e9a51-185">في القائمة، حدد **وقت الراحة من العمل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-185">In the list, select **break from work**.</span></span>

32. <span data-ttu-id="e9a51-186">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-186">Select **OK**.</span></span>

33. <span data-ttu-id="e9a51-187">حدد **إيقاف وقت الراحة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-187">Select **Stop break**.</span></span>

34. <span data-ttu-id="e9a51-188">حدد **نشاط**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-188">Select **Activity**.</span></span>

35. <span data-ttu-id="e9a51-189">في القائمة، ابحث عن وحدد **إصلاح المعدات**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-189">In the list, find and select **Equipment repair**.</span></span>

36. <span data-ttu-id="e9a51-190">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-190">Select **OK**.</span></span>

    
1. <span data-ttu-id="e9a51-191">ستتلقى رسالة خطأ تفيد بأنك بحاجة إلى الإبلاغ عن ملاحظات حول وظيفة أخرى.</span><span class="sxs-lookup"><span data-stu-id="e9a51-191">You will get an error message saying you need to report feedback on another job.</span></span> <span data-ttu-id="e9a51-192">حدد **موافق** للمتابعة.</span><span class="sxs-lookup"><span data-stu-id="e9a51-192">Select **OK** to continue.</span></span>

38. <span data-ttu-id="e9a51-193">قم بتعيين **كمية جيدة** إلى الفرق بين **الإجمالي المطلوب** و **مكتملة بالفعل**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-193">Set **Good quantity** to the difference between the **Total Requested** and **Already Completed**.</span></span>  
39. <span data-ttu-id="e9a51-194">في قسم **تغيير حالة الوظيفة إلى**، حدد **مكتملة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-194">In the **Change Job status to** section, select **Completed**.</span></span>
39. <span data-ttu-id="e9a51-195">حدد **إكمال.**</span><span class="sxs-lookup"><span data-stu-id="e9a51-195">Select **Complete.**</span></span>
40. <span data-ttu-id="e9a51-196">حدد **مغادرة**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-196">Select **Leaving**.</span></span>
42. <span data-ttu-id="e9a51-197">حدد **وقت الانصراف** في مربع الحوار الذي يتم فتحه.</span><span class="sxs-lookup"><span data-stu-id="e9a51-197">Select **Clock out** in the dialog box that opens.</span></span>
43. <span data-ttu-id="e9a51-198">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e9a51-198">Select **OK**.</span></span>
41. <span data-ttu-id="e9a51-199">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="e9a51-199">Close the page.</span></span> 

