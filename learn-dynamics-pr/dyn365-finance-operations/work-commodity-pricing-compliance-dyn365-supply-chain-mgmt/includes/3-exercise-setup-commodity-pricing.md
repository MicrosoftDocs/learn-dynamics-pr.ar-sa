---
ms.openlocfilehash: 967c4b3aeb1366b5f75cd26d53dedd652051d15a
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073096"
---

<span data-ttu-id="860b9-101">في الشركة USP2، يتم تعقب سعر التفاح (جزء M9103) استناداً إلى تسعير تبادل السلع NYMEX الخاص بالتفاح.</span><span class="sxs-lookup"><span data-stu-id="860b9-101">In company USP2, the price of apples (part M9103) is to be tracked based on the NYMEX commodity exchange pricing of apples.</span></span> <span data-ttu-id="860b9-102">يجب أن يعتمد سعر المبيعات لصوص التفاح (الجزء P9100)، الذي يتم تصنيعه من هذا التفاح، على هامش يبلغ 45 بالمائة ومضاعف التكلفة 1.25 لكافة الكميات.</span><span class="sxs-lookup"><span data-stu-id="860b9-102">The sales price of apple sauce (part P9100), which is manufactured from this apple, should be based on a margin of 45 percent and a cost multiple of 1.25 for all quantities.</span></span>
<span data-ttu-id="860b9-103">وبصفتك موظف تسعير في الشركة، فسوف تقوم بإعداد أساس التكلفة وقالب التسعير لهذا السيناريو.</span><span class="sxs-lookup"><span data-stu-id="860b9-103">As the pricing employee in the company, you will set up the cost basis and pricing template for this scenario.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="860b9-104">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="860b9-104">Before you begin</span></span>
<span data-ttu-id="860b9-105">للاستفادة إلى أقصى حد من هذه التدريبات وغيرها في هذه الوحدة، نوصي بأن يكون لديك بيانات العينة القياسية المتوفرة في Supply Chain Management والتي تم تثبيتها باستخدام Lifecycle Services‎‏ (LCS)‏‏‏‎.</span><span class="sxs-lookup"><span data-stu-id="860b9-105">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data available in Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

## <a name="configure-an-item"></a><span data-ttu-id="860b9-106">تكوين صنف</span><span class="sxs-lookup"><span data-stu-id="860b9-106">Configure an item</span></span>
1.    <span data-ttu-id="860b9-107">في الشركة USP2، انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="860b9-107">In company USP2, go to **Product information management > Products > Released products**.</span></span>
2.    <span data-ttu-id="860b9-108">استخدم **عامل التصفية السريع** للتصفية في حقل **رقم الصنف** بقيمة **P9100**.</span><span class="sxs-lookup"><span data-stu-id="860b9-108">Use the **Quick Filter** to filter on the **Item number** field with a value of **P9100**.</span></span>
3.    <span data-ttu-id="860b9-109">في جزء الإجراء، حدد **إدارة المخزون**.</span><span class="sxs-lookup"><span data-stu-id="860b9-109">On the Action Pane, select **Manage inventory**.</span></span>
4.    <span data-ttu-id="860b9-110">حدد **إعدادات الأمر الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="860b9-110">Select **Default order settings**.</span></span>
5.    <span data-ttu-id="860b9-111">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="860b9-111">Select **Edit**.</span></span>
6.    <span data-ttu-id="860b9-112">في حقل **نوع الأمر الافتراضي**، حدد **الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="860b9-112">In the **Default order type** field, select **Production**.</span></span>
7.    <span data-ttu-id="860b9-113">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="860b9-113">Select **Save**.</span></span>
8.    <span data-ttu-id="860b9-114">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="860b9-114">Close all pages.</span></span>


## <a name="create-a-cost-basis"></a><span data-ttu-id="860b9-115">إنشاء أساس تكلفة</span><span class="sxs-lookup"><span data-stu-id="860b9-115">Create a cost basis</span></span>

