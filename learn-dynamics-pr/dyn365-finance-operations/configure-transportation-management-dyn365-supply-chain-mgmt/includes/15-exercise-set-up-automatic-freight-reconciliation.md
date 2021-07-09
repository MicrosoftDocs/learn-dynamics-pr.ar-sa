---
ms.openlocfilehash: 9fc00c65854f6627e922a9589b656197637609d5
ms.sourcegitcommit: d13baa2f6c2b9f5fad9a26f7c64f7e4dbcceb6e2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/22/2020
ms.locfileid: "6073569"
---
## <a name="scenario"></a><span data-ttu-id="77fc5-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="77fc5-101">Scenario</span></span>

<span data-ttu-id="77fc5-102">لقد تم تكليفك بإعداد تسوية الشحن لـ Desert Wholesales.</span><span class="sxs-lookup"><span data-stu-id="77fc5-102">You have been tasked with setting up freight reconciliation for Desert Wholesales.</span></span>

## <a name="create-a-freight-reconciliation-reason-code-for-overtime"></a><span data-ttu-id="77fc5-103">إنشاء كود سبب تسوية الشحن للعمل الإضافي</span><span class="sxs-lookup"><span data-stu-id="77fc5-103">Create a freight reconciliation reason code for Overtime</span></span>

1.  <span data-ttu-id="77fc5-104">افتح **إدارة النقل > إعداد > تسوية الشحن > أسباب التسوية**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-104">Open **Transportation management > Setup > Freight reconciliation > Reconciliation reasons**.</span></span>
2.  <span data-ttu-id="77fc5-105">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-105">Select **New**.</span></span>
3.  <span data-ttu-id="77fc5-106">أدخل **OT** في حقل **سبب التسوية**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-106">Enter **OT** in the **Reconciliation reason** field.</span></span>
4.  <span data-ttu-id="77fc5-107">في الحقل **الوصف**، أدخل **‏‫العمل الإضافي‬**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-107">Enter **Overtime** in the **Description** field.</span></span>
5.  <span data-ttu-id="77fc5-108">أدخل **211650** في الحقل **الحساب المدين** ثم في القائمة المنسدلة التي تظهر، حدد قيمة مثل **الصفحة الرئيسية** في الحقل **وحدة الأعمال** و **العمليات** في الحقل **القسم**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-108">Enter **211650** in the **Debit account** field and then, in the dropdown that appears, select a value such as **Home** in the **BusinessUnit** field and **Operations** in **Department** field.</span></span>
6.  <span data-ttu-id="77fc5-109">حدد خانة الاختيار **دفع مورد الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-109">Select the **Pay the freight vendor** check box.</span></span> <span data-ttu-id="77fc5-110">(قد تحتاج إلى تحديد علامة التبويب **‬‏‫دفع مورد الشحن** واستخدم شريط المسافات لتحديدها.)</span><span class="sxs-lookup"><span data-stu-id="77fc5-110">(You may need to tab to the **Pay the freight vendor** check box and use the space bar to select it.)</span></span>
7.  <span data-ttu-id="77fc5-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="77fc5-111">Close the page.</span></span>

## <a name="verify-that-the-freight-bill-type-is-configured"></a><span data-ttu-id="77fc5-112">التحقق من تكوين نوع فاتورة الشحن</span><span class="sxs-lookup"><span data-stu-id="77fc5-112">Verify that the Freight bill type is configured</span></span> 

1.  <span data-ttu-id="77fc5-113">افتح **إدارة النقل > إعداد > تسوية الشحن > تسوية الشحن > نوع فاتورة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-113">Open **Transportation management > Setup > Freight reconciliation > Freight bill type**.</span></span>
2.  <span data-ttu-id="77fc5-114">حدد نوع فاتورة الشحن **TL**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-114">Select the **TL** Freight bill type.</span></span>
3.  <span data-ttu-id="77fc5-115">تحقق من تعبئة حقل **تجميع المحرك**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-115">Verify that the **Engine assembly** field is populated.</span></span>
4.  <span data-ttu-id="77fc5-116">تحقق من وجود سجلين: الأول **لمعرّف مجموعه الفوترة** والآخر **لكود خارجي**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-116">Verify that two records exist: one for **Billing group ID** and one for **External code**.</span></span>
5.  <span data-ttu-id="77fc5-117">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="77fc5-117">Close the page.</span></span>

