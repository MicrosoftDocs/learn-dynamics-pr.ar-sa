---
ms.openlocfilehash: bd2dc47dd9b499a1d4e773f15b8a8bde4bac5f24
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071164"
---
<span data-ttu-id="e6fbc-101">في هذا التمرين ستعمل مع إعداد الأصول وإجراء المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="e6fbc-101">In this exercise you will work with setting up assets, and perform the following tasks:</span></span>

- <span data-ttu-id="e6fbc-102">إنشاء نوع أصل</span><span class="sxs-lookup"><span data-stu-id="e6fbc-102">Create an asset type</span></span>
- <span data-ttu-id="e6fbc-103">إنشاء قالب تقييم حالات</span><span class="sxs-lookup"><span data-stu-id="e6fbc-103">Create a condition assessment template</span></span>
- <span data-ttu-id="e6fbc-104">إعداد مستويات خدمة الأصول</span><span class="sxs-lookup"><span data-stu-id="e6fbc-104">Set up asset service levels</span></span>
- <span data-ttu-id="e6fbc-105">إنشاء معلومات العاملين</span><span class="sxs-lookup"><span data-stu-id="e6fbc-105">Create workers</span></span>

## <a name="create-an-asset-type"></a><span data-ttu-id="e6fbc-106">إنشاء نوع أصل</span><span class="sxs-lookup"><span data-stu-id="e6fbc-106">Create an asset type</span></span>
<span data-ttu-id="e6fbc-107">تمتلك Munson’s Pickles and Preserves Farm أصولاً جديدة تحتاج إلى إعداد في إدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-107">Munson’s Pickles and Preserves Farm has new assets that they need set up in Asset Management.</span></span> <span data-ttu-id="e6fbc-108">في هذا التدريب، ستقوم بإعداد "الرافعة الشوكية" كأصل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-108">In this exercise, you will set up “Forklift” as an asset.</span></span>

1.  <span data-ttu-id="e6fbc-109">انتقل إلى **إدارة الأصول > الإعداد > أنواع الأصول > أنواع الأصول**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-109">Go to **Asset management > Setup > Asset types > Asset types**.</span></span>
2.  <span data-ttu-id="e6fbc-110">حدد **جديد** لإنشاء نوع أصل جديد.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-110">Select **New** to create a new asset type.</span></span>
3.  <span data-ttu-id="e6fbc-111">في الحقل **نوع الأصل**، أدخل **رافعة شوكية** كمعرف نوع الأصل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-111">In the **Asset type** field, enter **Forklift** as the asset type ID.</span></span>
4.  <span data-ttu-id="e6fbc-112">في الحقل **الاسم**، أدخل **رافعة شوكية** كاسم نوع الأصل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-112">In the **Name** field, enter **Forklift** as the name for the asset type.</span></span> 
5.  <span data-ttu-id="e6fbc-113">في القسم **حالة دورة الحياة**، حدد نموذج دورة حياة أصل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-113">In the **Lifecycle state** section, select an asset lifecycle model.</span></span> <span data-ttu-id="e6fbc-114">تذكر أن هذه هي حالات الحياة التي تم تجميعها في نماذج سير العمل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-114">Remember that these are the lifecycle states that are grouped into workflow models.</span></span> <span data-ttu-id="e6fbc-115">حدد **قياسي**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-115">Select **Standard**.</span></span>
6.  <span data-ttu-id="e6fbc-116">في القسم **مؤشرات الأداء الاساسية**، قم بتعيين شريط التبديل **إجمالي** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-116">In the **KPIS** section, set the **Total** toggle bar to **Yes**.</span></span>
7.  <span data-ttu-id="e6fbc-117">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-117">Select **Save**.</span></span>
8.  <span data-ttu-id="e6fbc-118">في علامة التبويب السريعة **أنواع وظيفة الصيانة**، حدد **المعايرة**، و **الفحص**، و **التشحيم**، و **الوقائي**، و **الإصلاح** انتقل إلى القسم **أنواع مهام الصيانة المحددة**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-118">On the **Maintenance job types** FastTab, select **Calibration**, **Inspection**, **Lubrication**, **Preventive**, and **Repair** and then move to the **Maintenance job types selected** section.</span></span>
    > [!NOTE]
    > <span data-ttu-id="e6fbc-119">لتحديد أنواع المهام في علامة التبويب السريعة **أنواع مهام الصيانة**، يجب أن تكون قد أنشأت **أنواع مهام الصيانة** في **إدارة الأصول > الإعداد > المهام > أنواع مهام الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-119">To select job types in the **Maintenance job types** FastTab, you must have created the **Maintenance job types** in **Asset Management > Setup > Jobs > Maintenance job types**.</span></span>

