---
ms.openlocfilehash: a117afe29847d1f456cb0b7a1de6aadcc3f5f272
ms.sourcegitcommit: 21873567450f1b38114ad9ed397ab7e898b7e640
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "6073599"
---
## <a name="scenario"></a><span data-ttu-id="d51f1-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="d51f1-101">Scenario</span></span>
<span data-ttu-id="d51f1-102">بصفتك موظف مستودع في شركة **‎USMF**، فأنت بحاجة إلى إنشاء إصدار التكاليف القياسي لتسجيل المنتجات التي تستخدم مجموعة نماذج الصنف مع نموذج المخزون **القياسي**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-102">As a warehouse employee at company **USMF**, you need to create a standard cost version to record products that use the item model group with inventory model of **Standard**.</span></span> <span data-ttu-id="d51f1-103">تحتاج أيضاً إلى تجميع الأصناف استناداً إلى نموذج المخزون FIFO.</span><span class="sxs-lookup"><span data-stu-id="d51f1-103">You also need to group items based on the FIFO inventory model.</span></span>

<span data-ttu-id="d51f1-104">لذلك، تحتاج إلى إنشاء مجموعة نماذج الصنف وإصدار التكاليف ومجموعة أرقام التعقب لتوزيع أرقام دُفعات وأرقام تسلسلية.</span><span class="sxs-lookup"><span data-stu-id="d51f1-104">Therefore, you need to create an item model group, a cost version, and tracking number group to allocate batch and serial numbers.</span></span>

## <a name="create-a-costing-version"></a><span data-ttu-id="d51f1-105">إنشاء إصدار تكاليف</span><span class="sxs-lookup"><span data-stu-id="d51f1-105">Create a costing version</span></span> 

1.  <span data-ttu-id="d51f1-106">انتقل إلى **إدارة التكلفة > إعداد سياسات التكلفة المحددة مسبقاً > إصدارات التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-106">Go to **Cost management > Predetermined cost policies setup > Costing versions**.</span></span>
2.  <span data-ttu-id="d51f1-107">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-107">Select **New**.</span></span>
3.  <span data-ttu-id="d51f1-108">في الحقل **نوع التكاليف**، حدد **التكلفة القياسية**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-108">In the **Costing type** field, select **Standard cost**.</span></span>
4.  <span data-ttu-id="d51f1-109">في الحقل **الإصدار**، اكتب **السنة المالية 2019**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-109">In the **Version** field, type **FY 2019**.</span></span>
5.  <span data-ttu-id="d51f1-110">في الحقل **اسم**، اكتب **تكاليف السنة المالية 2019**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-110">In the **Name** field, type **FY 2019 Costing**.</span></span>
6.  <span data-ttu-id="d51f1-111">في الحقل **حظر التنشيط**، حدد **لا**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-111">In the **Block activation** field, select **No**.</span></span>
7.  <span data-ttu-id="d51f1-112">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-112">Select **Save**.</span></span>
8.  <span data-ttu-id="d51f1-113">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="d51f1-113">Close the page.</span></span>


## <a name="create-an-item-model-group"></a><span data-ttu-id="d51f1-114">إنشاء مجموعه نماذج الصنف</span><span class="sxs-lookup"><span data-stu-id="d51f1-114">Create an item model group</span></span> 

