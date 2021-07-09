---
ms.openlocfilehash: 304442b80f86e70bbfd5217c01bbfd736ab23ff3
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073302"
---
## <a name="scenario"></a><span data-ttu-id="14285-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="14285-101">Scenario</span></span>

<span data-ttu-id="14285-102">يُطلب منك إعداد رمزين جديدين للتخلص.</span><span class="sxs-lookup"><span data-stu-id="14285-102">You are asked to set up two new disposition codes.</span></span> <span data-ttu-id="14285-103">الأول سيكون باسم "جاهز"، والذي سيكون متاحاً، والثاني سيكون "غير جاهز"، والذي سيتم حظره للاستخدام مع إدارة المستودعات.</span><span class="sxs-lookup"><span data-stu-id="14285-103">The first will be named "Ready," which will be available, and the second will be named "Not ready," which will be blocked for use with warehouse management.</span></span> 

1.  <span data-ttu-id="14285-104">في شركة **USP2**، انتقل إلى **إدارة المستودعات > الإعداد > الجهاز المحمول > رموز التخلص**.</span><span class="sxs-lookup"><span data-stu-id="14285-104">In company **USP2**, go to **Warehouse management > Setup > Mobile device > Disposition codes**.</span></span>
2.  <span data-ttu-id="14285-105">حدد **جديد** لإنشاء رمز تخلص.</span><span class="sxs-lookup"><span data-stu-id="14285-105">Select **New** to create a disposition code.</span></span>
3.  <span data-ttu-id="14285-106">في حقل **رمز التخلص**، أدخل **جاهز**.</span><span class="sxs-lookup"><span data-stu-id="14285-106">In the **Disposition code** field, enter **Ready**.</span></span>
4.  <span data-ttu-id="14285-107">في حقل **حالة المخزون**، حدد **متوفر**.</span><span class="sxs-lookup"><span data-stu-id="14285-107">In the **Inventory status** field, select **Available**.</span></span>
5.  <span data-ttu-id="14285-108">حدد **جديد** لإنشاء رمز تخلص.</span><span class="sxs-lookup"><span data-stu-id="14285-108">Select **New** to create a disposition code.</span></span>
6.  <span data-ttu-id="14285-109">في حقل **رمز التخلص**، أدخل **غير جاهز**.</span><span class="sxs-lookup"><span data-stu-id="14285-109">In the **Disposition code** field, enter **Not ready**.</span></span>
7.  <span data-ttu-id="14285-110">في حقل **حالة المخزون**، حدد **محظور**.</span><span class="sxs-lookup"><span data-stu-id="14285-110">In the **Inventory status** field, select **Blocked**.</span></span>
8.  <span data-ttu-id="14285-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="14285-111">Close the page.</span></span>

## <a name="create-inbound-location-directives"></a><span data-ttu-id="14285-112">إنشاء توجيهات الموقع الواردة</span><span class="sxs-lookup"><span data-stu-id="14285-112">Create inbound location directives</span></span> 

<span data-ttu-id="14285-113">تحتاج إلى تكوين توجيه موقع وارد جديد لاستلام البضائع إلى المستودع ثم واحد سيضع البضائع بعيداً في المواقع المجمعة.</span><span class="sxs-lookup"><span data-stu-id="14285-113">You need to configure a new inbound location directive that will receive goods to the warehouse and then one that will put away goods in bulk locations.</span></span> 

1.   <span data-ttu-id="14285-114">افتح **إدارة المستودعات > إعداد > توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="14285-114">Open **Warehouse management > Setup > Location directives**.</span></span>
2.   <span data-ttu-id="14285-115">حدد **أوامر الشراء** في حقل **نوع أمر العمل**.</span><span class="sxs-lookup"><span data-stu-id="14285-115">Select **Purchase orders** in the **Work order type** field.</span></span>
3.   <span data-ttu-id="14285-116">حدد **جديد** في جزء الإجراءات لإنشاء توجيه موقع جديد.</span><span class="sxs-lookup"><span data-stu-id="14285-116">Select **New** in the Action Pane to create a new location directive.</span></span>
4.   <span data-ttu-id="14285-117">أدخل **MAIN DC** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="14285-117">Type **MAIN DC** in the **Name** field.</span></span>
5.   <span data-ttu-id="14285-118">حدد **وضع** في حقل **نوع العمل** لأنك تريد إبعاد الأصناف المستلمة في أوامر الشراء.</span><span class="sxs-lookup"><span data-stu-id="14285-118">Select **Put** in the **Work type** field because you want to put away the received items on purchase orders.</span></span>
6.   <span data-ttu-id="14285-119">حدد **3** في حقل **الموقع‏‎**.</span><span class="sxs-lookup"><span data-stu-id="14285-119">Select **3** in the **Site** field.</span></span>
7.  <span data-ttu-id="14285-120">حدد **30** في حقل **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="14285-120">Select **30** in the **Warehouse** field.</span></span>
8.   <span data-ttu-id="14285-121">حدد **مرحلة** في حقل **رمز التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="14285-121">Select **Stage** in the **Directive code** field.</span></span>
9. <span data-ttu-id="14285-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="14285-122">Select **Save**.</span></span>

