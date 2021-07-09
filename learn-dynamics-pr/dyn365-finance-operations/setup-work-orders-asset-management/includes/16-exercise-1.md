---
ms.openlocfilehash: 6078417c193bbc4aafda191895986d19b4fa0a4d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071581"
---
<span data-ttu-id="2cb99-101">في هذا التمرين، ستقوم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="2cb99-101">In this exercise you will:</span></span>

- <span data-ttu-id="2cb99-102">إنشاء فئة نوع مهمة صيانة</span><span class="sxs-lookup"><span data-stu-id="2cb99-102">Create a maintenance job type category</span></span>
- <span data-ttu-id="2cb99-103">إنشاء تجارة وظيفة صيانة</span><span class="sxs-lookup"><span data-stu-id="2cb99-103">Create a maintenance job trade</span></span>
- <span data-ttu-id="2cb99-104">إنشاء نوع مهمة الصيانة</span><span class="sxs-lookup"><span data-stu-id="2cb99-104">Create a maintenance job type</span></span>
- <span data-ttu-id="2cb99-105">إنشاء مستوى خدمة</span><span class="sxs-lookup"><span data-stu-id="2cb99-105">Create a service level</span></span>
- <span data-ttu-id="2cb99-106">اعداد مصمم الأخطاء</span><span class="sxs-lookup"><span data-stu-id="2cb99-106">Set up the fault designer</span></span>

## <a name="create-a-maintenance-job-type-category"></a><span data-ttu-id="2cb99-107">إنشاء فئة نوع مهمة صيانة</span><span class="sxs-lookup"><span data-stu-id="2cb99-107">Create a maintenance job type category</span></span>
<span data-ttu-id="2cb99-108">لقد بدأت Munson’s Pickles and Preserves Farm إعداد النظام الخاص بها ويحتاج إلى إعداد فئات أنواع مهام إضافية.</span><span class="sxs-lookup"><span data-stu-id="2cb99-108">Munson’s Pickles and Preserves Farm has begun setting up their system and needs additional job type categories set up.</span></span> <span data-ttu-id="2cb99-109">ولكنها تقوم حالياً بإعداد أنواع خدمات تصحيحية ووقائية وترغب في إضافتها إلى مجموعة جديدة تمت إضافتها إلى **الفحص**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-109">They currently have Corrective, Preventive, and Service types set up and want a new one added named **Inspection**.</span></span>

1.  <span data-ttu-id="2cb99-110">انتقل إلى **إدارة الأصول > الإعداد > المهام > فئات أنواع مهام الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-110">Go to **Asset Management > Setup > Jobs > Maintenance job type categories**.</span></span>
2.  <span data-ttu-id="2cb99-111">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-111">Select **New**.</span></span>
3.  <span data-ttu-id="2cb99-112">في الحقل **فئة نوع مهمة الصيانة**، أدخل فئة نوع مهمة صيانة جديدة بالاسم **الفحص**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-112">In the **Maintenance job type category** field, enter a new maintenance job type category named **Inspection**.</span></span>
4.  <span data-ttu-id="2cb99-113">في الحقل **الاسم**، أدخل **نوع وظيفة الفحص** كاسم وصفي.</span><span class="sxs-lookup"><span data-stu-id="2cb99-113">In the **Name** field, enter **Inspection job type** as a descriptive name.</span></span>
5.  <span data-ttu-id="2cb99-114">**احفظ** فئة نوع الوظيفة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-114">**Save** your new job type category.</span></span> 

## <a name="create-a-maintenance-job-trade"></a><span data-ttu-id="2cb99-115">إنشاء تجارة وظيفة صيانة</span><span class="sxs-lookup"><span data-stu-id="2cb99-115">Create a maintenance job trade</span></span>
<span data-ttu-id="2cb99-116">ونظراً لأن الحفاظ على درجة الحرارة الداخلية مهم لبعض الماكينات والعمليات التي تحدث في مصنعهم، فان Munson’s Pickles and Preserves Farm قد قررت توظيف عاملي HVAC لمواقعهم.</span><span class="sxs-lookup"><span data-stu-id="2cb99-116">Because maintaining the indoor temperature is important to some of the machinery and processes that are occurring in their plant, Munson’s Pickles and Preserves Farm has decided to hire HVAC workers for their locations.</span></span> <span data-ttu-id="2cb99-117">المهمة الخاصة بك هي إضافة تجارة مهمة صيانة جديدة في إدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="2cb99-117">Your task is to add a new maintenance job trade in Asset Management.</span></span>

1. <span data-ttu-id="2cb99-118">انتقل إلى **إدارة الأصول > الإعداد > المهام > تجارة مهمة الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-118">Go to **Asset Management > Setup > Jobs > Maintenance job trade**.</span></span>
1.  <span data-ttu-id="2cb99-119">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-119">Select **New**.</span></span>
2.  <span data-ttu-id="2cb99-120">في حقل **التجارة**، أدخل **HVAC** كعنوان للمساعدة في تحديد تجارة مهمة الصيانة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-120">In the **Trade** field, enter **HVAC** as a title to help identify the maintenance job trade.</span></span>
3.  <span data-ttu-id="2cb99-121">في حقل **الوصف**، أدخل **التسخين، التهوية، تكييف الهواء** كوصف تجاري.</span><span class="sxs-lookup"><span data-stu-id="2cb99-121">In the **Description** field, enter **Heating, ventilation, air conditioning** as the trade description.</span></span> 
4.  <span data-ttu-id="2cb99-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-122">Select **Save**.</span></span>

