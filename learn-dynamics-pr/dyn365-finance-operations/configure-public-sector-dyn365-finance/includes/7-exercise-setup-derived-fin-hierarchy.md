---
ms.openlocfilehash: 60b141aec7ad652dcc5bbd89cfac39f82a0a675d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070614"
---
> [!NOTE] 
> <span data-ttu-id="93935-101">يجب تنفيذ تدريب هذا المعمل في إطار متابعة تدريب المعمل السابق.</span><span class="sxs-lookup"><span data-stu-id="93935-101">This lab should be performed in continuation of the previous lab.</span></span> 

## <a name="create-a-category-hierarchy"></a><span data-ttu-id="93935-102">إنشاء تدرج هرمي للفئات</span><span class="sxs-lookup"><span data-stu-id="93935-102">Create a category hierarchy</span></span> 

1.  <span data-ttu-id="93935-103">في شركة USMF، انتقل إلى **إدارة معلومات المنتجات > إعداد > الفئات والسمات > التدرجات الهرمية للفئات**.</span><span class="sxs-lookup"><span data-stu-id="93935-103">In company USMF, go to **Product information management > Setup > Categories and attributes > Category hierarchies**.</span></span>
2.  <span data-ttu-id="93935-104">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="93935-104">Select **New**.</span></span>
3.  <span data-ttu-id="93935-105">في حقل **الاسم**، اكتب **GTL-Derived Hierarchy**.</span><span class="sxs-lookup"><span data-stu-id="93935-105">In the **Name** field, type **GTL-Derived Hierarchy**.</span></span>
4.  <span data-ttu-id="93935-106">في حقل **الوصف**، اكتب **Derived Hierarchy**.</span><span class="sxs-lookup"><span data-stu-id="93935-106">In the **Description** field, type **Derived Hierarchy**.</span></span>
5.  <span data-ttu-id="93935-107">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="93935-107">Select **Create**.</span></span>
6.  <span data-ttu-id="93935-108">حدد **عقدة فئة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="93935-108">Select **New category node**.</span></span>
7.  <span data-ttu-id="93935-109">في حقل **الاسم**، اكتب **GTL-Custom‎**.</span><span class="sxs-lookup"><span data-stu-id="93935-109">In the **Name** field, type **GTL-Custom**.</span></span>
8.  <span data-ttu-id="93935-110">في حقل **الكود**، اكتب **0819**.</span><span class="sxs-lookup"><span data-stu-id="93935-110">In the **Code** field, type **0819**.</span></span>
9.  <span data-ttu-id="93935-111">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="93935-111">Select **Save**.</span></span>
10.  <span data-ttu-id="93935-112">حدد **عقدة فئة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="93935-112">Select **New category node**.</span></span>
10. <span data-ttu-id="93935-113">في حقل **الاسم**، اكتب **GTL-Education‎**.</span><span class="sxs-lookup"><span data-stu-id="93935-113">In the **Name** field, type **GTL-Education**.</span></span>
11. <span data-ttu-id="93935-114">في حقل **الكود**، اكتب **08191**.</span><span class="sxs-lookup"><span data-stu-id="93935-114">In the **Code** field, type **08191**.</span></span>
12. <span data-ttu-id="93935-115">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="93935-115">Select **Save**.</span></span>
12. <span data-ttu-id="93935-116">في الجزء الأيمن، حدد **GTL-Custom**.</span><span class="sxs-lookup"><span data-stu-id="93935-116">Select **GTL-Custom** in the left pane.</span></span>
13. <span data-ttu-id="93935-117">حدد **عقدة فئة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="93935-117">Select **New category node**.</span></span>
14. <span data-ttu-id="93935-118">في حقل **الاسم**، اكتب **GTL-Public Service**.</span><span class="sxs-lookup"><span data-stu-id="93935-118">In the **Name** field, type **GTL-Public Service**.</span></span>
15. <span data-ttu-id="93935-119">في حقل **الكود**، اكتب **08192**.</span><span class="sxs-lookup"><span data-stu-id="93935-119">In the **Code** field, type **08192**.</span></span>
16. <span data-ttu-id="93935-120">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="93935-120">Select **Save**.</span></span>
17. <span data-ttu-id="93935-121">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="93935-121">Close all pages.</span></span>

## <a name="assign-the-derived-financial-hierarchy-category-type"></a><span data-ttu-id="93935-122">تعيين نوع فئة التدرج الهرمي المالي المشتق</span><span class="sxs-lookup"><span data-stu-id="93935-122">Assign the Derived financial hierarchy category type</span></span> 

