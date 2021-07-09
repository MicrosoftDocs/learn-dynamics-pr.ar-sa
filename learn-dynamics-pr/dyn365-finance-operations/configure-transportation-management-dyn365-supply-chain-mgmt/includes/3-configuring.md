---
ms.openlocfilehash: f2ac813f9c2f80350232cc69f43fe693a435289c
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073795"
---
## <a name="rate-masters"></a><span data-ttu-id="514e4-101">أصول السعر</span><span class="sxs-lookup"><span data-stu-id="514e4-101">Rate masters</span></span> 

<span data-ttu-id="514e4-102">تعد أصول السعر جزءاً رئيسياً من إعداد التصنيف لشركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-102">Rate masters are a key part of the rating setup for a shipping carrier.</span></span> <span data-ttu-id="514e4-103">يمكنك استخدام أصول السعر لتحديد الأسعار المتوفرة لشركة الشحن ولتحديد ما إذا كانت الأسعار تبرر مراعاة شركة الشحن لتعيينٍ ما.</span><span class="sxs-lookup"><span data-stu-id="514e4-103">You can use rate masters to determine the available rates for the shipping carrier and to determine whether the rates justify considering the shipping carrier for an assignment.</span></span> <span data-ttu-id="514e4-104">يقترن أصل السعر بشركة شحن في ملف تعريف تصنيف شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-104">The rate master is associated with a shipping carrier in the carrier's rating profile.</span></span> <span data-ttu-id="514e4-105">بالنسبة لكل أصل سعر، يجب تحديد بيانات تعريف التصنيف وأساس سعر.</span><span class="sxs-lookup"><span data-stu-id="514e4-105">For each rate master, you must define rating metadata and a rate base.</span></span>

![الرسم التخطيطي لعملية التصنيف في إدارة النقل.](../media/rating-process.png)

<span data-ttu-id="514e4-107">قبل إعداد أصل سعر، يجب إعداد مجموعة واحدة على الأقل من بيانات تعريف التصنيف.</span><span class="sxs-lookup"><span data-stu-id="514e4-107">Before setting up a rate master, you must set up at least one set of rating metadata.</span></span> <span data-ttu-id="514e4-108">يمكن تطبيق بيانات تعريف التصنيف على أي أصل سعر،، وتحدد معايير البحث المستخدمة لتحديد أسعار شركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-108">The rating metadata can be applied to any rate master, and it defines lookup criteria that are used to determine rates of a shipping carrier.</span></span>

<span data-ttu-id="514e4-109">يتطلب إعداد بيانات تعريف التصنيف إجراء المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-109">Setting up rating metadata requires the following tasks:</span></span>

-   <span data-ttu-id="514e4-110">إعداد بيانات تعريف التصنيف بمعايير البحث، مثل الرمز البريدي وخدمة شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-110">Set up rating metadata with lookup criteria, such as a postal code and carrier service.</span></span>
-   <span data-ttu-id="514e4-111">إقران أصل السعر ببيانات تعريف التصنيف، وفي أصل السعر، قم بتوفير قيم المعايير، مثل الرمز البريدي وخدمة شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-111">Associate a rate master with the rating metadata and, on the rate master, provide values for criteria, such as a postal code and carrier service.</span></span> <span data-ttu-id="514e4-112">يقترن أصل سعر واحد أو أكثر بشركة شحن في علامة التبويب السريعة **ملف تعريف التصنيف**.</span><span class="sxs-lookup"><span data-stu-id="514e4-112">One or more rate masters are associated with a shipping carrier on the **Rating profile** FastTab.</span></span> <span data-ttu-id="514e4-113">يمكنك استخدام أصول السعر لتحديد الأسعار المتوفرة لشركة الشحن ولتحديد ما إذا كانت الأسعار تبرر مراعاة شركة الشحن لتعيينٍ ما.</span><span class="sxs-lookup"><span data-stu-id="514e4-113">You can use rate masters to determine the available rates for the shipping carrier and to determine whether the rates justify considering the shipping carrier for an assignment.</span></span>

<span data-ttu-id="514e4-114">يحدد الفاصل الرئيسي قيم الفاصل التي يجب ربطها بأساس السعر.</span><span class="sxs-lookup"><span data-stu-id="514e4-114">The break master defines the break values that you must associate with the rate base.</span></span>

<span data-ttu-id="514e4-115">على سبيل المثال، يتم تنظيم المسافات إلى نقاط التوقف من 50 و100 و150 ميلاً.</span><span class="sxs-lookup"><span data-stu-id="514e4-115">For example, distances are structured into breakpoints of 50, 100, and 150 miles.</span></span> <span data-ttu-id="514e4-116">يتم فرض رسوم بمبلغ 10.00 دولارات أمريكية على ما يصل إلى 50 ميلاً لكل تعيين، ويتم فرض رسوم بمبلغ 18.00 دولار أمريكي على ما يتراوح بين 50 و100 ميل، و20.00 دولاراً أمريكياً على ما يتراوح بين 100 و150 ميلاً.</span><span class="sxs-lookup"><span data-stu-id="514e4-116">Up to 50 miles is charged with USD 10.00 for each assignment, between 50 and 100 miles is charged with USD 18.00, and from 100 to 150 miles is charged with USD 20.00.</span></span>

<span data-ttu-id="514e4-117">إذا كنت تريد إعداد بنية تعريفة لأصل السعر، فيمكنك إنشاء أساس سعر.</span><span class="sxs-lookup"><span data-stu-id="514e4-117">If you want to set up a tariff structure for the rate master, you can create a rate base.</span></span> <span data-ttu-id="514e4-118">سيقوم أساس السعر بهيكلة الأسعار في نقاط توقف.</span><span class="sxs-lookup"><span data-stu-id="514e4-118">The rate base will structure rates in breakpoints.</span></span>

<span data-ttu-id="514e4-119">ولحساب الأسعار، يجب إنشاء محرك واحد أو أكثر أو تهيئة بيانات المحرك الأساسي تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="514e4-119">To calculate rates, you must create one or more engines or automatically initialize the base engine data.</span></span> <span data-ttu-id="514e4-120">يمكنك البحث عن أسعار الشحن المتوفرة استناداً إلى معلومات مثل مسافة السفر أو المناطق في منطقة ما.</span><span class="sxs-lookup"><span data-stu-id="514e4-120">You can search for available shipment rates based on information such as travel distance or zones in a region.</span></span> <span data-ttu-id="514e4-121">يتم تفسير معايير البحث بواسطة محركات إدارة النقل التي تحسب الأسعار المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="514e4-121">The search criteria are interpreted by transportation management engines that calculate the available rates.</span></span>

<span data-ttu-id="514e4-122">وأخيراً، سيمكنك القيام بربط جميع معلومات التصنيف بشركة نقل من خلال إنشاء ملف تعريف تصنيف ثم تحديد ملف تعريف تصنيف واحد أو أكثر في علامة التبويب السريعة **ملفات تعريف التصنيف** بالصفحة **شركات الشحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-122">Finally, you will link all the rating information to a carrier by creating a rating profile and then selecting one or more rating profiles on the **Rating profiles** FastTab of the **Shipping carriers** page.</span></span>

## <a name="rating-metadata"></a><span data-ttu-id="514e4-123">بيانات تعريف التصنيف</span><span class="sxs-lookup"><span data-stu-id="514e4-123">Rating metadata</span></span> 

<span data-ttu-id="514e4-124">تشير بيانات تعريف التصنيف إلى مجموعة فريدة من المحددات أو الحقول التي تستخدمها شركات النقل والخدمات لتحديد تعريفة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-124">Rating metadata refers to a unique set of determinants or fields that are used by the carriers and services to determine the transportation tariff.</span></span> <span data-ttu-id="514e4-125">تحتوي كل مجموعة من بيانات التعريف على تعيينات الأسعار، والتي هي الحد الأدنى من مجموعة السمات المطلوبة لحساب التعريفة لشحنة محددة.</span><span class="sxs-lookup"><span data-stu-id="514e4-125">Each set of metadata includes rate assignments, which are a minimum set of attributes that are required to calculate the tariff for a given shipment.</span></span>

<span data-ttu-id="514e4-126">على سبيل المثال، قد تتضمن السمات دولة أو منطقة الأصل والرمز البريدي إلى جانب الدولة أو المنطقة الوجهة للشحنة والرمز البريدي.</span><span class="sxs-lookup"><span data-stu-id="514e4-126">For example, attributes might include the origin's country or region and zip code, along with the shipment's destination country or region and zip code.</span></span> <span data-ttu-id="514e4-127">يتم تعيين بيانات التعيينات إلى نوع بحث، وهو حقل بيانات رئيسية مقابل في النظام مثل رمز أقل من حمولة شاحنة (LTL) ورمز سلعة النقل القياسي (STCC) والرمز البريدي وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="514e4-127">The data for the assignments are assigned to a lookup type, which is a corresponding master data field in the system such as a less than truckload (LTL) code, Standard transportation commodity code (STCC), postal code, and so on.</span></span>

<span data-ttu-id="514e4-128">اتبع الخطوات الواردة في هذا الإجراء لإعداد أصل سعر لشركة نقل جوي:</span><span class="sxs-lookup"><span data-stu-id="514e4-128">Follow the steps in this procedure to set up a rate master for an air carrier:</span></span>

1.  <span data-ttu-id="514e4-129">انتقل إلى **إدارة النقل > إعداد > تصنيف > أصل السعر**.</span><span class="sxs-lookup"><span data-stu-id="514e4-129">Go to **Transportation management > Setup > Rating > Rate master**.</span></span>
2.  <span data-ttu-id="514e4-130">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-130">Select **New**.</span></span>
3.  <span data-ttu-id="514e4-131">في حقل **أصل السعر**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="514e4-131">In the **Rate master** field, enter a value.</span></span>
4.  <span data-ttu-id="514e4-132">في حقل **الاسم**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="514e4-132">In the **Name** field, enter a value.</span></span>
5.  <span data-ttu-id="514e4-133">في حقل **معرف بيانات تعريف التصنيف**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="514e4-133">In the **Rating metadata ID** field, select the drop-down button to open the lookup.</span></span> 
    <span data-ttu-id="514e4-134">سيحدد معرف بيانات تعريف التصنيف البيانات المطلوبة لأصل السعر لأنه يحدد بيانات التعريف المتوقعة بواسطة محرك ‬‏‫إدارة النقل (TMS) الذي يستخدم أصل السعر هذا.</span><span class="sxs-lookup"><span data-stu-id="514e4-134">The rating metadata ID will determine the data that is needed for the rate master because it defines the metadata that is expected by the TMS engine that is using this rate master.</span></span>
