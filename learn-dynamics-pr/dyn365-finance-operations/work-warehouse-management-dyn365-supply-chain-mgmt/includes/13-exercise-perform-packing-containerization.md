---
ms.openlocfilehash: c622d0249ca0fb1dda9b0aa89d73708007143109
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073165"
---
## <a name="scenario-set-up-manual-packing"></a><span data-ttu-id="0ff4f-101">السيناريو: إعداد التعبئة اليدوية</span><span class="sxs-lookup"><span data-stu-id="0ff4f-101">Scenario: Set up manual packing</span></span>

<span data-ttu-id="0ff4f-102">تتم مطالبتك بإعداد التعبئة اليدوية لعصير البرتقال في Contoso.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-102">You are asked to set up manual packing for Contoso Orange Juice.</span></span> <span data-ttu-id="0ff4f-103">يجب إنشاء نوع حاوية وملف تعريف التعبئة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-103">You need to create a container type and packing profile.</span></span> <span data-ttu-id="0ff4f-104">ثم ستقوم بعد ذلك بربط ملف تعريف التعبئة بالمستخدم Julia Funderburk.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-104">You will then link the packing profile to the user Julia Funderburk.</span></span>

### <a name="create-container-types"></a><span data-ttu-id="0ff4f-105">إنشاء أنواع الحاويات</span><span class="sxs-lookup"><span data-stu-id="0ff4f-105">Create container types</span></span>

1.  <span data-ttu-id="0ff4f-106">في شركة USP2، افتح **إدارة المستودع > إعداد > الحاويات > أنواع الحاويات**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-106">In the company USP2, open **Warehouse management > Setup > Containers > Container types**.</span></span>

2.  <span data-ttu-id="0ff4f-107">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-107">Select **New**.</span></span>

3.  <span data-ttu-id="0ff4f-108">في الحقل **رمز نوع الحاوية**، أدخل **صندوق التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-108">In the **Container type code** field, enter **PackingBox**.</span></span>

4.  <span data-ttu-id="0ff4f-109">في حقل **الوصف**، أدخل **صندوق التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-109">In the **Description** field, enter **PackingBox**.</span></span>

5.  <span data-ttu-id="0ff4f-110">في الحقل **الوزن الفارغ**، أدخل **0.5**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-110">In the **Tare weight** field, enter **0.5**.</span></span>

6.  <span data-ttu-id="0ff4f-111">في الحقل **الحد الأقصى للوزن الصافي**، أدخل **15.00**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-111">In the **Maximum net weight** field, enter **15.00**.</span></span>

7.  <span data-ttu-id="0ff4f-112">في الحقل **طول الحاوية**، أدخل **12.00**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-112">In the **Container length** field, enter **12.00**.</span></span>

8.  <span data-ttu-id="0ff4f-113">في الحقل **عرض الحاوية**، أدخل **16.00**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-113">In the **Container width** field, enter **16.00**.</span></span>

9.  <span data-ttu-id="0ff4f-114">في الحقل **ارتفاع الحاوية**، أدخل **10.00**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-114">In the **Container height** field, enter **10.00**.</span></span>

10. <span data-ttu-id="0ff4f-115">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-115">Select **Save**.</span></span>

### <a name="create-a-container-packing-policy"></a><span data-ttu-id="0ff4f-116">إنشاء نهج تعبئة الحاويات</span><span class="sxs-lookup"><span data-stu-id="0ff4f-116">Create a Container packing policy</span></span> 

