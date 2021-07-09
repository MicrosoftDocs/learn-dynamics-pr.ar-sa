---
ms.openlocfilehash: 683db1fb278ca620dcf13f8ca3c00e6ae41a7395
ms.sourcegitcommit: 4ce9caef7d38158f172e82412bc70ae36883e42f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "6073649"
---
> [!NOTE]
> <span data-ttu-id="fdde9-101">قبل أن تبدأ هذا التدريب، يجب أن تكون قد أكملت التدريب السابق، **إنشاء قاعدة تعاقد من الباطن قائمة على النشاط**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-101">Before you begin this exercise, you must have completed the previous exercise, **Create an activity-based subcontracting rule**.</span></span>

## <a name="prerequisite"></a><span data-ttu-id="fdde9-102">المتطلب الأساسي</span><span class="sxs-lookup"><span data-stu-id="fdde9-102">Prerequisite</span></span> 
<span data-ttu-id="fdde9-103">يجب عليك إعداد تحويل الوحدة في بيانات العرض التوضيحي حتى تتمكن من أداء هذا التدريب.</span><span class="sxs-lookup"><span data-stu-id="fdde9-103">You must set up unit conversion in the demo data to be able to perform this exercise.</span></span>

1.  <span data-ttu-id="fdde9-104">انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-104">Go to **Product information management > Products > Released products**.</span></span>
2.  <span data-ttu-id="fdde9-105">تصفية القائمة لتحديد المنتج **L0001**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-105">Filter the list to select the product **L0001**.</span></span>
3.  <span data-ttu-id="fdde9-106">في علامة التبويب السريعة **منتج**، حدد **تحويلات الوحدات** من مجموعة **إعداد**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-106">On the **Product** FastTab, select **Unit conversions** from the **Set up** group.</span></span>
4.  <span data-ttu-id="fdde9-107">ضع المؤشر على **تحويلات بين الفئات**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-107">Place your cursor on **Inter-class conversions**.</span></span>
5.  <span data-ttu-id="fdde9-108">حدد **جديد**،</span><span class="sxs-lookup"><span data-stu-id="fdde9-108">Select **New**.</span></span>
6.  <span data-ttu-id="fdde9-109">في **من الوحدة**، حدد **ساعة**؛ في **إلى الوحدة**، حدد **ea**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-109">In the **From unit**, select **hr**; in the **To unit**, select **ea**.</span></span>
6. <span data-ttu-id="fdde9-110">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-110">Select **OK**.</span></span>
7.  <span data-ttu-id="fdde9-111">أغلق النموذج، ثم أغلق صفحة **تفاصيل المنتج الصادر**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-111">Close the form, and then close the **Released product details** page.</span></span>


## <a name="scenario"></a><span data-ttu-id="fdde9-112">السيناريو</span><span class="sxs-lookup"><span data-stu-id="fdde9-112">Scenario</span></span>
<span data-ttu-id="fdde9-113">في هذا التدريب، ستقوم بإنشاء بطاقات كانبان لكل تعاقد من الباطن وجدولتها.</span><span class="sxs-lookup"><span data-stu-id="fdde9-113">In this exercise you will create and schedule kanbans for subcontracting.</span></span>