6.  <span data-ttu-id="514e4-135">حدد الخيار **P2P** (على سبيل المثال).</span><span class="sxs-lookup"><span data-stu-id="514e4-135">Select the **P2P** option (for example).</span></span>
7.  <span data-ttu-id="514e4-136">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="514e4-136">Select **Save**.</span></span>
8.  <span data-ttu-id="514e4-137">لإعداد أساس السعر، حدد **أساس السعر** في القائمة الموجودة أعلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-137">To set up the rate base, select **Rate base** on the menu at the top of the page.</span></span>
9.  <span data-ttu-id="514e4-138">حدد **جديد**،</span><span class="sxs-lookup"><span data-stu-id="514e4-138">Select **New**.</span></span>
10. <span data-ttu-id="514e4-139">في حقل **أساس السعر**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="514e4-139">In the **Rate base** field, enter a value.</span></span>
11. <span data-ttu-id="514e4-140">في حقل **الاسم**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="514e4-140">In the **Name** field, enter a value.</span></span>
12. <span data-ttu-id="514e4-141">في حقل **الفاصل الرئيسي**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="514e4-141">In the **Break master** field, select the drop-down button to open the lookup.</span></span>
13. <span data-ttu-id="514e4-142">بالنسبة لهذا المثال، حدد **الوزن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-142">For this example, select **Weight**.</span></span>
14. <span data-ttu-id="514e4-143">قم بتوسيع قسم **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-143">Expand the **Details** section.</span></span>
15. <span data-ttu-id="514e4-144">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-144">Select **New**.</span></span>
16. <span data-ttu-id="514e4-145">في حقل **الرمز البريدي للتسليم من**، أدخل **30301**.</span><span class="sxs-lookup"><span data-stu-id="514e4-145">In the **Drop-off postal code from** field, enter **30301**.</span></span>
17. <span data-ttu-id="514e4-146">في حقل **الرمز البريدي للتسليم إلى**، أدخل **30318**.</span><span class="sxs-lookup"><span data-stu-id="514e4-146">In the **Drop-off postal code to** field, enter **30318**.</span></span>
18. <span data-ttu-id="514e4-147">في حقل **بلد/منطقة التسليم**، أدخل **الولايات المتحدة الأمريكية**.</span><span class="sxs-lookup"><span data-stu-id="514e4-147">In the **Drop-off country region** field, enter **USA**.</span></span>
19. <span data-ttu-id="514e4-148">في حقل **<1.00 رطل**، أدخل **100**.</span><span class="sxs-lookup"><span data-stu-id="514e4-148">In the **<1.00 Lbs** field, enter **100**.</span></span> <span data-ttu-id="514e4-149">قم بإدراج السعر لكل رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-149">Insert the rate per lbs.</span></span> <span data-ttu-id="514e4-150">إذا كان الوزن الإجمالي للحمل أقل من 1 رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-150">if the total weight of the load is less than 1 pound.</span></span>
20. <span data-ttu-id="514e4-151">في حقل **<5.00 أرطال**، أدخل **300**.</span><span class="sxs-lookup"><span data-stu-id="514e4-151">In the **<5.00 Lbs** field, enter **300**.</span></span> <span data-ttu-id="514e4-152">قم بإدراج السعر لكل رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-152">Insert the rate per lbs.</span></span> <span data-ttu-id="514e4-153">إذا كان الوزن الإجمالي للحمل أقل من 5 أرطال.</span><span class="sxs-lookup"><span data-stu-id="514e4-153">if the total weight of the load is less than 5 pounds.</span></span>
21. <span data-ttu-id="514e4-154">في حقل **<20.00 رطلاً**، أدخل **500**.</span><span class="sxs-lookup"><span data-stu-id="514e4-154">In the **<20.00 Lbs** field, enter **500**.</span></span> <span data-ttu-id="514e4-155">قم بإدراج السعر لكل رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-155">Insert the rate per lbs.</span></span> <span data-ttu-id="514e4-156">إذا كان الوزن الإجمالي للحمل أقل من 20 رطلاً.</span><span class="sxs-lookup"><span data-stu-id="514e4-156">if the total weight of the load is less than 20 pounds.</span></span>
22. <span data-ttu-id="514e4-157">في حقل **<100.00 رطل**، أدخل **1000**.</span><span class="sxs-lookup"><span data-stu-id="514e4-157">In the **<100.00 Lbs** field, enter **1000**.</span></span> <span data-ttu-id="514e4-158">قم بإدراج السعر لكل رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-158">Insert the rate per lbs.</span></span> <span data-ttu-id="514e4-159">إذا كان الوزن الإجمالي للحمل أقل من 100 رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-159">if the total weight of the load is less than 100 pounds.</span></span>
23. <span data-ttu-id="514e4-160">في حقل **<1,000.00 رطل**، أدخل **3000**.</span><span class="sxs-lookup"><span data-stu-id="514e4-160">In the **<1,000.00 Lbs** field, enter **3000**.</span></span> <span data-ttu-id="514e4-161">قم بإدراج السعر لكل رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-161">Insert the rate per lbs.</span></span> <span data-ttu-id="514e4-162">إذا كان الوزن الإجمالي للحمل أقل من 1000 رطل.</span><span class="sxs-lookup"><span data-stu-id="514e4-162">if the total weight of the load is less than 1000 pounds.</span></span>
24. <span data-ttu-id="514e4-163">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="514e4-163">Select **Save**.</span></span>
25. <span data-ttu-id="514e4-164">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-164">Close the page.</span></span>
26. <span data-ttu-id="514e4-165">لتعيين أساس السعر، قم بتوسيع قسم **تعيينات أسس الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="514e4-165">To assign the rate base, expand the **Rate base assignments** section.</span></span>
27. <span data-ttu-id="514e4-166">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-166">Select **New**.</span></span> <span data-ttu-id="514e4-167">يمكن أن يكون لديك العديد من تعيينات أسس الأسعار لكل أصل سعر.</span><span class="sxs-lookup"><span data-stu-id="514e4-167">You can have several rate base assignments for each rate master.</span></span> <span data-ttu-id="514e4-168">يسمح لك وجود تعيينات متعددة بإنشاء عدة نقاط أسعار مختلفة لكل شركة نقل اعتماداً على الوجهات أو الخدمات أو أسس الأسعار المختلفة.</span><span class="sxs-lookup"><span data-stu-id="514e4-168">Having several assignments allows you to create several different price points for each carrier depending on destinations, services, or different rate bases.</span></span> <span data-ttu-id="514e4-169">ستقوم في هذا الإجراء بإنشاء تعيين أساس سعر واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="514e4-169">In this procedure, you will only create one rate base assignment.</span></span>
28. <span data-ttu-id="514e4-170">في حقل **الاسم**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="514e4-170">In the **Name** field, enter a value.</span></span>
29. <span data-ttu-id="514e4-171">في حقل **أساس السعر**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="514e4-171">In the **Rate base** field, select the drop-down button to open the lookup.</span></span>
30. <span data-ttu-id="514e4-172">في القائمة، ابحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="514e4-172">In the list, find and select the desired record.</span></span>
31. <span data-ttu-id="514e4-173">في حقل **الخدمة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="514e4-173">In the **Service** field, select the drop-down button to open the lookup.</span></span>
32. <span data-ttu-id="514e4-174">في القائمة، ابحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="514e4-174">In the list, find and select the desired record.</span></span>
33. <span data-ttu-id="514e4-175">في حقل **الرمز البريدي لمكان الانتقاء**، أدخل **98052**.</span><span class="sxs-lookup"><span data-stu-id="514e4-175">In the **Pick-up Postal Code** field, enter **98052**.</span></span> <span data-ttu-id="514e4-176">حدد الرمز البريدي الذي يجب أن يكون تعيين أسس الأسعار صالحاً بداية منه.</span><span class="sxs-lookup"><span data-stu-id="514e4-176">Specify which postal code this rate base assignment should be valid from.</span></span>
34. <span data-ttu-id="514e4-177">في حقل **بلد/منطقة الانتقاء**، أدخل **الولايات المتحدة الأمريكية**.</span><span class="sxs-lookup"><span data-stu-id="514e4-177">In the **Pick-up Country Region** field, enter **USA**.</span></span>
35. <span data-ttu-id="514e4-178">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="514e4-178">Select **Save**.</span></span>

<span data-ttu-id="514e4-179">بيانات تعريف التصنيف خاصة بالمحرك.</span><span class="sxs-lookup"><span data-stu-id="514e4-179">Rating metadata is engine-specific.</span></span> <span data-ttu-id="514e4-180">يجب إعداد بيانات تعريف التصنيف قبل إعداد محرك أسعار.</span><span class="sxs-lookup"><span data-stu-id="514e4-180">You must set up rating metadata before setting up a rate engine.</span></span>

<span data-ttu-id="514e4-181">يتم إنشاء بيانات تعريف التصنيف المطلوبة للمحركات التي يتم شحنها مع إدارة سلاسل التوريدات مع المحركات عند تحديد الزر **تهيئة بيانات المحرك الأساسي** في الصفحة **إدارة النقل > إعداد > معلمات أداره النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-181">The rating metadata that is required for the engines that are shipped with Supply Chain Management is generated with the engines when you select the **Initialize base engine data** button on the **Transportation management > Setup > Transportation management parameters** page.</span></span>

![تم تمييز لقطة شاشة صفحة معلمات أداره النقل بتهيئة بيانات المحرك الأساسي.](../media/initialize-base-engine-data.png) 

<span data-ttu-id="514e4-183">لا نوصي بإنشاء بيانات تعريف التصنيف الخاصة بك للمحركات الموجودة؛ فهذه الطريقة معرضة للأخطاء لأنها يمكن أن تتسبب في فشل المحرك ما لم تتوافق بيانات تعريف التصنيف بدقة مع قواعد المحرك.</span><span class="sxs-lookup"><span data-stu-id="514e4-183">We don't recommend that you create your own rating metadata for existing engines; this approach is error-prone because it can cause the engine to fail unless the rating metadata strictly conforms to the rules of the engine.</span></span>

