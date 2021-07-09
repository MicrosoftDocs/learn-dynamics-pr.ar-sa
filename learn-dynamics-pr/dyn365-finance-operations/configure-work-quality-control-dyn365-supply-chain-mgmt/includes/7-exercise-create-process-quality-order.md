---
ms.openlocfilehash: 29848ae325c0f91b0924f4ea943894e4d75338de
ms.sourcegitcommit: d9d731bb071133aa102da6c7c602825acae008a2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2021
ms.locfileid: "6073710"
---
<span data-ttu-id="5b456-101">بصفتك مدير الجودة في شركة **USMF**، تريد تمكين عملية إدارة الجودة حيث يجب فحص المخزون على الفور في وقت انتقاء منتج Surface pro.</span><span class="sxs-lookup"><span data-stu-id="5b456-101">As a quality manager in the **USMF** company, you want to enable a quality management process where inventory must be inspected immediately at the time of picking for the Surface pro product.</span></span>

<span data-ttu-id="5b456-102">تحتاج إلى بدء عملية إنشاء مجموعة جودة لتحديد العناصر التي سيتم أخذ عينات منها، ثم إنشاء مجموعة اختبار لتجميع الاختبارات التي سيتم إجراؤها على عناصر في مجموعة الجودة.</span><span class="sxs-lookup"><span data-stu-id="5b456-102">You need to start the process of creating a quality group to define the items that are going to be sampled, and then create a test group to group the tests that are to be performed on items in the quality group.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="5b456-103">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="5b456-103">Before you begin</span></span>

<span data-ttu-id="5b456-104">للاستفادة إلى أقصى حد من هذه التدريبات وغيرها في هذه الوحدة، نوصي بأن يكون لديك بيانات العينة القياسية المتوفرة في Supply Chain Management والتي تم تثبيتها باستخدام Lifecycle Services‎‏ (LCS)‏‏‏‎.</span><span class="sxs-lookup"><span data-stu-id="5b456-104">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data available in Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

## <a name="enable-quality-management"></a><span data-ttu-id="5b456-105">تمكين إدارة الجودة</span><span class="sxs-lookup"><span data-stu-id="5b456-105">Enable quality management</span></span> 

1.  <span data-ttu-id="5b456-106">انتقل إلى **إدارة المخزون > الإعداد > معلمات إدارة المستودع والمخزون**.</span><span class="sxs-lookup"><span data-stu-id="5b456-106">Go to **Inventory management > Setup > Inventory and warehouse management parameters**.</span></span>
2.  <span data-ttu-id="5b456-107">حدد علامة التبويب **إدارة الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-107">Select the **Quality management** tab.</span></span>
3.  <span data-ttu-id="5b456-108">قم بتعيين خيار **استخدام إدارة الجودة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="5b456-108">Set the **Use quality management** option to **Yes**.</span></span>
4.  <span data-ttu-id="5b456-109">حدد **إعداد التقرير**.</span><span class="sxs-lookup"><span data-stu-id="5b456-109">Select **Report setup**.</span></span> <span data-ttu-id="5b456-110">في USMF، تم تحديد إعداد التقرير لإدارة الجودة بالفعل.</span><span class="sxs-lookup"><span data-stu-id="5b456-110">In USMF, the report setup for quality management is already defined.</span></span> <span data-ttu-id="5b456-111">إذا لم يتم ذلك، فأنت بحاجة إلى إضافة سطور جديدة في هذه الصفحة لأنواع التقارير المختلفة وتحديد نوع المستند الذي سيتم استخدامه لكل تقرير.</span><span class="sxs-lookup"><span data-stu-id="5b456-111">If this is not done, you need to add new lines on this page for the different report types and select the type of document to be used for each report.</span></span>
5.  <span data-ttu-id="5b456-112">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-112">Close all pages.</span></span>

## <a name="create-a-test"></a><span data-ttu-id="5b456-113">إنشاء اختبار</span><span class="sxs-lookup"><span data-stu-id="5b456-113">Create a test</span></span> 

