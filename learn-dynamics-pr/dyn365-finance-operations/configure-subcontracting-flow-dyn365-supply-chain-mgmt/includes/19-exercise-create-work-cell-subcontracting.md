---
ms.openlocfilehash: 0d1ff97f3d760db804558266631ee93bbfdf41a5
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073311"
---
> [!NOTE]
> <span data-ttu-id="519c8-101">قبل أن تبدأ هذا التدريب، يجب أن تكون قد أكملت التدريب السابق، **إعداد مورد افتراضي وإنشاء اتفاقية شراء**.</span><span class="sxs-lookup"><span data-stu-id="519c8-101">Before you begin this exercise, you must have completed the previous exercise, **Set up a default vendor and create a purchase agreement**.</span></span>

## <a name="scenario"></a><span data-ttu-id="519c8-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="519c8-102">Scenario</span></span>
<span data-ttu-id="519c8-103">في هذا التدريب، ستقوم بإنشاء خلية عمل للتعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="519c8-103">In this exercise you will create a work cell for subcontracting.</span></span>  <span data-ttu-id="519c8-104">لتكوين خلية عمل على أنها متعاقد عليها من الباطن، يجب إنشاء مَورد نوع المُورّد وربطه بخلية العمل (مجموعة الموارد).</span><span class="sxs-lookup"><span data-stu-id="519c8-104">To configure a work cell as subcontracted, a resource of the vendor type needs to be created and associated with the work cell (resource group).</span></span>