1.  <span data-ttu-id="514e4-184">افتح **إدارة النقل > إعداد > تصنيف > بيانات تعريف التصنيف**.</span><span class="sxs-lookup"><span data-stu-id="514e4-184">Open **Transportation management > Setup > Rating > Rating metadata**.</span></span>
2.  <span data-ttu-id="514e4-185">حدد **جديد** لإنشاء بيانات تعريف تصنيف جديدة.</span><span class="sxs-lookup"><span data-stu-id="514e4-185">Select **New** to create new rating metadata.</span></span>
3.  <span data-ttu-id="514e4-186">أدخل معرفاً واسماً فريدين لنوع أساس السعر.</span><span class="sxs-lookup"><span data-stu-id="514e4-186">Enter a unique ID and name for the rate base type.</span></span>

<span data-ttu-id="514e4-187">في هذا المثال، ستقوم بإعداد أساسين للسعر وإعداد تعيين، ثم جعلها كلها إلزامية.</span><span class="sxs-lookup"><span data-stu-id="514e4-187">In this example, you will set up two rate bases, set up an assignment, and then make them all mandatory.</span></span>

1.  <span data-ttu-id="514e4-188">في حقل **نوع البيانات الموصوفة**، حدد **أساس السعر** لإعداد حقول المعايير.</span><span class="sxs-lookup"><span data-stu-id="514e4-188">In the **Described data type** field, select **Rate base** to set up criteria fields.</span></span>
2.  <span data-ttu-id="514e4-189">في علامة التبويب السريعة **بيانات تعريف نوع أساس السعر**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-189">In the **Rate base type metadata** FastTab, select **New**.</span></span>
3.  <span data-ttu-id="514e4-190">في حقل **نوع البيانات**، حدد **عدداً صحيحاً** لنوع إدخال البيانات.</span><span class="sxs-lookup"><span data-stu-id="514e4-190">In the **Data type** field, select **Integer** for the input type of the data.</span></span>
4.  <span data-ttu-id="514e4-191">في حقل **نوع البحث**، حدد **الرمز البريدي**.</span><span class="sxs-lookup"><span data-stu-id="514e4-191">In the **Lookup type** field, select **ZIP/Postal code**.</span></span>
5.  <span data-ttu-id="514e4-192">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="514e4-192">Select the **Mandatory** check box.</span></span>
6.  <span data-ttu-id="514e4-193">في حقل **نوع البيانات الموصوفة**، حدد **أساس السعر** لإعداد حقول المعايير.</span><span class="sxs-lookup"><span data-stu-id="514e4-193">In the **Described data type** field, select **Rate base** to set up criteria fields.</span></span>
7.  <span data-ttu-id="514e4-194">في علامة التبويب السريعة **بيانات تعريف نوع أساس السعر**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-194">In the **Rate base type metadata** FastTab, select **New**.</span></span>
8.  <span data-ttu-id="514e4-195">في حقل **نوع البيانات**، حدد **سلسلة** لنوع إدخال البيانات.</span><span class="sxs-lookup"><span data-stu-id="514e4-195">In the **Data type** field, select **String** for the input type of the data.</span></span>
9.  <span data-ttu-id="514e4-196">في حقل **نوع البحث**، حدد **المنطقة**.</span><span class="sxs-lookup"><span data-stu-id="514e4-196">In the **Lookup type** field, select **Region**.</span></span>
10. <span data-ttu-id="514e4-197">حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="514e4-197">Select the **Mandatory** check box.</span></span>
11. <span data-ttu-id="514e4-198">في حقل **نوع البيانات الموصوفة**، حدد **التعيين** لإعداد حقول المعايير.</span><span class="sxs-lookup"><span data-stu-id="514e4-198">In the **Described data type** field, select **Assignment** to set up criteria fields.</span></span>
12. <span data-ttu-id="514e4-199">في علامة التبويب السريعة **بيانات تعريف نوع أساس السعر**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-199">In the **Rate base type metadata** FastTab, select **New**.</span></span>
13. <span data-ttu-id="514e4-200">في حقل **نوع البيانات**، حدد **حقيقي** لنوع إدخال البيانات.</span><span class="sxs-lookup"><span data-stu-id="514e4-200">In the **Data type** field, select **Real** for the input type of the data.</span></span>
14. <span data-ttu-id="514e4-201">في حقل **نوع البحث**، حدد النوع.</span><span class="sxs-lookup"><span data-stu-id="514e4-201">In the **Lookup type** field, select a type.</span></span>
15. <span data-ttu-id="514e4-202">اختيارياً، حدد خانة الاختيار **إلزامي**.</span><span class="sxs-lookup"><span data-stu-id="514e4-202">Optionally, select the **Mandatory** check box.</span></span>
16. <span data-ttu-id="514e4-203">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-203">Close the page.</span></span>

<span data-ttu-id="514e4-204">إذا كنت تقوم بإنشاء نوع أساس سعر بثلاثة أسس أسعار وأربعة تعيينات، فيمكنك تحديد أحد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-204">If you are creating a rate base type with three rate bases and four assignments, you could select one of the following options:</span></span>

-   <span data-ttu-id="514e4-205">فئة رمز سلعة النقل القياسية (STCC) - سلسلة</span><span class="sxs-lookup"><span data-stu-id="514e4-205">STCC class - string</span></span>
-   <span data-ttu-id="514e4-206">‬‏‫المسافة بالميل - عدد صحيح أو حقيقي</span><span class="sxs-lookup"><span data-stu-id="514e4-206">Mileage - integer or real</span></span>
-   <span data-ttu-id="514e4-207">الوزن - حقيقي</span><span class="sxs-lookup"><span data-stu-id="514e4-207">Weight - real</span></span>

<span data-ttu-id="514e4-208">الخيارات الخاصة بأسس الأسعار هي:</span><span class="sxs-lookup"><span data-stu-id="514e4-208">The options for the rate bases are:</span></span>

-   <span data-ttu-id="514e4-209">بلد/منطقه الأصل - سلسلة</span><span class="sxs-lookup"><span data-stu-id="514e4-209">Origin country/region - string</span></span>
-   <span data-ttu-id="514e4-210">الرمز البريدي للأصل - عدد صحيح</span><span class="sxs-lookup"><span data-stu-id="514e4-210">Origin zip code - integer</span></span>
-   <span data-ttu-id="514e4-211">بلد/منطقه الوجهة - سلسلة</span><span class="sxs-lookup"><span data-stu-id="514e4-211">Destination country/region - string</span></span>
-   <span data-ttu-id="514e4-212">الرمز البريدي للوجهة - عدد صحيح</span><span class="sxs-lookup"><span data-stu-id="514e4-212">Destination zip code - integer</span></span>

<span data-ttu-id="514e4-213">رمز سلعة النقل القياسي (STCC) هو منشور يحتوي على معلومات منتج محددة يتم استخدامها في بيانات الشحن ومستندات الشحن الأخرى.</span><span class="sxs-lookup"><span data-stu-id="514e4-213">The Standard transportation commodity code (STCC) is a publication that contains specific product information that is used on waybills and other shipping documents.</span></span> <span data-ttu-id="514e4-214">رمز سلعة النقل القياسي (STCC) هو رمز رقمي مكون من سبعة أرقام يمثل سلعة.</span><span class="sxs-lookup"><span data-stu-id="514e4-214">An STCC is a seven-digit numeric code that represents a commodity.</span></span>

<span data-ttu-id="514e4-215">يرتبط تعيين رمز سلعة النقل القياسي بوصف السلعة الذي تم تطويره ليتوافق مع الأوصاف الدقيقة في تصنيفات نقل الشحن للسكك الحديدية وشركات نقل السيارات.</span><span class="sxs-lookup"><span data-stu-id="514e4-215">Assignment of an STCC is associated by a commodity description that was developed to conform to exact descriptions in freight transportation classifications of rail and motor carriers.</span></span> <span data-ttu-id="514e4-216">ويرافق رمز سلعة النقل القياسي رمزان مقابلان هما: نظام الترميز المنسق لوصف السلع، أو الرمز المنسق، وفئة التصنيف القياسي للبضائع المنقولة (SCTG).</span><span class="sxs-lookup"><span data-stu-id="514e4-216">Accompanying an STCC are two corresponding codes: the Harmonized commodity description coding system, or Harmonized code, and a Standard classification of transported goods (SCTG) category.</span></span>

<span data-ttu-id="514e4-217">تشير فئة أقل من حمولة شاحنة (LTL) إلى رمز التصنيف الوطني للشحن بالمحركات (NMFC) وهي فئة من فئات شحن LTL الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="514e4-217">The less-than-truckload (LTL) class refers to the National motor freight classification (NMFC) code and is a category of your LTL freight.</span></span> <span data-ttu-id="514e4-218">تحدد فئة الشحن رسوم الشحن الخاصة بشركة النقل من خلال تحديد حجم الشحن طويل الأمد وقيمته وصعوبة نقله.</span><span class="sxs-lookup"><span data-stu-id="514e4-218">The freight class determines the carrier shipping charges by identifying the size, value, and difficulty of transporting your LTL freight.</span></span>

### <a name="set-up-a-new-ltl-class"></a><span data-ttu-id="514e4-219">إعداد فئة أقل من حمولة شاحنة (LTL) جديدة</span><span class="sxs-lookup"><span data-stu-id="514e4-219">Set up a new LTL class</span></span>

<span data-ttu-id="514e4-220">لإعداد فئة أقل من حمولة شاحنة (LTL) جديدة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-220">To set up a new LTL class, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-221">افتح **إدارة النقل > إعداد > معايير النقل > فئات ‬‏‫أقل من حمولة شاحنة (LTL)**.</span><span class="sxs-lookup"><span data-stu-id="514e4-221">Open **Transportation Management > Setup > Transportation standards > LTL classes**.</span></span>
2.  <span data-ttu-id="514e4-222">حدد **جديد** وقم بإنشاء رموز فئات أقل من حمولة شاحنة (LTL) (أو تحرير الموجودة).</span><span class="sxs-lookup"><span data-stu-id="514e4-222">Select **New** and create (or edit existing) LTL class codes.</span></span>
3.  <span data-ttu-id="514e4-223">أدخل قيمة في حقل **فئة أقل من حمولة شاحنة (LTL)**.</span><span class="sxs-lookup"><span data-stu-id="514e4-223">Enter a value in the **LTL class** field.</span></span>
4.  <span data-ttu-id="514e4-224">أدخل قيمة في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="514e4-224">Enter a value in the **Name** field.</span></span>
5.  <span data-ttu-id="514e4-225">أدخل قيمة في حقل **الفئة**.</span><span class="sxs-lookup"><span data-stu-id="514e4-225">Enter a value in the **Class** field.</span></span>
6.  <span data-ttu-id="514e4-226">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-226">Close the page.</span></span>

