---
ms.openlocfilehash: d49cb4cbb6cfbc4f3a52cb41b1cc469790446ddc
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073564"
---
## <a name="scenario"></a><span data-ttu-id="7d926-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="7d926-101">Scenario</span></span>
<span data-ttu-id="7d926-102">في هذا المعمل، ستقوم بإنشاء قاعدة موعد جديدة وأمر مبيعات ومهمة تحميل جديدة.</span><span class="sxs-lookup"><span data-stu-id="7d926-102">In this lab you will create a new appointment rule, sales order and a new load assignment.</span></span> <span data-ttu-id="7d926-103">ستقوم أيضاً بالتدريب على تسجيل دخول سائق وإنشاء موعد فوري.</span><span class="sxs-lookup"><span data-stu-id="7d926-103">You will also practice checking in a driver and creating an instant appointment.</span></span>

## <a name="create-a-new-appointment-rule"></a><span data-ttu-id="7d926-104">إنشاء قاعدة موعد جديد</span><span class="sxs-lookup"><span data-stu-id="7d926-104">Create a new appointment rule</span></span> 

1.  <span data-ttu-id="7d926-105">في شركة USMF، افتح **إدارة النقل > إعداد > جدولة المواعيد > قواعد المواعيد**.</span><span class="sxs-lookup"><span data-stu-id="7d926-105">In company USMF, open **Transportation management > Setup > Appointment scheduling > Appointment rules**.</span></span>
2.  <span data-ttu-id="7d926-106">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7d926-106">Select **New**.</span></span>
3.  <span data-ttu-id="7d926-107">في الحقل **قاعدة الموعد**، أدخل **المستودع 62**.</span><span class="sxs-lookup"><span data-stu-id="7d926-107">In the **Appointment rule** field, enter **Warehouse 62**.</span></span>
4.  <span data-ttu-id="7d926-108">في حقل **الموقع**، حدد **6**.</span><span class="sxs-lookup"><span data-stu-id="7d926-108">In the **Site** field, select **6**.</span></span>
5.  <span data-ttu-id="7d926-109">حدد **62** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="7d926-109">In the **Warehouse** field, select **62**.</span></span>
6.  <span data-ttu-id="7d926-110">في حقل **المدة**، أدخل **30**.</span><span class="sxs-lookup"><span data-stu-id="7d926-110">In the **Duration** field, enter **30**.</span></span>
7.  <span data-ttu-id="7d926-111">في الحقل **أقصى عدد مواعيد**، أدخل **5**.</span><span class="sxs-lookup"><span data-stu-id="7d926-111">In the **Max. number of appointments** field, enter **5**.</span></span>
8.  <span data-ttu-id="7d926-112">في حقل **اتجاه حركة الصنف**، حدد **كلاهما‬**.</span><span class="sxs-lookup"><span data-stu-id="7d926-112">In the **Item movement direction** field, select **Both**.</span></span>
9.  <span data-ttu-id="7d926-113">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7d926-113">Select **Save**.</span></span>
9.  <span data-ttu-id="7d926-114">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7d926-114">Close the page.</span></span>

## <a name="create-and-pick-a-new-sales-order"></a><span data-ttu-id="7d926-115">إنشاء أمر مبيعات جديد وانتقاؤه</span><span class="sxs-lookup"><span data-stu-id="7d926-115">Create and pick a new sales order</span></span> 

