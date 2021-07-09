---
ms.openlocfilehash: 1051b0c7d1fb946f463d4f5254f7036ac1813646
ms.sourcegitcommit: 4ce9caef7d38158f172e82412bc70ae36883e42f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "6073648"
---
> [!NOTE]
> <span data-ttu-id="06596-101">قبل أن تبدأ هذا التدريب، يجب أن تكون قد أكملت التدريب السابق، **إنشاء خلية عمل لتعاقد من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-101">Before you begin this exercise, you must have completed the previous exercise, **Create a work cell for subcontracting**.</span></span>

## <a name="prerequisite"></a><span data-ttu-id="06596-102">المتطلب الأساسي</span><span class="sxs-lookup"><span data-stu-id="06596-102">Prerequisite</span></span>
<span data-ttu-id="06596-103">يجب عليك إعداد تحويل الوحدة في بيانات العرض التوضيحي حتى تتمكن من أداء هذا التدريب.</span><span class="sxs-lookup"><span data-stu-id="06596-103">You must set up unit conversion in the demo data to be able to perform this exercise.</span></span>
1.  <span data-ttu-id="06596-104">انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="06596-104">Go to **Product information management > Products > Released products**.</span></span>
2.  <span data-ttu-id="06596-105">تصفية القائمة لتحديد المنتج **S0001**.</span><span class="sxs-lookup"><span data-stu-id="06596-105">Filter the list to select the product **S0001**.</span></span>
3.  <span data-ttu-id="06596-106">في علامة التبويب **منتج**، حدد **تحويلات الوحدات** من مجموعة **إعداد**.</span><span class="sxs-lookup"><span data-stu-id="06596-106">On the **Product** tab, select **Unit conversions** from the **Set up** group.</span></span>
4.  <span data-ttu-id="06596-107">ضع المؤشر على **تحويلات بين الفئات**.</span><span class="sxs-lookup"><span data-stu-id="06596-107">Place your cursor on **Inter-class conversions**.</span></span>
5.  <span data-ttu-id="06596-108">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="06596-108">Select **New**.</span></span>
6.  <span data-ttu-id="06596-109">في **من وحدة**، حدد **ea**؛ في **إلى وحدة**، حدد **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="06596-109">In the **From unit**, select **ea**; in the **To unit**, select **hr**.</span></span>
6.  <span data-ttu-id="06596-110">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="06596-110">Select **OK**.</span></span>
7.  <span data-ttu-id="06596-111">أغلق الصفحة، ثم أغلق صفحة **تفاصيل المنتج الصادر**.</span><span class="sxs-lookup"><span data-stu-id="06596-111">Close the page, and then close the **Released product details** page.</span></span>

## <a name="scenario"></a><span data-ttu-id="06596-112">السيناريو</span><span class="sxs-lookup"><span data-stu-id="06596-112">Scenario</span></span>
<span data-ttu-id="06596-113">في هذا التدريب ستنشئ قاعدة تعاقد من الباطن على أساس النشاط.</span><span class="sxs-lookup"><span data-stu-id="06596-113">In this exercise you will create an activity-based subcontracting rule.</span></span>

