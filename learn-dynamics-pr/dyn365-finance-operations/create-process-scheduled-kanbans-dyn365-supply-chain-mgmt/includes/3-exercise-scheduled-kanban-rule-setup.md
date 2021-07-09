---
ms.openlocfilehash: cda11d9cff958b6d5625786e7539069150c58b2f
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073112"
---
## <a name="before-you-begin"></a><span data-ttu-id="42487-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="42487-101">Before you begin</span></span> 
<span data-ttu-id="42487-102">للحصول على أقصى استفادة من هذا التدريب، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Supply Chain Management والتي يتم تثبيتها باستخدام Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="42487-102">To get the most benefit from this exercise, we recommend that you have the standard sample data available in Dynamics 365 Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

## <a name="scenario"></a><span data-ttu-id="42487-103">السيناريو</span><span class="sxs-lookup"><span data-stu-id="42487-103">Scenario</span></span> 

<span data-ttu-id="42487-104">قررت شركة USMF أنه سيتم تخطيط منتج برنامج راديو شبكة اتصال لاسلكية L0025 من جدول إنتاج ينتج من تشغيل تخطيط رئيسي.</span><span class="sxs-lookup"><span data-stu-id="42487-104">The company USMF has decided that the L0025 WLAN Radio software product is going to be planned off of a production schedule that results from a master planning run.</span></span>

## <a name="configure-item-coverage"></a><span data-ttu-id="42487-105">تكوين تغطية الصنف</span><span class="sxs-lookup"><span data-stu-id="42487-105">Configure item coverage</span></span> 

1.  <span data-ttu-id="42487-106">انتقل إلى **التخطيط الرئيسي > الإعداد > تغطية الصنف**.</span><span class="sxs-lookup"><span data-stu-id="42487-106">Go to **Master planning > Setup > Item coverage**.</span></span>

2.  <span data-ttu-id="42487-107">استخدم مربع بحث **عامل التصفية** للتصفية في حقل **رقم الصنف** بقيمة **L0025**.</span><span class="sxs-lookup"><span data-stu-id="42487-107">Use the **Filter** search box to filter on the **Item number** field with a value of **L0025**.</span></span>

3.  <span data-ttu-id="42487-108">حدد **تغطية الصنف** في القائمة العليا.</span><span class="sxs-lookup"><span data-stu-id="42487-108">Select **Item coverage** in the top menu.</span></span>

4.  <span data-ttu-id="42487-109">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="42487-109">Select **New**.</span></span>

5.  <span data-ttu-id="42487-110">عيّن **الحد الأدنى** إلى **150.00**.</span><span class="sxs-lookup"><span data-stu-id="42487-110">Set **Minimum** to **150.00**.</span></span>

6.  <span data-ttu-id="42487-111">في حقل **المستودع**، أدخل أو حدد **13**.</span><span class="sxs-lookup"><span data-stu-id="42487-111">In the **Warehouse** field, enter or select **13**.</span></span>

7.  <span data-ttu-id="42487-112">حدد علامة التبويب **عام**.</span><span class="sxs-lookup"><span data-stu-id="42487-112">Select the **General** tab.</span></span>

8.  <span data-ttu-id="42487-113">حدد خانة الاختيار **تجاوز الحدود الزمنية**.</span><span class="sxs-lookup"><span data-stu-id="42487-113">Select the **Override time fences** check box.</span></span>

9.  <span data-ttu-id="42487-114">في حقل **الحد الزمني للتأكيد التلقائي (أيام)**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="42487-114">In the **Automatic firming time fence (days)** field, enter **1**.</span></span>

10. <span data-ttu-id="42487-115">حدد علامة التبويب **وقت الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="42487-115">Select the **Lead time** tab.</span></span>

11. <span data-ttu-id="42487-116">حدد خانة الاختيار **الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="42487-116">Select the **Production** check box.</span></span>

12. <span data-ttu-id="42487-117">في حقل **وقت الإنتاج**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="42487-117">In the **Production time** field, enter **1**.</span></span>

13. <span data-ttu-id="42487-118">حدد **نعم** في حقل **أيام العمل**.</span><span class="sxs-lookup"><span data-stu-id="42487-118">Select **Yes** in the **Working days** field.</span></span>

14. <span data-ttu-id="42487-119">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="42487-119">Select **Save**.</span></span>

15. <span data-ttu-id="42487-120">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="42487-120">Close all pages.</span></span>

## <a name="create-a-scheduled-kanban-rule"></a><span data-ttu-id="42487-121">إنشاء قاعدة كانبان مجدولة</span><span class="sxs-lookup"><span data-stu-id="42487-121">Create a scheduled kanban rule</span></span>

1.  <span data-ttu-id="42487-122">انتقل إلى **إدارة معلومات المنتج > Lean manufacturing > قواعد كانبان**.</span><span class="sxs-lookup"><span data-stu-id="42487-122">Go to **Product information management > Lean manufacturing > Kanban rules**.</span></span>