1.  <span data-ttu-id="7d926-116">افتح **الحسابات المدينة > الأوامر > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="7d926-116">Open **Accounts receivable > Orders > All sales orders**.</span></span>
2.  <span data-ttu-id="7d926-117">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7d926-117">Select **New**.</span></span>
3.  <span data-ttu-id="7d926-118">في الحقل **حساب العميل**، أدخل **US-007**.</span><span class="sxs-lookup"><span data-stu-id="7d926-118">In the **Customer account** field, select **US-007**.</span></span>
4.  <span data-ttu-id="7d926-119">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7d926-119">Select **OK**.</span></span>
5.  <span data-ttu-id="7d926-120">حدد **A0001** لـ **رقم الصنف** ضمن **بنود أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="7d926-120">Select **A0001** for **Item number** on the **Sales order lines**.</span></span>
6.  <span data-ttu-id="7d926-121">في الحقل **الكمية** أدخل **3**؛ حدد **6** لـ **الموقع** و **62** لـ **المستودع**؛ أدخل **15** لـ **سعر الوحدة**.</span><span class="sxs-lookup"><span data-stu-id="7d926-121">In the **Quantity** field enter **3**; select **6** for **Site** and **62** for **Warehouse**; enter **15** for the **unit price**.</span></span>
1.  <span data-ttu-id="7d926-122">في جزء الإجراء، من الصفحة **أمر المبيعات**، حدد علامة التبويب **مستودع**.</span><span class="sxs-lookup"><span data-stu-id="7d926-122">On the **Sales order** page, select the **Warehouse** tab on the Action Pane.</span></span>
2.  <span data-ttu-id="7d926-123">في المنطقة **تحميل**، حدد **منضدة عمل إنشاء الحِمل**.</span><span class="sxs-lookup"><span data-stu-id="7d926-123">In the **Loads** area, select **Load planning workbench**.</span></span>
3.  <span data-ttu-id="7d926-124">في علامة التبويب **بنود المبيعات**، حدد البند لأمر المبيعات الحالي.</span><span class="sxs-lookup"><span data-stu-id="7d926-124">In the **Sales lines** tab, select the line for your current sales order.</span></span>
4.  <span data-ttu-id="7d926-125">في جزء الإجراء، حدد **التوريد والطلب**.</span><span class="sxs-lookup"><span data-stu-id="7d926-125">On the Action Pane, select **Supply and demand**.</span></span>
5.  <span data-ttu-id="7d926-126">في منطقة **الإضافة**، حدد **لتحميل الجديد**.</span><span class="sxs-lookup"><span data-stu-id="7d926-126">In the **Add** area, select **To new load**.</span></span>
6.  <span data-ttu-id="7d926-127">في الصفحة **مهمة قالب التحميل**، من القائمة المنسدلة **معرّف قالب التحميل**، حدد **قالب تحميل Stnd**.</span><span class="sxs-lookup"><span data-stu-id="7d926-127">On the **Load template assignment** page, select **Stnd Load Template** from the **Load template ID** drop-down menu.</span></span>
7.  <span data-ttu-id="7d926-128">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7d926-128">Select **OK**.</span></span>
8.  <span data-ttu-id="7d926-129">حدد **موافق** لتأكيد تجاوز القدرة.</span><span class="sxs-lookup"><span data-stu-id="7d926-129">Select **OK** to confirm exceeding capacity.</span></span>
11. <span data-ttu-id="7d926-130">حدد **إصدار إلى المستودع** من القائمة المنسدلة **إصدار**.</span><span class="sxs-lookup"><span data-stu-id="7d926-130">Select **Release to warehouse** from the **Release** drop-down menu.</span></span>
12. <span data-ttu-id="7d926-131">في مربع الحوار، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7d926-131">Select **OK** on the dialog box.</span></span>  

> [!Note] 
> <span data-ttu-id="7d926-132">استخدم معرّف التحميل الذي تم إنشاؤه بواسطة الخطوات السابقة كحمل العمل لتحديد باقي التدريب.</span><span class="sxs-lookup"><span data-stu-id="7d926-132">Use the Load ID that is generated by the above steps as the load to select for the rest of the exercise.</span></span>


## <a name="create-a-new-load-assignment"></a><span data-ttu-id="7d926-133">إنشاء مهمة تحميل جديدة</span><span class="sxs-lookup"><span data-stu-id="7d926-133">Create a new load assignment</span></span>
<span data-ttu-id="7d926-134">لقد تم إرشادك لإنشاء مهمة تحميل جديدة لأمر مبيعات قائم للمستودع 62.</span><span class="sxs-lookup"><span data-stu-id="7d926-134">You have been instructed to create a new load assignment for an existing sales order for Warehouse 62.</span></span>

1.  <span data-ttu-id="7d926-135">افتح **إدارة النقل > تخطيط > منضدة عمل إنشاء الحِمل**.</span><span class="sxs-lookup"><span data-stu-id="7d926-135">Open **Transportation management > Planning > Load planning workbench**.</span></span>
2.  <span data-ttu-id="7d926-136">في القسم **تحميلات**، حدد **معرّف التحميل**، الذي تم إنشاؤه سابقاً.</span><span class="sxs-lookup"><span data-stu-id="7d926-136">In the **Loads** section, select **Load ID**, which was generated earlier.</span></span>
3.  <span data-ttu-id="7d926-137">حدد **جدولة المواعيد** من القائمة المنسدلة **نقل**.</span><span class="sxs-lookup"><span data-stu-id="7d926-137">Select **Appointment scheduling** from the **Transportation** drop-down menu.</span></span>
4.  <span data-ttu-id="7d926-138">في الصفحة **جدولة المواعيد**، حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7d926-138">On the **Appointment scheduling** page, select **New** on the Action Pane.</span></span>
5.  <span data-ttu-id="7d926-139">في علامة التبويب السريعة **تفاصيل الموعد**، في الحقل **قاعدة الموعد**، حدد **المستودع 62**.</span><span class="sxs-lookup"><span data-stu-id="7d926-139">On the **Appointment details** FastTab, in the **Appointment rule** field, select **Warehouse 62**.</span></span>
6.  <span data-ttu-id="7d926-140">في جزء الإجراء، حدد **تأكيد** من القائمة المنسدلة **حالة التحديث**.</span><span class="sxs-lookup"><span data-stu-id="7d926-140">On the Action Pane, select **Firm** from the **Update status** drop-down menu.</span></span> <span data-ttu-id="7d926-141">إذا كانت القائمة **حالة التحديث** معطلة، فقم بالرجوع إلى الصفحة السابقة وإعادة تحديد **جدولة المواعيد** من القائمة المنسدلة **النقل** ثم قم بتحديد **تأكيد** من القائمة المنسدلة **حالة التحديث**.</span><span class="sxs-lookup"><span data-stu-id="7d926-141">If the **Update status** menu is disabled, go back to the previous page and reselect **Appointment scheduling** from the **Transportation** drop-down menu and then select **Firm** from the **Update status** drop-down menu.</span></span> 

