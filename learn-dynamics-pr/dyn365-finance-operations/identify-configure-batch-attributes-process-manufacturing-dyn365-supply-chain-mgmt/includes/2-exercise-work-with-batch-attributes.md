---
ms.openlocfilehash: 6ffca2f325e28cfad7f965138afa911b628c7192
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073446"
---
## <a name="before-you-begin"></a><span data-ttu-id="d3543-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="d3543-101">Before you begin</span></span>
<span data-ttu-id="d3543-102">للحصول على أقصى استفادة من هذا التدريب، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Supply Chain Management والتي يتم تثبيتها باستخدام Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="d3543-102">To get the most benefit from this exercise, we recommend that you have the standard sample data available in Dynamics 365 Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

<span data-ttu-id="d3543-103">في شركة USPI، هناك حاجة إلى متطلب جديد للقطعة P4000، وهي حبيبات البولي بروبيلين، لاختبار نقطة الانصهار لكل دفعة وتسجيلها.</span><span class="sxs-lookup"><span data-stu-id="d3543-103">In the USPI company, a new requirement for part P4000, Polypropylene Pellets, is needed to test and record the melting point for each batch.</span></span> <span data-ttu-id="d3543-104">بصفتك موظف تعريف المنتج، فأنت بحاجة إلى إنشاء سمة الدُفعة لنقطة الانصهار كسمة عدد صحيح بحد أدنى 145 درجة مئوية وحد أقصى 175 درجة مئوية.</span><span class="sxs-lookup"><span data-stu-id="d3543-104">As the product definition employee, you need to create the batch attribute for melting point as an integer attribute with a min of 145° C and a max of 175° C.</span></span>

## <a name="create-a-new-batch-attribute"></a><span data-ttu-id="d3543-105">إنشاء سمة دفعة جديدة</span><span class="sxs-lookup"><span data-stu-id="d3543-105">Create a new batch attribute</span></span>

1.  <span data-ttu-id="d3543-106">انتقل إلى **إدارة معلومات المنتج > الإعداد > الفئات والسمات > سمات الدُفعة**.</span><span class="sxs-lookup"><span data-stu-id="d3543-106">Go to **Product information management > Setup > Categories and attributes > Batch attributes**.</span></span>

2.  <span data-ttu-id="d3543-107">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="d3543-107">Select **New**.</span></span>

3.  <span data-ttu-id="d3543-108">في حقل **السمة**، أدخل **MeltingPoint‎**.</span><span class="sxs-lookup"><span data-stu-id="d3543-108">In the **Attribute** field, enter **MeltingPoint**.</span></span>

4.  <span data-ttu-id="d3543-109">في حقل **الوصف**، أدخِل **نقطة الانصهار (ج)**.</span><span class="sxs-lookup"><span data-stu-id="d3543-109">In the **Description** field, enter **Melting Point (C)**.</span></span>

5.  <span data-ttu-id="d3543-110">في حقل **نوع السمة**، حدد الخيار **عدد صحيح**.</span><span class="sxs-lookup"><span data-stu-id="d3543-110">In the **Attribute type** field, select **Integer**.</span></span> <span data-ttu-id="d3543-111">قم بتعيين حقلي **الحد الأدنى للسمة** و **الحد الأقصى**.</span><span class="sxs-lookup"><span data-stu-id="d3543-111">Set the **Attribute MIN** and **MAX** fields.</span></span> 

6.  <span data-ttu-id="d3543-112">في حقل **الحد الأدنى**، أدخل **145**.</span><span class="sxs-lookup"><span data-stu-id="d3543-112">In the **Minimum** field, enter **145**.</span></span>

7.  <span data-ttu-id="d3543-113">في حقل **الحد الأقصى**، أدخل **175**.</span><span class="sxs-lookup"><span data-stu-id="d3543-113">In the **Maximum** field, enter **175**.</span></span>

8.  <span data-ttu-id="d3543-114">في حقل **الزيادة**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="d3543-114">In the **Increment** field, enter **1**.</span></span>

9.  <span data-ttu-id="d3543-115">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d3543-115">Select **Save**.</span></span>

10. <span data-ttu-id="d3543-116">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="d3543-116">Close the page.</span></span>

## <a name="assign-a-batch-attribute"></a><span data-ttu-id="d3543-117">تعيين سمة الدفعة</span><span class="sxs-lookup"><span data-stu-id="d3543-117">Assign a batch attribute</span></span> 

<span data-ttu-id="d3543-118">في شركة USPI، هناك حاجة إلى متطلب جديد للقطعة P4000، وهي حبيبات البولي بروبيلين، لاختبار نقطة الانصهار لكل دفعة وتسجيلها.</span><span class="sxs-lookup"><span data-stu-id="d3543-118">In the USPI company, a new requirement for part P4000, Polypropylene Pellets, is needed to test and record the melting point for each batch.</span></span> 

<span data-ttu-id="d3543-119">تتمثل المتطلبات الخاصة بالصنف في توفير 130-171 درجة مئوية. يتطلب العميل US-024 نقطة انصهار تبلغ 135-165 درجة مئوية للاستخدام في عمليات التصنيع الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="d3543-119">The item-specific requirements are 130 - 171° C. Customer US-024 requires a melting point of 135 - 165° C for use in their manufacturing processes.</span></span> 