### <a name="create-an-stcc-code"></a><span data-ttu-id="514e4-227">إنشاء رمز ‏‫ سلعة نقل قياسي (STCC)</span><span class="sxs-lookup"><span data-stu-id="514e4-227">Create an STCC code</span></span>

<span data-ttu-id="514e4-228">لإنشاء ‏‫رمز سلعة النقل القياسي (STCC)، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="514e4-228">To create an STCC code, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-229">افتح **إدارة النقل > إعداد > معايير النقل > رموز سلع النقل القياسية (STCC)**.</span><span class="sxs-lookup"><span data-stu-id="514e4-229">Open **Transportation management > Setup > Transportation standards > STCC codes**.</span></span>
2.  <span data-ttu-id="514e4-230">حدد **جديد** لإنشاء ‏‫رمز سلعة نقل قياسي (STCC) جديد.</span><span class="sxs-lookup"><span data-stu-id="514e4-230">Select **New** to create a new STCC code.</span></span>
3.  <span data-ttu-id="514e4-231">أدخل معرفاً واسماً وصفياً فريدين ل‏‫رمز سلعة النقل القياسي (STCC) .</span><span class="sxs-lookup"><span data-stu-id="514e4-231">Enter a unique ID and descriptive name for the STCC code.</span></span>
4.  <span data-ttu-id="514e4-232">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-232">Close the page.</span></span>

<span data-ttu-id="514e4-233">يحدد رمز التصنيف الوطني للشحن بالمحركات (NMFC) كيفية تصنيف الصنف لشركات نقل معينة.</span><span class="sxs-lookup"><span data-stu-id="514e4-233">The National motor freight classification (NMFC) code determines how the item is rated for certain carriers.</span></span> <span data-ttu-id="514e4-234">من المهم أيضاً تحديد رمز بوليصة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-234">It is also important to specify the code for the bill of lading.</span></span>  

<span data-ttu-id="514e4-235">بعد إنشاء رموز LTL، يمكنك إنشاء رموز NMFC في إدارة سلاسل التوريدات.</span><span class="sxs-lookup"><span data-stu-id="514e4-235">After you have created the LTL codes, you can create the NMFC codes in Supply Chain Management.</span></span> <span data-ttu-id="514e4-236">في معظم الحالات، ستكون الفئة هي نفسها لفئة NMFC وLTL.</span><span class="sxs-lookup"><span data-stu-id="514e4-236">In most cases, the class will be the same for the NMFC and the LTL class.</span></span> <span data-ttu-id="514e4-237">ومع ذلك، في بعض الحالات، قد تتسبب شحنة LTL في وجود نفس المنتج في فئة مختلفة.</span><span class="sxs-lookup"><span data-stu-id="514e4-237">However, in some cases, an LTL shipment might cause the same product to be in a different class.</span></span> <span data-ttu-id="514e4-238">بعد إنشاء رمز NMFC، يمكنك ربطه بالمنتجات.</span><span class="sxs-lookup"><span data-stu-id="514e4-238">After you create the NMFC code, you can link them to the products.</span></span>

### <a name="create-an-nmfc-code"></a><span data-ttu-id="514e4-239">إنشاء رمز تصنيف وطني للشحن بالمحركات (NMFC)</span><span class="sxs-lookup"><span data-stu-id="514e4-239">Create an NMFC code</span></span>

<span data-ttu-id="514e4-240">لإنشاء رمز التصنيف الوطني للشحن بالمحركات (NMFC)، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-240">To create an NMFC code, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-241">افتح **إدارة النقل > إعداد > معايير النقل > رموز التصنيف الوطني للشحن بالمحركات (NMFC)**.</span><span class="sxs-lookup"><span data-stu-id="514e4-241">Open **Transportation management > Setup > Transportation standards > NMFC Codes**.</span></span>
2.  <span data-ttu-id="514e4-242">حدد **جديد** لإنشاء ‏‫رمز تصنيف وطني للشحن بالمحركات (NMFC) جديد.</span><span class="sxs-lookup"><span data-stu-id="514e4-242">Select **New** to create a new NMFC code.</span></span>
3.  <span data-ttu-id="514e4-243">أدخل معرفاً واسماً وصفياً فريدين ‏لرمز التصنيف الوطني للشحن بالمحركات (NMFC).</span><span class="sxs-lookup"><span data-stu-id="514e4-243">Enter a unique ID and descriptive name for the NMFC code.</span></span>
4.  <span data-ttu-id="514e4-244">اختياري: ادخل فئة أقل من حمولة شاحنة (LTL) الذي يقابلها رمز التصنيف الوطني للشحن بالمحركات (NMFC).</span><span class="sxs-lookup"><span data-stu-id="514e4-244">Optional: Enter the LTL class that the NMFC corresponds to.</span></span>
5.  <span data-ttu-id="514e4-245">اختياري: أدخل نوع بوليصة الشحن لرمز التصنيف الوطني للشحن بالمحركات (NMFC).</span><span class="sxs-lookup"><span data-stu-id="514e4-245">Optional: Enter the bill of lading type for the NMFC code.</span></span>
6.  <span data-ttu-id="514e4-246">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-246">Close the page.</span></span>

<span data-ttu-id="514e4-247">الرمز المنسق هو نظام موحد دولًيا مكون من أسماء وأرقام لتصنيف المنتجات المتداولة التي تم تطويرها من قبل منظمة الجمارك العالمية، وهو يرافق ‏‫رمز سلعة النقل القياسي (STCC).</span><span class="sxs-lookup"><span data-stu-id="514e4-247">The Harmonized code is an internationally standardized system of names and numbers for classifying traded products that were developed by the World Customs Organization, and it accompanies the STCC code.</span></span>

### <a name="set-up-a-harmonized-tariff-schedule-code"></a><span data-ttu-id="514e4-248">إعداد رمز جدول تعريفة منسق</span><span class="sxs-lookup"><span data-stu-id="514e4-248">Set up a Harmonized tariff schedule code</span></span>

<span data-ttu-id="514e4-249">لإعداد رمز جدول تعريفة منسق، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-249">To set up a Harmonized tariff schedule code, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-250">افتح **إدارة النقل > إعداد > معايير النقل > جداول التعريفة المنسقة**.</span><span class="sxs-lookup"><span data-stu-id="514e4-250">Open **Transportation Management > Setup > Transportation Standards > Harmonized Tariff Schedules**.</span></span>
2.  <span data-ttu-id="514e4-251">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-251">Select **New**.</span></span>
3.  <span data-ttu-id="514e4-252">أدخل قيمه في حقل **جدول التعريفة المنسق**.</span><span class="sxs-lookup"><span data-stu-id="514e4-252">Enter a value in the **Harmonized tariff schedule** field.</span></span>
4.  <span data-ttu-id="514e4-253">أدخل اسماً في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="514e4-253">Enter a name in the **Name** field.</span></span>
5.  <span data-ttu-id="514e4-254">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-254">Close the page.</span></span>

### <a name="link-an-nmfc-stcc-and-harmonized-code-to-a-product"></a><span data-ttu-id="514e4-255">ربط رمز التصنيف الوطني للشحن بالمحركات (NMFC) ورمز سلعة النقل القياسي (STCC) والرمز المنسق بمنتج</span><span class="sxs-lookup"><span data-stu-id="514e4-255">Link an NMFC, STCC, and Harmonized code to a product</span></span>

<span data-ttu-id="514e4-256">لربط رمز التصنيف الوطني للشحن بالمحركات (NMFC) ورمز سلعة النقل القياسي (STCC) والرمز المنسق بمنتج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-256">To link an NMFC, STCC, and Harmonized code to a product, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-257">افتح **إدارة معلومات المنتج > المنتجات > المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="514e4-257">Open **Product information management > Products > Products**.</span></span>
2.  <span data-ttu-id="514e4-258">حدد منتجاً من القائمة.</span><span class="sxs-lookup"><span data-stu-id="514e4-258">Select a product from the list.</span></span>
3.  <span data-ttu-id="514e4-259">حدد **تحرير** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="514e4-259">Select **Edit** in the Action Pane.</span></span>
4.  <span data-ttu-id="514e4-260">افتح علامة التبويب السريعة **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="514e4-260">Open the **Warehouse** FastTab.</span></span>
5.  <span data-ttu-id="514e4-261">أدخل رمزاً في حقل ‏‫**رمز التصنيف الوطني للشحن بالمحركات (NMFC)**.</span><span class="sxs-lookup"><span data-stu-id="514e4-261">Enter a code in the **NMFC code** field.</span></span>
6.  <span data-ttu-id="514e4-262">أدخل رمزاً في حقل ‏‫**‏‫رمز سلعة النقل القياسي (STCC)**.</span><span class="sxs-lookup"><span data-stu-id="514e4-262">Enter a code in the **STCC code** field.</span></span>
7.  <span data-ttu-id="514e4-263">أدخل رمزاً في حقل ‏‫**النظام المنسق**.</span><span class="sxs-lookup"><span data-stu-id="514e4-263">Enter a code in the **Harmonized system** field.</span></span>
8.  <span data-ttu-id="514e4-264">قم بإغلاق الصفحات.</span><span class="sxs-lookup"><span data-stu-id="514e4-264">Close the pages.</span></span>

## <a name="shipping-carrier"></a><span data-ttu-id="514e4-265">شركة الشحن</span><span class="sxs-lookup"><span data-stu-id="514e4-265">Shipping carrier</span></span> 

<span data-ttu-id="514e4-266">شركة الشحن هي إحدى الإعدادات الأساسية المطلوبة لإدارة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-266">The shipping carrier is one of the required basic setups for transportation management.</span></span> <span data-ttu-id="514e4-267">شركة النقل هي إدخال أساسي للأوامر والأحمال التي يتم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="514e4-267">The carrier is a key input for the orders and loads that are created.</span></span>

<span data-ttu-id="514e4-268">استخدم صفحة **شركه الشحن** لإعداد خدمة نقل ووضع الشحن وطريقة نقل الشحن وملف تعريف التصنيف لشركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-268">Use the **Shipping carrier** page to set up a carrier service, mode of shipment, transportation tender, and rating profile for the shipping carrier.</span></span>