2.  <span data-ttu-id="42487-123">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="42487-123">Select **New**.</span></span>

3.  <span data-ttu-id="42487-124">في حقل **استراتيجية التزويد**، حدد **مجدول**.</span><span class="sxs-lookup"><span data-stu-id="42487-124">In the **Replenishment strategy** field, select **Scheduled**.</span></span>

4.  <span data-ttu-id="42487-125">في حقل **نشاط الخطة الأول**، أدخل أو حدد **التجميع النهائي**.</span><span class="sxs-lookup"><span data-stu-id="42487-125">In the **First plan activity** field, enter or select **Final assembly**.</span></span>

5.  <span data-ttu-id="42487-126">قم بطي قسم **قاعدة كانبان**.</span><span class="sxs-lookup"><span data-stu-id="42487-126">Collapse the **Kanban rule** section.</span></span>

6.  <span data-ttu-id="42487-127">قم بتوسيع قسم **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="42487-127">Expand the **Details** section.</span></span>

7.  <span data-ttu-id="42487-128">في حقل **الإنتاج**، أدخل أو حدد **L0025**.</span><span class="sxs-lookup"><span data-stu-id="42487-128">In the **Product** field, enter or select **L0025**.</span></span>

8.  <span data-ttu-id="42487-129">في القائمة، حدد الارتباط في الصف المميز.</span><span class="sxs-lookup"><span data-stu-id="42487-129">In the list, select the link in the highlighted row.</span></span>

9.  <span data-ttu-id="42487-130">في حقل **التكوين**، أدخل أو حدد **01**.</span><span class="sxs-lookup"><span data-stu-id="42487-130">In the **Configuration** field, enter or select **01**.</span></span>

10. <span data-ttu-id="42487-131">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="42487-131">Select **Save**.</span></span>

11. <span data-ttu-id="42487-132">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="42487-132">Close the page.</span></span>

## <a name="run-master-planning"></a><span data-ttu-id="42487-133">تشغيل التخطيط الرئيسي</span><span class="sxs-lookup"><span data-stu-id="42487-133">Run master planning</span></span>

1.  <span data-ttu-id="42487-134">انتقل إلى **التخطيط الرئيسي > التخطيط الرئيسي > تشغيل > تخطيط رئيسي**.</span><span class="sxs-lookup"><span data-stu-id="42487-134">Go to **Master planning > Master planning > Run > Master planning**.</span></span>

2.  <span data-ttu-id="42487-135">في حقل **الخطة الرئيسية**، أدخل أو حدد **DynPlan**.</span><span class="sxs-lookup"><span data-stu-id="42487-135">In the **Master plan** field, enter or select **DynPlan**.</span></span>

3.  <span data-ttu-id="42487-136">قم بتوسيع قسم **السجلات المطلوب تضمينها**.</span><span class="sxs-lookup"><span data-stu-id="42487-136">Expand the **Records to include** section.</span></span>

4.  <span data-ttu-id="42487-137">حدد **عامل تصفية**.</span><span class="sxs-lookup"><span data-stu-id="42487-137">Select **Filter**.</span></span>

5.  <span data-ttu-id="42487-138">في الحقل **المعايير**، أدخل **L0025**.</span><span class="sxs-lookup"><span data-stu-id="42487-138">In the **Criteria** field, enter **L0025**.</span></span>

6.  <span data-ttu-id="42487-139">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="42487-139">Select **OK**.</span></span>

7.  <span data-ttu-id="42487-140">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="42487-140">Select **OK**.</span></span>


1.  <span data-ttu-id="42487-141">افتح **التخطيط الرئيسي > التخطيط الرئيسي > الأوامر المخططة**.</span><span class="sxs-lookup"><span data-stu-id="42487-141">Go to **Master planning > Master planning > Planned orders**.</span></span>

2.  <span data-ttu-id="42487-142">في حقل **عامل التصفية السريع**، أدخل قيمة **L0025** كـ **رقم الصنف**، ثم اضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="42487-142">In the **Quick filter** field, enter a value of **L0025** as the **Item number** and then press **Enter**.</span></span>

3.  <span data-ttu-id="42487-143">مراجعة بطاقات كانبان المخططة لـ L0025.</span><span class="sxs-lookup"><span data-stu-id="42487-143">Review planned kanbans for L0025.</span></span>

4.  <span data-ttu-id="42487-144">حدد البند الذي يحتوي على الكمية **150**.</span><span class="sxs-lookup"><span data-stu-id="42487-144">Select the line with the quantity of **150**.</span></span>

5.  <span data-ttu-id="42487-145">حدد **جدول التوريد**.</span><span class="sxs-lookup"><span data-stu-id="42487-145">Select **Supply schedule**.</span></span>

6.  <span data-ttu-id="42487-146">تحقق من نتائج بطاقات كانبان التي تم إنشاؤها بواسطة التخطيط الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="42487-146">Verify the results of the kanbans that were generated by Master planning.</span></span>
 