<span data-ttu-id="d3543-120">بصفتك موظف تعريف المنتج، تحتاج إلى ربط سمة الدُفعة بالصنف والعميل بنطاقات السمات الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="d3543-120">As the product definition employee, you need to associate the batch attribute with the item and the customer with the correct attribute ranges.</span></span>

### <a name="associate-a-batch-attribute-to-the-item"></a><span data-ttu-id="d3543-121">إقران سمة الدفعة للصنف</span><span class="sxs-lookup"><span data-stu-id="d3543-121">Associate a batch attribute to the item</span></span>

1.  <span data-ttu-id="d3543-122">انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="d3543-122">Go to **Product information management > Products >   Released products**.</span></span>

2.  <span data-ttu-id="d3543-123">استخدم **عامل التصفية السريع** للتصفية في حقل **رقم الصنف** بقيمة **P4000**.</span><span class="sxs-lookup"><span data-stu-id="d3543-123">Use the **Quick Filter** to filter on the **Item number** field with a value of **P4000**.</span></span>

3.  <span data-ttu-id="d3543-124">حدد **خاص بالمنتج** في المجموعة **سمات الدفعة** بعلامة التبويب **إدارة المخزون**.</span><span class="sxs-lookup"><span data-stu-id="d3543-124">Select **Product specific** in the **Batch Attributes** group on the **Manage Inventory** tab.</span></span>

4.  <span data-ttu-id="d3543-125">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="d3543-125">Select **New**.</span></span>

5.  <span data-ttu-id="d3543-126">في الحقل **علاقة السمة**، حدد **نقطة الانصهار**.</span><span class="sxs-lookup"><span data-stu-id="d3543-126">In the **Attribute relation** field, select **Melting Point**.</span></span> <span data-ttu-id="d3543-127">قم بتعيين حقلي **الحد الأدنى لسمة الصنف** و **الحد الأقصى**.</span><span class="sxs-lookup"><span data-stu-id="d3543-127">Set the **Item Attribute MIN** and **MAX** fields.</span></span>

6.  <span data-ttu-id="d3543-128">في حقل **إجراء السماح**، حدد **غير مسموح به**.</span><span class="sxs-lookup"><span data-stu-id="d3543-128">In the **Tolerance action** field, select **Not allowed**.</span></span>

7.  <span data-ttu-id="d3543-129">عيّن **الحد الأدنى** إلى **130**.</span><span class="sxs-lookup"><span data-stu-id="d3543-129">Set **Minimum** to **130**.</span></span>

8.  <span data-ttu-id="d3543-130">عيّن **الحد الأقصى** إلى **171**.</span><span class="sxs-lookup"><span data-stu-id="d3543-130">Set **Maximum** to **171**.</span></span>

9.  <span data-ttu-id="d3543-131">في حقل **الهدف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="d3543-131">In the **Target** field, enter a value.</span></span>

10. <span data-ttu-id="d3543-132">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d3543-132">Select **Save**.</span></span>
 

### <a name="associate-a-batch-attribute-to-the-customer"></a><span data-ttu-id="d3543-133">إقران سمة الدفعة للعميل</span><span class="sxs-lookup"><span data-stu-id="d3543-133">Associate a batch attribute to the customer</span></span>

1. <span data-ttu-id="d3543-134">قم بتحديث صفحة **المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="d3543-134">Refresh the **Released products** page.</span></span>

2. <span data-ttu-id="d3543-135">حدد **خاص بالعميل** في المجموعة **سمات الدفعة** بعلامة التبويب **إدارة المخزون**.</span><span class="sxs-lookup"><span data-stu-id="d3543-135">Select **Customer specific** in the **Batch Attributes** group on the **Manage Inventory** tab.</span></span>

3. <span data-ttu-id="d3543-136">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="d3543-136">Select **New**.</span></span>

4. <span data-ttu-id="d3543-137">في الحقل **علاقة السمة**، أدخل أو حدد **نقطة الانصهار**.</span><span class="sxs-lookup"><span data-stu-id="d3543-137">In the **Attribute relation** field, enter or select **Melting Point**.</span></span>

5. <span data-ttu-id="d3543-138">في الحقل **تحديد العميل**، أدخل **US-024**.</span><span class="sxs-lookup"><span data-stu-id="d3543-138">In the **Account selection** field, enter **US-024**.</span></span>  <span data-ttu-id="d3543-139">قم بتعيين حقلي **الحد الأدنى لسمة العميل** و **الحد الأقصى**.</span><span class="sxs-lookup"><span data-stu-id="d3543-139">Set the **Customer Attribute MIN** and **MAX** fields.</span></span>

6. <span data-ttu-id="d3543-140">عيّن **الحد الأدنى** إلى **135**.</span><span class="sxs-lookup"><span data-stu-id="d3543-140">Set **Minimum** to **135**.</span></span>

7. <span data-ttu-id="d3543-141">عيّن **الحد الأقصى** إلى **165**.</span><span class="sxs-lookup"><span data-stu-id="d3543-141">Set **Maximum** to **165**.</span></span>

8. <span data-ttu-id="d3543-142">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d3543-142">Select **Save**.</span></span>

9. <span data-ttu-id="d3543-143">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="d3543-143">Close the page.</span></span>