### <a name="create-a-shipping-carrier"></a><span data-ttu-id="514e4-269">إنشاء شركه شحن</span><span class="sxs-lookup"><span data-stu-id="514e4-269">Create a shipping carrier</span></span>

<span data-ttu-id="514e4-270">لإنشاء إنشاء شركه شحن، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-270">To create a shipping carrier, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-271">افتح **إدارة النقل > إعداد > شركات النقل > شركات الشحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-271">Open **Transportation management > Setup > Carriers > Shipping carriers**.</span></span>
2.  <span data-ttu-id="514e4-272">حدد **جديد** لإنشاء شركة شحن جديدة.</span><span class="sxs-lookup"><span data-stu-id="514e4-272">Select **New** to create a new shipping carrier.</span></span>
3.  <span data-ttu-id="514e4-273">في حقل **شركة الشحن**، أدخل نوع شركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-273">In the **Shipping Carrier** field, enter the type of the shipping carrier.</span></span>
4.  <span data-ttu-id="514e4-274">في حقل **الاسم**، أدخِل اسماً لشركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-274">In the **Name** field, enter a name for the shipping carrier.</span></span>
5.  <span data-ttu-id="514e4-275">في حقل **الوضع**، حدد نوع وضع الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-275">In the **Mode** field, select the shipment mode type.</span></span>
6.  <span data-ttu-id="514e4-276">في علامة التبويب السريعة **النظرة العامة**، حدد تفاصيل شركة الشحن باستخدام الحقول التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-276">On the **Overview** FastTab, specify the shipping carrier details by using the following fields:</span></span>  
    - <span data-ttu-id="514e4-277">**تنشيط شركة الشحن** - قم بتعيين شريط التمرير هذا إلى **نعم** لاستخدام شركة الشحن المحددة للشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-277">**Activate shipping carrier** - Set this slider bar to **Yes** to use the specified shipping carrier for the shipment.</span></span>
    - <span data-ttu-id="514e4-278">**المورد** - حدد حساب المورد الذي تريد تعيين شركة الشحن إليه.</span><span class="sxs-lookup"><span data-stu-id="514e4-278">**Vendor** - Select the vendor account to which you want to assign the shipping carrier.</span></span>
    - <span data-ttu-id="514e4-279">**SCAC** - أدخل معرفاً لكود ألفا القياسي لشركات النقل (SCAC).</span><span class="sxs-lookup"><span data-stu-id="514e4-279">**SCAC** - Enter an ID for the Standard Carrier Alpha Code (SCAC).</span></span>
    - <span data-ttu-id="514e4-280">**تنشيط تصنيف شركة النقل** - قم بتعيين مربع التمرير هذا إلى **نعم** لتمكين التصنيف التلقائي لشركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-280">**Activate carrier rating** - Set this slider to **Yes** to enable automatic rating for the shipping carrier.</span></span>
7.  <span data-ttu-id="514e4-281">اختياري: في حقل **نوع طريقة الدفع للنقل**، حدد أحدي الطرق التالية لتحديث تفاصيل طريقه الدفع للنقل:</span><span class="sxs-lookup"><span data-stu-id="514e4-281">Optional: In the **Transportation tender type** field, select one of the following methods for updating the details of transportation tender:</span></span>
    - <span data-ttu-id="514e4-282">**يدوي** - تحديث تفاصيل طريقه الدفع للنقل يدوياً باستخدام صفحة **طرق الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-282">**Manual** - Manually update the transportation tender details by using the **Transportation tenders** page.</span></span>
    - <span data-ttu-id="514e4-283">**EDI** - تحديث تفاصيل طريقة الدفع للنقل تلقائياً باستخدام تبادل البيانات الإلكتروني (EDI) في صفحة **طريقة الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-283">**EDI** - Automatically update the transportation tender details by using an Electronic Data Interchange (EDI) on the **Transportation tenders** page.</span></span>
8.  <span data-ttu-id="514e4-284">اختياري: في حقل **تسلسل الرقم المبدئي**، يمكنك تحديد تسلسل رقمي مرتبط بمحرك عام، إن وجد.</span><span class="sxs-lookup"><span data-stu-id="514e4-284">Optional: In the **Pro number sequence** field, you can select a number sequence that is associated with a generic engine, if any are available.</span></span>
9.  <span data-ttu-id="514e4-285">في علامة التبويب السريعة **العناوين**، حدد **جديد**، ثم ادخل عنوان شركه الشحن وغرضها.</span><span class="sxs-lookup"><span data-stu-id="514e4-285">On the **Addresses** FastTab, select **New**, and then enter the address and purpose of the shipping carrier.</span></span>
10. <span data-ttu-id="514e4-286">حدد **موافق** لحفظ العناوين.</span><span class="sxs-lookup"><span data-stu-id="514e4-286">Select **OK** to save the address.</span></span>
11. <span data-ttu-id="514e4-287">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-287">Close the page.</span></span>

## <a name="transportation-mode"></a><span data-ttu-id="514e4-288">وضع النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-288">Transportation mode</span></span>

<span data-ttu-id="514e4-289">يمثل وضع النقل نوع النقل الذي تستخدمه شركة النقل للتسليم الشحنات، مثل أقل من حمولة الشاحنة (LTL) أو حمولة الشاحنة (TL) أو الطرود.</span><span class="sxs-lookup"><span data-stu-id="514e4-289">The transportation mode represents the type of transport that the carrier uses for freight deliveries, such as Less than load (LTL), Truckload (TL), or Parcel.</span></span> <span data-ttu-id="514e4-290">إن طريقة النقل تمثل شكل النقل الذي تستخدمه شركة النقل لتسليم الشحنات، مثل الجو أو الأرض أو المحيط أو السكك الحديدية.</span><span class="sxs-lookup"><span data-stu-id="514e4-290">The transportation method represents the form of transport that the carrier uses for freight deliveries, such as air, ground, ocean, or rail.</span></span>

### <a name="create-a-transportation-mode"></a><span data-ttu-id="514e4-291">إنشاء وضع نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-291">Create a transportation mode</span></span>

<span data-ttu-id="514e4-292">لإنشاء وضع نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-292">To create a transportation mode, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-293">افتح **إدارة النقل > إعداد > شركات النقل > الوضع**.</span><span class="sxs-lookup"><span data-stu-id="514e4-293">Open **Transportation management > Setup > Carriers > Mode**.</span></span>
2.  <span data-ttu-id="514e4-294">حدد **جديد** لإنشاء ‏‫وضع جديد.</span><span class="sxs-lookup"><span data-stu-id="514e4-294">Select **New** to create a new mode.</span></span>
3.  <span data-ttu-id="514e4-295">أدخل معرفاً واسماً وصفياً فريدين للوضع.</span><span class="sxs-lookup"><span data-stu-id="514e4-295">Enter a unique ID and a descriptive name for the mode.</span></span>
4.  <span data-ttu-id="514e4-296">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-296">Close the page.</span></span>

### <a name="associate-a-shipping-carrier-with-a-transportation-mode"></a><span data-ttu-id="514e4-297">إقران شركة شحن بوضع نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-297">Associate a shipping carrier with a transportation mode</span></span>

<span data-ttu-id="514e4-298">لإقران شركة شحن بوضع نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-298">To associate a shipping carrier with a transportation mode, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-299">افتح **إدارة النقل > إعداد > شركات النقل > شركات الشحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-299">Open **Transportation management > Setup > Carriers > Shipping carriers**.</span></span>
2.  <span data-ttu-id="514e4-300">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="514e4-300">Select **Edit**.</span></span>
3.  <span data-ttu-id="514e4-301">حدد شركة شحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-301">Select a shipping carrier.</span></span>
4.  <span data-ttu-id="514e4-302">في الحقل **الوضع**، حدد وضع نقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-302">In the **Mode** field, select a transportation mode.</span></span>
5.  <span data-ttu-id="514e4-303">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-303">Close the page.</span></span>

### <a name="create-a-transportation-method"></a><span data-ttu-id="514e4-304">إنشاء طريقة نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-304">Create a transportation method</span></span>

<span data-ttu-id="514e4-305">لإنشاء طريقة نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-305">To create a transportation method, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-306">افتح **إدارة النقل > إعداد > معايير النقل > طرق النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-306">Open **Transportation management > Setup > Carriers > Transportation methods**.</span></span>
2.  <span data-ttu-id="514e4-307">حدد **جديد** لإنشاء طريقة نقل جديدة.</span><span class="sxs-lookup"><span data-stu-id="514e4-307">Select **New** to create a new transportation method.</span></span>
3.  <span data-ttu-id="514e4-308">أدخل معرفاً واسماً وصفياً فريدين لطريقة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-308">Enter a unique ID and descriptive name for the transportation  method.</span></span>
4.  <span data-ttu-id="514e4-309">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-309">Close the page.</span></span>

## <a name="carrier-services"></a><span data-ttu-id="514e4-310">خدمات شركة النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-310">Carrier services</span></span> 

<span data-ttu-id="514e4-311">يجب تكوين خدمة شركة نقل واحدة أو أكثر لشركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-311">One or more carrier services must be configured for a carrier.</span></span> <span data-ttu-id="514e4-312">تحدد خدمة شركة النقل الخدمات التي تقدمها شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-312">The carrier service defines the services that are offered by the carrier.</span></span> <span data-ttu-id="514e4-313">ومن الأمثلة على خدمات شركات النقل، الهواء في اليوم التالي أو الهواء في اليوم الثاني أو الأرض.‬</span><span class="sxs-lookup"><span data-stu-id="514e4-313">Examples of carrier services would be next day air, second day air, and ground.</span></span>

### <a name="create-a-carrier-service"></a><span data-ttu-id="514e4-314">إنشاء خدمة شركة نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-314">Create a carrier service</span></span>

