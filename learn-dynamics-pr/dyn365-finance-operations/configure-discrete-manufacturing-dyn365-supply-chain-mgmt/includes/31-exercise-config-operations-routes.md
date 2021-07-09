---
ms.openlocfilehash: 765d0c88268ba391a2f900761cb60b34c842ed57
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073034"
---
<span data-ttu-id="3d9f8-101">بصفتك مدير إنتاج في **USMF**، فإنك تحتاج إلى إنشاء عملية لدفتر إلكتروني كصنف منتهٍ، وتعيين علاقات للمورد 1211، وإنشاء مسار باستخدام مجموعة أصناف التلفزيون والفيديو باسم **مسار الدفتر الإلكتروني**، مع العمليات التالية:</span><span class="sxs-lookup"><span data-stu-id="3d9f8-101">As a production manager at **USMF**, you need to create an operation for an e-book as a finished item, assign relations to resource 1211, create a route by using the TV&Video item group with the name of **e-book Route**, with the following operations:</span></span>

-   <span data-ttu-id="3d9f8-102">**رقم العملية 10**: ربط عملية الدفتر الإلكتروني بـ 20</span><span class="sxs-lookup"><span data-stu-id="3d9f8-102">**Operation number 10**: e-book operation links to 20</span></span>

-   <span data-ttu-id="3d9f8-103">**ارتباط مبدئي برقم العملية 20**: ربط الحشو بـ 30</span><span class="sxs-lookup"><span data-stu-id="3d9f8-103">**Soft link to Operation number 20**: Padding links to 30</span></span>

-   <span data-ttu-id="3d9f8-104">**ارتباط ثابت برقم العملية 30**: تعبئة ثانوية</span><span class="sxs-lookup"><span data-stu-id="3d9f8-104">**Hard link to Operation number 30**: secondary Packing</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="3d9f8-105">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="3d9f8-105">Before you begin</span></span>

<span data-ttu-id="3d9f8-106">للحصول على أقصى استفادة من هذا التدريب، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Supply Chain Management والتي يتم تثبيتها عن طريق Lifecycle services (LCS).</span><span class="sxs-lookup"><span data-stu-id="3d9f8-106">To get the most out of this exercise, we recommend that you have the standard sample data available in Dynamics 365 Supply Chain Management that is installed via Lifecycle services (LCS).</span></span>