## <a name="add-lines-to-the-location-directive"></a><span data-ttu-id="14285-123">إضافة بنود إلى توجيه الموقع</span><span class="sxs-lookup"><span data-stu-id="14285-123">Add lines to the location directive</span></span>

1.   <span data-ttu-id="14285-124">ضمن علامة التبويب السريعة **البنود**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="14285-124">Select **New** in the **Lines** FastTab.</span></span>
2.   <span data-ttu-id="14285-125">تأكد أن **الرقم التسلسلي** هو **1**.</span><span class="sxs-lookup"><span data-stu-id="14285-125">Verify that the **Sequence number** is **1**.</span></span>
3.   <span data-ttu-id="14285-126">أدخل **200** في حقل **إلى الكمية**.</span><span class="sxs-lookup"><span data-stu-id="14285-126">Type **200** in the **To quantity** field.</span></span>
4.   <span data-ttu-id="14285-127">حدد **ea** في حقل **الوحدة**.</span><span class="sxs-lookup"><span data-stu-id="14285-127">Select **ea** in the **Unit** field.</span></span>
5.   <span data-ttu-id="14285-128">حدد **بلا‬** في الحقل **تحديد موقع الكمية**.</span><span class="sxs-lookup"><span data-stu-id="14285-128">Select **None** in the **Locate quantity** field.</span></span>
6.   <span data-ttu-id="14285-129">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="14285-129">Select **Save** in the Action Pane.</span></span>
7.   <span data-ttu-id="14285-130">حدد **جديد** في علامة التبويب السريعة **إجراءات توجيه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="14285-130">Select **New** in the **Location directive actions** FastTab.</span></span>
8.   <span data-ttu-id="14285-131">اكتب **تحديث** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="14285-131">Type **Fresh** in the **Name** field.</span></span>
9.   <span data-ttu-id="14285-132">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="14285-132">Select **Save** in the Action Pane.</span></span>

## <a name="add-location-directive-actions-to-the-location-directive"></a><span data-ttu-id="14285-133">إضافة إجراءات توجيه الموقع إلى توجيه الموقع</span><span class="sxs-lookup"><span data-stu-id="14285-133">Add location directive actions to the location directive</span></span>

1.  <span data-ttu-id="14285-134">حدد **تحرير استعلام** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="14285-134">Select **Edit query** in the Action Pane.</span></span>
2.  <span data-ttu-id="14285-135">حدد **إضافة** في صفحة **تحديد الاستعلام**.</span><span class="sxs-lookup"><span data-stu-id="14285-135">Select **Add** on the **Select query** page.</span></span>
3.  <span data-ttu-id="14285-136">حدد **أوامر الشراء** في عمود **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="14285-136">Select **Purchase Orders** in the **Table** column.</span></span>
4.  <span data-ttu-id="14285-137">حدد **الموقع** في عمود **الحقل**.</span><span class="sxs-lookup"><span data-stu-id="14285-137">Select **Location** in the **Field** column.</span></span>
5.  <span data-ttu-id="14285-138">حدد **30** في عمود **المعايير**.</span><span class="sxs-lookup"><span data-stu-id="14285-138">Select **30** in the **Criteria** column.</span></span>
6.  <span data-ttu-id="14285-139">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="14285-139">Select **OK**.</span></span>
7.  <span data-ttu-id="14285-140">قم بإغلاق صفحة **توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="14285-140">Close the **Location directives** page.</span></span>