1.  <span data-ttu-id="0ff4f-117">افتح **إدارة المستودع > إعداد > الحاويات > نهج تعبئة الحاويات**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-117">Open **Warehouse management > Setup > Containers > Container packing policies**.</span></span>
2.  <span data-ttu-id="0ff4f-118">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-118">Select **New**.</span></span>
3.  <span data-ttu-id="0ff4f-119">في الحقل **نهج تعبئة الحاوية**، أدخل **WH30Close**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-119">In the **Container packing policy** field, enter **WH30Close**.</span></span>
4.  <span data-ttu-id="0ff4f-120">في الحقل **الوصف**، أدخل **إغلاق الحاوية**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-120">In the  **Description** field, enter **Close container**.</span></span>
5.  <span data-ttu-id="0ff4f-121">في علامة التبويب السريعة **نظرة عامة**، حدد القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="0ff4f-121">On the **Overview** Fast tab select the following values:</span></span>
    - <span data-ttu-id="0ff4f-122">في **المستودع**، حدد **30**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-122">**Warehouse**, select **30**.</span></span>
    - <span data-ttu-id="0ff4f-123">في **الموقع الافتراضي للشحنة النهائية**، حدد **Baydoor**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-123">**Default location for final shipment**, select **Baydoor**.</span></span>
    - <span data-ttu-id="0ff4f-124">في **وحدة الوزن**، حدد **كجم**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-124">**Weight unit**, select **kg**.</span></span>
    - <span data-ttu-id="0ff4f-125">في **سياسة إغلاق الحاوية**، حدد **الإصدار التلقائي**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-125">**Container closing policy**, select **Automatic release**.</span></span>
    - <span data-ttu-id="0ff4f-126">في **سياسة إصدار الحاوية**، حدد **إتاحة في موقع الشحن النهائي**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-126">**Container release policy**, select **Make available at final shipping location**.</span></span>
    - <span data-ttu-id="0ff4f-127">اترك كافة الخيارات الأخرى بالإعداد الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-127">Leave all others at default.</span></span>
6.  <span data-ttu-id="0ff4f-128">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-128">Select **Save**.</span></span>
7.  <span data-ttu-id="0ff4f-129">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-129">Close the page.</span></span>

### <a name="create-a-packing-profile"></a><span data-ttu-id="0ff4f-130">إنشاء ملف تعريف التعبئة</span><span class="sxs-lookup"><span data-stu-id="0ff4f-130">Create a packing profile</span></span>

1.  <span data-ttu-id="0ff4f-131">افتح **إدارة المستودعات > إعداد > تعبئة > ملفات تعريف التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-131">Open **Warehouse management > Setup > Packing > Packing profiles**.</span></span>

2.  <span data-ttu-id="0ff4f-132">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-132">Select **New**.</span></span>

3.  <span data-ttu-id="0ff4f-133">في حقل **معرّف ملف تعريف التعبئة**، أدخل **PACK2**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-133">Enter **PACK2** in the **Packing profile ID** field.</span></span>

4.  <span data-ttu-id="0ff4f-134">في حقل **الوصف**، أدخل **محطة التعبئة 2**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-134">Enter **Packing station 2** in the **Description** field.</span></span>

5.  <span data-ttu-id="0ff4f-135">حدد **WH30Close** في الحقل **نهج تعبئة الحاوية**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-135">Select **WH30Close** in the **Container packing policy** field.</span></span>

6.  <span data-ttu-id="0ff4f-136">حدد **تلقائي** في الحقل **وضع معرّف الحاوية**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-136">Select **Auto** in the **Container ID mode** field.</span></span>

7.  <span data-ttu-id="0ff4f-137">في الحقل **نوع الحاوية**، حدد **صندوق التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-137">In the **Container type** field, select **PackingBox**.</span></span>

8.  <span data-ttu-id="0ff4f-138">اضغط على المفتاح Tab وشريط المسافات لتحديد خانة الاختيار **إنشاء تلقائي للحاوية في إغلاق الحاوية**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-138">Press the  tab  key and the space bar to select the **Autocreate container at container close** check  box.</span></span>

9.  <span data-ttu-id="0ff4f-139">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-139">Select **Save**.</span></span>


### <a name="link-the-profile-to-a-work-user"></a><span data-ttu-id="0ff4f-140">ربط ملف التعريف بمستخدم عمل</span><span class="sxs-lookup"><span data-stu-id="0ff4f-140">Link the profile to a work user</span></span>

1. <span data-ttu-id="0ff4f-141">افتح **إدارة المستودعات > إعداد > العامل**</span><span class="sxs-lookup"><span data-stu-id="0ff4f-141">Open **Warehouse management > Setup > Worker**.</span></span>