<span data-ttu-id="514e4-315">لإنشاء خدمة شركة نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-315">To create a carrier service, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-316">افتح **إدارة النقل > إعداد > شركات النقل > شركات الشحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-316">Open **Transportation management > Setup > Carriers > Shipping carriers**.</span></span>
2.  <span data-ttu-id="514e4-317">حدد **أقل من حمولة شاحنة (LTL)** في الجزء الأيسر.</span><span class="sxs-lookup"><span data-stu-id="514e4-317">Select **LTL** on the left-hand pane.</span></span>
3.  <span data-ttu-id="514e4-318">قم بتوسيع علامة التبويب السريعة **الخدمات**.</span><span class="sxs-lookup"><span data-stu-id="514e4-318">Expand the **Services** FastTab.</span></span>
4.  <span data-ttu-id="514e4-319">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-319">Select **New**.</span></span>
5.  <span data-ttu-id="514e4-320">أدخِل معرفاً فريداً في حقل **خدمة شركة النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-320">Enter a unique ID in the **Carrier service** field.</span></span>
6.  <span data-ttu-id="514e4-321">أدخل **اسماً** لخدمة شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-321">Enter a **Name** for the carrier service.</span></span>
7.  <span data-ttu-id="514e4-322">اختياري: حدد **معرف قالب حمل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-322">Optional: Select a **Load template ID**.</span></span>
8.  <span data-ttu-id="514e4-323">حدد **طريقة نقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-323">Select a **Transportation method**.</span></span>
9.  <span data-ttu-id="514e4-324">أدخل **وضع تسليم**.</span><span class="sxs-lookup"><span data-stu-id="514e4-324">Enter a **Mode of delivery**.</span></span>
10. <span data-ttu-id="514e4-325">اختياري: أدخل **رمزاً خارجياً**.</span><span class="sxs-lookup"><span data-stu-id="514e4-325">Optional: Enter an **External code**.</span></span>
11. <span data-ttu-id="514e4-326">حدد **معرف مجموعة فوترة**.</span><span class="sxs-lookup"><span data-stu-id="514e4-326">Select a **Billing group ID**.</span></span>
12. <span data-ttu-id="514e4-327">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-327">Close the page.</span></span>

## <a name="carrier-groups"></a><span data-ttu-id="514e4-328">مجموعات شركات النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-328">Carrier groups</span></span> 

<span data-ttu-id="514e4-329">يتم استخدام مجموعات شركات النقل لتجميع شركات الشحن بخدمات الشحن المقابلة لها.</span><span class="sxs-lookup"><span data-stu-id="514e4-329">Carrier groups are used to group shipping carriers with their corresponding shipping services.</span></span>

### <a name="create-a-carrier-group"></a><span data-ttu-id="514e4-330">إنشاء مجموعة شركات نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-330">Create a carrier group</span></span>

<span data-ttu-id="514e4-331">لإنشاء مجموعة شركات نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-331">To create a carrier group, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-332">افتح **إدارة النقل > إعداد > شركات النقل > مجموعة شركات النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-332">Open **Transportation management > Setup > Carriers > Carrier group**.</span></span>
2.  <span data-ttu-id="514e4-333">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-333">Select **New**.</span></span>
3.  <span data-ttu-id="514e4-334">أدخل **معرف مجموعة شركات النقل** واسماً لها.</span><span class="sxs-lookup"><span data-stu-id="514e4-334">Enter a **Carrier group ID** and a name.</span></span>
4.  <span data-ttu-id="514e4-335">في علامة التبويب السريعة **التفاصيل**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-335">On the **Details** FastTab, select **New**.</span></span>
5.  <span data-ttu-id="514e4-336">حدد **شركة شحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-336">Select a **Shipping carrier**.</span></span>
6.  <span data-ttu-id="514e4-337">حدد **خدة شركة نقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-337">Select a **Carrier service**.</span></span>
7.  <span data-ttu-id="514e4-338">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-338">Close the page.</span></span>

## <a name="transportation-status"></a><span data-ttu-id="514e4-339">حالة النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-339">Transportation status</span></span> 

<span data-ttu-id="514e4-340">يمكنك إعداد الرموز الرئيسية لحالات النقل لتفسير الرموز التي توفرها شركات الشحن الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="514e4-340">You can set up master codes for transportation statuses to interpret codes that are provided by your shipping carriers.</span></span> <span data-ttu-id="514e4-341">يتم استخدام هذه الطريقة لتكامل تبادل البيانات الإلكتروني (EDI) مع شركات الشحن لتوفير حالة.</span><span class="sxs-lookup"><span data-stu-id="514e4-341">This method is used for EDI integration with shipping carriers to provide a status.</span></span> <span data-ttu-id="514e4-342">يمكن أن تساعدك حالة النقل التي توفرها لرمز حالة السجل الرئيسي للنقل في تتبع حالة حمل أو شحنة أو حاوية.</span><span class="sxs-lookup"><span data-stu-id="514e4-342">The transportation status that you provide for a transportation master status code can help you track the status of a load, shipment, or container.</span></span>

### <a name="create-a-transportation-status"></a><span data-ttu-id="514e4-343">إنشاء حالة نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-343">Create a transportation status</span></span>
<span data-ttu-id="514e4-344">لإنشاء حالة نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-344">To create a transportation status, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-345">افتح **إدارة النقل > إعداد > معايير النقل > السجلات الرئيسية لحالة النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-345">Open **Transportation management > Setup > Transportation status masters**.</span></span>
2.  <span data-ttu-id="514e4-346">حدد **جديد** لإنشاء سجل رئيسي جديد لحالة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-346">Select **New** to create a transportation status master.</span></span>
3.  <span data-ttu-id="514e4-347">في حقل **السجل الرئيسي لحالة النقل**، أدخل رمزاً فريداً لحالة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-347">In the **Transportation status master** field, enter a unique code for the transportation status.</span></span>
4.  <span data-ttu-id="514e4-348">في حقل **نوع النقل**، حدد إما **شركة الشحن** أو **المركز** كنوع النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-348">In the **Transportation type** field, select either **Shipping carrier** or **Hub** as the type of transportation.</span></span>
5.  <span data-ttu-id="514e4-349">أدخل اسماً وحالة نقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-349">Enter a name and transportation status.</span></span>
6.  <span data-ttu-id="514e4-350">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-350">Close the page.</span></span>

### <a name="map-a-transportation-status-to-a-carrier-status"></a><span data-ttu-id="514e4-351">تعيين حالة النقل إلى حالة شركة النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-351">Map a transportation status to a carrier status</span></span>

<span data-ttu-id="514e4-352">لتعيين حالة النقل إلى حالة شركة النقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-352">To map a transportation status to a carrier status, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-353">افتح **إدارة النقل > إعداد > معايير النقل > حالة نقل شركة النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-353">Open **Transportation management > Setup > Carriers > Carrier transportation status**.</span></span>
2.  <span data-ttu-id="514e4-354">حدد **جديد** لتعيين رمز من شركة شحن إلى رمز سجل رئيسي لحالة نقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-354">Select **New** to map a code from a shipping carrier to a transportation status master code.</span></span>
3.  <span data-ttu-id="514e4-355">حدد المعرف الفريد لشركة الشحن وخدمة شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-355">Select the unique ID for the shipping carrier and the carrier service.</span></span>
4.  <span data-ttu-id="514e4-356">حدد رمز حالة النقل الذي تريد تعيينه إلى رمز شركة الشحن المحدد.</span><span class="sxs-lookup"><span data-stu-id="514e4-356">Select the transportation status code that you want to map to the selected shipping carrier's code.</span></span>
5.  <span data-ttu-id="514e4-357">أدخل الرمز الخارجي الذي تستخدمه شركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-357">Enter the external code that is used by the shipping carrier.</span></span>
6.  <span data-ttu-id="514e4-358">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-358">Close the page.</span></span>

## <a name="number-sequence"></a><span data-ttu-id="514e4-359">التسلسل الرقمي</span><span class="sxs-lookup"><span data-stu-id="514e4-359">Number sequence</span></span> 

<span data-ttu-id="514e4-360">تتيح لك صفحة **التسلسلات الرقمية** الموجودة في الوحدة النمطية لإدارة النقل إعداد أرقام أولية متنوعة لكي تستخدمها شركات نقل أقل من حمولة الشاحنة (LTL) أو حمولة الشاحنة (TL).</span><span class="sxs-lookup"><span data-stu-id="514e4-360">The **Number sequences** page in the Transportation management module lets you set up various pro-numbers to be used by the LTL and TL carriers.</span></span>

### <a name="create-a-number-sequence-for-a-pro-number"></a><span data-ttu-id="514e4-361">إنشاء تسلسل رقمي للرقم المبدئي</span><span class="sxs-lookup"><span data-stu-id="514e4-361">Create a number sequence for a pro number</span></span>

<span data-ttu-id="514e4-362">لإنشاء تسلسل رقمي للرقم المبدئي، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-362">To create a number sequence for a pro number, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-363">افتح **إدارة النقل > إعداد > شركات النقل > التسلسلات الرقمية**.</span><span class="sxs-lookup"><span data-stu-id="514e4-363">Open **Transportation management > Setup > Carriers > Number sequences**.</span></span>
2.  <span data-ttu-id="514e4-364">حدد **جديد** لإنشاء تسلسل رقمي جديد.</span><span class="sxs-lookup"><span data-stu-id="514e4-364">Select **New** to create a new number sequence.</span></span>
3.  <span data-ttu-id="514e4-365">أدخل معرفاً واسماً وصفياً فريدين للتسلسل الرقمي.</span><span class="sxs-lookup"><span data-stu-id="514e4-365">Enter a unique ID and descriptive name for the number sequence.</span></span>
4.  <span data-ttu-id="514e4-366">في حقل **نوع التسلسل الرقمي**، يُعد **الرقم المبدئي** هو الخيار الوحيد.</span><span class="sxs-lookup"><span data-stu-id="514e4-366">In the **Number sequence type** field, **Pro number** is the only option.</span></span>
5.  <span data-ttu-id="514e4-367">في حقل **التحقق من الرقم**، يُعد **التحقق من الرقم** هو الخيار الوحيد الذي تم إعداده كمحرك عام.</span><span class="sxs-lookup"><span data-stu-id="514e4-367">In the **Check digit** field, **Check digit** is the only option and is set up as a generic engine.</span></span>
6.  <span data-ttu-id="514e4-368">في علامة التبويب السريعة **التسلسل**، قم بتقديم معلومات حول التسلسل.</span><span class="sxs-lookup"><span data-stu-id="514e4-368">On the **Sequence** FastTab, provide information on the sequence.</span></span>
7.  <span data-ttu-id="514e4-369">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-369">Close the page.</span></span>

### <a name="link-a-number-sequence-to-a-carrier"></a><span data-ttu-id="514e4-370">ربط تسلسل رقمي بشركة نقل</span><span class="sxs-lookup"><span data-stu-id="514e4-370">Link a number sequence to a carrier</span></span>

