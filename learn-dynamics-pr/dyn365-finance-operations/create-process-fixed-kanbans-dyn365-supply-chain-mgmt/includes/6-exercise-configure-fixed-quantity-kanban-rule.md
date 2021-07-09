---
ms.openlocfilehash: b5ca5f22209d9ad7243f29003608dc739cc37855
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073493"
---
## <a name="before-you-begin"></a><span data-ttu-id="df9a9-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="df9a9-101">Before you begin</span></span>
<span data-ttu-id="df9a9-102">للحصول على أقصى استفادة من هذا التدريب وغيره من التدريبات الأخرى في هذه الوحدة، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Supply Chain Management والتي يتم تثبيتها باستخدام Lifecycle Services ‏(LCS).</span><span class="sxs-lookup"><span data-stu-id="df9a9-102">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data available in Dynamics 365 Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

## <a name="scenario"></a><span data-ttu-id="df9a9-103">السيناريو</span><span class="sxs-lookup"><span data-stu-id="df9a9-103">Scenario</span></span>

<span data-ttu-id="df9a9-104">تم تطوير جهاز تحكم عن بعد جديد لمكبرات الصوت للسيارة لاستكمال مجموعات مكبرات صوت السيارة التي تُباع في **USMF**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-104">A new car speaker remote has been developed to complement the car speaker kits that are sold at **USMF**.</span></span> <span data-ttu-id="df9a9-105">تم تكوين سير مهام الإنتاج بالفعل مع أنشطة متعددة والآن يجب إنشاء المنتجات ووحدات كانبان المطلوبة لمعالجة سير المهام.</span><span class="sxs-lookup"><span data-stu-id="df9a9-105">The production flow is already configured with multiple activities and now the products and kanbans that are required to process the flow must be created.</span></span>

<span data-ttu-id="df9a9-106">تم إعداد المنتجات لجهاز التحكم عن بُعد الذي تم شراؤه وغير المبرمج ولجهاز التحكم عن بُعد الذي سيتم برمجته من خلال أنشطة سير مهام الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="df9a9-106">Products have been set up for the purchased unprogrammed remote and for the remote that will be programmed through the activities of the production flow.</span></span> <span data-ttu-id="df9a9-107">تم أيضاً إنشاء قائمة مكونات الصنف (BOM)، مع إضافة وحدة التحكم عن بُعد المشتراة غير المبرمجة كبند قائمة مكونات صنف.</span><span class="sxs-lookup"><span data-stu-id="df9a9-107">The bill of material (BOM) has also been created, adding the purchased unprogrammed remote as a BOM line.</span></span>

<span data-ttu-id="df9a9-108">بعد إنشاء قائمة مكونات الصنف، يتم إعداد قواعد كانبان لنشاط العملية لبرمجة جهاز التحكم عن بُعد ولنشاط النقل لنقل وحدة التحكم عن بُعد المبرمجة (أصبحت الآن سلعة منتهية) إلى المستودع والموقع حيث سيتم تخزينها حتى يتم بيعها.</span><span class="sxs-lookup"><span data-stu-id="df9a9-108">After the BOM has been created, kanban rules are set up for the process activity to program the remote and for the transfer activity to transfer the programmed remote (now a finished good) to the warehouse and location where it will be stored until it is sold.</span></span>

## <a name="create-the-kanban-rule-for-the-process-activity"></a><span data-ttu-id="df9a9-109">إنشاء قاعدة كانبان لنشاط العملية</span><span class="sxs-lookup"><span data-stu-id="df9a9-109">Create the kanban rule for the process activity</span></span>

1.  <span data-ttu-id="df9a9-110">لإنشاء قاعدة كانبان جديدة لنشاط العملية، انتقل إلى **إدارة معلومات المنتج> Lean manufacturing> قواعد كانبان**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-110">To create a new kanban rule for the process activity, go to **Product information management > Lean manufacturing > Kanban rules**.</span></span>

