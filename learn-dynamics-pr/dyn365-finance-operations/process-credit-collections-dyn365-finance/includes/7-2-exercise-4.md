---
ms.openlocfilehash: 9d207e64d1e6b19e0fc4b99d790a2aef5cf81cda
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070721"
---
## <a name="scenario"></a><span data-ttu-id="8b067-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="8b067-101">Scenario</span></span>

<span data-ttu-id="8b067-102">بصفتك مدير الائتمان لشركة **USMF‎**، فقد قررت استخدام ميزات إدارة الائتمان في Finance.</span><span class="sxs-lookup"><span data-stu-id="8b067-102">As the Credit manager for the company **USMF**, you have decided to use the features of Credit management in Finance.</span></span> <span data-ttu-id="8b067-103">لبدء الاستخدام، ستحصل على النظام الجاهز عن طريق قيامك بإنشاء مجموعات النقاط وتصنيفات المخاطر وقواعد الحظر.</span><span class="sxs-lookup"><span data-stu-id="8b067-103">To get started, you will be getting the system ready by creating Scoring groups, Risk classifications, and Blocking rules.</span></span> 

<span data-ttu-id="8b067-104">بالنسبة لهذه المعامل، عليك باستخدام شركة **USMF‎**.</span><span class="sxs-lookup"><span data-stu-id="8b067-104">For these labs, use the **USMF** company.</span></span> 

## <a name="scoring-groups"></a><span data-ttu-id="8b067-105">مجموعات النقاط</span><span class="sxs-lookup"><span data-stu-id="8b067-105">Scoring groups</span></span>

<span data-ttu-id="8b067-106">ستقوم بإعداد **مجموعة نقاط** جديدة مرتبطة بعدد أوامر المبيعات المتوقعة من العميل.</span><span class="sxs-lookup"><span data-stu-id="8b067-106">You will set up a new **Scoring group** tied to the number of sales orders expected from a customer.</span></span> 

1. <span data-ttu-id="8b067-107">انتقل إلى **‎الائتمان والتحصيلات > إعداد > إعداد إدارة الائتمان > المخاطر > مجموعات النقاط**</span><span class="sxs-lookup"><span data-stu-id="8b067-107">Go to **Credit and collections > Setup > Credit management setup > Risk > Scoring groups**</span></span>
2. <span data-ttu-id="8b067-108">حدد **جديد**</span><span class="sxs-lookup"><span data-stu-id="8b067-108">Select **New**</span></span>
3. <span data-ttu-id="8b067-109">في الحقل **مجموعة النقاط**، أدخل **SO_Year**.</span><span class="sxs-lookup"><span data-stu-id="8b067-109">In the **Scoring group** field, enter **SO_Year**</span></span>
4. <span data-ttu-id="8b067-110">في الحقل **الوصف**، أدخل **‎أوامر المبيعات كل سنة**</span><span class="sxs-lookup"><span data-stu-id="8b067-110">In the **Description** field, enter  **Sales orders per year**</span></span>
5. <span data-ttu-id="8b067-111">في الحقل **‎نوع المجموعة**، حدد **‎معرّف من قبل المستخدم**</span><span class="sxs-lookup"><span data-stu-id="8b067-111">In the  **Group type** field, select **User defined**</span></span>
6. <span data-ttu-id="8b067-112">في الحقل **نوع النقاط**، حدد **النطاق**.</span><span class="sxs-lookup"><span data-stu-id="8b067-112">In the **Score type** field, select **Range**</span></span>
7. <span data-ttu-id="8b067-113">في علامة التبويب السريعة **البنود**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="8b067-113">On the **Lines** FastTab, select **Add**</span></span>
8. <span data-ttu-id="8b067-114">قم بإعداد هذه النطاقات:</span><span class="sxs-lookup"><span data-stu-id="8b067-114">Set up these ranges:</span></span>

    <span data-ttu-id="8b067-115">أ.</span><span class="sxs-lookup"><span data-stu-id="8b067-115">a.</span></span> <span data-ttu-id="8b067-116">1-29 - النقطة 5</span><span class="sxs-lookup"><span data-stu-id="8b067-116">1-29   - Score 5</span></span>

    <span data-ttu-id="8b067-117">ب.</span><span class="sxs-lookup"><span data-stu-id="8b067-117">b.</span></span> <span data-ttu-id="8b067-118">30-59 - النقطة 10</span><span class="sxs-lookup"><span data-stu-id="8b067-118">30-59  - Score 10</span></span>

    <span data-ttu-id="8b067-119">جـ.</span><span class="sxs-lookup"><span data-stu-id="8b067-119">c.</span></span> <span data-ttu-id="8b067-120">60-200 - النقطة 15</span><span class="sxs-lookup"><span data-stu-id="8b067-120">60-200 - Score 15</span></span>

1. <span data-ttu-id="8b067-121">حدد **حفظ** و **أغلق** الصفحة</span><span class="sxs-lookup"><span data-stu-id="8b067-121">**Save** and **Close** the page</span></span>

## <a name="risk-classification"></a><span data-ttu-id="8b067-122">تصنيف المخاطر</span><span class="sxs-lookup"><span data-stu-id="8b067-122">Risk classification</span></span>