1.  <span data-ttu-id="93935-123">انتقل إلى **إدارة معلومات المنتجات > إعداد > الفئات والسمات > إقرانات أدوار التدرج الهرمي للفئة**.</span><span class="sxs-lookup"><span data-stu-id="93935-123">Go to **Product information management > Setup > Categories and attributes > Category hierarchy role associations**.</span></span>
2.  <span data-ttu-id="93935-124">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="93935-124">Select **New**.</span></span>
3.  <span data-ttu-id="93935-125">في حقل **نوع التدرج الهرمي للفئة**، حدد **تدرجاً مالياً مشتقاً**.</span><span class="sxs-lookup"><span data-stu-id="93935-125">In the **Category hierarchy type** field, select **Derived financial hierarchy**.</span></span>
4.  <span data-ttu-id="93935-126">في حقل **التدرج الهرمي للفئة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="93935-126">In the **Category hierarchy** field, select the drop-down button to open the lookup.</span></span>
5.  <span data-ttu-id="93935-127">في القائمة، حدد التدرج الهرمي للفئة **GTL-Derived Hierarchy** للإقران مع نوع التدرج الهرمي المالي المشتق.</span><span class="sxs-lookup"><span data-stu-id="93935-127">In the list, select the Category hierarchy **GTL-Derived Hierarchy** to associate with the Derived financial hierarchy type.</span></span>
6.  <span data-ttu-id="93935-128">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="93935-128">Select **Save**.</span></span>
7.  <span data-ttu-id="93935-129">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="93935-129">Close the page.</span></span>

## <a name="associate-the-derived-financial-hierarchy-with-a-legal-entity"></a><span data-ttu-id="93935-130">إقران التدرج الهرمي المالي المشتق بكيان قانوني</span><span class="sxs-lookup"><span data-stu-id="93935-130">Associate the derived financial hierarchy with a legal entity</span></span> 

1.  <span data-ttu-id="93935-131">انتقل إلى **دفتر الأستاذ العام > مخطط الحسابات > الأبعاد > إقران التدرجات الهرمية المالية**.</span><span class="sxs-lookup"><span data-stu-id="93935-131">Go to **General ledger > Chart of accounts > Dimensions > Associate financial hierarchies**.</span></span>
2.  <span data-ttu-id="93935-132">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="93935-132">Select **New**.</span></span>
3.  <span data-ttu-id="93935-133">في حقل **الكيان القانوني**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="93935-133">In the **Legal entity** field, select the drop-down button to open the lookup.</span></span>
4.  <span data-ttu-id="93935-134">في القائمة، حدد الكيان القانوني لـ **USMF** للإقران مع نوع التدرج الهرمي المالي المشتق.</span><span class="sxs-lookup"><span data-stu-id="93935-134">In the list, select the **USMF** legal entity to associate with the derived financial hierarchy.</span></span>
5.  <span data-ttu-id="93935-135">في حقل **التدرج الهرمي المالي المشتق**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="93935-135">In the **Derived financial hierarchy** field, select the drop-down button to open the lookup.</span></span>
6.  <span data-ttu-id="93935-136">في القائمة، حدد التدرج الهرمي المالي المشتق لـ **GTL-Derived Hierarchy** للإقران مع الكيان القانوني.</span><span class="sxs-lookup"><span data-stu-id="93935-136">In the list, select the **GTL-Derived Hierarchy** derived financial hierarchy to associate with the legal entity.</span></span>
7.  <span data-ttu-id="93935-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="93935-137">Select **Save**.</span></span>
8.  <span data-ttu-id="93935-138">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="93935-138">Close the page.</span></span>

## <a name="create-filter-rules-for-the-derived-financial-hierarchy"></a><span data-ttu-id="93935-139">إنشاء قواعد التصفية للتدرج الهرمي المالي المشتق</span><span class="sxs-lookup"><span data-stu-id="93935-139">Create filter rules for the derived financial hierarchy</span></span> 

1.  <span data-ttu-id="93935-140">انتقل إلى **دفتر الأستاذ العام > مخطط الحسابات > الأبعاد > التدرجات الهرمية المالية المشتقة**.</span><span class="sxs-lookup"><span data-stu-id="93935-140">Go to **General ledger > Chart of accounts > Dimensions > Derived financial hierarchies**.</span></span>
2.  <span data-ttu-id="93935-141">في حقل **التدرج الهرمي المالي المشتق**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="93935-141">In the **Derived financial hierarchy** field, select the drop-down button to open the lookup.</span></span>
3.  <span data-ttu-id="93935-142">في القائمة، حدد **GTL-Derived Hierarchy** لإنشاء قواعد عامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="93935-142">In the list, select the **GTL-Derived Hierarchy** for which to create filter rules.</span></span>
4.  <span data-ttu-id="93935-143">في الشجرة، حدد **GTL-Education.**</span><span class="sxs-lookup"><span data-stu-id="93935-143">In the tree, select **GTL-Education.**</span></span>
5.  <span data-ttu-id="93935-144">حدد **تحرير عامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="93935-144">Select **Edit filter**.</span></span>
6.  <span data-ttu-id="93935-145">حدد **إضافة معايير جديدة** للبدء في إضافة القواعد إلى عامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="93935-145">Select **Add new criteria** to begin adding rules to the filter.</span></span> <span data-ttu-id="93935-146">على سبيل المثال، لديك قاعدة يكون فيها Department هو "بين" ويتضمن 024 إلى 029.</span><span class="sxs-lookup"><span data-stu-id="93935-146">For example, have a rule where Department is between and includes 024 through 029.</span></span>
7.  <span data-ttu-id="93935-147">بعد قيامك بإضافة كافة المعايير، حدد **تنشيط عامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="93935-147">After you've added all criteria, select **Activate filter**.</span></span>
8.  <span data-ttu-id="93935-148">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="93935-148">Close the page.</span></span>