1.  <span data-ttu-id="5b456-114">انتقل إلى **إدارة المخزون > الإعداد > التحكم في الجودة > الاختبارات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-114">Go to **Inventory management > Setup > Quality control > Tests**.</span></span>
2.  <span data-ttu-id="5b456-115">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-115">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-116">في حقل **الاختبار**، اكتب **SurfaceTest**.</span><span class="sxs-lookup"><span data-stu-id="5b456-116">In the **Test** field, type **SurfaceTest**.</span></span>
4.  <span data-ttu-id="5b456-117">في حقل **الوصف**، اكتب **اختبار Surface**.</span><span class="sxs-lookup"><span data-stu-id="5b456-117">In the **Description** field, type **Test Surface**.</span></span>
5.  <span data-ttu-id="5b456-118">في حقل **الإدخال**، حدد **الخيار** لتعيين نتائج الاختبار بناءً على قيم محددة مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="5b456-118">In the **Type** field, select **Option** to assign the test results based on pre-defined values.</span></span>
6.  <span data-ttu-id="5b456-119">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-119">Select **Save**.</span></span>
7.  <span data-ttu-id="5b456-120">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-120">Close all pages.</span></span>

## <a name="create-test-variables-to-define-the-way-test-results-are-recorded"></a><span data-ttu-id="5b456-121">إنشاء متغيرات الاختبار لتحديد طريقة تسجيل نتائج الاختبار</span><span class="sxs-lookup"><span data-stu-id="5b456-121">Create test variables to define the way test results are recorded</span></span> 

1.  <span data-ttu-id="5b456-122">انتقل إلى **إدارة المخزون > الإعداد > التحكم في الجودة > اختبار المتغيرات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-122">Go to **Inventory management > Setup > Quality control > Test variables**.</span></span>
2.  <span data-ttu-id="5b456-123">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-123">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-124">في حقل **المتغير**، اكتب **الطاقة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-124">In the **Variable** field, type **Power**.</span></span>
4.  <span data-ttu-id="5b456-125">في حقل **الوصف**، اكتب **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-125">In the **Description** field, type **Power up**.</span></span>
5.  <span data-ttu-id="5b456-126">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-126">Select **Save**.</span></span>
6.  <span data-ttu-id="5b456-127">حدد **النتائج**.</span><span class="sxs-lookup"><span data-stu-id="5b456-127">Select **Outcomes**.</span></span>
7.  <span data-ttu-id="5b456-128">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-128">Select **New**.</span></span>
8.  <span data-ttu-id="5b456-129">في حقل **النتيجة**، اكتب **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-129">In the **Outcome** field, type **ON**.</span></span>
9.  <span data-ttu-id="5b456-130">في حقل **الوصف**، اكتب **بدء تشغيل الجهاز بشكل طبيعي**.</span><span class="sxs-lookup"><span data-stu-id="5b456-130">In the **Description** field, type **Device starts normally**.</span></span>
10. <span data-ttu-id="5b456-131">في حقل **حالة النتيجة**، حدد **نجاح**.</span><span class="sxs-lookup"><span data-stu-id="5b456-131">In the **Outcome status** field, select **Pass**.</span></span>
11. <span data-ttu-id="5b456-132">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-132">Select **Save**.</span></span>
12. <span data-ttu-id="5b456-133">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-133">Select **New**.</span></span>
13. <span data-ttu-id="5b456-134">في حقل **النتيجة**، اكتب **إيقاف تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-134">In the **Outcome** field, type **OFF**.</span></span>
14. <span data-ttu-id="5b456-135">في حقل **الوصف**، اكتب **لا يتم تشغيل الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="5b456-135">In the **Description** field, type **Device does not power up**.</span></span>
15. <span data-ttu-id="5b456-136">في حقل **حالة النتيجة**، حدد **فشل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-136">In the **Outcome status** field, select **Fail**.</span></span>
16. <span data-ttu-id="5b456-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-137">Select **Save**.</span></span>
17. <span data-ttu-id="5b456-138">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-138">Close all pages.</span></span>