<span data-ttu-id="8b067-123">ستقوم بتغيير **تصنيف المخاطر** وإضافة تصنيف جديد.</span><span class="sxs-lookup"><span data-stu-id="8b067-123">You will change a **Risk classification** and add a new one.</span></span> <span data-ttu-id="8b067-124">يجب تغيير تصنيف المخاطر الحالي لتتمكن من إدخال تصنيف جديد.</span><span class="sxs-lookup"><span data-stu-id="8b067-124">The existing risk classification has to change to be able to insert a new one.</span></span> <span data-ttu-id="8b067-125">لا يمكن أن تكون هناك نطاقات متراكبة في أي وقت.</span><span class="sxs-lookup"><span data-stu-id="8b067-125">There cannot be overlapping ranges at any time.</span></span> 

1. <span data-ttu-id="8b067-126">انتقل إلى **‎الائتمان والتحصيلات > إعداد > إعداد إدارة الائتمان > المخاطر > تصنيف المخاطر**.</span><span class="sxs-lookup"><span data-stu-id="8b067-126">Go to **Credit and collections > Setup > Credit management setup > Risk > Risk classification**.</span></span>
2. <span data-ttu-id="8b067-127">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="8b067-127">Select **Edit**.</span></span>
3. <span data-ttu-id="8b067-128">في الصف الذي تكون فيه **مجموعة المخاطر** بالقيمة **عالٍ**، قم بتغيير رقم القيمة **من** إلى 80.</span><span class="sxs-lookup"><span data-stu-id="8b067-128">On the row where the **Risk group** is **High**, change the **From** number to 80.</span></span>
4. <span data-ttu-id="8b067-129">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="8b067-129">Select **New**.</span></span>
5. <span data-ttu-id="8b067-130">في الحقل **مجموعة المخاطر**، أدخل **متوسط عالي**.</span><span class="sxs-lookup"><span data-stu-id="8b067-130">In the **Risk group** field, enter **MediumHigh**.</span></span>
6. <span data-ttu-id="8b067-131">في حقل **الوصف**، أدخِل **متوسط عالي**.</span><span class="sxs-lookup"><span data-stu-id="8b067-131">In the **Description** field, enter **Medium High**.</span></span>
7. <span data-ttu-id="8b067-132">في حقل **من**، أدخِل **60**.</span><span class="sxs-lookup"><span data-stu-id="8b067-132">In the **From** field, enter **60**.</span></span>
8. <span data-ttu-id="8b067-133">في حقل **إلى**، أدخل **79**.</span><span class="sxs-lookup"><span data-stu-id="8b067-133">In the **To** field, enter **79**.</span></span>
8. <span data-ttu-id="8b067-134">في الحقل **مؤشر مجموعة المخاطر**، حدد **برتقالي**.</span><span class="sxs-lookup"><span data-stu-id="8b067-134">In the **Risk group indicator** field, select **Orange**.</span></span>
8. <span data-ttu-id="8b067-135">حدد **حفظ** و **أغلق** الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8b067-135">**Save** and **Close** the page.</span></span>

## <a name="blocking-rules"></a><span data-ttu-id="8b067-136">قواعد الحظر</span><span class="sxs-lookup"><span data-stu-id="8b067-136">Blocking rules</span></span>

<span data-ttu-id="8b067-137">ستقوم بإعداد قاعدة جديدة لإضافة قواعد لأكثر من عميل واحد موجود في البيانات الأساسية.</span><span class="sxs-lookup"><span data-stu-id="8b067-137">You will set up a new rule to add rules for more than the one customer that is there in the base data.</span></span>

1. <span data-ttu-id="8b067-138">انتقل إلى **الائتمان والتحصيلات > الإعداد > إعداد إدارة الائتمان > قواعد الحظر**</span><span class="sxs-lookup"><span data-stu-id="8b067-138">Go to **Credit and collections > Setup > Credit management setup > Blocking rules**.</span></span>
2. <span data-ttu-id="8b067-139">حدد علامة تبويب **المبلغ المتأخر**.</span><span class="sxs-lookup"><span data-stu-id="8b067-139">Select the tab for **Overdue amount**.</span></span>
3. <span data-ttu-id="8b067-140">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="8b067-140">Select **New**.</span></span>
4. <span data-ttu-id="8b067-141">في الحقل **كود الحساب**، حدد **مجموعة**</span><span class="sxs-lookup"><span data-stu-id="8b067-141">In the **Account code** field, select **Group**.</span></span>
5. <span data-ttu-id="8b067-142">في الحقل **رقم الحساب/المجموعة**، حدد **رئيسي**.</span><span class="sxs-lookup"><span data-stu-id="8b067-142">In the **Account/Group number** field select **Major**.</span></span>
6. <span data-ttu-id="8b067-143">في الحقل **مجموعة المخاطر**، حدد **عالٍ**.</span><span class="sxs-lookup"><span data-stu-id="8b067-143">In the **Risk group** field, select **High**.</span></span>
7. <span data-ttu-id="8b067-144">في الحقل **نوع القاعدة**، حدد **حظر**.</span><span class="sxs-lookup"><span data-stu-id="8b067-144">In the **Rule type** field, select **Blocking**.</span></span>
8. <span data-ttu-id="8b067-145">في حقل **المبلغ المتأخر**، أدخِل **50.000**.</span><span class="sxs-lookup"><span data-stu-id="8b067-145">In the **Overdue amount** field, enter **50,000**.</span></span>
9. <span data-ttu-id="8b067-146">في الحقل **عتبة الحد الائتماني**، أدخل **100**.</span><span class="sxs-lookup"><span data-stu-id="8b067-146">In the **Credit limit threshold** field, enter **100**.</span></span>
10. <span data-ttu-id="8b067-147">حدد **حفظ** و **أغلق** الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8b067-147">**Save** and **Close** the page.</span></span>
 