## <a name="create-a-maintenance-job-type"></a><span data-ttu-id="2cb99-123">إنشاء نوع مهمة الصيانة</span><span class="sxs-lookup"><span data-stu-id="2cb99-123">Create a maintenance job type</span></span>
<span data-ttu-id="2cb99-124">وبسبب أنواع الماكينات المستخدمة في إنتاج منتجاتها، فان Munson’s Pickles and Preserves Farm قد قررت أنها تحتاج إلى فئة نوع وظيفة مسماة **المعايرة** التي تمت إضافتها بحيث يمكنها تجميع أنواع الوظائف هذه وتعقبها.</span><span class="sxs-lookup"><span data-stu-id="2cb99-124">Because of the types of machinery that are used in the production of their product, Munson’s Pickles and Preserves Farm has decided that they need a job type category named **Calibration** added so they can group and track these job types.</span></span>

1. <span data-ttu-id="2cb99-125">انتقل إلى **إدارة الأصول > الإعداد > المهام > أنواع مهام الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-125">Go to **Asset Management > Setup > Jobs > Maintenance job types**.</span></span>
1.  <span data-ttu-id="2cb99-126">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-126">Select **New**.</span></span>
2.  <span data-ttu-id="2cb99-127">في الحقل **نوع مهمة الصيانة**، أدخل **المعايرة** كعنوان للمساعدة في تحديد نوع مهمة الصيانة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-127">In the **Maintenance job type** field, enter **Calibration** as the title to help identify the maintenance job type.</span></span> 
3.  <span data-ttu-id="2cb99-128">في الحقل **الاسم**، أدخل **المعايرة** كاسم وصفي لنوع مهمة الصيانة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-128">In the **Name** field, enter **Calibration** as a descriptive name for the maintenance job type.</span></span>
4.  <span data-ttu-id="2cb99-129">في علامة التبويب السريعة **عام**:</span><span class="sxs-lookup"><span data-stu-id="2cb99-129">On the **General** FastTab:</span></span>
    - <span data-ttu-id="2cb99-130">في الحقل **فئة نوع مهمة الصيانة**، حدد **وقائي** من القائمة المنسدلة **فئة نوع مهمة الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-130">In the **Maintenance job type category** field, select **Preventive** from the **Maintenance job type category** drop-down menu.</span></span>
    - <span data-ttu-id="2cb99-131">في الحقل **أنشطة تعطل الصيانة**، قم بتبديل زر التبديل إلى **نعم** لتعيين نوع مهمة الصيانة **متوقف** لكي يتم تنفيذ الوظيفة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-131">In the **Maintenance downtime activities** field, switch the toggle button to **Yes** to set the maintenance job type to **Stopped** for the job to be performed.</span></span>
5.  <span data-ttu-id="2cb99-132">في علامة التبويب السريعة **الوصف**، أدخل **معدات المعايرة** كوصف.</span><span class="sxs-lookup"><span data-stu-id="2cb99-132">On the **Description** FastTab, enter **Calibrate equipment** as a description.</span></span>
6.  <span data-ttu-id="2cb99-133">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-133">Select **Save**.</span></span> 
    
<span data-ttu-id="2cb99-134">يتم سرد نوع مهمة صيانة **المعايرة** في القائمة الموجودة علي اليسار ويحتوي على فئة نوع مهمة الصيانة **الوقائية** التي يتم عرضها تحته.</span><span class="sxs-lookup"><span data-stu-id="2cb99-134">The **Calibration** maintenance job type is listed in the menu at the left and has the Maintenance job type category of **Preventive** displayed underneath it.</span></span>

## <a name="create-a-service-level"></a><span data-ttu-id="2cb99-135">إنشاء مستوى خدمة</span><span class="sxs-lookup"><span data-stu-id="2cb99-135">Create a service level</span></span>
<span data-ttu-id="2cb99-136">تحدد مستويات الخدمة أولوية طلب أمر العمل وتأثيره على المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-136">Service levels define the priority of the work order request and its impact to the organization.</span></span> <span data-ttu-id="2cb99-137">وتقوم Munson’s Pickles and Preserves Farm بتأسيس معظم مستويات الخدمة، لكنهم يحتاجون إلى تعيين مستوى خدمة منخفض لتعقب أوامر العمل الأصغر.</span><span class="sxs-lookup"><span data-stu-id="2cb99-137">Munson’s Pickles and Preserves Farm has most of their service levels established, but they do need a low service level assignment to track smaller work orders.</span></span> 