<span data-ttu-id="514e4-371">لربط تسلسل رقمي بشركة نقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-371">To link a number sequence to a carrier, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-372">افتح **إدارة النقل > إعداد > شركات النقل > شركات الشحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-372">Open **Transportation management > Setup > Carriers > Shipping carriers**.</span></span>
2.  <span data-ttu-id="514e4-373">حدد شركة شحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-373">Select a shipping carrier.</span></span>
3.  <span data-ttu-id="514e4-374">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="514e4-374">Select **Edit**.</span></span>
4.  <span data-ttu-id="514e4-375">في علامة التبويب السريعة **النظرة العامة**، حدد خياراً في حقل **التسلسل الرقمي المبدئي**.</span><span class="sxs-lookup"><span data-stu-id="514e4-375">On the **Overview** FastTab, select an option in the **Pro number sequence** field.</span></span>
5.  <span data-ttu-id="514e4-376">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-376">Close the page.</span></span>

## <a name="load-templates"></a><span data-ttu-id="514e4-377">قوالب حمل العمل</span><span class="sxs-lookup"><span data-stu-id="514e4-377">Load templates</span></span> 

<span data-ttu-id="514e4-378">يتم استخدام قوالب حمل العمل في منضدة عمل تخطيط الحمل للسماح بالإعدادات الافتراضية لقيود الوزن و/أو قيود المعدات للحمل.</span><span class="sxs-lookup"><span data-stu-id="514e4-378">Load templates are used in the load planning workbench to allow for the defaults for weight restrictions and/or equipment restrictions for the load.</span></span> <span data-ttu-id="514e4-379">على سبيل المثال، إذا كان الحمل عبارة عن بضائع مجمدة، فسيتم إعداد قالب حمل يحدد شاحنة مبردة والوزن الذي تقتصر عليه المعدات المحددة.</span><span class="sxs-lookup"><span data-stu-id="514e4-379">For example, if the load is frozen goods, then a load template would be set up that identifies a refrigerated truck and the weight that the selected equipment is restricted to.</span></span>

### <a name="create-a-load-template"></a><span data-ttu-id="514e4-380">إنشاء قالب حمل</span><span class="sxs-lookup"><span data-stu-id="514e4-380">Create a load template</span></span>

<span data-ttu-id="514e4-381">لإنشاء قالب حمل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-381">To create a load template, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-382">افتح **إدارة النقل > إعداد > إنشاء حِمل > قوالب الأحمال**.</span><span class="sxs-lookup"><span data-stu-id="514e4-382">Open **Transportation management > Setup > Load building > Load templates**.</span></span>
2.  <span data-ttu-id="514e4-383">حدد **جديد** لإنشاء قالب حمل جديد.</span><span class="sxs-lookup"><span data-stu-id="514e4-383">Select **New** to create a new load template.</span></span>
3.  <span data-ttu-id="514e4-384">أدخل معرفاً واسماً وصفياً فريدين لقالب الحمل.</span><span class="sxs-lookup"><span data-stu-id="514e4-384">Enter a unique ID and descriptive name for the load template.</span></span>
4.  <span data-ttu-id="514e4-385">أدخل **ارتفاع الحمل** و **عرض الحمل** و **عمق الحمل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-385">Enter the **Load height**, **Load width**, and **Load depth**.</span></span>
5.  <span data-ttu-id="514e4-386">أدخل **الحد الأقصى لحجم الحمل المسموح به**.</span><span class="sxs-lookup"><span data-stu-id="514e4-386">Enter the **Max. allowed load volume**.</span></span>
6.  <span data-ttu-id="514e4-387">أدخل **الحد الأقصى لوزن الحمل المسموح به**.</span><span class="sxs-lookup"><span data-stu-id="514e4-387">Enter the **Max. allowed load weight**.</span></span>
7.  <span data-ttu-id="514e4-388">أدخل **الحد الأقصى للوزن الإجمالي للحمل المسموح به**.</span><span class="sxs-lookup"><span data-stu-id="514e4-388">Enter the **Maximum allowed load gross weight**.</span></span>
8.  <span data-ttu-id="514e4-389">أدخل **الحد الأقصى لعدد قطع الشحن المسموح بها**.</span><span class="sxs-lookup"><span data-stu-id="514e4-389">Enter the **Maximum number of freight pieces allowed**.</span></span> <span data-ttu-id="514e4-390">ويمكن أن يرتبط هذا الاختيار بعدد منصات النقل والصناديق الملفوفة وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="514e4-390">This selection can relate to the number of pallets, loosed boxes, and so on.</span></span>
9.  <span data-ttu-id="514e4-391">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-391">Close the page.</span></span>

## <a name="transportation-tender"></a><span data-ttu-id="514e4-392">طريقة الدفع للنقل</span><span class="sxs-lookup"><span data-stu-id="514e4-392">Transportation tender</span></span> 

<span data-ttu-id="514e4-393">طريقه الدفع للنقل هي مستند شحن يحتوي على تعيين لحمل أو مسار أو جزء من مسار.</span><span class="sxs-lookup"><span data-stu-id="514e4-393">A transportation tender is a shipping document that has an assignment for a load, a route, or part of a route.</span></span> <span data-ttu-id="514e4-394">يمكنك استخدام طريقة الدفع للنقل هذه لتعقب التواريخ والأسعار المعتمدة بين العميل وشركة الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-394">You can use this transportation tender to keep track of the dates and rates that are approved between the customer and a shipping carrier.</span></span>

<span data-ttu-id="514e4-395">يمكنك إنشاء طريقة دفع للنقل من مسار أو مقطع مسار أو من حمل في مقطع مسار.</span><span class="sxs-lookup"><span data-stu-id="514e4-395">You can create a transportation tender from a route, a route segment, or from a load on a route segment.</span></span> <span data-ttu-id="514e4-396">يمكنك أيضاً إنشاء هذه المستندات وتحديثها في صفحة **طريقة الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-396">You can also create and update these documents on the **Transportation tenders** page.</span></span>

<span data-ttu-id="514e4-397">بعد الانتهاء من إنشاء طريقة الدفع للنقل، يمكنك إرسالها، مما ستنتج عنه تحديث حالة سير العمل من **معلق** إلى **تم الإرسال**.</span><span class="sxs-lookup"><span data-stu-id="514e4-397">After you have finished creating the transportation tender, you can submit it, which will update the workflow status from **Pending** to **Submitted**.</span></span> <span data-ttu-id="514e4-398">عند استلام تأكيد من شركة النقل، يمكنك تأكيده وإدخال التفاصيل المؤكدة مثل السعر وتاريخ الالتقاط.</span><span class="sxs-lookup"><span data-stu-id="514e4-398">When you have received confirmation from the carrier, you can confirm it and enter confirmed details such as the rate and pickup date.</span></span>

<span data-ttu-id="514e4-399">يمكنك أيضاً إنشاء هذه المستندات وتحديثها في صفحة **طريقة الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-399">You can also create and update these documents on the **Transportation tenders** page.</span></span>

<span data-ttu-id="514e4-400">**لإنشاء طريقة دفع للنقل، اتبع الخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="514e4-400">**To create a transportation tender, follow these steps:**</span></span>

1.  <span data-ttu-id="514e4-401">افتح **إدارة النقل > التخطيط > إرساء جدولة المواعيد > طرق الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-401">Open **Transportation management > Planning > Dock appointment scheduling > Transportation tenders**.</span></span>
2.  <span data-ttu-id="514e4-402">في حقل **تصفية حسب**، حدد أحد الخيارات التالية للإشارة إلى نوع التعيين المطلوب.</span><span class="sxs-lookup"><span data-stu-id="514e4-402">In the **Filter by** field, select one of the following options to indicate the type of assignment that is requested.</span></span>
    - <span data-ttu-id="514e4-403">**الحمل** - يشير إلى التقاط حمل محدد.</span><span class="sxs-lookup"><span data-stu-id="514e4-403">**Load** - Refers to a pickup of a specific load.</span></span>
    - <span data-ttu-id="514e4-404">**المسار** - يشير إلى حمل سيتم نقله باستخدام مسار.</span><span class="sxs-lookup"><span data-stu-id="514e4-404">**Route** - Refers to a load that will be transported by using a route.</span></span>
    - <span data-ttu-id="514e4-405">**مقطع المسار** - يشير إلى حمل سيتم نقله باستخدام جزء من مسار.</span><span class="sxs-lookup"><span data-stu-id="514e4-405">**Route segment** - Refers to a load that will be transported by using part of a route.</span></span>
    - <span data-ttu-id="514e4-406">**مقطع المسار للحمل** - يشير إلى حمل محدد سيتم نقله باستخدام جزء من مسار.</span><span class="sxs-lookup"><span data-stu-id="514e4-406">**Route segment for a load** - Refers to a specific load that will be transported by using part of a route.</span></span>
