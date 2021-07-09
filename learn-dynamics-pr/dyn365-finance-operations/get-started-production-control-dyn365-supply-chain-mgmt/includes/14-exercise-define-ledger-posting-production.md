---
ms.openlocfilehash: b55e6d55919dfb2c38aecc1599070eb9c5062537
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6072985"
---
## <a name="scenario"></a><span data-ttu-id="40e69-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="40e69-101">Scenario</span></span>
<span data-ttu-id="40e69-102">في هذا المعمل، ستقوم بإنشاء مجموعة أصناف جديدة لأصناف دراجة وتكوين ترحيل دفتر الأستاذ لأوامر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="40e69-102">In this lab, you will create a new item group for bicycle items and configure the ledger posting for production orders.</span></span> 


- <span data-ttu-id="40e69-103">سيكون حساب المخزون المستخدم للدراجات الجيدة المنتهية الجديدة هو رقم مخزون السلع المنتهية 140200.</span><span class="sxs-lookup"><span data-stu-id="40e69-103">The inventory account that is used for the new finished good bicycles will be the Finished goods inventory account number 140200.</span></span> 
- <span data-ttu-id="40e69-104">سيكون حساب الأعمال تحت التنفيذ هو رقم حساب المواد القابل للأعمال تحت التنفيذ 150150.</span><span class="sxs-lookup"><span data-stu-id="40e69-104">The WIP account will be the Production WIP-material account number 150150.</span></span> 

<span data-ttu-id="40e69-105">باستخدام المعلومات المتوفرة، قم بإنشاء مجموعة الأصناف وتكوين ترحيلات أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="40e69-105">By using the information provided, create the item group and configure the production order postings.</span></span>

## <a name="create-an-item-group-for-bicycles"></a><span data-ttu-id="40e69-106">إنشاء مجموعة أصناف للدراجات</span><span class="sxs-lookup"><span data-stu-id="40e69-106">Create an item group for bicycles</span></span> 

1.  <span data-ttu-id="40e69-107">افتح **إدارة المخزون > إعداد > المخزون > مجموعات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="40e69-107">Open **Inventory management > Setup > Inventory > Item groups**.</span></span>
2.  <span data-ttu-id="40e69-108">حدد **جديد** لإنشاء مجموعة صنف جديدة.</span><span class="sxs-lookup"><span data-stu-id="40e69-108">Select **New** to create a new item group.</span></span>
3.  <span data-ttu-id="40e69-109">أدخل **دراجة** في الحقل **مجموعة الصنف**.</span><span class="sxs-lookup"><span data-stu-id="40e69-109">Enter **Bicycle** in the **Item group** field.</span></span>
4.  <span data-ttu-id="40e69-110">أدخل **سلع الدراجات المنتهية** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="40e69-110">Enter **Bicycle Finished Goods** in the **Name** field.</span></span>
5.  <span data-ttu-id="40e69-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="40e69-111">Close the page.</span></span>


## <a name="configure-the-finished-goods-inventory-accounts-for-production-postings"></a><span data-ttu-id="40e69-112">تكوين حسابات مخزون البضائع المنتهية لعمليات ترحيل الإنتاج</span><span class="sxs-lookup"><span data-stu-id="40e69-112">Configure the finished goods inventory accounts for production postings</span></span> 

