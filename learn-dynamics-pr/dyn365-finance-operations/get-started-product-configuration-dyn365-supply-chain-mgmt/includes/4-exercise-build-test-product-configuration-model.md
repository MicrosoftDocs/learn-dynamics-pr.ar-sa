---
ms.openlocfilehash: 6002cedf43c06f620d69772d8be8a6014d3520b7
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073251"
---
## <a name="before-you-begin"></a><span data-ttu-id="e0c4c-101">قبل البدء:</span><span class="sxs-lookup"><span data-stu-id="e0c4c-101">Before you begin:</span></span> 
<span data-ttu-id="e0c4c-102">لتحقيق الاستفادة القصوى من هذا التمرين، ننصحك بأن تكون عينة البيانات القياسية متوفرة في Supply Chain Management التي يتم تثبيتها باستخدام Lifecycle Services ‏(LCS).</span><span class="sxs-lookup"><span data-stu-id="e0c4c-102">To get the most benefit from this exercise, we recommend that you have the standard sample data available in Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

## <a name="create-components-for-product-configuration-models"></a><span data-ttu-id="e0c4c-103">إنشاء مكونات لنماذج تكوين المنتجات</span><span class="sxs-lookup"><span data-stu-id="e0c4c-103">Create components for product configuration models</span></span>


<span data-ttu-id="e0c4c-104">بصفتك مصمم إنتاج في شركة **USMF**، تحتاج إلى إنشاء المكونات قبل إنشاء نموذج المنتج.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-104">As a product designer in the **USMF** company, you need to create components before a product model can be built.</span></span> <span data-ttu-id="e0c4c-105">تقوم نماذج تكوين المنتجات المستندة إلى القيود باستخدام المكونات ككتل إنشاء لتأسيس بنية نموذج المنتج.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-105">Constraint-based product configuration models use components as building blocks to establish the product model structure.</span></span>

1.  <span data-ttu-id="e0c4c-106">انتقل إلى **المنتجات > إدارة معلومات المنتج > نماذج تكوين المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-106">Go to **Product information management > Products > Product configuration models**.</span></span>
2.  <span data-ttu-id="e0c4c-107">حدد **المكونات**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-107">Select **Components**.</span></span>
3.  <span data-ttu-id="e0c4c-108">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-108">Select **New**.</span></span>
4.  <span data-ttu-id="e0c4c-109">في حقل **الاسم** في الأعلى وفي الأسفل، أدخل **مكبر صوت منزلي عالي الجودة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-109">In the **Name** field at the top and at the bottom, enter **Home Audio High End Speaker**.</span></span>
5.  <span data-ttu-id="e0c4c-110">في حقل **الوصف**، أدخل **مكبر صوت منزلي عالي الجودة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-110">In the **Description** field, enter **Home Audio High End Speaker**.</span></span>
6.  <span data-ttu-id="e0c4c-111">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-111">Select **Save**.</span></span>

## <a name="create-a-product-configuration-model"></a><span data-ttu-id="e0c4c-112">إنشاء نموذج تكوين منتج</span><span class="sxs-lookup"><span data-stu-id="e0c4c-112">Create a product configuration model</span></span>


