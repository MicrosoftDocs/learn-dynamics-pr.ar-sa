---
ms.openlocfilehash: e03fefdc8b1fcd30f9fca23c60409abf6cd5bee5
ms.sourcegitcommit: 13594cb3c8f0b1478f14aac7e239bc20317f480c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/15/2021
ms.locfileid: "6072504"
---
<span data-ttu-id="c0188-101">تحدد أهمية الأصول أهمية الأصل خارج نطاق الإنتاج للوقت المطلوب للصيانة.</span><span class="sxs-lookup"><span data-stu-id="c0188-101">Asset criticality defines importance of the asset being out of production for the time that is needed for maintenance.</span></span> <span data-ttu-id="c0188-102">تحدد أهمية الأصول ما إذا كان سيضر بالإنتاج والمؤسسة إذا كان الأصل الحرج خارج الإنتاج للصيانة.</span><span class="sxs-lookup"><span data-stu-id="c0188-102">Asset criticality determines if it will be harmful to production and the organization if a critical asset is out of production for maintenance.</span></span> <span data-ttu-id="c0188-103">بمعنى آخر، يقوم بحساب مدى تأثير مهمة الصيانة الخاصة بأحد الأصول على جدول الإنتاج والإنتاجية في شركتك.</span><span class="sxs-lookup"><span data-stu-id="c0188-103">In other words, it calculates the extent to which a maintenance job on an asset affects the production schedule and productivity in your company.</span></span> <span data-ttu-id="c0188-104">لمزيد من المعلومات حول الإعداد المرتبط بحساب نقاط التصنيف لجدولة أمر العمل، راجع وحدة **إدارة معلمات الأصول** في هذه الوحدة النمطية.</span><span class="sxs-lookup"><span data-stu-id="c0188-104">For more information about the setup that is related to the calculation of rating scores for work order scheduling, refer to the **Set up asset management parameters** unit in this module.</span></span>

<span data-ttu-id="c0188-105">يعد إعداد درجات الأهمية عملية من خطوتين:</span><span class="sxs-lookup"><span data-stu-id="c0188-105">Setting up criticalities is a two-step process:</span></span>

1.  <span data-ttu-id="c0188-106">يستخدم في إنشاء أنواع الأهمية المستخدمة في إعداد الأصول.</span><span class="sxs-lookup"><span data-stu-id="c0188-106">Create the criticality types that are used in the asset setup.</span></span> 
2.  <span data-ttu-id="c0188-107">قم بإعداد درجات أهمية الأصل.</span><span class="sxs-lookup"><span data-stu-id="c0188-107">Set up asset criticalities.</span></span>

## <a name="set-up-criticality-types"></a><span data-ttu-id="c0188-108">إعداد أنواع الأهمية</span><span class="sxs-lookup"><span data-stu-id="c0188-108">Set up criticality types</span></span>
<span data-ttu-id="c0188-109">لإعداد أنواع الأهمية‬، اتبع هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="c0188-109">To set up criticality types, follow these steps:</span></span>

1.  <span data-ttu-id="c0188-110">انتقل إلى **إدارة الأصول > إعداد > الأصول > أنواع الأهمية**.</span><span class="sxs-lookup"><span data-stu-id="c0188-110">Go to **Asset Management > Setup > Assets > Criticality types**.</span></span>
2.  <span data-ttu-id="c0188-111">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="c0188-111">Select **New**.</span></span>
3.  <span data-ttu-id="c0188-112">في الحقل **الأهمية**، أدخل رقماً يشير إلى الأهمية.</span><span class="sxs-lookup"><span data-stu-id="c0188-112">In the **Criticality** field, enter a number that indicates the criticality.</span></span>
4.  <span data-ttu-id="c0188-113">في الحقل **الاسم**، أدخِل اسماً لنوع الأهمية.</span><span class="sxs-lookup"><span data-stu-id="c0188-113">In the **Name** field, enter a name for the criticality type.</span></span>
5.  <span data-ttu-id="c0188-114">في حقل **العامل**، أدخل رقم عامل.</span><span class="sxs-lookup"><span data-stu-id="c0188-114">In the **Factor** field, enter a factor number.</span></span> 
    - <span data-ttu-id="c0188-115">يتم استخدام هذا الرقم أثناء حساب جدولة أمر العمل لتحديد سجل الأهمية الذي ينبغي استخدامه.</span><span class="sxs-lookup"><span data-stu-id="c0188-115">This number is used during the calculation of work order scheduling to determine the criticality record that should be used.</span></span> <span data-ttu-id="c0188-116">(يتم دائماً استخدام السجل صاحب أعلى عامل.)</span><span class="sxs-lookup"><span data-stu-id="c0188-116">(The record with the highest factor is always used.)</span></span> 
    - <span data-ttu-id="c0188-117">يصبح هذا الرقم مناسباً إذا تم إنشاء بنود الأهمية بنفس قيمة الأهمية.</span><span class="sxs-lookup"><span data-stu-id="c0188-117">This number becomes relevant if criticality lines are created with the same criticality value.</span></span>
    