1.  <span data-ttu-id="519c8-105">انتقل إلى **التحكم في الإنتاج > إعداد > الموارد > الموارد**</span><span class="sxs-lookup"><span data-stu-id="519c8-105">Go to **Production control > Setup > Resources > Resources**.</span></span>
2.  <span data-ttu-id="519c8-106">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-106">Select **New**.</span></span>
3.  <span data-ttu-id="519c8-107">في الحقل **مورد**، أدخل **GTL-Sub1**.</span><span class="sxs-lookup"><span data-stu-id="519c8-107">In the **Resource** field, enter **GTL-Sub1**.</span></span>
4.  <span data-ttu-id="519c8-108">في الحقل **وصف**، أدخل **مقاول من الباطن 1**.</span><span class="sxs-lookup"><span data-stu-id="519c8-108">In the **Description** field, enter **Subcontractor 1**.</span></span>
5.  <span data-ttu-id="519c8-109">في الحقل **نوع**، حدد **مورد**.</span><span class="sxs-lookup"><span data-stu-id="519c8-109">In the **Type** field, select **Vendor**.</span></span>
6.  <span data-ttu-id="519c8-110">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="519c8-110">Select **Save**.</span></span>
7.  <span data-ttu-id="519c8-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="519c8-111">Close the page.</span></span>
8.  <span data-ttu-id="519c8-112">انتقل إلى **التحكم في الإنتاج > إعداد > الموارد > مجموعات الموارد**</span><span class="sxs-lookup"><span data-stu-id="519c8-112">Go to **Production control > Setup > Resources > Resource groups**.</span></span>
9.  <span data-ttu-id="519c8-113">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-113">Select **New**.</span></span>
10. <span data-ttu-id="519c8-114">في الحقل **مجموعة الموارد**، أدخل **eBookSub**.</span><span class="sxs-lookup"><span data-stu-id="519c8-114">In the **Resource group** field, enter **eBookSub**.</span></span>
11. <span data-ttu-id="519c8-115">في الحقل **وصف**، أدخل **eBooksubcontractor**.</span><span class="sxs-lookup"><span data-stu-id="519c8-115">In the **Description** field, enter **eBooksubcontractor**.</span></span>
12. <span data-ttu-id="519c8-116">ضمن الحقل **موقع**، أدخل أو حدد **1‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-116">Under the **Site** field, enter or select site **1**.</span></span>
13. <span data-ttu-id="519c8-117">في علامة التبويب **عام**، حدد **نعم** في الحقل **خلية عمل**.</span><span class="sxs-lookup"><span data-stu-id="519c8-117">In the **General** tab, select **Yes** in the **Work cell** field.</span></span>
14. <span data-ttu-id="519c8-118">في الحقل **مستودع المدخلات**، أدخل أو حدد **11‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-118">In the **Input warehouse** field, enter or select **11**.</span></span>
15. <span data-ttu-id="519c8-119">في الحقل **موقع الإدخالات**، أدخل أو حدد **11‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-119">In the **Input location** field, enter or select **11**.</span></span>
16. <span data-ttu-id="519c8-120">في الحقل **مستودع المخرجات**، أدخل أو حدد **12-801**.</span><span class="sxs-lookup"><span data-stu-id="519c8-120">In the **Output warehouse** field, enter or select **12-801**.</span></span>
17. <span data-ttu-id="519c8-121">في الحقل **موقع المخرجات**، أدخل أو حدد **801‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-121">In the **Output location** field, enter or select **801**.</span></span>
18. <span data-ttu-id="519c8-122">قم بتوسيع علامة التبويب السريعة **تقويمات**.</span><span class="sxs-lookup"><span data-stu-id="519c8-122">Expand the **Calendars** FastTab.</span></span>
19. <span data-ttu-id="519c8-123">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="519c8-123">Select **Add**.</span></span>
19. <span data-ttu-id="519c8-124">في الحقل **تقويم**، أدخل أو حدد **إنتاج‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-124">In the **Calendar** field, enter or select **Production**.</span></span>
20. <span data-ttu-id="519c8-125">قم بتصغير القسم **تقويمات**.</span><span class="sxs-lookup"><span data-stu-id="519c8-125">Collapse the **Calendars** section.</span></span>
21. <span data-ttu-id="519c8-126">قم بتوسيع علامة التبويب **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="519c8-126">Expand the **Resources** tab.</span></span>
22. <span data-ttu-id="519c8-127">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="519c8-127">Select **Add**.</span></span>
22. <span data-ttu-id="519c8-128">في الحقل **مورد**، أدخل أو حدد **8821‎**.</span><span class="sxs-lookup"><span data-stu-id="519c8-128">In the **Resource** field, enter or select **8821**.</span></span>
23. <span data-ttu-id="519c8-129">قم بتصغير القسم **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="519c8-129">Collapse the **Resources** section.</span></span>
24. <span data-ttu-id="519c8-130">قم بتوسيع علامة التبويب **قدرة خلية العمل**.</span><span class="sxs-lookup"><span data-stu-id="519c8-130">Expand the **Work cell capacity** tab.</span></span>
25. <span data-ttu-id="519c8-131">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="519c8-131">Select **Add**.</span></span>
25. <span data-ttu-id="519c8-132">في الحقل **نموذج تدفق الإنتاج**، أدخل أو حدد **نموذج تدفق سماعة 2 متوسطة المدى**.</span><span class="sxs-lookup"><span data-stu-id="519c8-132">In the **Production flow model** field, enter or select **Mid-Range Speaker 2 Flow Model**.</span></span>
26. <span data-ttu-id="519c8-133">في الحقل **فترة القدرة**، حدد **يوم العمل القياسي**.</span><span class="sxs-lookup"><span data-stu-id="519c8-133">In the **Capacity period** field, select **Standard workday**.</span></span>
27. <span data-ttu-id="519c8-134">عيّن **متوسط كمية الإنتاجية** على **100.00**.</span><span class="sxs-lookup"><span data-stu-id="519c8-134">Set the **Average throughput quantity** to **100.00**.</span></span>
28. <span data-ttu-id="519c8-135">في حقل **الوحدة**، أدخل **pcs**.</span><span class="sxs-lookup"><span data-stu-id="519c8-135">In the **Unit** field, enter **pcs**.</span></span>
29. <span data-ttu-id="519c8-136">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="519c8-136">Select **Save**.</span></span>
30. <span data-ttu-id="519c8-137">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="519c8-137">Close all pages.</span></span>