1.  <span data-ttu-id="e0c4c-113">انتقل إلى **المنتجات > إدارة معلومات المنتج > نماذج تكوين المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-113">Go to **Product information management > Products > Product configuration models**.</span></span>
2.  <span data-ttu-id="e0c4c-114">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-114">Select **New**.</span></span>
3.  <span data-ttu-id="e0c4c-115">في حقل **الاسم**، أدخل **مكبرات صوت منزلية عالية الجودة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-115">In the **Name** field, enter **Home Audio HE Speakers**.</span></span>
4.  <span data-ttu-id="e0c4c-116">ضمن **المكون الجذر‬**، اختر  **تحديد مكون موجود**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-116">Under the **Root component** section, choose  **Select existing component**.</span></span>
5.  <span data-ttu-id="e0c4c-117">حدد **مكبر صوت منزلي عالي الجودة** من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-117">Select **Home Audio High End Speaker** from the drop down menu.</span></span>
5. <span data-ttu-id="e0c4c-118">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-118">Select **OK**.</span></span>
6. <span data-ttu-id="e0c4c-119">ضمن علامة التبويب السريعة **عام**، حدد **نعم** في القائمة **إعادة استخدام التكوينات**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-119">Under the **General** FastTab, select **Yes** in the **Reuse configurations** menu.</span></span>
7. <span data-ttu-id="e0c4c-120">وسّع علامة التبويب السريعة **السمات**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-120">Expand the **Attributes** FastTab.</span></span>
7. <span data-ttu-id="e0c4c-121">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-121">Select **Add**.</span></span>
8. <span data-ttu-id="e0c4c-122">في حقل **الاسم**، أدخل **لون العلبة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-122">In the **Name** field, enter **Case color**.</span></span>
9. <span data-ttu-id="e0c4c-123">في حقل **اسم الحلّال**، أدخل **لون العلبة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-123">In the **Solver name** field, enter **CaseColor**.</span></span>
10. <span data-ttu-id="e0c4c-124">في حقل **الوصف**، أدخل **الألوان المتوفرة لمكبر الصوت عالي الجودة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-124">In the **Description** field, enter **Available colors for HE Speaker**.</span></span>
11. <span data-ttu-id="e0c4c-125">في حقل **نوع** **السمة**، أدخل أو حدد **التشطيب النهائي للخزانة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-125">In the **Attribute** **type** field, enter or select **Cabinet finish**.</span></span>
12. <span data-ttu-id="e0c4c-126">حدد خانة الاختيار **تعيين الافتراضي**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-126">Select the **Set default** check box.</span></span>
13. <span data-ttu-id="e0c4c-127">في حقل **القيمة الافتراضية**، أدخل أو حدد **بلوط**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-127">In the **Default value** field, enter or select **Oak**.</span></span>
14. <span data-ttu-id="e0c4c-128">حدد خانة الاختيار **تضمين في إعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-128">Select the **Include in reuse** check box.</span></span>
15. <span data-ttu-id="e0c4c-129">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-129">Select **Add**.</span></span>
16. <span data-ttu-id="e0c4c-130">في حقل **الاسم**، أدخل **الشبكة الأمامية**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-130">In the **Name** field, enter **Front grill**.</span></span>
17. <span data-ttu-id="e0c4c-131">في حقل **اسم الحلّال**، أدخل **الشبكة الأمامية**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-131">In the **Solver name** field, enter **FrontGrill**.</span></span>
18. <span data-ttu-id="e0c4c-132">في حقل **الوصف**، أدخل **تحديد نوع الشبكة الأمامية لمكبر الصوت عالي الجودة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-132">In the **Description** field, enter **Select the type of front grill for your HE Speaker**.</span></span>
19. <span data-ttu-id="e0c4c-133">في حقل **نوع السمة**، أدخل أو حدد **الشبكة الأمامية**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-133">In the **Attribute type** field, enter or select **Front grill**.</span></span>
20. <span data-ttu-id="e0c4c-134">حدد خانة الاختيار **تعيين الافتراضي**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-134">Select the **Set default** check box.</span></span>
21. <span data-ttu-id="e0c4c-135">حدد خانة الاختيار **تضمين في إعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-135">Select the **Include in reuse** check box.</span></span>
22. <span data-ttu-id="e0c4c-136">في **حقل القيمة الافتراضية**، أدخل أو حدد **أسود**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-136">In the **Default value** field, enter or select **Black**.</span></span> 
23. <span data-ttu-id="e0c4c-137">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-137">Select **Add**.</span></span>
24. <span data-ttu-id="e0c4c-138">في حقل **الاسم**، أدخل **حماية الزوايا**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-138">In the **Name** field, enter **Corner protection**.</span></span>
25. <span data-ttu-id="e0c4c-139">في حقل **اسم الحلّال**، أدخل **حماية الزوايا**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-139">In the **Solver name** field, enter **CornerProtection**.</span></span>
26. <span data-ttu-id="e0c4c-140">في حقل **الوصف**، أدخل **هل يجب أن تكون حماية الزوايا متوفرة للكتاب الإلكتروني؟**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-140">In the **Description** field, enter **Should the eBook have corner protection?**.</span></span>
27. <span data-ttu-id="e0c4c-141">في حقل **نوع السمة**، أدخل أو حدد **حماية الزوايا**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-141">In the **Attribute type** field, enter or select **Corner protection**.</span></span>
28. <span data-ttu-id="e0c4c-142">قم بإلغاء تحديد خانة الاختيار **تعيين الافتراضي**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-142">Clear the **Set default** check box.</span></span>
28. <span data-ttu-id="e0c4c-143">حدد خانة الاختيار **تضمين في إعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-143">Select the **Include in reuse** check box.</span></span>
29. <span data-ttu-id="e0c4c-144">قم بطي علامة تبويب **السمات**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-144">Collapse the **Attributes** tab.</span></span>