3.  <span data-ttu-id="514e4-407">حدد **جديد** لإنشاء طريقة دفع للنقل جديدة.</span><span class="sxs-lookup"><span data-stu-id="514e4-407">Select **New** to create a new transportation tender.</span></span> <span data-ttu-id="514e4-408">يعرض مستند طريقة الدفع تلقائياً معرفاً في حقل **طريقة الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-408">The tender document automatically displays an ID in the **Transportation tender** field.</span></span>
4.  <span data-ttu-id="514e4-409">في علامة التبويب السريعة **المراجع**، في حقل **معرف المرجع**، حدد معرفاً فريداً للحمل.</span><span class="sxs-lookup"><span data-stu-id="514e4-409">On the **References** FastTab, in the **Reference ID** field, select a unique ID for the load.</span></span> <span data-ttu-id="514e4-410">تتم تصفية الأحمال وفقاً لتحديدك في حقل **تصفية حسب**.</span><span class="sxs-lookup"><span data-stu-id="514e4-410">The loads are filtered according to your selection in the **Filter by** field.</span></span>
5.  <span data-ttu-id="514e4-411">في علامة التبويب السريعة **عام**، وفي حقل **شركة الشحن**، حدد شركة الشحن التي يجب أن تقوم بالتقاط الحمل.</span><span class="sxs-lookup"><span data-stu-id="514e4-411">On the **General** FastTab, in the **Shipping carrier** field, select the shipping carrier that should pick up the load.</span></span>
6.  <span data-ttu-id="514e4-412">في حقل **خدمة شركة النقل**، حدد خدمة تقدمها شركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-412">In the **Carrier service** field, select a service that is offered by the carrier.</span></span>
7.  <span data-ttu-id="514e4-413">أدخل المعلومات المتبقية في مجموعة حقول **الشحن**.</span><span class="sxs-lookup"><span data-stu-id="514e4-413">Enter the remaining information in the **Shipping** field group.</span></span>
8.  <span data-ttu-id="514e4-414">في مجموعة حقول **الأسعار**، أدخل التاريخ وطلب السعر لشركة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-414">In the **Rates** field group, enter the date and rate request for the carrier.</span></span> <span data-ttu-id="514e4-415">حقل **تاريخ الالتقاط المطلوب ووقته** وحقل **الأسعار المطلوبة** مخصصان لطلب العميل.</span><span class="sxs-lookup"><span data-stu-id="514e4-415">The **Requested pickup date and time** and the **Requested rates** fields are for the customer request.</span></span> <span data-ttu-id="514e4-416">إذا أرادت شركة النقل تحديث المعلومات قبل التأكيد، فيجب إدخال هذه المعلومات في الحقلين **تاريخ الالتقاط المؤكد ووقته** و **الأسعار المؤكدة**.</span><span class="sxs-lookup"><span data-stu-id="514e4-416">If the carrier wants to update the information before confirmation, this information must be entered in the **Confirmed pickup date and time** and the **Confirmed rates** fields.</span></span> <span data-ttu-id="514e4-417">يمكنك عرض تبادل المعلومات بين العميل وشركة النقل في علامة التبويب السريعة **المحفوظات**.</span><span class="sxs-lookup"><span data-stu-id="514e4-417">You can view the exchange of information between the customer and the carrier on the **History** FastTab.</span></span>
9.  <span data-ttu-id="514e4-418">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-418">Close the page.</span></span>

<span data-ttu-id="514e4-419">شاهد الفيديو التالي للاطلاع على إنشاء طريقة دفع للنقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-419">Watch the following video to see the creation of a transportation tender.</span></span> 

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE47Zz5]

<span data-ttu-id="514e4-420">**لإرسال طريقه دفع للنقل وتأكيدها وقبولها، اتبع الخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="514e4-420">**To submit, confirm, and accept a transportation tender, follow these steps:**</span></span>

1.  <span data-ttu-id="514e4-421">افتح **إدارة النقل > التخطيط > إرساء جدولة المواعيد > طرق الدفع للنقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-421">Open **Transportation management > Planning > Dock appointment scheduling > Transportation tenders**.</span></span>
2.  <span data-ttu-id="514e4-422">حدد **حالة التحديث**.</span><span class="sxs-lookup"><span data-stu-id="514e4-422">Select **Update status**.</span></span>
3.  <span data-ttu-id="514e4-423">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="514e4-423">Select **Submit**.</span></span>
4.  <span data-ttu-id="514e4-424">حدد **تأكيد**.</span><span class="sxs-lookup"><span data-stu-id="514e4-424">Select **Confirm**.</span></span>
5.  <span data-ttu-id="514e4-425">أدخل **السعر والتاريخ**.</span><span class="sxs-lookup"><span data-stu-id="514e4-425">Enter the **Rate and Date**.</span></span>
6.  <span data-ttu-id="514e4-426">اضغط على **موافق**.</span><span class="sxs-lookup"><span data-stu-id="514e4-426">Press **OK**.</span></span>
7.  <span data-ttu-id="514e4-427">حدد **حالة التحديث**.</span><span class="sxs-lookup"><span data-stu-id="514e4-427">Select **Update status**.</span></span>
8.  <span data-ttu-id="514e4-428">حدد **قبول**.</span><span class="sxs-lookup"><span data-stu-id="514e4-428">Select **Accept**.</span></span>
9.  <span data-ttu-id="514e4-429">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="514e4-429">Close the page.</span></span>

## <a name="transportation-management-parameters"></a><span data-ttu-id="514e4-430">معلمات إدارة النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-430">Transportation management parameters</span></span> 

<span data-ttu-id="514e4-431">لمراجعه معلمات أدارة النقل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-431">To review the transportation management parameters, follow these steps:</span></span>

1.  <span data-ttu-id="514e4-432">افتح **إدارة النقل > إعداد > معلمات إدارة النقل**.</span><span class="sxs-lookup"><span data-stu-id="514e4-432">Open **Transportation management > Setup > Transportation management parameters**.</span></span>
2.  <span data-ttu-id="514e4-433">من علامة التبويب **عام**، راجع علامات التبويب السريعة التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-433">On the **General** tab, review the following FastTabs:</span></span>
    -  <span data-ttu-id="514e4-434">**جدولة المواعيد** - تعيين المدة الافتراضية لموعد مجدول للتسليم أو التقاط الشحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-434">**Appointment scheduling** - Set the default duration of an appointment that is scheduled for delivery or pickup of shipment.</span></span>
    - <span data-ttu-id="514e4-435">**‏‫تسجيل دخول السائق وتسجيل خروجه** - إدخال فاصل تنبيه لتسجيل دخول السائق أو تسجيل خروجه.</span><span class="sxs-lookup"><span data-stu-id="514e4-435">**Driver check-in and check-out** - Enter an alert interval for driver check-in or check-out.</span></span>
    - <span data-ttu-id="514e4-436">**فاتورة المورد** - تحديد خيارات لفواتير المورّدين.</span><span class="sxs-lookup"><span data-stu-id="514e4-436">**Vendor invoice** - Select options for vendor invoices.</span></span>
    - <span data-ttu-id="514e4-437">**نوع المركز** تحديد نوع مركز منافذ.</span><span class="sxs-lookup"><span data-stu-id="514e4-437">**Hub type** - Select a Port hub type.</span></span>
    - <span data-ttu-id="514e4-438">**الشحن** - يشير إلى ما إذا كانت الشحنات قد تم تخطيطها بواسطة الشحنات.</span><span class="sxs-lookup"><span data-stu-id="514e4-438">**Shipment** - Indicate whether shipments are planned by shipments.</span></span>
    - <span data-ttu-id="514e4-439">**تخطيط الشحن بالطريق** - الإشارة إلى ما إذا كان يتم استخدام تخطيط الشحن بالطريق أم لا.</span><span class="sxs-lookup"><span data-stu-id="514e4-439">**In transit planning** - Indicate whether in transit planning is used.</span></span>
    - <span data-ttu-id="514e4-440">**الأحمال** - تحديد ما إذا كنت تريد:</span><span class="sxs-lookup"><span data-stu-id="514e4-440">**Loads** - Determine whether to:</span></span>
        - <span data-ttu-id="514e4-441">إنشاء تلقائي لإدخال أمر مبيعات</span><span class="sxs-lookup"><span data-stu-id="514e4-441">Automatically create at sales order entry</span></span>
        - <span data-ttu-id="514e4-442">إنشاء تلقائي عند إدخال أمر الشراء</span><span class="sxs-lookup"><span data-stu-id="514e4-442">Automatically create at purchase order entry</span></span>
        - <span data-ttu-id="514e4-443">إنشاء تلقائي عند إدخال أمر النقل</span><span class="sxs-lookup"><span data-stu-id="514e4-443">Automatically create at transfer order entry</span></span>
        - <span data-ttu-id="514e4-444">تجاوز تاريخ تأكيد الشحن الصادر</span><span class="sxs-lookup"><span data-stu-id="514e4-444">Override outbound shipped confirmation date</span></span>
        - <span data-ttu-id="514e4-445">تمكين تأكيد تقسيم شحن أمر التحويل وترحيل تحويل الشحنة</span><span class="sxs-lookup"><span data-stu-id="514e4-445">Enable split of transfer order ship confirmation and posting transfer ship</span></span>
    - <span data-ttu-id="514e4-446">**التسليم المباشر** - إنشاء رسوم للعميل للتسليم المباشر.</span><span class="sxs-lookup"><span data-stu-id="514e4-446">**Direct delivery** - Create customer charges for direct delivery.</span></span>
    - <span data-ttu-id="514e4-447">**المحركات** - تهيئة بيانات المحرك الأساسي.</span><span class="sxs-lookup"><span data-stu-id="514e4-447">**Engines** - Initialize base engine data.</span></span>
    - <span data-ttu-id="514e4-448">**تسوية الشحن** - الإشارة إلى ما إذا كان سيتم تمكين تسوية الشحن أم لا.</span><span class="sxs-lookup"><span data-stu-id="514e4-448">**Freight reconciliation** - Indicate whether to enable freight reconciliation.</span></span> <span data-ttu-id="514e4-449">في حالة تعطيل هذا الخيار، لن يتم إنشاء أي فواتير شحن.</span><span class="sxs-lookup"><span data-stu-id="514e4-449">If this option is disabled, no freight bills will be generated.</span></span>
    - <span data-ttu-id="514e4-450">**بوليصة الشحن** - الإشارة إلى ما إذا كان سيتم إنشاء بوليصة شحن رئيسية عند وجود أكثر من شحن واحد في الحمل.</span><span class="sxs-lookup"><span data-stu-id="514e4-450">**Bill of lading** - Indicate whether to create a master bill of lading when there is more than one shipment on a load.</span></span>
3.  <span data-ttu-id="514e4-451">من علامة التبويب **التقارير**، راجع علامات التبويب السريعة التالية:</span><span class="sxs-lookup"><span data-stu-id="514e4-451">On the **Reports** tab, review the following FastTabs:</span></span>
    - <span data-ttu-id="514e4-452">**تقرير الحمل** - تحديد نوع ملاحظة تقرير الحمل.</span><span class="sxs-lookup"><span data-stu-id="514e4-452">**Load report** - Select a load report note type.</span></span>
    -  <span data-ttu-id="514e4-453">**بوليصة الشحن** - تحديد غرض شركة نقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-453">**Bill of lading** - Select a carrier purpose.</span></span>

<span data-ttu-id="514e4-454">في علامة التبويب **إدارة الطباعة**، يتم سرد المستندات المتنوعة في إدارة النقل المُدارة بواسطة إدارة الطباعة.</span><span class="sxs-lookup"><span data-stu-id="514e4-454">On the **Print management** tab, the various documents in transportation management that are managed by print management are listed.</span></span>

<span data-ttu-id="514e4-455">في علامة التبويب **التسلسلات الرقمية**، يتم سرد التسلسلات الرقمية القياسية في إدارة النقل.</span><span class="sxs-lookup"><span data-stu-id="514e4-455">On the **Number sequences** tab, standard number sequences in transportation management are listed.</span></span>