2. <span data-ttu-id="0ff4f-142">حدد **Julia Funderburk** من الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-142">Select **Julia Funderburk** from the left-hand pane.</span></span>

3. <span data-ttu-id="0ff4f-143">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-143">Select **Edit**.</span></span>

4. <span data-ttu-id="0ff4f-144">قم بتحديث حقل **معرّف ملف تعريف التعبئة** إلى **PACK2**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-144">Update the **Packing profile ID** field to **PACK2**.</span></span>

5. <span data-ttu-id="0ff4f-145">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-145">Select **Save**.</span></span>


## <a name="set-up-a-wave-template"></a><span data-ttu-id="0ff4f-146">إعداد قالب موجة</span><span class="sxs-lookup"><span data-stu-id="0ff4f-146">Set up a wave template</span></span>

1.  <span data-ttu-id="0ff4f-147">انتقل إلى **إدارة المستودعات > إعداد > الموجات > قوالب الموجات**</span><span class="sxs-lookup"><span data-stu-id="0ff4f-147">Go to **Warehouse management > Setup > Waves > Wave templates**.</span></span>

2.  <span data-ttu-id="0ff4f-148">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-148">Select **New**.</span></span>

3.  <span data-ttu-id="0ff4f-149">في الحقل **اسم قالب الموجة**، أدخل **NewWave30**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-149">In the **Wave template name** field, enter **NewWave30**.</span></span>

4.  <span data-ttu-id="0ff4f-150">في الحقل **وصف قالب الموجة**، أدخل **NewWave30**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-150">In the **Wave template description** field, enter **NewWave30**.</span></span>

5.  <span data-ttu-id="0ff4f-151">في الحقل **الموقع**، أدخل أو حدد 3.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-151">In the **Site** field, enter or select 3.</span></span>

6.  <span data-ttu-id="0ff4f-152">في الحقل **المستودع**، أدخل أو حدد 30.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-152">In the **Warehouse** field, enter or select 30.</span></span>

7.  <span data-ttu-id="0ff4f-153">قم بتوسيع قسم **الأساليب**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-153">Expand the **Methods** section.</span></span> <span data-ttu-id="0ff4f-154">يسرد جزء **الأساليب المحددة** الأساليب الخاصة بنوع قالب الموجة المحدد.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-154">The **Selected methods** pane lists the methods for the selected wave template type.</span></span> <span data-ttu-id="0ff4f-155">يجب أن يتضمن قالب الموجة الأسلوب **‏‫التعبئة في حاويات‬**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-155">The wave template must include the **Containerization** method.</span></span> <span data-ttu-id="0ff4f-156">تظهر الرسالة التحذيرية **يُعد رمز خطوة الموجة إلزامياً لأسلوب الموجة التعبئة في حاويات**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-156">A warning message **Wave step code is mandatory for wave method Containerization** appears.</span></span>

8.  <span data-ttu-id="0ff4f-157">في القائمة، قم بالبحث عن الأسلوب الذي تفضله وحدده.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-157">In the list, find and select the desired method.</span></span>

9.  <span data-ttu-id="0ff4f-158">أدخل القيمة في الحقل **رمز خطوة الموجة** ضمن القسم **الأساليب المحددة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-158">In the **Wave step code** field in the **Selected methods** section, enter a value.</span></span> <span data-ttu-id="0ff4f-159">أدخل **رمز خطوة الموجة** للأسلوب المضاف، والذي يمكن أن يكون أي رمز تختاره.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-159">Enter a **Wave step code** for the added method, which can be any code you choose.</span></span> <span data-ttu-id="0ff4f-160">لذا على سبيل المثال، أدخل **1** كقيمة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-160">So, for example, enter **1** as the value.</span></span> <span data-ttu-id="0ff4f-161">من الممكن إضافة الأسلوب أكثر من مرة وتعيين رموز موجات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-161">It's possible to add the method more than once and assign different wave step codes.</span></span> <span data-ttu-id="0ff4f-162">للقيام بذلك، حدد **جعل الأسلوب قابلاً للتكرار** في الصفحة **أساليب معالجة الموجة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-162">To do this, select **Make method repeatable** on the **Wave process methods** page.</span></span>