1.  <span data-ttu-id="d51f1-115">انتقل إلى **إدارة المخزون> إعداد> مخزون> مجموعات نماذج الصنف**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-115">Go to **Inventory management > Setup > Inventory > Item model groups**.</span></span>
2.  <span data-ttu-id="d51f1-116">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-116">Select **New**.</span></span>
3.  <span data-ttu-id="d51f1-117">في الحقل **مجموعه نماذج الصنف**، اكتب **STDN**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-117">In the **Item model group** field, type **STDN**.</span></span>
4.  <span data-ttu-id="d51f1-118">في الحقل **اسم**، اكتب **التكلفة القياسية**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-118">In the **Name** field, type **Standard Cost**.</span></span>
5.  <span data-ttu-id="d51f1-119">في الحقل **نموذج المخزون**، أدخل **التكلفة القياسية**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-119">In the **Inventory model** field, enter **Standard cost**.</span></span>
6.  <span data-ttu-id="d51f1-120">قم بتوسيع القسم **سياسات المخزون**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-120">Expand the **Inventory policies** section.</span></span>
7.  <span data-ttu-id="d51f1-121">في الحقل **أسلوب التحقق من المورد المعتمد**، أدخل **لا يوجد فحص**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-121">In the **Approved vendor check method** field, enter **No check**.</span></span>
8.  <span data-ttu-id="d51f1-122">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="d51f1-122">Select **Save**</span></span>
8.  <span data-ttu-id="d51f1-123">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-123">Select **New**.</span></span>
9.  <span data-ttu-id="d51f1-124">في الحقل **مجموعه نماذج الصنف**، اكتب **FirstIn**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-124">In the **Item model group** field, type **FirstIn**.</span></span>
10. <span data-ttu-id="d51f1-125">في الحقل **اسم**، اكتب **ما يرد أولاً يصرف أولاً**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-125">In the **Name** field, type **First in First Out**.</span></span>
11. <span data-ttu-id="d51f1-126">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="d51f1-126">Close the page.</span></span>


## <a name="create-a-tracking-number-group"></a><span data-ttu-id="d51f1-127">إنشاء مجموعه أرقام التعقب</span><span class="sxs-lookup"><span data-stu-id="d51f1-127">Create a tracking number group</span></span> 