1.  <span data-ttu-id="fdde9-114">انتقل إلى **إدارة معلومات المنتج > Lean manufacturing > قواعد كانبان**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-114">Go to **Product information management > Lean manufacturing > Kanban rules**.</span></span>
2.  <span data-ttu-id="fdde9-115">حدد **جديد**،</span><span class="sxs-lookup"><span data-stu-id="fdde9-115">Select **New**.</span></span>
3.  <span data-ttu-id="fdde9-116">في حقل **نشاط الخطة الأول**، أدخل أو حدد **GTL-نشاط تعاقد من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-116">In the **First plan activity** field, enter or select **GTL-Subcontracting activity**.</span></span>
4.  <span data-ttu-id="fdde9-117">حدد خانة الاختيار **أنشطه متعددة**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-117">Select the **Multiple activities** check box.</span></span>
5.  <span data-ttu-id="fdde9-118">في حقل **نشاط الخطة الأخير**، أدخل أو حدد **GTL-تحويل إلى مقاول من الباطن**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-118">In the **Last plan activity** field, enter or select **GTL-Transfer to subcontractor**.</span></span> 
1.  <span data-ttu-id="fdde9-119">في صفحة **اختيار تدفق كانبان**، حدد **إنشاء تدفقات**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-119">On the **Choose Kanban flow** page, select **Generate flows**.</span></span>
1.  <span data-ttu-id="fdde9-120">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-120">Select **OK**.</span></span>
6.   <span data-ttu-id="fdde9-121">قم بتوسيع علامة التبويب السريعة **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-121">Expand the **Details** FastTab.</span></span>
6.  <span data-ttu-id="fdde9-122">في حقل **المنتج**، أدخل **L0001**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-122">In the **Product** field, enter **L0001**.</span></span>
7.  <span data-ttu-id="fdde9-123">قم بتوسيع قسم **الكميات**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-123">Expand the **Quantities** section.</span></span>
8.  <span data-ttu-id="fdde9-124">قم بتعيين **الكمية الافتراضية** على **50.00**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-124">Set **Default quantity** to **50.00**.</span></span>
9.  <span data-ttu-id="fdde9-125">في الحقل **كمية كانبان الثابتة**، أدخل **25**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-125">In the **Fixed kanban quantity** field, enter **25**.</span></span>
10. <span data-ttu-id="fdde9-126">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-126">Select **Save**.</span></span>
11. <span data-ttu-id="fdde9-127">قم بتوسيع علامة التبويب السريعة **بطاقات كانبان**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-127">Expand the **Kanbans** FastTab.</span></span>
11. <span data-ttu-id="fdde9-128">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-128">Select **Add**.</span></span>
12. <span data-ttu-id="fdde9-129">في الحقل **عدد بطاقات كانبان الجديدة**، أدخل 1.</span><span class="sxs-lookup"><span data-stu-id="fdde9-129">In the **Number of new kanbans** field, enter 1.</span></span>
12. <span data-ttu-id="fdde9-130">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-130">Select **Create**.</span></span>
13. <span data-ttu-id="fdde9-131">حدد **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-131">Select **Details**.</span></span>
14. <span data-ttu-id="fdde9-132">قم بتوسيع قسم **الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-132">Expand the **Jobs** section.</span></span>
15. <span data-ttu-id="fdde9-133">عرض الوظائف للمعالجة والتحويل إلى مقاول من الباطن.</span><span class="sxs-lookup"><span data-stu-id="fdde9-133">View jobs for process and transfer to a subcontractor.</span></span>
16. <span data-ttu-id="fdde9-134">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="fdde9-134">Close all pages.</span></span>
17. <span data-ttu-id="fdde9-135">انتقل إلى **التحكم بالإنتاج > كانبان > جدولة وظيفة كانبان**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-135">Go to **Production control > Kanban > Kanban job scheduling**.</span></span>
18. <span data-ttu-id="fdde9-136">في الحقل **خلية عمل**، حدد **eBookSub**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-136">In the **Work cell** field, select **eBookSub**.</span></span>
19. <span data-ttu-id="fdde9-137">في القائمة، حدد الصف الأول.</span><span class="sxs-lookup"><span data-stu-id="fdde9-137">In the list, select the first row.</span></span>
20. <span data-ttu-id="fdde9-138">حدد **الجدول الزمني من التاريخ** لفتح مربع الحوار المنسدل.</span><span class="sxs-lookup"><span data-stu-id="fdde9-138">Select **Schedule from date** to open the drop-down dialog box.</span></span>
21. <span data-ttu-id="fdde9-139">حدد **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="fdde9-139">Select **Schedule**.</span></span>
22. <span data-ttu-id="fdde9-140">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="fdde9-140">Close all pages.</span></span>