## <a name="set-up-item-sampling"></a><span data-ttu-id="5b456-139">إعداد أخذ عينات للصنف</span><span class="sxs-lookup"><span data-stu-id="5b456-139">Set up item sampling</span></span>

1.  <span data-ttu-id="5b456-140">انتقل إلى **إدارة المخزون > الإعداد > التحكم في الجودة > أخذ عينات للصنف**.</span><span class="sxs-lookup"><span data-stu-id="5b456-140">Go to **Inventory management > Setup > Quality control > Item sampling.**</span></span>
2.  <span data-ttu-id="5b456-141">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-141">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-142">في حقل **أخذ عينات للصنف**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="5b456-142">In the **Item sampling** field, type **1**.</span></span>
4.  <span data-ttu-id="5b456-143">في حقل **الوصف**، اكتب **عينة واحدة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-143">In the **Description** field, type **one sample**.</span></span>
5.  <span data-ttu-id="5b456-144">في حقل **مواصفات الكمية**، حدد **كمية ثابتة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-144">In the **Quantity specification** field, select **Fixed quantity**.</span></span>
6.  <span data-ttu-id="5b456-145">في حقل **القيمة**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="5b456-145">In the **Value** field, enter **1**.</span></span> <span data-ttu-id="5b456-146">ترتبط هذه القيمة بـ **مواصفات الجودة** التي تم تحديدها في الحقل المجاور.</span><span class="sxs-lookup"><span data-stu-id="5b456-146">This value relates to the **Quantity specification** that's selected in the adjacent field.</span></span>
7.  <span data-ttu-id="5b456-147">قم بتوسيع قسم **‎‏‫العملية** أو طيه.</span><span class="sxs-lookup"><span data-stu-id="5b456-147">Expand or collapse the **Process** section.</span></span>
8.  <span data-ttu-id="5b456-148">قم بتحديد أو إلغاء تحديد خيار **الحظر الكامل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-148">Select or clear the **Full blocking** option.</span></span> <span data-ttu-id="5b456-149">إذا حددت هذا الخيار، فسيتم حظر الكمية بالكامل أو كمية بند الأمر في حالة فشل الاختبار.</span><span class="sxs-lookup"><span data-stu-id="5b456-149">If you select this option, the whole lot or order line quantity is blocked if a test is failed.</span></span> <span data-ttu-id="5b456-150">إذا لم تحدده، فسيتم حظر العناصر الموجودة في أمر الجودة فقط.</span><span class="sxs-lookup"><span data-stu-id="5b456-150">If you don't select it, only the items in the quality order are blocked.</span></span>
9.  <span data-ttu-id="5b456-151">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-151">Select **Save**.</span></span>
10. <span data-ttu-id="5b456-152">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-152">Close all pages.</span></span>

## <a name="create-a-quality-and-item-group"></a><span data-ttu-id="5b456-153">إنشاء مجموعة الجودة والعناصر</span><span class="sxs-lookup"><span data-stu-id="5b456-153">Create a quality and item group</span></span> 

