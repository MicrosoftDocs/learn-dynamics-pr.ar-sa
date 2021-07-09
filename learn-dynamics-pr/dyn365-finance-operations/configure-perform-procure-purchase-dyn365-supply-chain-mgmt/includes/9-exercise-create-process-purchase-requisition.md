---
ms.openlocfilehash: ecc094e79d451a30ee0181397278841eff33324b
ms.sourcegitcommit: 92dc7d01a500c2ef16f130203f4ebfe1a7950200
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "6073580"
---
## <a name="before-you-begin"></a><span data-ttu-id="26e83-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="26e83-101">Before you begin</span></span>

<span data-ttu-id="26e83-102">قبل أن تبدأ العمل في هذا التمرين المعملي، تحتاج إلى التأكد من بدء تشغيل "خدمة إدارة الدُفعات".</span><span class="sxs-lookup"><span data-stu-id="26e83-102">Before you start work on this lab, you need to ensure that the Batch Management Service has been started.</span></span> <span data-ttu-id="26e83-103">للقيام بذلك، نفذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="26e83-103">To do this, perform the following steps:</span></span>

1.  <span data-ttu-id="26e83-104">حدد زر **بدء** أسفل يسار الجهاز الظاهري وابحث عن وحدد تطبيق **الخدمات**.</span><span class="sxs-lookup"><span data-stu-id="26e83-104">Select the **Start** button at the bottom left of the VM and search for and select the **Services** app.</span></span>
2.  <span data-ttu-id="26e83-105">في التطبيق، قم بالتمرير إلى أسفل للبحث عن **Microsoft Dynamics 365 Unified Operations: خدمة إدارة الدُفعات**.</span><span class="sxs-lookup"><span data-stu-id="26e83-105">In the app, scroll down to find **Microsoft Dynamics 365 Unified Operations: Batch Management Service**.</span></span> 
3.  <span data-ttu-id="26e83-106">وبعد ذلك، انقر بزر الماوس الأيمن فوقه وحدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="26e83-106">Then right-click on it and select **Start**.</span></span>

## <a name="scenario"></a><span data-ttu-id="26e83-107">السيناريو</span><span class="sxs-lookup"><span data-stu-id="26e83-107">Scenario</span></span>

<span data-ttu-id="26e83-108">أنشئ طلب شراء 5 قطع من كبلات HDMI مقاس 24 بوصة باستخدام فئة المشتريات الخاصة بأجهزة الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="26e83-108">Create a purchase requisition for 5 pieces of 24-inch HDMI cables by using the procurement category of Computers.</span></span>

<span data-ttu-id="26e83-109">تأكد من أن المستخدم الخاص بك مرتبط بعامل.</span><span class="sxs-lookup"><span data-stu-id="26e83-109">Ensure that your user is associated with a worker.</span></span> <span data-ttu-id="26e83-110">تحدد الشركة التي يعمل فيها العامل الكيان القانوني للشراء، ومن ثم السياسة المطبقة.</span><span class="sxs-lookup"><span data-stu-id="26e83-110">The company in which the worker is employed determines the buying legal entity, hence the policy applied.</span></span>

## <a name="create-a-purchase-requisition"></a><span data-ttu-id="26e83-111">إنشاء طلب شراء</span><span class="sxs-lookup"><span data-stu-id="26e83-111">Create a purchase requisition</span></span>

1.  <span data-ttu-id="26e83-112">في USMF، انتقل إلى **التدبير والتوريد > طلبات الشراء > جميع طلبات الشراء**.</span><span class="sxs-lookup"><span data-stu-id="26e83-112">In USMF, go to **Procurement and sourcing > Purchase requisitions > All purchase requisitions**.</span></span>
2.  <span data-ttu-id="26e83-113">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="26e83-113">Select **New**.</span></span>
3.  <span data-ttu-id="26e83-114">في حقل **الاسم**، أدخل **كبلات HDMI الجديدة**.</span><span class="sxs-lookup"><span data-stu-id="26e83-114">In the **Name** field, enter **New HDMI Cables**.</span></span>
4.  <span data-ttu-id="26e83-115">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="26e83-115">Select **OK**.</span></span>
5.  <span data-ttu-id="26e83-116">في حقل **السبب**، حدد **عام** (المستلزمات العامة).</span><span class="sxs-lookup"><span data-stu-id="26e83-116">In the **Reason** field, select **General** (General supplies).</span></span>
6.  <span data-ttu-id="26e83-117">في حقل **التفاصيل**، أدخل **كبلات HDMI أطول وجديدة**.</span><span class="sxs-lookup"><span data-stu-id="26e83-117">In the **Details** field, enter **New, longer HDMI cables**.</span></span>

## <a name="add-an-item-to-the-purchase-requisition"></a><span data-ttu-id="26e83-118">إضافة صنف إلى طلب الشراء</span><span class="sxs-lookup"><span data-stu-id="26e83-118">Add an item to the purchase requisition</span></span>