9.  <span data-ttu-id="e6fbc-120">قم بتعيين **عداد** لساعات الإنتاج، ثم حدده وقم بنقله إلى القسم **عدادات الأصول المحددة**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-120">Assign a **Counter** for Production Hours, and then select and move it to the **Asset counters selected** section.</span></span> <span data-ttu-id="e6fbc-121">لن تتم إضافة **نوع السمة** في هذا الوقت.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-121">You won’t be adding an **Attribute type** at this time.</span></span>
10. <span data-ttu-id="e6fbc-122">اترك علامة التبويب السريعة **تقييمات الشرط** الفارغة حاليا.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-122">Leave the **Condition assessments** FastTab blank for now.</span></span> 
11. <span data-ttu-id="e6fbc-123">**احفظ** نوع الأصل الجديد.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-123">**Save** the new asset type.</span></span>

## <a name="create-a-condition-assessment-template"></a><span data-ttu-id="e6fbc-124">إنشاء قالب تقييم حالات</span><span class="sxs-lookup"><span data-stu-id="e6fbc-124">Create a condition assessment template</span></span>
<span data-ttu-id="e6fbc-125">ترغب Munson’s Pickles and Preserves Farm في إنشاء قالب تقييم شرط لأجهزة المزج الخاصة بهم لضمان أن ضوضاء الشفرات تتم مراقبتها إذا حدث تغيير في مستواها.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-125">Munson’s Pickles and Preserves Farm wants to establish a condition assessment template for their blenders to ensure that the noise from the blades are monitored for changes in volume.</span></span> <span data-ttu-id="e6fbc-126">اتبع الخطوات التالية لإضافة قالب تقييم الشروط.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-126">Follow these steps to add a condition assessment template.</span></span>

1.  <span data-ttu-id="e6fbc-127">انتقل إلى **إدارة الأصول > الإعداد > أنواع الأصول > قوالب تقييمات الحالات**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-127">Go to **Asset Management > Setup > Asset types > Condition assessment templates**.</span></span>
2.  <span data-ttu-id="e6fbc-128">حدد **جديد** لإنشاء قالب جديد.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-128">Select **New** to create a new template.</span></span>
3.  <span data-ttu-id="e6fbc-129">أدخل **الضوضاء**، في الحقل **القالب** كمعرّف أو اسم.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-129">Enter **Noise** as the ID or name in the **Template** field.</span></span>
4.  <span data-ttu-id="e6fbc-130">أدخل **الضوضاء**، في الحقل **الاسم** كاسم للقالب.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-130">Enter **Noise** as the template name the **Name** field.</span></span>
5.  <span data-ttu-id="e6fbc-131">في علامة التبويب السريعة **بنود تقييم الشرط**، حدد الزر **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-131">On the **Condition assessment lines** FastTab, select the **Add** button.</span></span>
6.  <span data-ttu-id="e6fbc-132">في البند الأول، أدخل **اسم** تقييم الشرط بالقيمة **لا يزيد عن 100 ديسيبل**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-132">In the first line, enter the **Name** of the condition assessment as **No greater than 100 db**.</span></span>
7.  <span data-ttu-id="e6fbc-133">أدخل **وصف** تقييم الشرط بالقيمة **لا يزيد عن 100 ديسيبل**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-133">Enter the **Description** of the condition assessment as **No greater than 100 db**.</span></span>
8.  <span data-ttu-id="e6fbc-134">حدد **نوع البيانات** من القائمة المنسدلة الخاصة بتقييم الحالة.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-134">Select the **Data type** from the drop-down menu of the condition assessment.</span></span> <span data-ttu-id="e6fbc-135">حدد **سلسلة**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-135">Select **String**.</span></span>
9.  <span data-ttu-id="e6fbc-136">في علامة التبويب السريعة **أنواع الأصول**، أضف أنواع الأصول التي يجب تضمينها في قالب تقييم الحالة.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-136">On the **Asset types** FastTab, add the asset types that should be included on the condition assessment template.</span></span> <span data-ttu-id="e6fbc-137">حدد **إضافة**، ثم حدد **ضاغط هواء**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-137">Select **Add** and then select **Air compressor**.</span></span>
10. <span data-ttu-id="e6fbc-138">**حفظ** القالب.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-138">**Save** the template.</span></span>


## <a name="set-up-asset-service-levels"></a><span data-ttu-id="e6fbc-139">إعداد مستويات خدمة الأصول</span><span class="sxs-lookup"><span data-stu-id="e6fbc-139">Set up asset service levels</span></span>
<span data-ttu-id="e6fbc-140">يتم استخدام مستويات خدمة الأصل في طلبات الصيانة وأوامر العمل لتحديد أولوية أوامر العمل أثناء جدولة أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-140">Asset service levels are used on maintenance requests and work orders to determine the priority of work orders during work order scheduling.</span></span> <span data-ttu-id="e6fbc-141">في هذا التمرين، ستقوم بتعيين مستوى خدمة الأصل إلى ضاغط الهواء.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-141">In this exercise, you will assign an asset service level to your air compressor.</span></span>

