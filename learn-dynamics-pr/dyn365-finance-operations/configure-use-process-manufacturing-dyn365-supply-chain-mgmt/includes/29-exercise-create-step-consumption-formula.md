---
ms.openlocfilehash: cfe72e5d48645823e030b47668e3736b148e5c61
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073125"
---
<span data-ttu-id="e5067-101">يجب تحديث معادلة المنتج **P9500** في الشركة USP2 لتغيير سطر المعادلة **M9003** من الاستهلاك السطري إلى الاستهلاك التدريجي.</span><span class="sxs-lookup"><span data-stu-id="e5067-101">The formula for product **P9500** in company USP2 is to be updated to change the formula line **M9003** from a linear consumption to a stepwise consumption.</span></span> <span data-ttu-id="e5067-102">يجب أن يكون الاستهلاك في السطر كما يلي:</span><span class="sxs-lookup"><span data-stu-id="e5067-102">The consumption on the line should be as follows:</span></span>

-   <span data-ttu-id="e5067-103">0-1400: 5.5</span><span class="sxs-lookup"><span data-stu-id="e5067-103">0-1400: 5.5</span></span>
-   <span data-ttu-id="e5067-104">1400-2400: 10.6</span><span class="sxs-lookup"><span data-stu-id="e5067-104">1400-2400: 10.6</span></span>
-   <span data-ttu-id="e5067-105">2400+: 15.8</span><span class="sxs-lookup"><span data-stu-id="e5067-105">2400+: 15.8</span></span>

## <a name="copy-the-existing-formula-for-p9500"></a><span data-ttu-id="e5067-106">انسخ المعادلة الحالية لـ P9500</span><span class="sxs-lookup"><span data-stu-id="e5067-106">Copy the existing formula for P9500</span></span>

1.  <span data-ttu-id="e5067-107">انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="e5067-107">Go to **Product information management > Products > Released products**.</span></span>
2.  <span data-ttu-id="e5067-108">استخدم عامل التصفية السريع للتصفية في حقل **رقم الصنف** بقيمة **P9500**.</span><span class="sxs-lookup"><span data-stu-id="e5067-108">Use the Quick Filter to filter on the **Item number** field with a value of **P9500**.</span></span>
3.  <span data-ttu-id="e5067-109">في القائمة، حدد الارتباط في الصف المحدد لـ **P9500**.</span><span class="sxs-lookup"><span data-stu-id="e5067-109">In the list, select the link in the selected row for **P9500**.</span></span>
4.  <span data-ttu-id="e5067-110">حدد **إصدارات المعادلة**.</span><span class="sxs-lookup"><span data-stu-id="e5067-110">Select **Formula versions**.</span></span>
5.  <span data-ttu-id="e5067-111">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e5067-111">Select **New**.</span></span>
6.  <span data-ttu-id="e5067-112">حدد **المعادلة وإصدار المعادلة**.</span><span class="sxs-lookup"><span data-stu-id="e5067-112">Select **Formula and formula version**.</span></span>
7.  <span data-ttu-id="e5067-113">في حقل **رقم المعادلة**، أدخل **P9500V1**.</span><span class="sxs-lookup"><span data-stu-id="e5067-113">In the **Formula number** field, enter **P9500V1**.</span></span>
8.  <span data-ttu-id="e5067-114">في الحقل **الاسم**، أدخل **V1**.</span><span class="sxs-lookup"><span data-stu-id="e5067-114">In the **Name** field, enter **V1**.</span></span>
9.  <span data-ttu-id="e5067-115">حدد الخيار **نسخ**.</span><span class="sxs-lookup"><span data-stu-id="e5067-115">Select the **Copy** option.</span></span>
10. <span data-ttu-id="e5067-116">في حقل **الموقع**، أدخل أو حدد **1**.</span><span class="sxs-lookup"><span data-stu-id="e5067-116">In the **Site** field, enter or select **1**.</span></span>
11. <span data-ttu-id="e5067-117">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e5067-117">Select **OK**.</span></span>
12. <span data-ttu-id="e5067-118">في حقل **إصدار المعادلة**، حدد الإصدار الحالي.</span><span class="sxs-lookup"><span data-stu-id="e5067-118">In the **Formula version** field, select the current version.</span></span>
13. <span data-ttu-id="e5067-119">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e5067-119">Select **OK**.</span></span>


## <a name="set-the-line-for-m9003-in-the-new-formula-to-stepwise-consumption-and-set-the-step-levels"></a><span data-ttu-id="e5067-120">قم بتعيين سطر M9003 في المعادلة الجديدة على الاستهلاك التدريجي وقم بتعيين مستويات الخطوة</span><span class="sxs-lookup"><span data-stu-id="e5067-120">Set the line for M9003 in the new formula to stepwise consumption and set the step levels</span></span>