1.  <span data-ttu-id="3d9f8-107">انتقل إلى **التحكم في الإنتاج > الإعداد > المسارات > العمليات**</span><span class="sxs-lookup"><span data-stu-id="3d9f8-107">Go to **Production control > Setup > Routes > Operations**.</span></span>
2.  <span data-ttu-id="3d9f8-108">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-108">Select **New**.</span></span>
3.  <span data-ttu-id="3d9f8-109">في حقل **العملية**، اكتب **دفتر إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-109">In the **Operation** field, type **eBook**.</span></span>
4.  <span data-ttu-id="3d9f8-110">في الحقل **الاسم**، اكتب **مجموعة الدفتر الإلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-110">In the **Name** field, type **eBook assembly**.</span></span>
5.  <span data-ttu-id="3d9f8-111">حدد **العلاقات**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-111">Select **Relations**.</span></span>
6.  <span data-ttu-id="3d9f8-112">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-112">Select **New**.</span></span>
7.  <span data-ttu-id="3d9f8-113">في حقل **مجموعة المسارات**، أدخِل أو حدد **منفصل**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-113">In the **Route group** field, enter or select **Discrete**.</span></span>
8.  <span data-ttu-id="3d9f8-114">قم بتوسيع قسم **الإعداد**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-114">Expand the **Setup** section.</span></span>
9.  <span data-ttu-id="3d9f8-115">في حقل **المعادلة**، حدد **القدرة الإنتاجية**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-115">In the **Formula** field, select **Capacity**.</span></span>
10. <span data-ttu-id="3d9f8-116">في الحقل **مورد التكلفة**، أدخل أو حدد **1211‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-116">In the **Costing resource** field, enter or select **1211**.</span></span>
10. <span data-ttu-id="3d9f8-117">وإذا ظهر التحذير **سيتم إدراج الوقت الافتراضي وقيم التكلفة من 1211. هل تريد المتابعة؟**، فحدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-117">If the warning **Default time and cost values from 1211 will be inserted. Do you want to continue?** appears, select **Yes**.</span></span>
11. <span data-ttu-id="3d9f8-118">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-118">Select **Save**.</span></span>
12. <span data-ttu-id="3d9f8-119">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-119">Close all pages.</span></span>
13. <span data-ttu-id="3d9f8-120">انتقل إلى **التحكم بالإنتاج > كافة المسارات**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-120">Go to **Production control > All routes**.</span></span>
14. <span data-ttu-id="3d9f8-121">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-121">Select **New**.</span></span>
15. <span data-ttu-id="3d9f8-122">في الحقل **الاسم**، اكتب **مسار الدفتر الإلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-122">In the **Name** field, type **eBook route**.</span></span>
16. <span data-ttu-id="3d9f8-123">في حقل **مجموعة الصنف**، أدخِل أو حدد **التليفزيون والفيديو**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-123">In the **Item group** field, enter or select **TV&Video**.</span></span>
17. <span data-ttu-id="3d9f8-124">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-124">Select **Save**.</span></span>
18. <span data-ttu-id="3d9f8-125">أسفل مجموعة **MAINTAIN**، حدد **تفاصيل المسار**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-125">Under the **MAINTAIN** group, select **Route details**.</span></span>
19. <span data-ttu-id="3d9f8-126">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-126">Select **New**.</span></span>
20. <span data-ttu-id="3d9f8-127">في حقل **رقم العملية**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-127">In the **Oper. No.**</span></span> <span data-ttu-id="3d9f8-128"> أدخل **10**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-128">field, enter **10**.</span></span>
21. <span data-ttu-id="3d9f8-129">في الحقل حقل **العملية**، أدخل أو حدد **دفتر إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-129">In the **Operation** field, enter or select **eBook**.</span></span>
21. <span data-ttu-id="3d9f8-130">في حقل **التالي**، أدخل **20**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-130">In the **Next** field, enter **20**.</span></span>
22. <span data-ttu-id="3d9f8-131">في حقل **نوع** **الارتباط**، حدد **مبدئي**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-131">In the **Link** **type** field, select **Soft**.</span></span>
23. <span data-ttu-id="3d9f8-132">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-132">Select **New**.</span></span>
24. <span data-ttu-id="3d9f8-133">في حقل **رقم العملية**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-133">In the **Oper. No.**</span></span> <span data-ttu-id="3d9f8-134"> أدخل **20**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-134">field, enter **20**.</span></span>
25. <span data-ttu-id="3d9f8-135">في حقل **العملية**، أدخل أو حدد **حشو**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-135">In the **Operation** field, enter or select **Padding**.</span></span>
26. <span data-ttu-id="3d9f8-136">في حقل **التالي**، أدخل **30**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-136">In the **Next** field, enter **30**.</span></span>
27. <span data-ttu-id="3d9f8-137">في حقل **نوع الارتباط**، حدد **ثابت**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-137">In the **Link type** field, select **Hard**.</span></span>
28. <span data-ttu-id="3d9f8-138">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-138">Select **New**.</span></span>
29. <span data-ttu-id="3d9f8-139">في حقل **رقم العملية**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-139">In the **Oper. No**.</span></span> <span data-ttu-id="3d9f8-140"> أدخل **30**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-140">field, enter **30**.</span></span>
30. <span data-ttu-id="3d9f8-141">في حقل **الأولوية**، حدد **ثانوي 1**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-141">In the **Priority** field, select **Secondary 1**.</span></span>
31. <span data-ttu-id="3d9f8-142">في حقل **العملية**، أدخل أو حدد **تعبئة**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-142">In the **Operation** field, enter or select **Packing**.</span></span>
32. <span data-ttu-id="3d9f8-143">قم بتحديث الصفحة.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-143">Refresh the page.</span></span>
33. <span data-ttu-id="3d9f8-144">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-144">Select **Save**.</span></span>
34. <span data-ttu-id="3d9f8-145">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="3d9f8-145">Close all pages.</span></span>