1.  <span data-ttu-id="5b456-154">انتقل إلى **إدارة المخزون > الإعداد > التحكم في الجودة > مجموعات الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-154">Go to **Inventory management > Setup > Quality control > Quality groups**.</span></span>
2.  <span data-ttu-id="5b456-155">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-155">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-156">في حقل **مجموعة الجودة**، أدخل **Surface**.</span><span class="sxs-lookup"><span data-stu-id="5b456-156">In the **Quality group** field, type **Surface**.</span></span> <span data-ttu-id="5b456-157">استخدم اسماً وصفياً للمساعدة في تحديد نوع العناصر التي ستحتويها المجموعة (معايير أخذ العينات الخاصة بك).</span><span class="sxs-lookup"><span data-stu-id="5b456-157">Use a descriptive name to help identify which kind of items the group will contain (your sampling criteria).</span></span>
4.  <span data-ttu-id="5b456-158">في حقل **الوصف**، أدخل **مجموعة الجودة لـ Surface**.</span><span class="sxs-lookup"><span data-stu-id="5b456-158">In the **Description** field, type **Quality group for Surface**.</span></span>
5.  <span data-ttu-id="5b456-159">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-159">Select **Save**.</span></span>
6.  <span data-ttu-id="5b456-160">حدد **إضافة أصناف**.</span><span class="sxs-lookup"><span data-stu-id="5b456-160">Select **Add items**.</span></span>
7.  <span data-ttu-id="5b456-161">حدد صف **رقم الصنف**.</span><span class="sxs-lookup"><span data-stu-id="5b456-161">Select the **Item number** row.</span></span> <span data-ttu-id="5b456-162">في هذا المثال، سيتم تشغيل التصفية بناءً على رقم الصنف.</span><span class="sxs-lookup"><span data-stu-id="5b456-162">In this example, the filtering will be run based on the item number.</span></span>
8.  <span data-ttu-id="5b456-163">حقل **المعايير**، أدخل **1000** لتصفية أرقام الأصناف التي تبدأ بحرف T.</span><span class="sxs-lookup"><span data-stu-id="5b456-163">In the **Criteria** field, type **1000** to filter on the item numbers that start with T.</span></span>
9.  <span data-ttu-id="5b456-164">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-164">Select **OK**.</span></span>
10. <span data-ttu-id="5b456-165">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-165">Close all pages.</span></span>

## <a name="create-a-test-group"></a><span data-ttu-id="5b456-166">إنشاء مجموعة اختبار</span><span class="sxs-lookup"><span data-stu-id="5b456-166">Create a test group</span></span> 

1.  <span data-ttu-id="5b456-167">انتقل إلى **إدارة المخزون > الإعداد > التحكم في الجودة > مجموعات الاختبارات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-167">Go to **Inventory management > Setup > Quality control > Test groups**.</span></span>
2.  <span data-ttu-id="5b456-168">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-168">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-169">في حقل **مجموعة الاختبار**، أدخل **Surface**.</span><span class="sxs-lookup"><span data-stu-id="5b456-169">In the **Test group** field, type **Surface**.</span></span>
4.  <span data-ttu-id="5b456-170">امنح مجموعة الاختبار اسماً يساعدك على تذكر نوع الاختبارات التي يتم إجراؤها ومجموعة الجودة التي يجب أن ترتبط بها.</span><span class="sxs-lookup"><span data-stu-id="5b456-170">Give the test group a name that will help you remember what kind of tests are being run and which quality group it should be associated with.</span></span>
5.  <span data-ttu-id="5b456-171">في حقل **الوصف**، أدخل **مجموعة الاختبارات لـ Surface**.</span><span class="sxs-lookup"><span data-stu-id="5b456-171">In the **Description** field, type **Test group for Surface**.</span></span>
6.  <span data-ttu-id="5b456-172">في حقل **أخذ عينات للصنف**، حدد **1**.</span><span class="sxs-lookup"><span data-stu-id="5b456-172">In the **Item sampling** field, select **1**.</span></span>
7.  <span data-ttu-id="5b456-173">في علامة التبويب **نظرة عامة**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-173">On the **Overview** tab, select **Add**.</span></span>
8.  <span data-ttu-id="5b456-174">في حقل **الرقم التسلسلي**، أدخِل **1**.</span><span class="sxs-lookup"><span data-stu-id="5b456-174">In the **Sequence number** field, enter **1**.</span></span>
9.  <span data-ttu-id="5b456-175">في حقل **الاختبار**، حدد **SurfaceTest**.</span><span class="sxs-lookup"><span data-stu-id="5b456-175">In the **Test** field, select **SurfaceTest**.</span></span>
10. <span data-ttu-id="5b456-176">حدد علامة التبويب **الاختبار**.</span><span class="sxs-lookup"><span data-stu-id="5b456-176">Select the **Test** tab.</span></span>
11. <span data-ttu-id="5b456-177">في حقل **المتغير**، حدد **الطاقة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-177">In the **Variable** field, select **Power**.</span></span>
12. <span data-ttu-id="5b456-178">في حقل **النتيجة الافتراضية**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="5b456-178">In the **Default outcome** field, select the drop-down button to open the lookup.</span></span>
13. <span data-ttu-id="5b456-179">حدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-179">Select **ON**.</span></span>
14. <span data-ttu-id="5b456-180">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-180">Select **Save**.</span></span>
15. <span data-ttu-id="5b456-181">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-181">Close all pages.</span></span>