## <a name="create-a-freight-bill-type-assignment-for-the-truck-carrier-service"></a><span data-ttu-id="77fc5-118">إنشاء تعيين نوع فاتورة شحن لخدمة شركة النقل‬</span><span class="sxs-lookup"><span data-stu-id="77fc5-118">Create a freight bill type assignment for the Truck Carrier service</span></span>

1.  <span data-ttu-id="77fc5-119">افتح **إدارة النقل > إعداد > تسوية الشحن > مهام نوع فاتورة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-119">Open **Transportation management > Setup > Freight reconciliation > Freight bill type assignments**.</span></span>
2.  <span data-ttu-id="77fc5-120">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-120">Select **New**.</span></span>
3.  <span data-ttu-id="77fc5-121">حدد **بلا‬** في الحقل **الاتجاه**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-121">Select **None** in the **Direction** field.</span></span>
4.  <span data-ttu-id="77fc5-122">في حقل **الوضع‬**، حدد **أساسي**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-122">Select **Ground** in the **Mode** field.</span></span>
5.  <span data-ttu-id="77fc5-123">حدد **ناقل عبر الشاحنات** في حقل **شركة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-123">Select **TruckCarrier** in the **Shipping carrier** field.</span></span>
6.  <span data-ttu-id="77fc5-124">حدد **TL** في الحقل **نوع فاتورة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-124">Select **TL** in the **Freight bill type** field.</span></span>
7.  <span data-ttu-id="77fc5-125">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="77fc5-125">Close the page.</span></span>

## <a name="create-a-billing-group-named-duties"></a><span data-ttu-id="77fc5-126">إنشاء مجموعة فوترة باسم "المهام"</span><span class="sxs-lookup"><span data-stu-id="77fc5-126">Create a billing group named "Duties"</span></span>

1.  <span data-ttu-id="77fc5-127">افتح **إدارة النقل > إعداد > تسوية الشحن > مجموعة الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-127">Open **Transportation management > Setup > Freight reconciliation > Billing Group**.</span></span>
2.  <span data-ttu-id="77fc5-128">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-128">Select **New**.</span></span>
3.  <span data-ttu-id="77fc5-129">أدخل **المهام** في الحقل **معرّف مجموعة الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-129">Enter **Duties** in the **Billing group ID** field.</span></span>
4.  <span data-ttu-id="77fc5-130">أدخل **المهام** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-130">Enter **Duties** in the **Name** field.</span></span>
5.  <span data-ttu-id="77fc5-131">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="77fc5-131">Close the page.</span></span>

## <a name="create-an-audit-master-for-overtime"></a><span data-ttu-id="77fc5-132">إنشاء عملية رئيسية للتدقيق الإضافي</span><span class="sxs-lookup"><span data-stu-id="77fc5-132">Create an audit master for overtime</span></span>

1.  <span data-ttu-id="77fc5-133">افتح **إدارة النقل > إعداد > تسوية الشحن > التدقيق الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-133">Open **Transportation management > Setup > Freight reconciliation > Audit master**.</span></span>
2.  <span data-ttu-id="77fc5-134">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-134">Select **New**.</span></span>
3.  <span data-ttu-id="77fc5-135">أدخل **الوقت الإضافي** في الحقل **المعرّف الرئيسي للتدقيق**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-135">Enter **Overtime** in the **Audit master ID** field.</span></span>
4.  <span data-ttu-id="77fc5-136">حدد **ناقل عبر الشاحنات** في حقل **شركة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-136">Select **TruckCarrier** in the **Shipping carrier** field.</span></span>
5.  <span data-ttu-id="77fc5-137">حدد **TL** في الحقل **نوع فاتورة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-137">Select **TL** in the **Freight bill type** field.</span></span>
6.  <span data-ttu-id="77fc5-138">في علامة التبويب السريعة **النتيجة**، حدد **OT** في الحقل **كود سبب الدفع بالزيادة**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-138">On the **Result** FastTab, select **OT** in the **Overpayment reason code** field.</span></span>
7.  <span data-ttu-id="77fc5-139">حدد **دعوى التلف** في الحقل **كود سبب الدفع بالنقصان**.</span><span class="sxs-lookup"><span data-stu-id="77fc5-139">Select **Damage claim** in the **Underpayment reason code** field.</span></span>
8.  <span data-ttu-id="77fc5-140">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="77fc5-140">Close the page.</span></span>