10. <span data-ttu-id="0ff4f-163">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-163">Select **Save**.</span></span>

11. <span data-ttu-id="0ff4f-164">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-164">Close the page.</span></span>


## <a name="enable-license-plate-label-printing"></a><span data-ttu-id="0ff4f-165">تمكين طباعة بطاقة لوحة الترخيص</span><span class="sxs-lookup"><span data-stu-id="0ff4f-165">Enable license plate label printing</span></span>
 
<span data-ttu-id="0ff4f-166">يمكنك تمكين الطباعة التلقائية لتسمية **كود مسلسل حاوية شحن (SSCC)** بعد انتقاء الصنف الأخير من المخزون في عملية انتقاء المبيعات.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-166">You can enable the automatic printing of a **Serial shipping container code** (SSCC) label after the last item is picked from inventory in a sales picking work process.</span></span> 

### <a name="set-up-the-gs1-company-prefix"></a><span data-ttu-id="0ff4f-167">إعداد بادئة شركة GS1</span><span class="sxs-lookup"><span data-stu-id="0ff4f-167">Set up the GS1 company prefix</span></span>

1.  <span data-ttu-id="0ff4f-168">في شركة **USMF**، انتقل إلى **إدارة المستودع > إعداد > معلمات إدارة المستودع**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-168">In company **USMF**, go to **Warehouse management > Setup > Warehouse management parameters**.</span></span>

2.  <span data-ttu-id="0ff4f-169">في الحقل **بادئة شركة GS1**، أدخل الـ 7 أرقام الخاصة بشركة GS1.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-169">In the **GS1 company prefix** field, enter the 7 numbers for your GS1 company number.</span></span>

3.  <span data-ttu-id="0ff4f-170">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-170">Select **Save**.</span></span>

4.  <span data-ttu-id="0ff4f-171">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-171">Close the page.</span></span>


### <a name="set-up-the-sscc-license-plate-number-sequence"></a><span data-ttu-id="0ff4f-172">إعداد التسلسل الرقمي للوحة الترخيص SSCC</span><span class="sxs-lookup"><span data-stu-id="0ff4f-172">Set up the SSCC license plate number sequence</span></span>

1.  <span data-ttu-id="0ff4f-173">انتقل إلى **إدارة المؤسسة > التسلسلات الرقمية > التسلسلات الرقمية**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-173">Go to **Organization administration > Number sequences > Number sequences**.</span></span>

2.  <span data-ttu-id="0ff4f-174">حدد **رقم التسلسل** في الحقل **جديد**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-174">Select **Number sequence** in the **NEW** section.</span></span>

2.  <span data-ttu-id="0ff4f-175">في الحقل **النطاق**، حدد **الشركة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-175">In the **Scope** field, select **Company**.</span></span>

3.  <span data-ttu-id="0ff4f-176">في الحقل **الشركة**، حدد **USMF**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-176">In the **Company** field, select **USMF**.</span></span>

4.  <span data-ttu-id="0ff4f-177">قم بتوسيع القسم **المقاطع‬**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-177">Expand the **Segments** section.</span></span>

5.  <span data-ttu-id="0ff4f-178">حدد صف **الشركة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-178">Select the **Company** row.</span></span>

6.  <span data-ttu-id="0ff4f-179">حدد **إزالة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-179">Select **Remove**.</span></span>

7.  <span data-ttu-id="0ff4f-180">حدد صف **الثوابت‬**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-180">Select the **Constant** row.</span></span>

8.  <span data-ttu-id="0ff4f-181">حدد **إزالة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-181">Select **Remove**.</span></span>

9.  <span data-ttu-id="0ff4f-182">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-182">Select **Save**.</span></span>

10. <span data-ttu-id="0ff4f-183">أدخل القيمة في الحقل **رمز التسلسل الرقمي**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-183">Enter a value in **Number sequence code** field.</span></span>

10. <span data-ttu-id="0ff4f-184">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-184">Close the page.</span></span>