## <a name="check-in-a-driver"></a><span data-ttu-id="7d926-142">‏‫تسجيل دخول السائق‬</span><span class="sxs-lookup"><span data-stu-id="7d926-142">Check in a driver</span></span> 

<span data-ttu-id="7d926-143">تمت مطالبتك بإنشاء موعد فوري للسائق Kim Anderson، وبعد ذلك ستقوم بتسجيل وصول Kim للموعد.</span><span class="sxs-lookup"><span data-stu-id="7d926-143">You have been asked to create an instant appointment for driver Kim Anderson, and then you will check in Kim for the appointment.</span></span>

### <a name="create-an-instant-appointment"></a><span data-ttu-id="7d926-144">إنشاء موعد فوري</span><span class="sxs-lookup"><span data-stu-id="7d926-144">Create an instant appointment</span></span>

1.  <span data-ttu-id="7d926-145">افتح **إدارة النقل > التخطيط > إرساء جدولة المواعيد > تسجيل دخول وخروج السائق لموعد**.</span><span class="sxs-lookup"><span data-stu-id="7d926-145">Open **Transportation management > Planning > Dock appointment scheduling > Driver check-in and check-out**.</span></span>
2.  <span data-ttu-id="7d926-146">في جزء الإجراء، حدد مفتاح السهم لأسفل **جدولة الموعد الفوري**.</span><span class="sxs-lookup"><span data-stu-id="7d926-146">On the Action Pane, select the **Schedule an instant appointment** drop-down arrow.</span></span>
3.  <span data-ttu-id="7d926-147">في الحقل **قاعدة الموعد**، حدد **المستودع 62**.</span><span class="sxs-lookup"><span data-stu-id="7d926-147">In the **Appointment rule** field, select **Warehouse 62**.</span></span>
4.  <span data-ttu-id="7d926-148">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7d926-148">Select **OK**.</span></span>

### <a name="check-in-a-driver-for-the-instant-appointment"></a><span data-ttu-id="7d926-149">تسجيل دخول السائق للموعد الفوري</span><span class="sxs-lookup"><span data-stu-id="7d926-149">Check in a driver for the instant appointment</span></span>

1.  <span data-ttu-id="7d926-150">في الصفحة **تسجيل دخول وخروج السائق**، حدد معرّف الموعد الذي تم إنشاؤه للتو.</span><span class="sxs-lookup"><span data-stu-id="7d926-150">On the **Driver check-in and check-out** list page, select the appointment ID that has just been created.</span></span>
2.  <span data-ttu-id="7d926-151">حدد **تسجيل دخول السائق** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7d926-151">On the Action Pane, select **Driver check-in**.</span></span>
3.  <span data-ttu-id="7d926-152">في الصفحة **تفاصيل تسجيل دخول السائق**، في الحقل **شركة الشحن**، حدد **TruckCarrier**.</span><span class="sxs-lookup"><span data-stu-id="7d926-152">On the **Driver check-in details** page, in the **Shipping carrier** field, select **TruckCarrier**.</span></span>
4.  <span data-ttu-id="7d926-153">في حقل **اسم السائق**، أدخل **Kim Anderson**.</span><span class="sxs-lookup"><span data-stu-id="7d926-153">In the **Driver name** field, enter **Kim Anderson**.</span></span>
5.  <span data-ttu-id="7d926-154">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7d926-154">Select **OK**.</span></span>
6.  <span data-ttu-id="7d926-155">حدد **تسجيل خروج السائق** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="7d926-155">Select **Driver check-out** in the Action Pane.</span></span> 
7.  <span data-ttu-id="7d926-156">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7d926-156">Select **OK**.</span></span>
7.  <span data-ttu-id="7d926-157">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="7d926-157">Close all pages.</span></span>