1.  <span data-ttu-id="40e69-113">افتح **إعداد > إعداد > ترحيل > ترحيل**</span><span class="sxs-lookup"><span data-stu-id="40e69-113">Open **Inventory management > Setup > Posting > Posting**.</span></span>
2.  <span data-ttu-id="40e69-114">حدد علامة التبويب **الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="40e69-114">Select the **Production** tab.</span></span>
3.  <span data-ttu-id="40e69-115">حدد زر **التكلفة المقدرة للمواد المستهلكة** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-115">Select the **Estimated cost of materials consumed** button on the left pane.</span></span>
4.  <span data-ttu-id="40e69-116">حدد **جديد** لإضافة صف.</span><span class="sxs-lookup"><span data-stu-id="40e69-116">Select **New** to add a row.</span></span>
5.  <span data-ttu-id="40e69-117">في حقل **كود الصنف**، حدد **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-117">Select **Group** in the **Item code** field.</span></span>
6.  <span data-ttu-id="40e69-118">في حقل **علاقة الصنف**، حدد **دراجة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-118">Select **Bicycle** in the **Item relation** field.</span></span>
7.  <span data-ttu-id="40e69-119">في الحقل **الحساب الرئيسي**، أدخل **140200**.</span><span class="sxs-lookup"><span data-stu-id="40e69-119">Select **140200** in the **Main account** field.</span></span>
8.  <span data-ttu-id="40e69-120">حدد زر **التكلفة المقدرة للتصنيع** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-120">Select the **Estimated manufactured cost** button on the left pane.</span></span>
9.  <span data-ttu-id="40e69-121">حدد **جديد** لإضافة صف.</span><span class="sxs-lookup"><span data-stu-id="40e69-121">Select **New** to add a row.</span></span>
10. <span data-ttu-id="40e69-122">في حقل **كود الصنف**، حدد **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-122">Select **Group** in the **Item code** field.</span></span>
11. <span data-ttu-id="40e69-123">في حقل **علاقة الصنف**، حدد **دراجة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-123">Select **Bicycle** in the **Item relation** field.</span></span>
12. <span data-ttu-id="40e69-124">في الحقل **الحساب الرئيسي**، أدخل **140200**.</span><span class="sxs-lookup"><span data-stu-id="40e69-124">Select **140200** in the **Main account** field.</span></span>
13. <span data-ttu-id="40e69-125">حدد زر **تكلفة المواد المستهلكة** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-125">Select the **Cost of materials consumed** button on the left pane.</span></span>
14. <span data-ttu-id="40e69-126">حدد **جديد** لإضافة صف.</span><span class="sxs-lookup"><span data-stu-id="40e69-126">Select **New** to add a row.</span></span>
15. <span data-ttu-id="40e69-127">في حقل **كود الصنف**، حدد **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-127">Select **Group** in the **Item code** field.</span></span>
16. <span data-ttu-id="40e69-128">في حقل **علاقة الصنف**، حدد **دراجة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-128">Select **Bicycle** in the **Item relation** field.</span></span>
17. <span data-ttu-id="40e69-129">في الحقل **الحساب الرئيسي**، أدخل **140200**.</span><span class="sxs-lookup"><span data-stu-id="40e69-129">Select **140200** in the **Main account** field.</span></span>
18. <span data-ttu-id="40e69-130">حدد زر **تكلفة التصنيع** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-130">Select the **Manufactured cost** button on the left pane.</span></span>
19. <span data-ttu-id="40e69-131">حدد **جديد** لإضافة صف.</span><span class="sxs-lookup"><span data-stu-id="40e69-131">Select **New** to add a row.</span></span>
20. <span data-ttu-id="40e69-132">في حقل **كود الصنف**، حدد **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-132">Select **Group** in the **Item code** field.</span></span>
21. <span data-ttu-id="40e69-133">في حقل **علاقة الصنف**، حدد **دراجة**.</span><span class="sxs-lookup"><span data-stu-id="40e69-133">Select **Bicycle** in the **Item relation** field.</span></span>
22. <span data-ttu-id="40e69-134">في الحقل **الحساب الرئيسي**، أدخل **140200**.</span><span class="sxs-lookup"><span data-stu-id="40e69-134">Select **140200** in the **Main account** field.</span></span>
23. <span data-ttu-id="40e69-135">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="40e69-135">Close the page.</span></span>

## <a name="configure-the-production-wip-material-account-for-production-postings"></a><span data-ttu-id="40e69-136">تكوين إنتاج حساب مواد الأعمال تحت التنفيذ لترحيلات الإنتاج</span><span class="sxs-lookup"><span data-stu-id="40e69-136">Configure the production WIP-material account for production postings</span></span> 

1.  <span data-ttu-id="40e69-137">افتح **إعداد > إعداد > ترحيل > ترحيل**</span><span class="sxs-lookup"><span data-stu-id="40e69-137">Open **Inventory management > Setup > Posting > Posting**.</span></span>
2.  <span data-ttu-id="40e69-138">حدد علامة التبويب **الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="40e69-138">Select the **Production** tab.</span></span>
3.  <span data-ttu-id="40e69-139">حدد زر **التكلفة المقدرة للمواد المستهلكة، الأعمال تحت التنفيذ** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-139">Select the **Estimated cost of materials consumed, WIP** button on the left pane.</span></span>
4.  <span data-ttu-id="40e69-140">تحقق من أن تكوين الصف هو **الكل** في الحقل **كود الصنف** و **الحساب الرئيسي** هو **150150**.</span><span class="sxs-lookup"><span data-stu-id="40e69-140">Verify that the row is configured for **All** in the **Item code** field and the **Main account** is **150150**.</span></span>
5.  <span data-ttu-id="40e69-141">حدد زر **التكلفة المقدرة للتصنيع، الأعمال تحت التنفيذ** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-141">Select the **Estimated manufactured cost, WIP** button on the left pane.</span></span>
6.  <span data-ttu-id="40e69-142">تحقق من أن تكوين الصف هو **الكل** في الحقل **كود الصنف** و **الحساب الرئيسي** هو **150150**.</span><span class="sxs-lookup"><span data-stu-id="40e69-142">Verify that the row is configured for **All** in the **Item code** field and the **Main account** is **150150**.</span></span>
7.  <span data-ttu-id="40e69-143">حدد زر **تكلفة المواد المستهلكة، الأعمال تحت التنفيذ** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-143">Select the **Cost of materials consumed, WIP** button on the left pane.</span></span>
8.  <span data-ttu-id="40e69-144">تحقق من أن تكوين الصف هو **الكل** في الحقل **كود الصنف** و **الحساب الرئيسي** هو **150100**.</span><span class="sxs-lookup"><span data-stu-id="40e69-144">Verify that the row is configured for **All** in the **Item code** field and the **Main account** is **150100**.</span></span>
9.  <span data-ttu-id="40e69-145">حدد زر **تكلفة التصنيع، الأعمال تحت التنفيذ** في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="40e69-145">Select the **Manufactured cost, WIP** button on the left pane.</span></span>
10. <span data-ttu-id="40e69-146">تحقق من أن تكوين الصف هو **الكل** في الحقل **كود الصنف** و **الحساب الرئيسي** هو **150100**.</span><span class="sxs-lookup"><span data-stu-id="40e69-146">Verify that the row is configured for **All** in the **Item code** field and the **Main account** is **150100**.</span></span>
11. <span data-ttu-id="40e69-147">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="40e69-147">Close the page.</span></span>