## <a name="define-when-quality-orders-will-be-created"></a><span data-ttu-id="5b456-182">تحديد متى سيتم إنشاء أوامر الجودة</span><span class="sxs-lookup"><span data-stu-id="5b456-182">Define when quality orders will be created</span></span> 

1.  <span data-ttu-id="5b456-183">انتقل إلى **إدارة المخزون > الإعداد > التحكم في الجودة > عمليات اقتران الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-183">Go to **Inventory management > Setup > Quality control > Quality associations**.</span></span>
2.  <span data-ttu-id="5b456-184">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-184">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-185">في حقل **نوع المرجع**، حدد **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-185">In the **Reference type** field, select **Sales**.</span></span>
4.  <span data-ttu-id="5b456-186">في حقل **كود الصنف**، حدد **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="5b456-186">In the **Item code** field, select **Table**.</span></span>
5.  <span data-ttu-id="5b456-187">في حقل **الصنف**، أدخل أو حدد **1000**.</span><span class="sxs-lookup"><span data-stu-id="5b456-187">In the **Item** field, enter or select **1000**.</span></span>
6.  <span data-ttu-id="5b456-188">قم بتوسيع قسم **العملية**.</span><span class="sxs-lookup"><span data-stu-id="5b456-188">Expand the **Process** section.</span></span>
7.  <span data-ttu-id="5b456-189">في حقل **نوع الحدث**، حدد **تمت جدولة عملية الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="5b456-189">In the **Event type** field, select **Picking process is scheduled**.</span></span>
8.  <span data-ttu-id="5b456-190">قم بتوسيع قسم **معالجة أمر الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-190">Expand the **Quality order process** section.</span></span>
9.  <span data-ttu-id="5b456-191">في حقل **منع الحدث**، أدخل أو حدد **عملية الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="5b456-191">In the **Event blocking** field, enter or select **Picking process**.</span></span>
10. <span data-ttu-id="5b456-192">قم بتوسيع قسم **المواصفات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-192">Expand the **Specifications** section.</span></span>
11. <span data-ttu-id="5b456-193">في حقل **مجموعة الاختبار**، أدخل أو حدد **Surface**.</span><span class="sxs-lookup"><span data-stu-id="5b456-193">In the **Test group** field, enter or select **Surface**.</span></span>
12. <span data-ttu-id="5b456-194">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b456-194">Select **Save**.</span></span>
13. <span data-ttu-id="5b456-195">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-195">Close all pages.</span></span>

## <a name="process-quality-orders"></a><span data-ttu-id="5b456-196">معالجة أوامر الجودة</span><span class="sxs-lookup"><span data-stu-id="5b456-196">Process quality orders</span></span> 