1.  <span data-ttu-id="26e83-119">حدد **إضافة المنتجات** في علامة التبويب السريعة **بنود طلبات الشراء**.</span><span class="sxs-lookup"><span data-stu-id="26e83-119">Select **Add products** on the **Purchase requisition lines** FastTab.</span></span>
2.  <span data-ttu-id="26e83-120">حدد فئة تدبير **أجهزه الكمبيوتر** (فئة فرعية لأجهزة Office).</span><span class="sxs-lookup"><span data-stu-id="26e83-120">Select the **Computers** procurement category (a subcategory of Office Machines).</span></span>
3.  <span data-ttu-id="26e83-121">حدد **إضافة منتجات غير مدرجة إلى البنود**.</span><span class="sxs-lookup"><span data-stu-id="26e83-121">Select **Add unlisted product to lines**.</span></span>
4.  <span data-ttu-id="26e83-122">في حقل **اسم المنتج**، أدخل **كبل HDMI مقاس 24 بوصة**.</span><span class="sxs-lookup"><span data-stu-id="26e83-122">In the **Product name** field, enter **24-inch HDMI Cable**.</span></span>
5.  <span data-ttu-id="26e83-123">في حقل **الوحدة**، أدخل **ea**.</span><span class="sxs-lookup"><span data-stu-id="26e83-123">In the **Unit** field, enter **ea**.</span></span>
6.  <span data-ttu-id="26e83-124">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="26e83-124">Select **OK**.</span></span>
7.  <span data-ttu-id="26e83-125">حدد علامة التبويب **التفاصيل** أسفل يمين الصفحة.</span><span class="sxs-lookup"><span data-stu-id="26e83-125">Select the **Details** tab in the bottom-right of the page.</span></span>
9.  <span data-ttu-id="26e83-126">في حقل **الكمية**، أدخِل **5**.</span><span class="sxs-lookup"><span data-stu-id="26e83-126">In the **Quantity** field, enter **5**.</span></span>
10. <span data-ttu-id="26e83-127">في حقل **سعر الوحدة**، أدخِل **41**.</span><span class="sxs-lookup"><span data-stu-id="26e83-127">In the **Unit price** field, enter **41**.</span></span>
11. <span data-ttu-id="26e83-128">في حقل **حساب المورد**، حدد **1001** (مستلزمات المكاتب من Acme).</span><span class="sxs-lookup"><span data-stu-id="26e83-128">In the **Vendor account** field, select **1001** (Acme Office Supplies).</span></span>
12. <span data-ttu-id="26e83-129">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="26e83-129">Select **OK**.</span></span>
13. <span data-ttu-id="26e83-130">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="26e83-130">Select **Save**.</span></span>

## <a name="submit-a-purchase-requisition-for-approval"></a><span data-ttu-id="26e83-131">تقديم طلب شراء للموافقة</span><span class="sxs-lookup"><span data-stu-id="26e83-131">Submit a purchase requisition for approval</span></span>

1.  <span data-ttu-id="26e83-132">حدد **سير العمل** أعلى الصفحة، ثم حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="26e83-132">Select **Workflow** at the top of the page, and then select **Submit**.</span></span>
2.  <span data-ttu-id="26e83-133">في حقل **التعليق**، أدخل **طلب كبلات HDMI أطول**.</span><span class="sxs-lookup"><span data-stu-id="26e83-133">In the **Comment** field, enter **Request for longer HDMI cables**.</span></span>
3.  <span data-ttu-id="26e83-134">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="26e83-134">Select **Submit**.</span></span>
4.  <span data-ttu-id="26e83-135">حدد **سير العمل > محفوظات سير العمل**</span><span class="sxs-lookup"><span data-stu-id="26e83-135">Select **Workflow > Workflow history**</span></span>
5.  <span data-ttu-id="26e83-136">حدد رمز **تحديث** أعلى يمين الصفحة عدة مرات، وانتظر حتى تعرض أصناف سير العمل السجلات.</span><span class="sxs-lookup"><span data-stu-id="26e83-136">Select the **Refresh** icon in the top-right of the page a few times, and wait until the workflow items show records.</span></span>
6.  <span data-ttu-id="26e83-137">حدد زر **إعادة تعيين** في علامة التبويب السريعة **أصناف العمل**.</span><span class="sxs-lookup"><span data-stu-id="26e83-137">Select the **Reassign** button in the **Work items** FastTab.</span></span>
7.  <span data-ttu-id="26e83-138">حدد **المسؤول** في حقل **المستخدم**.</span><span class="sxs-lookup"><span data-stu-id="26e83-138">Select **Admin** in the **User** field.</span></span>
8.  <span data-ttu-id="26e83-139">حدد **إعادة تعيين**.</span><span class="sxs-lookup"><span data-stu-id="26e83-139">Select **Reassign**.</span></span>
9.  <span data-ttu-id="26e83-140">أغلق صفحة **محفوظات سير العمل**</span><span class="sxs-lookup"><span data-stu-id="26e83-140">Close the **Workflow history** page</span></span>


## <a name="approve-the-purchase-requisition"></a><span data-ttu-id="26e83-141">الموافقة على طلب الشراء</span><span class="sxs-lookup"><span data-stu-id="26e83-141">Approve the purchase requisition</span></span>

1.  <span data-ttu-id="26e83-142">حدد **سير العمل** في الجزء العلوي، ثم حدد **موافقة**.</span><span class="sxs-lookup"><span data-stu-id="26e83-142">Select **Workflow** at the top, and then select **Approve**.</span></span>
2.  <span data-ttu-id="26e83-143">في حقل **التعليق**، أدخل **تمت الموافقة**.</span><span class="sxs-lookup"><span data-stu-id="26e83-143">In the **Comment** field, enter **Approved**.</span></span>
3.  <span data-ttu-id="26e83-144">حدد **موافقة**.</span><span class="sxs-lookup"><span data-stu-id="26e83-144">Select **Approve**.</span></span>