<span data-ttu-id="c0188-118">الصورة التالية تعرض مثالاً لصفحة **أنواع الأهمية**.</span><span class="sxs-lookup"><span data-stu-id="c0188-118">The following image shows an example of the **Criticality types** page.</span></span>

<span data-ttu-id="c0188-119">**إدارة الأصول > إعداد > الأصول > أنواع الأهمية**.</span><span class="sxs-lookup"><span data-stu-id="c0188-119">**Asset Management > Setup > Assets > Criticality types**</span></span>

![لقطة شاشة لصفحة أنواع الأهمية.](../media/criticality-types-ss.png) 


## <a name="set-up-asset-criticalities"></a><span data-ttu-id="c0188-121">إعداد درجات أهمية الأصل</span><span class="sxs-lookup"><span data-stu-id="c0188-121">Set up asset criticalities</span></span>
<span data-ttu-id="c0188-122">لإعداد درجات أهمية الأصول‬، اتبع هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="c0188-122">To set up asset criticalities, follow these steps:</span></span>

1.  <span data-ttu-id="c0188-123">انتقل إلى **إدارة الأصول > إعداد > درجات أهمية الأصول**.</span><span class="sxs-lookup"><span data-stu-id="c0188-123">Go to **Asset Management > Setup > Asset criticalities**.</span></span>
2.  <span data-ttu-id="c0188-124">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="c0188-124">Select **New**.</span></span>
3.  <span data-ttu-id="c0188-125">حدد المعلومات ذات الصلة، حسب الحاجة، في كل حقل لإنشاء أهمية أصل:</span><span class="sxs-lookup"><span data-stu-id="c0188-125">Select the relevant information, as applicable, in each field to create an asset criticality:</span></span>
    - <span data-ttu-id="c0188-126">موقع العمل</span><span class="sxs-lookup"><span data-stu-id="c0188-126">Functional location</span></span>
    - <span data-ttu-id="c0188-127">نوع الأصل</span><span class="sxs-lookup"><span data-stu-id="c0188-127">Asset type</span></span>
    - <span data-ttu-id="c0188-128">الشركة المصنعة</span><span class="sxs-lookup"><span data-stu-id="c0188-128">Manufacturer</span></span>
    - <span data-ttu-id="c0188-129">النموذج</span><span class="sxs-lookup"><span data-stu-id="c0188-129">Model</span></span>
    - <span data-ttu-id="c0188-130">الأصل</span><span class="sxs-lookup"><span data-stu-id="c0188-130">Asset</span></span>
    - <span data-ttu-id="c0188-131">فئة نوع مهمة الصيانة</span><span class="sxs-lookup"><span data-stu-id="c0188-131">Maintenance job type category</span></span>
    - <span data-ttu-id="c0188-132">نوع مهمة الصيانة</span><span class="sxs-lookup"><span data-stu-id="c0188-132">Maintenance job type</span></span>
    - <span data-ttu-id="c0188-133">متغير نوع مهمة الصيانة</span><span class="sxs-lookup"><span data-stu-id="c0188-133">Maintenance job type variant</span></span>
    - <span data-ttu-id="c0188-134">التجارة</span><span class="sxs-lookup"><span data-stu-id="c0188-134">Trade</span></span>
    - <span data-ttu-id="c0188-135">الأهمية</span><span class="sxs-lookup"><span data-stu-id="c0188-135">Criticality</span></span>
    
    <span data-ttu-id="c0188-136">على سبيل المثال، عند تقسيم سير ناقلة إلى بند الإنتاج الوحيد، يجب إعداد أهمية الأصل باستخدام نوع مهمة صيانة تصحيحية وأهمية عالية.</span><span class="sxs-lookup"><span data-stu-id="c0188-136">For example, when a conveyor belt breaks down on the only production line, the asset criticality should be set up with a corrective maintenance job type and a high criticality.</span></span>