1. <span data-ttu-id="e5067-121">ابحث في السطور عن سطر **M9003**.</span><span class="sxs-lookup"><span data-stu-id="e5067-121">In the lines, find the line for **M9003**.</span></span>
15. <span data-ttu-id="e5067-122">حدد علامة التبويب **الإعداد**.</span><span class="sxs-lookup"><span data-stu-id="e5067-122">Select the **Setup** tab.</span></span>
16. <span data-ttu-id="e5067-123">في حقل **المعادلة**، حدد **الخطوة**.</span><span class="sxs-lookup"><span data-stu-id="e5067-123">In the **Formula** field, select **Step**.</span></span>
17. <span data-ttu-id="e5067-124">حدد علامة التبويب **استهلاك الخطوة**.</span><span class="sxs-lookup"><span data-stu-id="e5067-124">Select the **Step consumption** tab.</span></span>
18. <span data-ttu-id="e5067-125">قم بتعيين **الكمية** إلى **5.5**.</span><span class="sxs-lookup"><span data-stu-id="e5067-125">Set **Quantity** to **5.5**.</span></span>
19. <span data-ttu-id="e5067-126">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e5067-126">Select **New**.</span></span>
20. <span data-ttu-id="e5067-127">قم بتعيين **السلسلة من** إلى **1400**.</span><span class="sxs-lookup"><span data-stu-id="e5067-127">Set **From series** to **1400**.</span></span>
21. <span data-ttu-id="e5067-128">قم بتعيين **الكمية** إلى **10.6**.</span><span class="sxs-lookup"><span data-stu-id="e5067-128">Set **Quantity** to **10.6**.</span></span>
22. <span data-ttu-id="e5067-129">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e5067-129">Select **New**.</span></span>
23. <span data-ttu-id="e5067-130">قم بتعيين **السلسلة من** إلى **2400**.</span><span class="sxs-lookup"><span data-stu-id="e5067-130">Set **From series** to **2400**.</span></span>
24. <span data-ttu-id="e5067-131">قم بتعيين **الكمية** إلى **15.8**.</span><span class="sxs-lookup"><span data-stu-id="e5067-131">Set **Quantity** to **15.8**.</span></span>
25. <span data-ttu-id="e5067-132">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e5067-132">Select **Save**.</span></span>
26. <span data-ttu-id="e5067-133">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="e5067-133">Close all pages.</span></span>


## <a name="date-out-the-old-formula-and-date-in-the-new-one"></a><span data-ttu-id="e5067-134">تاريخ خارج المعادلة القديمة والتاريخ في الجديدة</span><span class="sxs-lookup"><span data-stu-id="e5067-134">Date out the old formula and date in the new one</span></span>

1. <span data-ttu-id="e5067-135">في القائمة، ابحث عن المعادلة القديمة وحددها.</span><span class="sxs-lookup"><span data-stu-id="e5067-135">In the list, find and select the old formula.</span></span>
28. <span data-ttu-id="e5067-136">في حقل **إلى ‏‏تاريخ**، قم بتعيين التاريخ إلى **2016-12-27**.</span><span class="sxs-lookup"><span data-stu-id="e5067-136">In the **To date** field, set the date to **2016-12-27**.</span></span>
29. <span data-ttu-id="e5067-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e5067-137">Select **Save**.</span></span>
30. <span data-ttu-id="e5067-138">في القائمة، ابحث عن المعادلة الجديدة وحددها.</span><span class="sxs-lookup"><span data-stu-id="e5067-138">In the list, find and select the new formula.</span></span>
31. <span data-ttu-id="e5067-139">في حقل **من ‏‏تاريخ**، قم بتعيين التاريخ إلى **2016-12-28**.</span><span class="sxs-lookup"><span data-stu-id="e5067-139">In the **From date** field, set the date to **2016-12-28**.</span></span>
32. <span data-ttu-id="e5067-140">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e5067-140">Select **Save**.</span></span>


## <a name="approve-and-activate-the-formula"></a><span data-ttu-id="e5067-141">الموافقة على المعادلة وتنشيطها</span><span class="sxs-lookup"><span data-stu-id="e5067-141">Approve and activate the formula</span></span>

1. <span data-ttu-id="e5067-142">حدد **موافقة**.</span><span class="sxs-lookup"><span data-stu-id="e5067-142">Select **Approve**.</span></span>
34. <span data-ttu-id="e5067-143">في حقل **موافق عليه من قِبل**، أدخل موظفاً أو حدده.</span><span class="sxs-lookup"><span data-stu-id="e5067-143">In the **Approved by** field, enter or select an employee.</span></span>
35. <span data-ttu-id="e5067-144">حدد الخيار **هل تريد أيضاً الموافقة على المعادلة؟**.</span><span class="sxs-lookup"><span data-stu-id="e5067-144">Select the **Do you also want to approve the formula?** option.</span></span>
36. <span data-ttu-id="e5067-145">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e5067-145">Select **OK**.</span></span>
37. <span data-ttu-id="e5067-146">حدد **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="e5067-146">Select **Activate**.</span></span>