1.  <span data-ttu-id="d51f1-128">انتقل إلى **إدارة المخزون> الإعداد> الأبعاد > مجموعات أرقام التعقب**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-128">Go to **Inventory management > Setup > Dimensions > Tracking number groups**.</span></span>
2.  <span data-ttu-id="d51f1-129">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-129">Select **New**.</span></span>
3.  <span data-ttu-id="d51f1-130">في الحقل **مجموعة الأرقام**، اكتب **ASer**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-130">In the **Number group** field, type **ASer**.</span></span>
4.  <span data-ttu-id="d51f1-131">في الحقل **اسم**، اكتب **التسلسل التلقائي**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-131">In the **Name** field, type **Auto-Serial**.</span></span>
5.  <span data-ttu-id="d51f1-132">حدد **لا** في الحقل **التاريخ**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-132">Select **No** in the **Date** field.</span></span>
6.  <span data-ttu-id="d51f1-133">حدد **لا** في الحقل **كود الشحنة**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-133">Select **No** in the **Lot ID** field.</span></span>
7.  <span data-ttu-id="d51f1-134">حدد **نعم** في الحقل **رقم التسلسل الرقمي**</span><span class="sxs-lookup"><span data-stu-id="d51f1-134">Select **Yes** in the **Number sequence No.**</span></span> <span data-ttu-id="d51f1-135">.</span><span class="sxs-lookup"><span data-stu-id="d51f1-135">field.</span></span>
8.  <span data-ttu-id="d51f1-136">في الحقل **كود التسلسل الرقمي**، حدد أي تسلسل رقمي.</span><span class="sxs-lookup"><span data-stu-id="d51f1-136">In the **Number sequence code** field, select any number sequence.</span></span>
8.  <span data-ttu-id="d51f1-137">حدد **نعم** في الحقل **لحركات المخزون فقط**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-137">Select **Yes** in the **Only for inventory transactions** field.</span></span>
9.  <span data-ttu-id="d51f1-138">حدد **نعم** في الحقل **عند التحديث الفعلي**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-138">Select **Yes** in the **On physical update** field.</span></span>
10. <span data-ttu-id="d51f1-139">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-139">Select **New**.</span></span>
11. <span data-ttu-id="d51f1-140">في الحقل **مجموعة الأرقام**، اكتب **USer**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-140">In the **Number group** field, type **USer**.</span></span>
12. <span data-ttu-id="d51f1-141">في الحقل **اسم**، اكتب **التسلسل الفريد**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-141">In the **Name** field, type **Unique-Serial**.</span></span>
13. <span data-ttu-id="d51f1-142">حدد **لا** في الحقل **التاريخ**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-142">Select **No** in the **Date** field.</span></span>
14. <span data-ttu-id="d51f1-143">حدد **لا** في الحقل **كود الشحنة**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-143">Select **No** in the **Lot ID** field.</span></span>
15. <span data-ttu-id="d51f1-144">حدد **نعم** في الحقل **رقم التسلسل الرقمي**</span><span class="sxs-lookup"><span data-stu-id="d51f1-144">Select **Yes** in the **Number sequence No.**</span></span> <span data-ttu-id="d51f1-145">الحقل.</span><span class="sxs-lookup"><span data-stu-id="d51f1-145">field.</span></span>
16. <span data-ttu-id="d51f1-146">في الحقل **كود التسلسل الرقمي**، حدد أي تسلسل رقمي.</span><span class="sxs-lookup"><span data-stu-id="d51f1-146">In the **Number sequence code** field, select any number sequence.</span></span>
17. <span data-ttu-id="d51f1-147">حدد **نعم** في الحقل **لحركات المخزون فقط**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-147">Select **Yes** in the **Only for inventory transactions** field.</span></span>
18. <span data-ttu-id="d51f1-148">حدد **نعم** في الحقل **عند التحديث الفعلي**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-148">Select **Yes** in the **On physical update** field.</span></span>
19. <span data-ttu-id="d51f1-149">عيّن **لكل كمية** على **1**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-149">Set **Per qty.** to **1**.</span></span>
20. <span data-ttu-id="d51f1-150">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-150">Select **New**.</span></span>
21. <span data-ttu-id="d51f1-151">في الحقل **مجموعة الأرقام**، اكتب **الدُفعة**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-151">In the **Number group** field, type **Batch**.</span></span>
22. <span data-ttu-id="d51f1-152">في الحقل **اسم**، اكتب **الدُفعة التلقائية**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-152">In the **Name** field, type **Auto Batch**.</span></span>
23. <span data-ttu-id="d51f1-153">حدد **لا** في الحقل **التاريخ**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-153">Select **No** in the **Date** field.</span></span>
24. <span data-ttu-id="d51f1-154">حدد **لا** في الحقل **كود الشحنة**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-154">Select **No** in the **Lot ID** field.</span></span>
25. <span data-ttu-id="d51f1-155">حدد **نعم** في الحقل **رقم التسلسل الرقمي**</span><span class="sxs-lookup"><span data-stu-id="d51f1-155">Select **Yes** in the **Number sequence No.**</span></span> <span data-ttu-id="d51f1-156">الحقل.</span><span class="sxs-lookup"><span data-stu-id="d51f1-156">field.</span></span>
26. <span data-ttu-id="d51f1-157">في الحقل **كود التسلسل الرقمي**، حدد أي تسلسل رقمي.</span><span class="sxs-lookup"><span data-stu-id="d51f1-157">In the **Number sequence code** field, select any number sequence.</span></span>
27. <span data-ttu-id="d51f1-158">حدد **نعم** في الحقل **لحركات المخزون فقط**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-158">Select **Yes** in the **Only for inventory transactions** field.</span></span>
28. <span data-ttu-id="d51f1-159">حدد **لا** في الحقل **عند التحديث الفعلي**.</span><span class="sxs-lookup"><span data-stu-id="d51f1-159">Select **No** in the **On physical update** field.</span></span>
29. <span data-ttu-id="d51f1-160">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="d51f1-160">Close the page.</span></span>




