---
ms.openlocfilehash: fddca8dc97736a1a90dc595ab519262f7d0e9d86
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6073862"
---
## <a name="scenario"></a><span data-ttu-id="659cd-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="659cd-101">Scenario</span></span>
<span data-ttu-id="659cd-102">إذا كنت ترغب في إنشاء فئة تكلفة جديدة بمعدل 15.00 دولاراً أمريكياً في الساعة لإنتاج الدراجات.</span><span class="sxs-lookup"><span data-stu-id="659cd-102">You want to create a new cost category with an hourly rate of $15.00 per hour to produce bicycles.</span></span> <span data-ttu-id="659cd-103">يجب تعيين فئة التكلفة الجديدة لمجموعة موارد جديدة لإنتاج الدراجات.</span><span class="sxs-lookup"><span data-stu-id="659cd-103">The new cost category should be assigned to a new resource group for bicycle production.</span></span> <span data-ttu-id="659cd-104">تتمثل مهمتك في إنشاء فئة التكلفة وربطها بحساب المصروفات المناسب وحسابات الأعمال تحت التنفيذ للترحيل، ثم ربط فئة التكلفة الجديدة بمجموعة موارد جديدة لإنتاج الدراجات.</span><span class="sxs-lookup"><span data-stu-id="659cd-104">Your task is to create the cost category and link to the appropriate expense account and WIP accounts for posting, and then link the new cost category to a new resource group for bicycle production.</span></span>

## <a name="create-a-shared-category-for-bicycle-assembly"></a><span data-ttu-id="659cd-105">إنشاء فئة مشتركة لتجميع الدراجات</span><span class="sxs-lookup"><span data-stu-id="659cd-105">Create a shared category for bicycle assembly</span></span> 

1.  <span data-ttu-id="659cd-106">افتح **التحكم في الإنتاج > إعداد > المسارات > الفئات المشتركة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-106">Open **Production control > Setup > Routes > Shared categories**.</span></span>
2.  <span data-ttu-id="659cd-107">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="659cd-107">Select **New** in the Action Pane.</span></span>
3.  <span data-ttu-id="659cd-108">أدخل **دراجة** في الحقل **معرّف الفئة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-108">Enter **Bicycle** in the **Category ID** field.</span></span>
4.  <span data-ttu-id="659cd-109">أدخل **تجميع دراجة** في الحقل **اسم الفئة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-109">Enter **Bicycle Assembly** in the **Category name** field.</span></span>
5.  <span data-ttu-id="659cd-110">قم بتعيين شريط التمرير **يمكن استخدامه في الإنتاج** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="659cd-110">Set the **Can be used in Production** slider to **Yes**.</span></span>
6.  <span data-ttu-id="659cd-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="659cd-111">Close the page.</span></span>

## <a name="create-a-new-cost-category-for-bicycle-assembly"></a><span data-ttu-id="659cd-112">إنشاء فئة تكلفة جديدة لتجميع الدراجات</span><span class="sxs-lookup"><span data-stu-id="659cd-112">Create a new cost category for bicycle assembly</span></span> 

1.  <span data-ttu-id="659cd-113">افتح **التحكم في الإنتاج > إعداد > المسارات > فئات التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-113">Open **Production control > Setup > Routes > Cost categories**.</span></span>
2.  <span data-ttu-id="659cd-114">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="659cd-114">Select **New** in the Action Pane.</span></span>
3.  <span data-ttu-id="659cd-115">حدد **دراجة** في الحقل **معرّف الفئة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-115">Select **Bicycle** in the **Category ID** field.</span></span>
4.  <span data-ttu-id="659cd-116">أدخل **L2 للتجميع** في الحقل **اسم الفئة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-116">Enter **L2 for Assembly** in the **Category name** field.</span></span>
5.  <span data-ttu-id="659cd-117">حدد علامة التبويب **إعداد الفئة** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="659cd-117">Select the **Category setup** tab in the Action Pane.</span></span>
6.  <span data-ttu-id="659cd-118">حدد **السعر**.</span><span class="sxs-lookup"><span data-stu-id="659cd-118">Select **Price**.</span></span>
7.  <span data-ttu-id="659cd-119">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="659cd-119">Select **New**.</span></span>
8.  <span data-ttu-id="659cd-120">في حقل **الإصدار**، حدد **10** **للفترة المالية الحالية**.</span><span class="sxs-lookup"><span data-stu-id="659cd-120">In the **Version** field, select **10** for **Current Fiscal Period**.</span></span>
9.  <span data-ttu-id="659cd-121">حدد **1** في الحقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="659cd-121">Select **1** in the **Site** field.</span></span>
10. <span data-ttu-id="659cd-122">في حقل **السعر**، أدخل **15.00**.</span><span class="sxs-lookup"><span data-stu-id="659cd-122">Enter **15.00** in the **Price** field.</span></span>
11. <span data-ttu-id="659cd-123">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="659cd-123">Select **Save** in the Action Pane.</span></span> 
12. <span data-ttu-id="659cd-124">حدد **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="659cd-124">Select **Activate**.</span></span> <span data-ttu-id="659cd-125">سيظهر تحذير، يمكنك تجاهله لأغراض هذا المختبر.</span><span class="sxs-lookup"><span data-stu-id="659cd-125">A warning will appear, that you can ignore for the purposes of this lab.</span></span>
13. <span data-ttu-id="659cd-126">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="659cd-126">Close the page.</span></span>