1.  <span data-ttu-id="06596-114">في USMF، انتقل إلى **التحكم بالإنتاج > إعداد > تدفق الإنتاج محدود الفاقد > تدفقات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="06596-114">In USMF, go to **Production control > Setup > Lean production flow > Production flows**.</span></span>
2.  <span data-ttu-id="06596-115">في القائمة، ابحث عن رابط **برنامج تشغيل السماعات** وحدده للوصول إلى صفحة التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="06596-115">In the list, find and select the **Speaker driver** link to get to the details page.</span></span>
3.  <span data-ttu-id="06596-116">ضمن قسم **الإصدارات**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="06596-116">Under the **Versions** section, select **Add**.</span></span>
4.  <span data-ttu-id="06596-117">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="06596-117">Select **OK**.</span></span>
5.  <span data-ttu-id="06596-118">في القائمة، ابحث عن الإصدار الجديد وحدده بحالة **مسودة**.</span><span class="sxs-lookup"><span data-stu-id="06596-118">In the list, find and select the new version with status of **Draft**.</span></span>
6.  <span data-ttu-id="06596-119">حدد **أنشطة**.</span><span class="sxs-lookup"><span data-stu-id="06596-119">Select **Activities**.</span></span>
7.  <span data-ttu-id="06596-120">حدد **إنشاء نشاط خطة جديد** في الجزء العلوي من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="06596-120">Select **Create new plan activity** at the top of the screen.</span></span>
8.  <span data-ttu-id="06596-121">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-121">Select **Next**.</span></span>
9.  <span data-ttu-id="06596-122">في الحقل **اسم**، أدخل **GTL-نشاط التعاقد من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-122">In the **Name** field, enter **GTL-Subcontracting activity**.</span></span>
10. <span data-ttu-id="06596-123">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-123">Select **Next**.</span></span>
11. <span data-ttu-id="06596-124">في حقل **خلية عمل**، أدخل أو حدد **eBookSub‎**.</span><span class="sxs-lookup"><span data-stu-id="06596-124">In the **Work cell** field, enter or select **eBookSub**.</span></span> <span data-ttu-id="06596-125">أنت تقوم بتعيين خلية عمل مرتبطة بالمورد.</span><span class="sxs-lookup"><span data-stu-id="06596-125">You are assigning a work cell that is associated with the vendor.</span></span>
12. <span data-ttu-id="06596-126">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-126">Select **Next**.</span></span>
13. <span data-ttu-id="06596-127">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-127">Select **Next**.</span></span>
14. <span data-ttu-id="06596-128">في القائمة، ابحث عن الصف **وقت التشغيل** وحدده ثم أدخل **1** في الحقل **الوقت**.</span><span class="sxs-lookup"><span data-stu-id="06596-128">In the list, find and select the row for the **Runtime** time and then enter **1** in the **Time** field.</span></span>
15. <span data-ttu-id="06596-129">في الحقل **الوحدة الزمنية**، أدخل أو حدد **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="06596-129">In the **Time unit** field, enter or select **hr**.</span></span>
16. <span data-ttu-id="06596-130">قم بتعيين **لكل كمية** على **10.00**.</span><span class="sxs-lookup"><span data-stu-id="06596-130">Set **Per quantity** to **10.00**.</span></span>
17. <span data-ttu-id="06596-131">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-131">Select **Next**.</span></span>
18. <span data-ttu-id="06596-132">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="06596-132">Select **Finish**.</span></span>
19. <span data-ttu-id="06596-133">حدد **إنشاء نشاط خطة جديد**.</span><span class="sxs-lookup"><span data-stu-id="06596-133">Select **Create new plan activity**.</span></span>
20. <span data-ttu-id="06596-134">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-134">Select **Next**.</span></span>
21. <span data-ttu-id="06596-135">في الحقل **اسم**، أدخل **GTL-التحويل إلى مقاول من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-135">In the **Name** field, enter **GTL-Transfer to subcontractor**.</span></span>
22. <span data-ttu-id="06596-136">في الحقل **نوع النشاط**، حدد **تحويل**.</span><span class="sxs-lookup"><span data-stu-id="06596-136">In the **Activity type** field, select **Transfer**.</span></span>
23. <span data-ttu-id="06596-137">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-137">Select **Next**.</span></span>
24. <span data-ttu-id="06596-138">في الحقل **تزويد**، أدخل أو حدد **eBookSub**.</span><span class="sxs-lookup"><span data-stu-id="06596-138">In the **Replenishing** field, enter or select **eBookSub**.</span></span>
25. <span data-ttu-id="06596-139">في الحقل **تم تزويده**، أدخل أو حدد **eBookSub**.</span><span class="sxs-lookup"><span data-stu-id="06596-139">In the **Replenished** field, enter or select **eBookSub**.</span></span>
26. <span data-ttu-id="06596-140">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-140">Select **Next**.</span></span>
27. <span data-ttu-id="06596-141">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-141">Select **Next**.</span></span>
28. <span data-ttu-id="06596-142">في القائمة، ابحث عن الصف **وقت التشغيل** وحدده ثم أدخل **1** في الحقل **الوقت**.</span><span class="sxs-lookup"><span data-stu-id="06596-142">In the list, find and select the row for the **Runtime** time and then enter **1** in the **Time** field.</span></span>
29. <span data-ttu-id="06596-143">في الحقل **الوحدة الزمنية**، أدخل أو حدد **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="06596-143">In the **Time unit** field, enter or select **hr**.</span></span>
30. <span data-ttu-id="06596-144">قم بتعيين **لكل كمية** على **4.00**.</span><span class="sxs-lookup"><span data-stu-id="06596-144">Set **Per quantity** to **4.00**.</span></span>
31. <span data-ttu-id="06596-145">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-145">Select **Next**.</span></span>
32. <span data-ttu-id="06596-146">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="06596-146">Select **Finish**.</span></span>
33. <span data-ttu-id="06596-147">في القائمة، ابحث عن **GTL-نشاط تعاقد من الباطن** وحدده.</span><span class="sxs-lookup"><span data-stu-id="06596-147">In the list, find and select **GTL-Subcontracting activity**.</span></span>
34. <span data-ttu-id="06596-148">ضمن علامة التبويب **عناصر لاحقة**، حدد **إضافة عنصر لاحق**.</span><span class="sxs-lookup"><span data-stu-id="06596-148">Under the **Successors** tab, select **Add successor**.</span></span>
35. <span data-ttu-id="06596-149">في شريحة **إنشاء علاقة النشاط**، في حقل **النشاط**، أدخل أو حدد **GTL-التحويل إلى مقاول من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-149">In the **Create activity relation** slide-out, in the **Activity** field, enter or select **GTL-Transfer to subcontractor**.</span></span>
36. <span data-ttu-id="06596-150">في حقل **نسبة زمن الدورة**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="06596-150">In the **Cycle time ratio** field, enter **1**.</span></span>
37. <span data-ttu-id="06596-151">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="06596-151">Select **OK**.</span></span>
38. <span data-ttu-id="06596-152">حدد **GTL-نشاط التعاقد من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-152">Select **GTL-Subcontracting activity**.</span></span>
39. <span data-ttu-id="06596-153">حدد **التفاصيل** في القائمة في الأعلى.</span><span class="sxs-lookup"><span data-stu-id="06596-153">Select **Details** in the menu at the top.</span></span>
40. <span data-ttu-id="06596-154">قم بتوسيع علامة التبويب السريعة **شروط الخدمة**.</span><span class="sxs-lookup"><span data-stu-id="06596-154">Expand the **Service terms** FastTab.</span></span>
41. <span data-ttu-id="06596-155">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="06596-155">Select **Add**.</span></span>
42. <span data-ttu-id="06596-156">في الحقل **خدمة**، حدد **S0001**.</span><span class="sxs-lookup"><span data-stu-id="06596-156">In the **Service** field, select **S0001**.</span></span>
43. <span data-ttu-id="06596-157">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-157">Select **Next**.</span></span>
44. <span data-ttu-id="06596-158">في الحقل **نسبة الخدمة**، أدخل **1.2**.</span><span class="sxs-lookup"><span data-stu-id="06596-158">In the **Service ratio** field, enter **1.2**.</span></span>
45. <span data-ttu-id="06596-159">في الحقل **وحدة الخدمة**، حدد **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="06596-159">In the **Service unit** field, select **hr**.</span></span>
46. <span data-ttu-id="06596-160">بالنسبة للحقل **أساس كمية الخدمة**، حدد **وقت النشاط**.</span><span class="sxs-lookup"><span data-stu-id="06596-160">For the **Service quantity base** field, select **Activity time**.</span></span>
47. <span data-ttu-id="06596-161">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-161">Select **Next**.</span></span>
48. <span data-ttu-id="06596-162">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="06596-162">Select **Finish**.</span></span>
49. <span data-ttu-id="06596-163">أغلق صفحة **تفاصيل النشاط**.</span><span class="sxs-lookup"><span data-stu-id="06596-163">Close the **Activity details** page.</span></span>
50. <span data-ttu-id="06596-164">حدد **-GTLالتحويل إلى مقاول من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-164">Select **GTL-Transfer to Subcontractor**.</span></span>
51. <span data-ttu-id="06596-165">حدد **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="06596-165">Select **Details**.</span></span>
52. <span data-ttu-id="06596-166">قم بتوسيع علامة التبويب السريعة **شروط الخدمة**.</span><span class="sxs-lookup"><span data-stu-id="06596-166">Expand the **Service terms** FastTab.</span></span>
53. <span data-ttu-id="06596-167">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="06596-167">Select **Add**.</span></span>
54. <span data-ttu-id="06596-168">في الحقل **خدمة**، حدد **S0001**.</span><span class="sxs-lookup"><span data-stu-id="06596-168">In the **Service** field, select **S0001**.</span></span>
55. <span data-ttu-id="06596-169">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-169">Select **Next**.</span></span>
56. <span data-ttu-id="06596-170">في الحقل **نسبة الخدمة**، أدخل **1.0**.</span><span class="sxs-lookup"><span data-stu-id="06596-170">In the **Service ratio** field, enter **1.0**.</span></span>
57. <span data-ttu-id="06596-171">في الحقل **وحدة الخدمة**، حدد **ساعة**.</span><span class="sxs-lookup"><span data-stu-id="06596-171">In the **Service unit** field, select **hr**.</span></span>
58. <span data-ttu-id="06596-172">بالنسبة للحقل **أساس كمية الخدمة**، حدد **وقت النشاط**.</span><span class="sxs-lookup"><span data-stu-id="06596-172">For the **Service quantity base** field, select **Activity time**.</span></span>
59. <span data-ttu-id="06596-173">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="06596-173">Select **Next**.</span></span>
60. <span data-ttu-id="06596-174">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="06596-174">Select **Finish**.</span></span>
60. <span data-ttu-id="06596-175">أغلق نموذج **تفاصيل النشاط**.</span><span class="sxs-lookup"><span data-stu-id="06596-175">Close the **Activity details** form.</span></span> 
60. <span data-ttu-id="06596-176">حدد **GTL-نشاط التعاقد من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="06596-176">Select **GTL-Subcontracting activity**.</span></span>
61. <span data-ttu-id="06596-177">حدد **إضافة عنصر سابق**.</span><span class="sxs-lookup"><span data-stu-id="06596-177">Select **Add predecessor**.</span></span>
62. <span data-ttu-id="06596-178">في الحقل **النشاط**، حدد **برنامج تشغيل السماعات**.</span><span class="sxs-lookup"><span data-stu-id="06596-178">In the **Activity** field, select **Speaker driver**.</span></span>
63. <span data-ttu-id="06596-179">في حقل **نسبة زمن الدورة**، أدخل **1**.</span><span class="sxs-lookup"><span data-stu-id="06596-179">In the **Cycle time ratio** field, enter **1**.</span></span>
63. <span data-ttu-id="06596-180">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="06596-180">Select **OK**.</span></span>
67. <span data-ttu-id="06596-181">أغلق صفحة **أنشطة تدفق الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="06596-181">Close the **Production flow activities** page.</span></span>
68. <span data-ttu-id="06596-182">حدد **الإصدار 1** ثم حدد **إلغاء تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="06596-182">Select **version 1** and then select **Deactivate**.</span></span>
69. <span data-ttu-id="06596-183">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="06596-183">Select **OK**.</span></span>
70. <span data-ttu-id="06596-184">حدد **الإصدار 2** ثم حدد **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="06596-184">Select **version 2** and then select **Activate**.</span></span>
71. <span data-ttu-id="06596-185">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="06596-185">Select **OK**.</span></span>
73. <span data-ttu-id="06596-186">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="06596-186">Close all pages.</span></span>