1.  <span data-ttu-id="5b456-197">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-197">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>
2.  <span data-ttu-id="5b456-198">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="5b456-198">Select **New**.</span></span>
3.  <span data-ttu-id="5b456-199">في الحقل **حساب العميل**، أدخل **US-013**.</span><span class="sxs-lookup"><span data-stu-id="5b456-199">In the **Customer account** field, select **US-013**.</span></span>
4.  <span data-ttu-id="5b456-200">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-200">Select **OK**.</span></span>
5.  <span data-ttu-id="5b456-201">في الحقل **رقم الصنف**، أدخل أو حدد **1000**.</span><span class="sxs-lookup"><span data-stu-id="5b456-201">In the **Item number** field, enter or select **1000**.</span></span>
6.  <span data-ttu-id="5b456-202">في جزء الإجراء، حدد **الانتقاء والتعبئة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-202">On the Action Pane, select **Pick and pack**.</span></span>
7.  <span data-ttu-id="5b456-203">حدد **أوامر الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-203">Select **Quality orders**.</span></span> <span data-ttu-id="5b456-204">لاحظ أنه لا يوجد أمر جودة حالياً.</span><span class="sxs-lookup"><span data-stu-id="5b456-204">Note that there is currently no quality order.</span></span>
8.  <span data-ttu-id="5b456-205">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="5b456-205">Close the page.</span></span>
9.  <span data-ttu-id="5b456-206">حدد **إنشاء قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="5b456-206">Select **Generate picking list**.</span></span>
10. <span data-ttu-id="5b456-207">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-207">Select **OK**.</span></span>
11. <span data-ttu-id="5b456-208">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-208">Select **OK**.</span></span>
12. <span data-ttu-id="5b456-209">اقرأ رسالة الخطأ التي تم إنشاؤها والتي تمنعك من متابعة عملية الانتقاء والتعبئة لأن لديك الآن أمر جودة.</span><span class="sxs-lookup"><span data-stu-id="5b456-209">Read the generated error message that prevents you from continuing the process of picking and packing because you now have a quality order.</span></span>
13. <span data-ttu-id="5b456-210">حدد **أوامر الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-210">Select **Quality orders**.</span></span> <span data-ttu-id="5b456-211">لاحظ أنه يتم إنشاء أمر الجودة تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="5b456-211">Note that the quality order is automatically generated.</span></span>
14. <span data-ttu-id="5b456-212">راجع الاختبارات.</span><span class="sxs-lookup"><span data-stu-id="5b456-212">Review the tests.</span></span>
15. <span data-ttu-id="5b456-213">حدد **النتائج**.</span><span class="sxs-lookup"><span data-stu-id="5b456-213">Select **Results**.</span></span>
16. <span data-ttu-id="5b456-214">قم بتعيين **كمية النتيجة** إلى **1**.</span><span class="sxs-lookup"><span data-stu-id="5b456-214">Set the **Result quantity** to **1**.</span></span>
17. <span data-ttu-id="5b456-215">قم بتعيين **نتيجة الاختبار** إلى **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-215">Set **Test result** to **ON**.</span></span>
18. <span data-ttu-id="5b456-216">حدد **التحقق من الصحة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-216">Select **Validate**.</span></span>
21. <span data-ttu-id="5b456-217">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-217">Select **OK**.</span></span>
22. <span data-ttu-id="5b456-218">أغلق صفحة **أمر الجودة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-218">Close the **Quality order** page.</span></span>
23. <span data-ttu-id="5b456-219">حدد **إنشاء قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="5b456-219">Select **Generate picking list**.</span></span>
24. <span data-ttu-id="5b456-220">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-220">Select **OK**.</span></span>
25. <span data-ttu-id="5b456-221">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-221">Select **OK**.</span></span>
26. <span data-ttu-id="5b456-222">لاحظ أنه لم يحدث خطأ لأنك اجتزت اختبار أمر الجودة.</span><span class="sxs-lookup"><span data-stu-id="5b456-222">Note that no error occurs because you have passed the quality order test.</span></span>
27. <span data-ttu-id="5b456-223">حدد **تسجيل قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="5b456-223">Select **Picking list registration**.</span></span>
28. <span data-ttu-id="5b456-224">حدد **التحديثات**.</span><span class="sxs-lookup"><span data-stu-id="5b456-224">Select **Updates**.</span></span>
29. <span data-ttu-id="5b456-225">حدد **تحديث الكل**.</span><span class="sxs-lookup"><span data-stu-id="5b456-225">Select **Update all**.</span></span>
30. <span data-ttu-id="5b456-226">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="5b456-226">Close the page.</span></span>
31. <span data-ttu-id="5b456-227">حدد **نشر إيصال التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="5b456-227">Select **Post packing slip**.</span></span>
32. <span data-ttu-id="5b456-228">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-228">Select **OK**.</span></span>
33. <span data-ttu-id="5b456-229">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5b456-229">Select **OK**.</span></span>
34. <span data-ttu-id="5b456-230">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5b456-230">Close all pages.</span></span>