## <a name="add-ledger-postings-to-the-cost-category"></a><span data-ttu-id="659cd-127">إضافة ترحيلات دفتر الأستاذ إلى فئة التكلفة</span><span class="sxs-lookup"><span data-stu-id="659cd-127">Add ledger postings to the cost category</span></span> 

1.  <span data-ttu-id="659cd-128">في الصفحة **فئات التكلفة**، قم بتوسيع علامة التبويب السريعة **ترحيلات دفتر الأستاذ**.</span><span class="sxs-lookup"><span data-stu-id="659cd-128">On the **Cost categories** page, expand the **Ledger postings** FastTab.</span></span>
2.  <span data-ttu-id="659cd-129">في **تكلفة التصنيع المقدرة التي تم استيعابها**، حدد الحساب **600500 العمالة المباشرة المطبقة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-129">In  **Estimated manufacturing cost absorbed**, select the account  **600500  Direct Labor Applied**.</span></span>
3.  <span data-ttu-id="659cd-130">في **تكلفة التصنيع التي تم استيعابها**، حدد الحساب **600500 العمالة المباشرة المطبقة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-130">In **Manufacturing cost absorbed**, select the account **600500 Direct Labor Applied**.</span></span>
6.  <span data-ttu-id="659cd-131">في **التكلفة المقدرة للتصنيع المستهلك، الأعمال تحت التنفيذ**، حدد الحساب **150200** **إنتاج عمالة الأعمال تحت التنفيذ**.</span><span class="sxs-lookup"><span data-stu-id="659cd-131">In **Estimated cost of manufacturing consumed, WIP**, select the account **150200** **Production WIP-Labor**.</span></span>
8.  <span data-ttu-id="659cd-132">في **التكلفة للتصنيع المستهلك، الأعمال تحت التنفيذ**، حدد الحساب **150100** **إلغاء إنتاج الأعمال تحت التنفيذ**.</span><span class="sxs-lookup"><span data-stu-id="659cd-132">In **Cost of manufacturing consumed, WIP**, select the account **150100** **Production WIP-Clearing**.</span></span>
10. <span data-ttu-id="659cd-133">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="659cd-133">Close the page.</span></span>

## <a name="create-a-new-resource-group-for-bicycle-production"></a><span data-ttu-id="659cd-134">إنشاء مجموعة موارد جديدة لإنتاج الدراجات</span><span class="sxs-lookup"><span data-stu-id="659cd-134">Create a new resource group for bicycle production</span></span> 

1.  <span data-ttu-id="659cd-135">افتح **التحكم بالإنتاج > إعداد > الموارد > مجموعات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="659cd-135">Open **Production control > Setup > Resources > Resource groups**.</span></span>
2.  <span data-ttu-id="659cd-136">حدد **جديد** لإنشاء مجموعة جديدة.</span><span class="sxs-lookup"><span data-stu-id="659cd-136">Select **New** to create a new group.</span></span>
3.  <span data-ttu-id="659cd-137">في حقل **مجموعة المورد**، أدخل **1150**.</span><span class="sxs-lookup"><span data-stu-id="659cd-137">Enter **1150** in the **Resource group** field.</span></span>
4.  <span data-ttu-id="659cd-138">في حقل **الوصف**، أدخل **تجميع دراجة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-138">Enter **Bicycle Assembly** in the **Description** field.</span></span>
5.  <span data-ttu-id="659cd-139">حدد **1** في الحقل **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="659cd-139">Select **1** in the **Site** field.</span></span>


## <a name="assign-the-cost-category-for-setup-run-time-and-quantities"></a><span data-ttu-id="659cd-140">تعيين فئة التكلفة للإعداد ووقت التشغيل والكميات</span><span class="sxs-lookup"><span data-stu-id="659cd-140">Assign the cost category for setup, run time, and quantities</span></span> 

1.  <span data-ttu-id="659cd-141">قم بتوسيع علامة التبويب السريعة **العملية**.</span><span class="sxs-lookup"><span data-stu-id="659cd-141">Expand the **Operation** FastTab.</span></span>
2.  <span data-ttu-id="659cd-142">حدد **دراجة** في الحقل **إعداد الفئة**.</span><span class="sxs-lookup"><span data-stu-id="659cd-142">Select **Bicycle** in the **Setup category** field.</span></span>
3.  <span data-ttu-id="659cd-143">حدد **دراجة** في الحقل **تشغيل فئة الوقت**.</span><span class="sxs-lookup"><span data-stu-id="659cd-143">Select **Bicycle** in the **Run time category** field.</span></span>
4.  <span data-ttu-id="659cd-144">حدد **دراجة** في الحقل **فئة الكمية**.</span><span class="sxs-lookup"><span data-stu-id="659cd-144">Select **Bicycle** in the **Quantity category** field.</span></span>
5.  <span data-ttu-id="659cd-145">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="659cd-145">Select **Save** in the Action Pane.</span></span>
6.  <span data-ttu-id="659cd-146">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="659cd-146">Close the pages.</span></span>