1.  <span data-ttu-id="2cb99-138">انتقل إلى **إدارة الأصول > الإعداد > أوامر العمل > مستوى الخدمة**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-138">Go to **Asset Management > Setup > Work orders > Service level**.</span></span>
2.  <span data-ttu-id="2cb99-139">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-139">Select **New**.</span></span>
3.  <span data-ttu-id="2cb99-140">في الحقل **مستوى الخدمة**، أدخل **5** كقيمة لمستوى الخدمة.</span><span class="sxs-lookup"><span data-stu-id="2cb99-140">In the **Service level** field, enter **5** as the service level.</span></span>
4.  <span data-ttu-id="2cb99-141">في حقل **الاسم**، أدخل **منخفض** كاسم وصفي.</span><span class="sxs-lookup"><span data-stu-id="2cb99-141">In the **Name** field, enter **Low** as a descriptive name.</span></span>
5.  <span data-ttu-id="2cb99-142">في الحقل **يوم البدء**، أدخل عدد الأيام التي يجب أن يبدأ فيها أمر العمل عند إنشاء أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="2cb99-142">In the **Start day** field, enter the number of days that the work order should start when a work order is created.</span></span> <span data-ttu-id="2cb99-143">أدخل **3** لتبدأ خلال أيام العمل العديدة التالية.</span><span class="sxs-lookup"><span data-stu-id="2cb99-143">Enter **3** to start the within the next several workdays.</span></span>
6.  <span data-ttu-id="2cb99-144">في الحقل **يوم الانتهاء**، أدخل **2** إلى الحالة التي توضح أن العمل سيستغرق يومين لإكماله.</span><span class="sxs-lookup"><span data-stu-id="2cb99-144">In the **End day** field, enter **2** to state that the work will take two workdays to complete.</span></span>
7.  <span data-ttu-id="2cb99-145">اترك الحقل **تعيين وقت الانتهاء** معيناً على **لا**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-145">Leave the **Set end time** field set as **No**.</span></span>
8.  <span data-ttu-id="2cb99-146">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-146">Select **Save**.</span></span>

## <a name="set-up-the-fault-designer"></a><span data-ttu-id="2cb99-147">اعداد مصمم الأخطاء</span><span class="sxs-lookup"><span data-stu-id="2cb99-147">Set up the fault designer</span></span>
<span data-ttu-id="2cb99-148">وتستخدم Munson’s Pickles and Preserves Farm أجهزة المزج لمزج المواد الحافظة الخاصة بها، والتي قد تتسبب في تآكل وبلى الشفرات.</span><span class="sxs-lookup"><span data-stu-id="2cb99-148">Munson’s Pickles and Preserves Farm uses blenders to mix their preserves, which when used a lot ,can cause wear and tear on the blades.</span></span> <span data-ttu-id="2cb99-149">المهمة التالية هي إعداد أعراض الخطأ ومنطقة الخطأ ونوع الخطأ في مصمم الأخطاء لجهاز المزج.</span><span class="sxs-lookup"><span data-stu-id="2cb99-149">Your next task is to set up the fault symptoms, fault area, and fault type in the fault designer for the blender.</span></span> 

1.  <span data-ttu-id="2cb99-150">انتقل إلى **إدارة الأصول > الإعداد > الخطأ > مصمم الخطأ**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-150">Go to **Asset management > Setup > Fault > Fault designer**.</span></span>
2.  <span data-ttu-id="2cb99-151">في الجزء الأيمن، حدد **المازج**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-151">In the left pane, select **Blender**.</span></span>
3.  <span data-ttu-id="2cb99-152">في علامة التبويب السريعة **عرض الخطأ**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-152">On the **Fault symptom** FastTab, select **Add line**.</span></span>
4.  <span data-ttu-id="2cb99-153">في الحقل **عرض الخطأ**، حدد **الضوضاء الزائدة** كعرض خطأ.</span><span class="sxs-lookup"><span data-stu-id="2cb99-153">In the **Fault symptom** field, select **Excessive noise** as the fault symptom.</span></span>
5.  <span data-ttu-id="2cb99-154">قم بتوسيع علامة التبويب السريعة **منطقة الخطأ** وحدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-154">Expand the **Fault area** FastTab and select **Add line**.</span></span>
6.  <span data-ttu-id="2cb99-155">في الحقل **منطقة الخطأ**، حدد منطقة الخطأ **الميكانيكي**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-155">In the **Fault area** field, select the **Mechanical** fault area.</span></span>
7.  <span data-ttu-id="2cb99-156">قم بتوسيع علامة التبويب السريعة **نوع الخطأ** وحدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-156">Expand the **Fault type** FastTab and select **Add line**.</span></span>
8.  <span data-ttu-id="2cb99-157">في الحقل **نوع الخطأ**، حدد نوع الخطأ **تلف**.</span><span class="sxs-lookup"><span data-stu-id="2cb99-157">In the **Fault type** field, select the **Damaging** fault type.</span></span>
9.  <span data-ttu-id="2cb99-158">حدد **حفظ** لحفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="2cb99-158">Select **Save** to save your changes.</span></span>