### <a name="create-the-document-route-layout"></a><span data-ttu-id="0ff4f-185">إنشاء تخطيط مسار المستند</span><span class="sxs-lookup"><span data-stu-id="0ff4f-185">Create the document route layout</span></span>

1.  <span data-ttu-id="0ff4f-186">انتقل إلى **إدارة المستودع > إعداد > توجيه المستند > تخطيطات توجيه المستندات**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-186">Go to **Warehouse management > Setup > Document routing > Document routing layouts**.</span></span>

2.  <span data-ttu-id="0ff4f-187">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-187">Select **New**.</span></span>

3.  <span data-ttu-id="0ff4f-188">في حقل **معرّف التخطيط‬**، أدخل **GTLLayout**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-188">In the **Layout ID** field, enter **GTLLayout**.</span></span>

4.  <span data-ttu-id="0ff4f-189">يرجى إدخال أي قيمة في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-189">In the **Description** field, enter any value.</span></span>

5.  <span data-ttu-id="0ff4f-190">في القائمة، ابحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-190">In the list, find and select the desired record.</span></span>

6.  <span data-ttu-id="0ff4f-191">حدد **إدراج في نهاية النص**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-191">Select **Insert at end of text**.</span></span>

7.  <span data-ttu-id="0ff4f-192">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-192">Select **Save**.</span></span>

8.  <span data-ttu-id="0ff4f-193">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-193">Close the page.</span></span>


### <a name="set-up-the-document-routing"></a><span data-ttu-id="0ff4f-194">إعداد توجيه المستند</span><span class="sxs-lookup"><span data-stu-id="0ff4f-194">Set up the document routing</span></span>

1.  <span data-ttu-id="0ff4f-195">انتقل إلى **إدارة المستودع > إعداد > توجيه المستند > توجيه المستند**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-195">Go to **Warehouse management > Setup > Document routing > Document routing**.</span></span>

2.  <span data-ttu-id="0ff4f-196">في الحقل **نوع أمر العمل**، حدد خياراً (مثل **أوامر الشراء**).</span><span class="sxs-lookup"><span data-stu-id="0ff4f-196">In the **Work order type** field, select an option (such as **Purchase orders**).</span></span>

3.  <span data-ttu-id="0ff4f-197">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-197">Select **New**.</span></span>

5.  <span data-ttu-id="0ff4f-198">في الحقل **المستودع**، أدخل **61**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-198">In the **Warehouse** field, enter **61**.</span></span>

5.  <span data-ttu-id="0ff4f-199">في حقل **الاسم**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-199">In the **Name** field, enter a value.</span></span>

6.  <span data-ttu-id="0ff4f-200">حدد **جديد** في القسم **طابعات توجيه المستندات**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-200">Select **New** in the **Document routing printers** section.</span></span>

7.  <span data-ttu-id="0ff4f-201">في حقل **معرّف التخطيط‬**، أدخل أو حدد **GTLLayout**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-201">In the **Layout ID** field, enter or select **GTLLayout**.</span></span>

8.  <span data-ttu-id="0ff4f-202">في الحقل **الاسم**، أدخل اسم الطابعة التي ترغب في استخدامها.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-202">In the **Name** field, enter the printer name that you want to use.</span></span>

9.  <span data-ttu-id="0ff4f-203">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-203">Select **Save**.</span></span>

10. <span data-ttu-id="0ff4f-204">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-204">Close the page.</span></span>


### <a name="create-a-mobile-device-menu"></a><span data-ttu-id="0ff4f-205">إنشاء قائمة جهاز محمول</span><span class="sxs-lookup"><span data-stu-id="0ff4f-205">Create a mobile device menu</span></span>

1.  <span data-ttu-id="0ff4f-206">انتقل إلى **إدارة المستودعات > إعداد > الجهاز المحمول > عناصر قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-206">Go to **Warehouse management > Setup > Mobile device > Mobile device menu items**.</span></span>

2.  <span data-ttu-id="0ff4f-207">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-207">Select **New**.</span></span>

3.  <span data-ttu-id="0ff4f-208">في الحقل **اسم عنصر القائمة**، أدخل **‏‫GTLMnu**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-208">In the **Menu item name** field, enter **GTLMnu**.</span></span>