## <a name="add-sub-components"></a><span data-ttu-id="e0c4c-145">إضافة المكونات الفرعية</span><span class="sxs-lookup"><span data-stu-id="e0c4c-145">Add sub components</span></span>


1. <span data-ttu-id="e0c4c-146">قم بتوسيع علامة التبويب السريعة **المكونات الفرعية**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-146">Expand the **Subcomponents** FastTab.</span></span>
2. <span data-ttu-id="e0c4c-147">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-147">Select **Add**.</span></span>
3. <span data-ttu-id="e0c4c-148">في الحقل **الاسم**، اكتب **تأمين‎‎**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-148">In the **Name** field, type **Insurance**.</span></span>
4. <span data-ttu-id="e0c4c-149">في حقل **اسم الحلّال**، أدخل **تأمين**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-149">In the **Solver name** field, enter **Insurance**.</span></span>
5. <span data-ttu-id="e0c4c-150">أدخل **هل تحتاج إلى تأمين؟** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-150">Enter **Do you need Insurance?** in the **Description** field.</span></span>
6. <span data-ttu-id="e0c4c-151">في حقل **المكون**، أدخل أو حدد **تأمين‎**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-151">In the **Component** field, enter or select **Insurance**.</span></span>
7. <span data-ttu-id="e0c4c-152">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-152">Select **Save**.</span></span>
8. <span data-ttu-id="e0c4c-153">قم بطي قسم **المكونات الفرعية**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-153">Collapse the **Subcomponents** section.</span></span>

## <a name="add-sub-bom-lines"></a><span data-ttu-id="e0c4c-154">أضافه بنود قائمة مكونات الصنف الفرعية</span><span class="sxs-lookup"><span data-stu-id="e0c4c-154">Add sub-BOM lines</span></span>


1. <span data-ttu-id="e0c4c-155">قم بتوسيع علامة التبويب السريعة **بنود قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-155">Expand the **BOM lines** FastTab.</span></span>
2. <span data-ttu-id="e0c4c-156">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-156">Select **Add**.</span></span>
3. <span data-ttu-id="e0c4c-157">في الحقل **الاسم**، أدخل **M0055**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-157">In the **Name** field, enter **M0055**.</span></span>
4. <span data-ttu-id="e0c4c-158">في حقل **الوصف**، أدخل **M0055**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-158">In the **Description** field, enter **M0055**.</span></span>
5. <span data-ttu-id="e0c4c-159">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-159">Select **Save**.</span></span>
6. <span data-ttu-id="e0c4c-160">حدد الارتباط **تفاصيل بنود قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-160">Select **BOM line details** link.</span></span>
7. <span data-ttu-id="e0c4c-161">في الحقل **رقم الصنف**، أدخل أو حدد **M0055**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-161">In the **Item number** field, enter or select **M0055**.</span></span>
8. <span data-ttu-id="e0c4c-162">حدد خانة الاختيار، ثم حدد **نعم** بجوار شريط تبديل  **الحساب**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-162">Select the check box and then **Yes** next to the **Calculation** toggle bar.</span></span>
9. <span data-ttu-id="e0c4c-163">حدد علامة تبويب **الإعداد** باتجاه أعلى النافذة المنزلقة.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-163">Select the **Setup** tab towards the top of the slide out window.</span></span>
10. <span data-ttu-id="e0c4c-164">حدد خانة الاختيار إلى جانب **الكمية** وقم بتعيين القيمة إلى **1.0000**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-164">Select the check box next to **Quantity** and set the value to **1.0000**.</span></span>
11. <span data-ttu-id="e0c4c-165">حدد خانة الاختيار إلى جانب **لكل سلسلة** وقم بتعيين القيمة إلى **1**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-165">Select the check box next to **Per series** and set the value to **1**.</span></span>
12. <span data-ttu-id="e0c4c-166">حدد علامة تبويب **البُعد** باتجاه أعلى النافذة المنزلقة.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-166">Select the **Dimension** tab at the top of the slide out window.</span></span>
13. <span data-ttu-id="e0c4c-167">حدد خانة الاختيار إلى جانب حقل **المستودع** واكتب **11**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-167">Select the check box next to the **Warehouse** field and type **11**.</span></span>
14. <span data-ttu-id="e0c4c-168">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-168">Select **OK**.</span></span>
15. <span data-ttu-id="e0c4c-169">قم بطي قسم **بنود قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-169">Collapse the **BOM lines** section.</span></span>