1.  <span data-ttu-id="860b9-116">انتقل إلى **إدارة المخزون > الإعداد > تسعير السلعة > نوع أساس التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="860b9-116">Go to **Inventory management > Setup > Commodity pricing > Cost basis type**.</span></span>
2.  <span data-ttu-id="860b9-117">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="860b9-117">Select **New**.</span></span>
3.  <span data-ttu-id="860b9-118">في حقل **نوع أساس التكلفة**، أدخل **NYMEX**.</span><span class="sxs-lookup"><span data-stu-id="860b9-118">In the **Cost basis type** field, enter **NYMEX**.</span></span>
4.  <span data-ttu-id="860b9-119">في حقل **الوصف**، أدخل **بورصة نيويورك التجارية**.</span><span class="sxs-lookup"><span data-stu-id="860b9-119">In the **Description** field, enter **New York Mercantile Exchange**.</span></span>
5.  <span data-ttu-id="860b9-120">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="860b9-120">Select **Save**.</span></span>
6.  <span data-ttu-id="860b9-121">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="860b9-121">Close the page.</span></span>

## <a name="create-a-pricing-template"></a><span data-ttu-id="860b9-122">إنشاء قالب تسعير</span><span class="sxs-lookup"><span data-stu-id="860b9-122">Create a pricing template</span></span>

1.  <span data-ttu-id="860b9-123">انتقل إلى **إدارة المخزون > الإعداد > تسعير السلعة > قالب التسعير**.</span><span class="sxs-lookup"><span data-stu-id="860b9-123">Go to **Inventory management > Setup > Commodity pricing > Pricing template**.</span></span>
2.  <span data-ttu-id="860b9-124">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="860b9-124">Select **New**.</span></span>
3.  <span data-ttu-id="860b9-125">في حقل **قالب التسعير**، أدخل **تفاح**.</span><span class="sxs-lookup"><span data-stu-id="860b9-125">In the **Pricing template** field, enter **Apples**.</span></span>
4.  <span data-ttu-id="860b9-126">في الحقل **وصف**، أدخل **تفاح**.</span><span class="sxs-lookup"><span data-stu-id="860b9-126">In the **Description** field, enter **Apples**.</span></span>
5.  <span data-ttu-id="860b9-127">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="860b9-127">Select **Save**.</span></span>

## <a name="create-a-quantity-and-margin-template"></a><span data-ttu-id="860b9-128">إنشاء قالب الكمية والهامش</span><span class="sxs-lookup"><span data-stu-id="860b9-128">Create a Quantity and margin template</span></span>

1.  <span data-ttu-id="860b9-129">حدد **إنشاء قالب الكمية والهامش**.</span><span class="sxs-lookup"><span data-stu-id="860b9-129">Select **Quantity and margin template**.</span></span>
2.  <span data-ttu-id="860b9-130">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="860b9-130">Select **New**.</span></span>
3.  <span data-ttu-id="860b9-131">في حقل **علاقة الصنف**، أدخل **P9100**.</span><span class="sxs-lookup"><span data-stu-id="860b9-131">In the **Item relation** field, enter **P9100**.</span></span>
4.  <span data-ttu-id="860b9-132">في حقل **الموقع**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="860b9-132">In the **Site** field, enter **1**.</span></span>
5. <span data-ttu-id="860b9-133">قم بتعيين **مضاعف التكلفة** إلى **1.25**.</span><span class="sxs-lookup"><span data-stu-id="860b9-133">Set **Cost multiplier** to **1.25**.</span></span>
6. <span data-ttu-id="860b9-134">قم بتعيين **النسبة المئوية للهامش** إلى **45**.</span><span class="sxs-lookup"><span data-stu-id="860b9-134">Set **Margin percentage** to **45**.</span></span>
7. <span data-ttu-id="860b9-135">افتح علامة التبويب السريعة **البُعد**.</span><span class="sxs-lookup"><span data-stu-id="860b9-135">Open the **Dimension** FastTab.</span></span>
8. <span data-ttu-id="860b9-136">في الحقل **المستودع**، أدخل **12**.</span><span class="sxs-lookup"><span data-stu-id="860b9-136">In the **Warehouse** field, enter **12**.</span></span>
9. <span data-ttu-id="860b9-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="860b9-137">Select **Save**.</span></span>
10. <span data-ttu-id="860b9-138">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="860b9-138">Close the page.</span></span>