<span data-ttu-id="c0188-137">عند تحديد أهمية الأصل، ستبحث إدارة الأصول عن كافة سجلات الأهمية لفحص وجود تطابق محتمل.</span><span class="sxs-lookup"><span data-stu-id="c0188-137">When an asset criticality is selected, Asset Management searches all criticality records to check for a possible match.</span></span> 

<span data-ttu-id="c0188-138">وهي تقوم دائماً بفحص المجموعة الأكثر تحديداً.</span><span class="sxs-lookup"><span data-stu-id="c0188-138">It always checks the most specific combination first.</span></span>
 
- <span data-ttu-id="c0188-139">البدء في الحقل **تجارة**، في حالة عدم العثور على أي تطابق، فإنه يقوم بالتحقق من الحقل **متغير نوع مهمة الصيانة** ويستمر في الانتقال خلال كل حقل من اليمين إلى اليسار.</span><span class="sxs-lookup"><span data-stu-id="c0188-139">Starting in the **Trade** field, if no match is found, it checks the **Maintenance job type variant** field and continues to go through each field from right to left.</span></span> 
- <span data-ttu-id="c0188-140">في حالة عدم العثور على أي تطابق، يتم استخدام السجل "الافتراضي" الذي لا يحتوي على تحديدات.</span><span class="sxs-lookup"><span data-stu-id="c0188-140">If no match is found, the "default" record that has no selections is used.</span></span>

<span data-ttu-id="c0188-141">تعرض الصورة التالية مثالاً لصفحة **درجات أهمية الأصل**.</span><span class="sxs-lookup"><span data-stu-id="c0188-141">The following image shows an example of the **Asset criticalities** page.</span></span>

<span data-ttu-id="c0188-142">**إدارة الأصول > إعداد > درجات أهمية الأصول**.</span><span class="sxs-lookup"><span data-stu-id="c0188-142">**Asset Management > Setup > Asset criticalities**</span></span>
 
<span data-ttu-id="c0188-143">[![لقطة شاشة لصفحة درجات أهمية الأصل.](../media/asset-criticalities-ss.png)](../media/asset-criticalities-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="c0188-143">[![Screenshot of the Asset criticalities page.](../media/asset-criticalities-ss.png)](../media/asset-criticalities-ss.png#lightbox)</span></span> 


<span data-ttu-id="c0188-144">وهناك بعض الاعتبارات الخاصة بإعداد أهمية الأصول:</span><span class="sxs-lookup"><span data-stu-id="c0188-144">A few considerations about asset criticality setup:</span></span>

- <span data-ttu-id="c0188-145">إذا قمت بتغيير أهمية الأصل بعد استخدامه بالفعل في أمر العمل، فلن يتم تحديث الأهمية الجديدة في أمر العمل وفقا لذلك.</span><span class="sxs-lookup"><span data-stu-id="c0188-145">If you change an asset criticality after you've already used it on a work order, the new criticality on the work order isn't updated accordingly.</span></span>
- <span data-ttu-id="c0188-146">وتتم إعادة حساب الأهمية في أمر العمل في كل مرة يتم فيها إضافة بند أمر عمل أو حذفه من أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="c0188-146">The criticality on a work order is recalculated every time a work order line is added to or deleted from the work order.</span></span>
- <span data-ttu-id="c0188-147">إذا كان أمر العمل يحتوي على العديد من وظائف أمر العمل، فان أعلى أهمية، وفقا لحقل العامل في الصفحة أنواع الأهمية، يتم استخدامها دائماً في أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="c0188-147">If a work order contains several work order jobs, the highest criticality, according to the Factor field on the Criticality types page, is always used on the work order.</span></span>
- <span data-ttu-id="c0188-148">يمكن أن تتغير أهمية الأصول في فترة وتكون متأثرة عادة بشراء معدات جديدة وعمليات التجديد وغير ذلك.</span><span class="sxs-lookup"><span data-stu-id="c0188-148">Asset criticality can change over a period and is usually affected by the purchase of new equipment, refurbishments, and so on.</span></span> <span data-ttu-id="c0188-149">يجب مراعاة إعادة تقييم أهمية الأصل في فترات منتظمة لضمان مطابقة تعريفات الأهمية الخاصة بك لإعداد الإنتاج الحالي.</span><span class="sxs-lookup"><span data-stu-id="c0188-149">Consider reevaluating your asset criticalities at regular intervals to ensure that your criticality definitions match your current production setup.</span></span>