4.  <span data-ttu-id="0ff4f-209">يرجى إدخال قيمة في حقل **العنوان**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-209">In the **Title** field, enter a value.</span></span>

5.  <span data-ttu-id="0ff4f-210">في حقل **الوضع‬**، حدد **عمل**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-210">In the **Mode** field, select **Work**.</span></span>

6.  <span data-ttu-id="0ff4f-211">حدد **نعم** في حقل **استخدام العمل القائم**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-211">Select **Yes** in the **Use existing work** field.</span></span>

7.  <span data-ttu-id="0ff4f-212">حدد **نعم** في الحقل **إنشاء لوحة ترخيص**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-212">Select **Yes** in the **Generate license plate** field.</span></span>

8.  <span data-ttu-id="0ff4f-213">قم بتوسيع القسم **فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-213">Expand the **Work classes** section.</span></span>

9.  <span data-ttu-id="0ff4f-214">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-214">Select **New**.</span></span>

10. <span data-ttu-id="0ff4f-215">في الحقل **معرّف فئة العمل**، حدد القيمة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-215">In the **Work class ID** field, select a value.</span></span>

11. <span data-ttu-id="0ff4f-216">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-216">Select **Save**.</span></span>

12. <span data-ttu-id="0ff4f-217">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-217">Close the page.</span></span>

13. <span data-ttu-id="0ff4f-218">انتقل إلى **إدارة المستودعات > إعداد > الجهاز المحمول > قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-218">Go to **Warehouse management > Setup > Mobile device > Mobile device menu**.</span></span>

14. <span data-ttu-id="0ff4f-219">في القائمة، ابحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-219">In the list, find and select the desired record.</span></span>

15. <span data-ttu-id="0ff4f-220">في الشجرة، حدد **GTLMnu**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-220">In the tree, select **GTLMnu**.</span></span>

16. <span data-ttu-id="0ff4f-221">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-221">Select **Edit**.</span></span>

17. <span data-ttu-id="0ff4f-222">حدد السهم لإضافة عنصر القائمة إلى القائمة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-222">Select the arrow to add the menu item to the menu.</span></span>

18. <span data-ttu-id="0ff4f-223">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-223">Select **Save**.</span></span>

19. <span data-ttu-id="0ff4f-224">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-224">Close the page.</span></span>


### <a name="update-a-work-template"></a><span data-ttu-id="0ff4f-225">تحديث قالب عمل</span><span class="sxs-lookup"><span data-stu-id="0ff4f-225">Update a work template</span></span>

1.  <span data-ttu-id="0ff4f-226">انتقل إلى **إدارة المستودعات > إعداد > العمل > قوالب العمل**</span><span class="sxs-lookup"><span data-stu-id="0ff4f-226">Go to **Warehouse management > Setup > Work > Work templates**.</span></span>

2.  <span data-ttu-id="0ff4f-227">في القائمة، ابحث عن السجل المطلوب وحدده في القسم **تفاصيل قالب العمل**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-227">In the list, find and select the desired record in the **Work Template Details** section.</span></span>

3.  <span data-ttu-id="0ff4f-228">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-228">Select **Edit**.</span></span>

4.  <span data-ttu-id="0ff4f-229">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-229">Select **New**.</span></span>

5.  <span data-ttu-id="0ff4f-230">في الحقل **نوع العمل**، حدد **طباعة**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-230">In the **Work type** field, select **Print**.</span></span>

6.  <span data-ttu-id="0ff4f-231">في الحقل **معرّف فئة العمل**، حدد أو أدخل القيمة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-231">In the **Work class ID** field, enter or select a value.</span></span>

7.  <span data-ttu-id="0ff4f-232">قم بوضع المؤشر على حقل آخر ثم حدد القائمة وحدد **تحريك لأعلى**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-232">Place the cursor on another field and then select the list and select **Move up**.</span></span>

8.  <span data-ttu-id="0ff4f-233">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-233">Select **Save**.</span></span>

9.  <span data-ttu-id="0ff4f-234">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="0ff4f-234">Close the page.</span></span> 