## <a name="complete-the-inventory-parameter-setup"></a><span data-ttu-id="860b9-139">أكمل إعداد معلمة المخزون</span><span class="sxs-lookup"><span data-stu-id="860b9-139">Complete the inventory parameter setup</span></span>

1.  <span data-ttu-id="860b9-140">انتقل إلى **إدارة المخزون > الإعداد > معلمات إدارة المستودع والمخزون**.</span><span class="sxs-lookup"><span data-stu-id="860b9-140">Go to **Inventory management > Setup > Inventory and warehouse management parameters**.</span></span>
2.  <span data-ttu-id="860b9-141">حدد علامة تبويب **تسعير السلعة**.</span><span class="sxs-lookup"><span data-stu-id="860b9-141">Select the **Commodity pricing** tab.</span></span>
3.  <span data-ttu-id="860b9-142">في حقل **مجموعة الأبعاد**، أدخل قيمة أو حددها، مثل **مركز التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="860b9-142">In the **Dimension set** field, enter or select a value, such as **Cost Center**.</span></span>
4.  <span data-ttu-id="860b9-143">في حقل **نوع أساس التكلفة**، حدد **NYMEX**.</span><span class="sxs-lookup"><span data-stu-id="860b9-143">In the **Cost basis type** field, select **NYMEX**.</span></span>
5.  <span data-ttu-id="860b9-144">حدد **نعم** في مفتاح تبديل **الاحتفاظ بحسابات قائمة مكونات الصنف/الصيغة**.</span><span class="sxs-lookup"><span data-stu-id="860b9-144">Select **Yes** in the **Keep BOM/Formula calculations** toggle key.</span></span>
6.  <span data-ttu-id="860b9-145">حدد **تفاح** في **قالب التسعير**.</span><span class="sxs-lookup"><span data-stu-id="860b9-145">Select **Apples** in the **Pricing template**.</span></span>
7.  <span data-ttu-id="860b9-146">حدد **السعر** في حقل **الاتفاقية التجارية**.</span><span class="sxs-lookup"><span data-stu-id="860b9-146">Select **Price** in the **Trade Agreement** field.</span></span>
6.  <span data-ttu-id="860b9-147">حدد ارتباط **السعر** للوصول إلى شاشة **أسماء دفاتر يومية الاتفاقيات التجارية**.</span><span class="sxs-lookup"><span data-stu-id="860b9-147">Select the **Price** link to access the **Trade agreement journal names** screen.</span></span>
7.  <span data-ttu-id="860b9-148">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="860b9-148">Select **New**.</span></span>
8.  <span data-ttu-id="860b9-149">في حقل **الاسم**، أدخِل **Price_S**.</span><span class="sxs-lookup"><span data-stu-id="860b9-149">In the **Name** field, enter **Price_S**.</span></span>
9.  <span data-ttu-id="860b9-150">في حقل **الوصف**، أدخل **دفتر يومية تعديل سعر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="860b9-150">In the **Description** field, enter **Sales Price Adjustment Journal**.</span></span>
10. <span data-ttu-id="860b9-151">في الحقل **العلاقة**، حدد **السعر (مبيعات)**.</span><span class="sxs-lookup"><span data-stu-id="860b9-151">In the **Relation** field, select **Price (sales)**.</span></span>
11. <span data-ttu-id="860b9-152">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="860b9-152">Select **Save**.</span></span>
12. <span data-ttu-id="860b9-153">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="860b9-153">Close the page.</span></span>
13. <span data-ttu-id="860b9-154">في حقل **الاتفاقية التجارية**، حدد **Price_S**.</span><span class="sxs-lookup"><span data-stu-id="860b9-154">In the **Trade agreement** field, enter or select **Price_S**.</span></span>
14. <span data-ttu-id="860b9-155">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="860b9-155">Select **Save**.</span></span>
15. <span data-ttu-id="860b9-156">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="860b9-156">Close the page.</span></span> 