2.  <span data-ttu-id="df9a9-111">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-111">Select **New**.</span></span>

3.  <span data-ttu-id="df9a9-112">حدد **نشاط الخطة الأول** المسمى **SpeakerTestAndPackaging**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-112">Select the **First plan activity** called **SpeakerTestAndPackaging**.</span></span>

4.  <span data-ttu-id="df9a9-113">قم بتوسيع علامة التبويب السريعة **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-113">Expand the **Details** FastTab.</span></span>

5.  <span data-ttu-id="df9a9-114">في حقل **المنتج**، حدد **L0001**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-114">In the **Product** field, select **L0001**.</span></span>

6.  <span data-ttu-id="df9a9-115">قم بتوسيع علامة التبويب السريعة **الكميات**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-115">Expand the **Quantities** FastTab.</span></span>

7.  <span data-ttu-id="df9a9-116">أدخل **الكمية الافتراضية** البالغة **100**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-116">Enter a **Default quantity** of **100**.</span></span>

8.  <span data-ttu-id="df9a9-117">أدخل **كمية كانبان الثابتة** البالغة **4**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-117">Enter a **Fixed Kanban quantity** of **4**.</span></span>

9.  <span data-ttu-id="df9a9-118">قم بتوسيع علامة التبويب السريعة **كانبان والبطاقات**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-118">Expand the **Kanban and cards** FastTab.</span></span>

10. <span data-ttu-id="df9a9-119">حدد خانة الاختيار **البطاقات المتداولة**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-119">Select the **Circulating cards** check box.</span></span>

11. <span data-ttu-id="df9a9-120">قم بتغيير **تعيين البطاقة** إلى **تلقائي**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-120">Change the **Card assignment** to **Automatic**.</span></span>

12. <span data-ttu-id="df9a9-121">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-121">Select **Save**.</span></span>

13. <span data-ttu-id="df9a9-122">حدد زر **إنشاء البطاقات**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-122">Select the **Create cards** button.</span></span>

14. <span data-ttu-id="df9a9-123">قم بإلغاء تحديد خانة الاختيار **طباعة البطاقات الجديدة**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-123">Clear the **Print new cards** check box.</span></span>

15. <span data-ttu-id="df9a9-124">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-124">Select **Create**.</span></span>

16. <span data-ttu-id="df9a9-125">قم بالتبديل إلى علامة التبويب السريعة **وحدات كانبان**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-125">Switch to the **Kanbans** FastTab.</span></span>

17. <span data-ttu-id="df9a9-126">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-126">Select **Add**.</span></span>

18. <span data-ttu-id="df9a9-127">تحقق من أن العدد الافتراضي لوحدات كانبان الجديدة هو **4**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-127">Verify that the default number of new kanbans is **4**.</span></span>

19. <span data-ttu-id="df9a9-128">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-128">Select **Create**.</span></span>

20. <span data-ttu-id="df9a9-129">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="df9a9-129">Close all pages.</span></span>

## <a name="create-the-kanban-rule-for-the-transfer-activity"></a><span data-ttu-id="df9a9-130">إنشاء قاعدة كانبان لنشاط التحويل</span><span class="sxs-lookup"><span data-stu-id="df9a9-130">Create the kanban rule for the transfer activity</span></span>


1.  <span data-ttu-id="df9a9-131">لإنشاء قاعدة كانبان جديدة لنشاط التحويل، انتقل إلى **إدارة معلومات المنتج> Lean manufacturing> قواعد كانبان**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-131">To create a new kanban rule for the transfer activity, go to **Product information management > Lean manufacturing > Kanban rules**.</span></span>

2.  <span data-ttu-id="df9a9-132">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-132">Select **New**.</span></span>

3.  <span data-ttu-id="df9a9-133">قم بتغيير **النوع** إلى **السحب**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-133">Change the **Type** to **Withdrawal**.</span></span>