## <a name="add-an-expression-constraint-to-a-product-configuration-model"></a><span data-ttu-id="e0c4c-170">إضافة قيد تعبير إلى نموذج تكوين منتج</span><span class="sxs-lookup"><span data-stu-id="e0c4c-170">Add an expression constraint to a product configuration model</span></span>
 

1. <span data-ttu-id="e0c4c-171">وسّع علامة التبويب السريعة **القيود**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-171">Expand the **Constraints** FastTab.</span></span>
2. <span data-ttu-id="e0c4c-172">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-172">Select **Add**.</span></span>
3. <span data-ttu-id="e0c4c-173">في حقل **القيود**، حدد **قيد تعبير**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-173">In the **Constraints** field, select **Expression constraint**.</span></span>
4. <span data-ttu-id="e0c4c-174">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-174">Select **Create**.</span></span>
5. <span data-ttu-id="e0c4c-175">في حقل الاسم، أدخل **مكبر صوت عالي الجودة بلوط**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-175">In the name field, enter **HE Speaker Oak**.</span></span>
6. <span data-ttu-id="e0c4c-176">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-176">Select **Save**.</span></span>
7. <span data-ttu-id="e0c4c-177">حدد الارتباط **تحرير التعبير** في القسم نفسه.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-177">Select **Edit expression** link in the same section.</span></span>
8. <span data-ttu-id="e0c4c-178">في حقل **التعبير**، أدخل **Implies[FrontGrill != "Metal",!CornerProtection]**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-178">In the **Expression** field, enter **Implies[FrontGrill != "Metal",!CornerProtection]**.</span></span>
9. <span data-ttu-id="e0c4c-179">حدد **التحقق من الصحة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-179">Select **Validate**.</span></span>
10. <span data-ttu-id="e0c4c-180">تأكد من عدم حدوث أي أخطاء.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-180">Ensure that no errors occur.</span></span>
11. <span data-ttu-id="e0c4c-181">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-181">Select **Close**.</span></span>
12. <span data-ttu-id="e0c4c-182">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-182">Select **OK**.</span></span>
13. <span data-ttu-id="e0c4c-183">من جزء إجراءات **النموذج**، ضمن القائمة الفرعية **تشغيل**، حدد **التحقق من الصحة**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-183">From the **Model** action pane, under the sub menu **Run** select **Validate**.</span></span> <span data-ttu-id="e0c4c-184">يجب أن تكون النتيجة *لم يتم العثور على أخطاء*.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-184">The result should *"No errors found"*.</span></span>
14. <span data-ttu-id="e0c4c-185">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-185">Select **Close**</span></span>
15. <span data-ttu-id="e0c4c-186">من جزء إجراءات **النموذج**، ضمن القائمة الفرعية **تشغيل**، حدد **اختبار**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-186">From the **Model** action pane, under the **Run** sub menu, select **Test**.</span></span>
16. <span data-ttu-id="e0c4c-187">في حقل **لون العلبة**، أدخل **خشب الورد‬**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-187">In the **Case color** field, select **Rosewood**.</span></span>
17. <span data-ttu-id="e0c4c-188">في حقل **الشبكة الأمامية**، أدخل **أبيض**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-188">In the **Front grill** field, select **White**.</span></span>
18. <span data-ttu-id="e0c4c-189">لاحظ أن خيار **حماية الزوايا** غير متوفر وهو معيّن إلى **خطأ**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-189">Note that the **Corner protection** is not available and is set to **false**.</span></span>
19. <span data-ttu-id="e0c4c-190">في حقل **الشبكة الأمامية**، حدد **معدن**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-190">In the **Front grill** field, select **Metal**.</span></span>
20. <span data-ttu-id="e0c4c-191">لاحظة أنه يمكن تعيين **حماية الزوايا** إلى **صواب** أو **خطأ**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-191">Note that the **Corner protection** can be set to either **true** or **false**.</span></span>
21. <span data-ttu-id="e0c4c-192">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-192">Select **Next**.</span></span>
22. <span data-ttu-id="e0c4c-193">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-193">Select **OK**.</span></span>
23. <span data-ttu-id="e0c4c-194">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="e0c4c-194">Close all pages.</span></span> 
