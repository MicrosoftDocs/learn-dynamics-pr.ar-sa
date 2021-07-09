---
ms.openlocfilehash: 46834af8078ecb63f9cc3dbad315c6e72f31836f
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073499"
---
<span data-ttu-id="6373a-101">في شركة **USMF**، تم استلام أمر مبيعات للمنتج L0001‏، مكبر_الصوت_متوسط_المدى_2.</span><span class="sxs-lookup"><span data-stu-id="6373a-101">In the **USMF** company, a sales order has been received for product L0001, MidRangeSpeaker2.</span></span> <span data-ttu-id="6373a-102">أدى أمر المبيعات إلى تشغيل بطاقات كانبان للحدث لمكبر_الصوت_متوسط_المدى_2 في خلية عمل التغليف والتعبئة ومجموعة مواد مكبر الصوت في خلية عمل تجميع مكبرات الصوت.</span><span class="sxs-lookup"><span data-stu-id="6373a-102">The sales order has triggered event kanbans for the MidRangeSpeaker2 on the packaging work cell and the speaker kits on the speaker assembly work cell.</span></span> 

<span data-ttu-id="6373a-103">عليك إنتاج مجموعات مواد مكبر الصوت وأجهزة مكبرات الصوت لتنفيذ أمر مبيعات العميل.</span><span class="sxs-lookup"><span data-stu-id="6373a-103">Produce the speaker kits and speaker set to fulfill the customer sales order.</span></span>

## <a name="create-a-sales-order"></a><span data-ttu-id="6373a-104">إنشاء أمر مبيعات</span><span class="sxs-lookup"><span data-stu-id="6373a-104">Create a sales order</span></span>

1.  <span data-ttu-id="6373a-105">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="6373a-105">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>

2.  <span data-ttu-id="6373a-106">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="6373a-106">Select **New**.</span></span>

3.  <span data-ttu-id="6373a-107">في الحقل **حساب العميل**، أدخل أو حدد **US-003**.</span><span class="sxs-lookup"><span data-stu-id="6373a-107">In the **Customer account** field, enter or select **US-003**.</span></span>

4.  <span data-ttu-id="6373a-108">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="6373a-108">Select **OK**.</span></span>

5.  <span data-ttu-id="6373a-109">في الحقل **رقم الصنف**، أدخل أو حدد **L0001**.</span><span class="sxs-lookup"><span data-stu-id="6373a-109">In the **Item number** field, enter or select **L0001**.</span></span>

6.  <span data-ttu-id="6373a-110">في القائمة، حدد الارتباط في الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="6373a-110">In the list, select the link in the selected row.</span></span>

7.  <span data-ttu-id="6373a-111">قم بتعيين **الكمية** إلى **1.00**.</span><span class="sxs-lookup"><span data-stu-id="6373a-111">Set the **Quantity** to **1.00**.</span></span>

8.  <span data-ttu-id="6373a-112">حدد **المنتج والتوريد**.</span><span class="sxs-lookup"><span data-stu-id="6373a-112">Select **Product and supply**.</span></span>

9.  <span data-ttu-id="6373a-113">حدد **كانبان الحدث**.</span><span class="sxs-lookup"><span data-stu-id="6373a-113">Select **Event kanban**.</span></span>

10. <span data-ttu-id="6373a-114">حدد **المنتج والتوريد**.</span><span class="sxs-lookup"><span data-stu-id="6373a-114">Select **Product and supply**.</span></span>

11. <span data-ttu-id="6373a-115">حدد **عرض شجرة تثبيت السعر**.</span><span class="sxs-lookup"><span data-stu-id="6373a-115">Select **View pegging tree**.</span></span>

12. <span data-ttu-id="6373a-116">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="6373a-116">Close the page.</span></span>


## <a name="plan-the-kanbans"></a><span data-ttu-id="6373a-117">تخطيط كانبان</span><span class="sxs-lookup"><span data-stu-id="6373a-117">Plan the kanbans</span></span>

1.  <span data-ttu-id="6373a-118">انتقل إلى **التحكم بالإنتاج > كانبان > جدولة وظيفة كانبان**.</span><span class="sxs-lookup"><span data-stu-id="6373a-118">Go to **Production control > Kanban > Kanban job scheduling**.</span></span>

2.  <span data-ttu-id="6373a-119">حدد **تخطيط شجرة تثبيت السعر بالكامل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-119">Select **Plan entire pegging tree**.</span></span>

3.  <span data-ttu-id="6373a-120">حدد بضعة صفوف لحلول كانبان غير المخططة.</span><span class="sxs-lookup"><span data-stu-id="6373a-120">Select a few rows for those unplanned kanbans.</span></span>

4.  <span data-ttu-id="6373a-121">حدد **تخطيط شجرة تثبيت السعر بالكامل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-121">Select **Plan entire pegging tree**.</span></span>

5.  <span data-ttu-id="6373a-122">في الحقل **خلية عمل**، أدخل أو حدد **1250‎**.</span><span class="sxs-lookup"><span data-stu-id="6373a-122">In the **Work cell** field, enter or select **1250**.</span></span>

6.  <span data-ttu-id="6373a-123">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="6373a-123">Close the page.</span></span>

## <a name="process-jobs"></a><span data-ttu-id="6373a-124">مهام المعالجة</span><span class="sxs-lookup"><span data-stu-id="6373a-124">Process jobs</span></span>

1.  <span data-ttu-id="6373a-125">انتقل إلى **التحكم بالإنتاج > كانبان > لوحة كانبان لوظائف المعالجة**.</span><span class="sxs-lookup"><span data-stu-id="6373a-125">Go to **Production control > Kanban > Kanban board for process jobs**.</span></span>