<span data-ttu-id="e6fbc-142">لإعداد مستويات خدمة الأصول‬، اتبع هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="e6fbc-142">To set up asset service levels, follow these steps:</span></span>

1.  <span data-ttu-id="e6fbc-143">انتقل إلى **إدارة الأصول > إعداد > مستويات خدمة الأصل**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-143">Go to **Asset management > Setup > Asset service levels**.</span></span>
2.  <span data-ttu-id="e6fbc-144">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-144">Select **New**.</span></span>
3.  <span data-ttu-id="e6fbc-145">حدد **موقع العمل** بالقيمة **PP-01**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-145">Select the **Functional location** as **PP-01**.</span></span>
4.  <span data-ttu-id="e6fbc-146">حدد **نوع الأصل** لـ **ضاغط الهواء**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-146">Select the **Asset type** of **Air Compressor**.</span></span>
5.  <span data-ttu-id="e6fbc-147">حدد **نوع أمر العمل** بالقيمة **وقائي**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-147">Select the **Work order type** as **Preventive**.</span></span>
6.  <span data-ttu-id="e6fbc-148">حدد **مستوى الخدمة** بالقيمة **3**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-148">Select the **Service Level** as **3**.</span></span>
7.  <span data-ttu-id="e6fbc-149">**احفظ** مستوى خدمة الأصل الجديد.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-149">**Save** the new Asset service level.</span></span>

## <a name="create-workers"></a><span data-ttu-id="e6fbc-150">إنشاء معلومات العاملين</span><span class="sxs-lookup"><span data-stu-id="e6fbc-150">Create workers</span></span>
<span data-ttu-id="e6fbc-151">تقوم Munson’s Pickles Farm and Preserves بإنشاء بيانات كافة العمال في الوحدات النمطية للموارد البشرية وإدارة المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-151">Munson’s Pickles Farm and Preserves has all workers established in the Human resources and Organization administration modules.</span></span> <span data-ttu-id="e6fbc-152">يمكنك الآن تعيين العاملين لمجموعات العاملين الخاصة بالصيانة.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-152">You can now assign their workers to maintenance worker groups.</span></span> <span data-ttu-id="e6fbc-153">تتم إضافة عامل إلى مجموعة عاملي الصيانة "فنيو الكهرباء" بحيث يمكن تعيينها عند الحاجة إلى المهارات الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-153">You will add a worker to the “Electricians” maintenance worker group so they can be assigned when their skills are needed.</span></span>

1.  <span data-ttu-id="e6fbc-154">انتقل إلى **إدارة الأصول > إعداد > العاملون > عاملون**</span><span class="sxs-lookup"><span data-stu-id="e6fbc-154">Go to **Asset Management > Setup > Workers > Workers**.</span></span>
2.  <span data-ttu-id="e6fbc-155">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-155">Select **New**.</span></span>
3.  <span data-ttu-id="e6fbc-156">في الحقل **العامل**، حدد العامل من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-156">In the **Worker** field, select a worker from the drop-down menu.</span></span>
4.  <span data-ttu-id="e6fbc-157">قم بتعيين زر التبديل **نشط** إلى **نعم** لجدولة هذا العامل في أوامر العمل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-157">Set the **Active** toggle button to **Yes** to schedule this worker on work orders.</span></span>
5.  <span data-ttu-id="e6fbc-158">في علامة التبويب السريعة **المجموعات**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-158">On the **Groups** FastTab, select **Add**.</span></span>
6.  <span data-ttu-id="e6fbc-159">في الحقل **مجموعة عاملي الصيانة**، حدد **فنيو الكهرباء**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-159">In the **Maintenance worker group** field, select **Electricians**.</span></span>
7.  <span data-ttu-id="e6fbc-160">في علامة التبويب السريعة **مواقع العمل**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-160">On the **Functional locations** FastTab, select **Add line**.</span></span>
8.  <span data-ttu-id="e6fbc-161">في **موقع العمل**، حدد **PP-01**.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-161">In the **Functional location** field, select **PP-01**.</span></span> <span data-ttu-id="e6fbc-162">حدد هذه القيمة باعتبارها **كموقع رئيسي** للعامل.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-162">Select this as the worker's **Primary location**.</span></span> 
9.  <span data-ttu-id="e6fbc-163">**احفظ** العامل الجديد.</span><span class="sxs-lookup"><span data-stu-id="e6fbc-163">**Save** the new worker.</span></span>