4.  <span data-ttu-id="df9a9-134">قم بتحديث **نشاط الخطة الأول** إلى **ReplenishSpeakerComponents**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-134">Update the **First plan activity** to **ReplenishSpeakerComponents**.</span></span>

5.  <span data-ttu-id="df9a9-135">قم بتوسيع علامة التبويب السريعة **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-135">Expand the **Details** FastTab.</span></span>

6.  <span data-ttu-id="df9a9-136">أدخل **L0001** باعتباره **المنتج**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-136">Enter **L0001** as the **Product**.</span></span>

7.  <span data-ttu-id="df9a9-137">قم بالتبديل إلى علامة التبويب السريعة **الكميات**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-137">Switch to the **Quantities** FastTab.</span></span>

8.  <span data-ttu-id="df9a9-138">أدخل **الكمية الافتراضية** البالغة **10**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-138">Enter the **Default quantity** of **10**.</span></span>

9.  <span data-ttu-id="df9a9-139">أدخل **كمية كانبان الثابتة** البالغة **4**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-139">Enter the **Fixed Kanban quantity** of **4**.</span></span>

10. <span data-ttu-id="df9a9-140">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-140">Select **Save**.</span></span>

11. <span data-ttu-id="df9a9-141">قم بالتبديل إلى علامة التبويب السريعة **وحدات كانبان**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-141">Switch to the **Kanbans** FastTab.</span></span>

12. <span data-ttu-id="df9a9-142">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-142">Select **Add**.</span></span>

13. <span data-ttu-id="df9a9-143">تحقق من أن عدد وظائف كانبان الجديدة افتراضياً هو **4**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-143">Verify that the number of new kanbans defaults to **4**.</span></span>

14. <span data-ttu-id="df9a9-144">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-144">Select **Create**.</span></span>

15. <span data-ttu-id="df9a9-145">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="df9a9-145">Close all pages.</span></span>

## <a name="plan-a-kanban-on-the-kanban-schedule-board"></a><span data-ttu-id="df9a9-146">تخطيط كانبان على لوحة جدولة كانبان</span><span class="sxs-lookup"><span data-stu-id="df9a9-146">Plan a kanban on the Kanban schedule board</span></span>

<span data-ttu-id="df9a9-147">عندما لا يتم التخطيط لوظائف كانبان تلقائياً، يجب سحبها وإفلاتها في الفترة المطلوبة على لوحة جدولة كانبان.</span><span class="sxs-lookup"><span data-stu-id="df9a9-147">When the kanban jobs are not automatically planned, they must be dragged and dropped onto the desired period on the Kanban schedule board.</span></span>

1.  <span data-ttu-id="df9a9-148">لتخطيط الكانبان، انتقل إلى **التحكم في الإنتاج > كانبان > جدولة وظيفة كانبان**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-148">To plan the kanban, go to **Production control > Kanban > Kanban job scheduling**.</span></span>

2.  <span data-ttu-id="df9a9-149">قم بتغيير **خلية العمل** إلى **1250**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-149">Change **Work cell** to **1250**.</span></span>

3.  <span data-ttu-id="df9a9-150">في حقل **عرض حالة الوظيفة**، حدد **غير مجدولة**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-150">In the **Display job status** field, select **Not scheduled**.</span></span>

4.  <span data-ttu-id="df9a9-151">حدد وظيفة كانبان من وظائف كانبان غير المخطط لها، ثم حدد الزر **جدولة**.</span><span class="sxs-lookup"><span data-stu-id="df9a9-151">Select a kanban job from the unplanned kanban jobs, and then select the **Schedule** button.</span></span> <span data-ttu-id="df9a9-152">كرر ذلك مع وظائف كانبان المتبقية التي تختارها.</span><span class="sxs-lookup"><span data-stu-id="df9a9-152">Repeat for the  remaining kanban jobs of your choice.</span></span> 