2.  <span data-ttu-id="6373a-126">في الحقل **خلية عمل**، أدخل أو حدد **1250‎**.</span><span class="sxs-lookup"><span data-stu-id="6373a-126">In the **Work cell** field, enter or select **1250**.</span></span>

3.  <span data-ttu-id="6373a-127">حدد عدداً قليلاً من الصفوف لحلول كانبان المخططة هذه.</span><span class="sxs-lookup"><span data-stu-id="6373a-127">Select a few rows for those planned kanbans.</span></span>

4.  <span data-ttu-id="6373a-128">حدد **تحضير**.</span><span class="sxs-lookup"><span data-stu-id="6373a-128">Select **Prepare**.</span></span>

5.  <span data-ttu-id="6373a-129">قم بتوسيع قسم **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-129">Expand the **Details** section.</span></span> <span data-ttu-id="6373a-130">راجع التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="6373a-130">Note the details.</span></span>

6.  <span data-ttu-id="6373a-131">قم بطي قسم **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-131">Collapse the **Details** section.</span></span>

7.  <span data-ttu-id="6373a-132">قم بتوسيع قسم **قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-132">Expand the **Picking list** section.</span></span> <span data-ttu-id="6373a-133">راجع المواد الخام مطلوبة.</span><span class="sxs-lookup"><span data-stu-id="6373a-133">Note the raw materials needed.</span></span>

8.  <span data-ttu-id="6373a-134">حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-134">Select **Start**.</span></span>

9.  <span data-ttu-id="6373a-135">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="6373a-135">Select **Complete**.</span></span>

10. <span data-ttu-id="6373a-136">في جزء الإجراء، حدد **عرض**.</span><span class="sxs-lookup"><span data-stu-id="6373a-136">On the Action Pane, select **View**.</span></span>

11. <span data-ttu-id="6373a-137">حدد **قائمة مهام العملية**.</span><span class="sxs-lookup"><span data-stu-id="6373a-137">Select **Process job list**.</span></span>

12. <span data-ttu-id="6373a-138">حدد خانة الاختيار **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="6373a-138">Select the **Site** check box.</span></span>

13. <span data-ttu-id="6373a-139">حدد خانة الاختيار **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="6373a-139">Select the **Warehouse** check box.</span></span>

14. <span data-ttu-id="6373a-140">حدد **نعم** في حقل **حفظ الإعداد**.</span><span class="sxs-lookup"><span data-stu-id="6373a-140">Select **Yes** in the **Save setup** field.</span></span>

15. <span data-ttu-id="6373a-141">حدد خانة الاختيار **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="6373a-141">Select the **Location** check box.</span></span>

16. <span data-ttu-id="6373a-142">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="6373a-142">Select **OK**.</span></span>

17. <span data-ttu-id="6373a-143">حدد مهمة مخططة.</span><span class="sxs-lookup"><span data-stu-id="6373a-143">Select a planned job.</span></span>

18. <span data-ttu-id="6373a-144">في جزء الإجراء، حدد **انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-144">On the Action Pane, select **Pick**.</span></span>

19. <span data-ttu-id="6373a-145">حدد **تحديث قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-145">Select **Update picking list**.</span></span>

20. <span data-ttu-id="6373a-146">حدد **إضافة بند الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-146">Select **Add picking line**.</span></span>

21. <span data-ttu-id="6373a-147">حدد **تأكيد انتقاء الكل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-147">Select **Confirm pick all**.</span></span>

22. <span data-ttu-id="6373a-148">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="6373a-148">Close all pages.</span></span>

## <a name="perform-transfers"></a><span data-ttu-id="6373a-149">إجراء التحويلات</span><span class="sxs-lookup"><span data-stu-id="6373a-149">Perform transfers</span></span>

1.  <span data-ttu-id="6373a-150">انتقل إلى **التحكم بالإنتاج > كانبان > لوحة كانبان لمهام التحويل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-150">Go to **Production control > Kanban > Kanban board for transfer jobs**.</span></span>

2.  <span data-ttu-id="6373a-151">حدد مهمة لبدء التحويل.</span><span class="sxs-lookup"><span data-stu-id="6373a-151">Select a job to start the transfer.</span></span> 

3.  <span data-ttu-id="6373a-152">حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-152">Select **Start**.</span></span>

3.  <span data-ttu-id="6373a-153">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="6373a-153">Select **Complete**.</span></span>

4.  <span data-ttu-id="6373a-154">في جزء الإجراء، حدد **تحويل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-154">On the Action Pane, select **Transfer**.</span></span>

5.  <span data-ttu-id="6373a-155">حدد عدداً قليلاً من الصفوف لبدء التحويل لهذه المهام.</span><span class="sxs-lookup"><span data-stu-id="6373a-155">Select a few rows for those jobs to start transfer.</span></span> 

6.  <span data-ttu-id="6373a-156">حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-156">Select **Start**.</span></span>

6.  <span data-ttu-id="6373a-157">في جزء الإجراء، حدد **تحويل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-157">On the Action Pane, select **Transfer**.</span></span>

7.  <span data-ttu-id="6373a-158">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="6373a-158">Select **Complete**.</span></span>

7.  <span data-ttu-id="6373a-159">حدد **تحديث قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-159">Select **Update picking list**.</span></span>

8.  <span data-ttu-id="6373a-160">حدد **إضافة بند الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="6373a-160">Select **Add picking line**.</span></span>

9.  <span data-ttu-id="6373a-161">حدد **تأكيد انتقاء الكل**.</span><span class="sxs-lookup"><span data-stu-id="6373a-161">Select **Confirm pick all**.</span></span>

10. <span data-ttu-id="6373a-162">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="6373a-162">Close all pages.</span></span> 
