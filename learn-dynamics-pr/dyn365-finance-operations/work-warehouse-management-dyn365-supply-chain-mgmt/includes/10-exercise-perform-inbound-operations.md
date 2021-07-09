---
ms.openlocfilehash: 3f1e91d411573ff687de0c1c0f0ef8a2cad39aaf
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6073860"
---
## <a name="scenario"></a><span data-ttu-id="a9f75-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="a9f75-101">Scenario</span></span> 
<span data-ttu-id="a9f75-102">وكمدير مستودع Contoso لعصير البرتقال، تحتاج إلى معالجة إيصال أمر شراء باستخدام جهاز محمول.</span><span class="sxs-lookup"><span data-stu-id="a9f75-102">As a warehouse manager for Contoso Orange Juice, you need to process a purchase order receipt by using a mobile device.</span></span> <span data-ttu-id="a9f75-103">لقد طلبت صندوق واحد من عصير الجريب فروت.</span><span class="sxs-lookup"><span data-stu-id="a9f75-103">You have ordered one box of grapefruit juice.</span></span> <span data-ttu-id="a9f75-104">سيكون هذا الأمر من المورد US-112 ويتم شحنه إلى المستودع 30.</span><span class="sxs-lookup"><span data-stu-id="a9f75-104">This order will be from Vendor US-112 and shipped to Warehouse 30.</span></span> <span data-ttu-id="a9f75-105">سعر الوحدة سيكون 2.50 دولار أمريكي لكل صندوق.</span><span class="sxs-lookup"><span data-stu-id="a9f75-105">The unit price will be USD 2.50 for each box.</span></span>

## <a name="create-a-purchase-order"></a><span data-ttu-id="a9f75-106">إنشاء أمر شراء</span><span class="sxs-lookup"><span data-stu-id="a9f75-106">Create a purchase order</span></span>

1.  <span data-ttu-id="a9f75-107">حدد الشركة **USP2** من أعلى يسار شاشة Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="a9f75-107">Select the company **USP2** in the top-right corner of the Supply Chain Management screen.</span></span>
2.  <span data-ttu-id="a9f75-108">افتح **الحسابات الدائنة > أوامر الشراء > كافة أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-108">Open **Accounts payable > Purchase orders > All purchase orders**.</span></span>

2.  <span data-ttu-id="a9f75-109">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="a9f75-109">Select **New** in the Action Pane.</span></span>

3.  <span data-ttu-id="a9f75-110">حدد **حساب المورد US-112**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-110">Select **Vendor account US-112**.</span></span>

4.  <span data-ttu-id="a9f75-111">في علامة التبويب السريعة **عام**، أدخل أبعاد التخزين **للموقع 3** و **المستودع 30**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-111">On the **General** FastTab, enter storage dimensions of **Site 3** and **Warehouse 30**.</span></span>

5.  <span data-ttu-id="a9f75-112">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-112">Select **OK**.</span></span>

6.  <span data-ttu-id="a9f75-113">في علامة التبويب السريعة **بنود أمر الشراء**، حدد **رقم الصنف P9500**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-113">On the **Purchase order lines** FastTab, select **Item number P9500**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a9f75-114">ستحصل على رسالة تفيد بأن المورد غير مخول لهذا المنتج.</span><span class="sxs-lookup"><span data-stu-id="a9f75-114">You will get a message that the vendor is not authorized for this product.</span></span> <span data-ttu-id="a9f75-115">وهذا تحذير فقط.</span><span class="sxs-lookup"><span data-stu-id="a9f75-115">This is a warning only.</span></span> <span data-ttu-id="a9f75-116">يمكنك المتابعة بعد إغلاق الرسالة.</span><span class="sxs-lookup"><span data-stu-id="a9f75-116">You may continue after closing the message.</span></span> 

7.  <span data-ttu-id="a9f75-117">أدخل **الكمية** **1**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-117">Enter a **Quantity** of **1**.</span></span>

8.  <span data-ttu-id="a9f75-118">أدخل **سعر الوحدة** **2.50**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-118">Enter a **Unit price** of **2.50**.</span></span>

9.  <span data-ttu-id="a9f75-119">في جزء الإجراء، حدد علامة التبويب **شراء**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-119">On the Action Pane, select the **Purchase** tab.</span></span>
10. <span data-ttu-id="a9f75-120">قم بتوسيع علامة التبويب السريعة **تفاصيل البند**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-120">Expand the **Line details** fast tab.</span></span>
11. <span data-ttu-id="a9f75-121">حدد علامة التبويب **الأبعاد المالية**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-121">Select the **Financial dimensions** tab.</span></span>
12. <span data-ttu-id="a9f75-122">في **الأبعاد المالية**، ضمن حقل **مجموعة المنتج**، حدد **OJ B2B**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-122">In the **Financial dimensions**, the **Product Group** field, select **OJ B2B**.</span></span>

10. <span data-ttu-id="a9f75-123">في مجموعة **الإجراءات**، حدد **تأكيد** ولاحظ رقم أمر الشراء الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a9f75-123">In the **Actions** group, select **Confirm** and note your purchase order number.</span></span>

12. <span data-ttu-id="a9f75-124">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9f75-124">Close the page.</span></span>

## <a name="create-a-mobile-device-user"></a><span data-ttu-id="a9f75-125">إنشاء مستخدم جهاز محمول</span><span class="sxs-lookup"><span data-stu-id="a9f75-125">Create a mobile device user</span></span> 

1.  <span data-ttu-id="a9f75-126">افتح **إدارة المستودعات > إعداد > العامل**</span><span class="sxs-lookup"><span data-stu-id="a9f75-126">Open **Warehouse management > Setup > Worker**.</span></span>

2.  <span data-ttu-id="a9f75-127">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="a9f75-127">Select **New** in the Action Pane.</span></span>

3.  <span data-ttu-id="a9f75-128">في حقل الحقل القائمة المنسدلة الخاصة بـ **العامل**، حدد **John Emory** ثم اضغط على **تحديد**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-128">In the **Worker** drop-down field, select **John Emory** then click **Select**.</span></span>

4.  <span data-ttu-id="a9f75-129">ضمن علامة التبويب السريعة **المستخدمين**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-129">On the **Users** FastTab, select **New**.</span></span>

5.  <span data-ttu-id="a9f75-130">بالنسبة **لمعرّف المستخدم**، أدخل **jemory**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-130">For **User ID**, enter **jemory**.</span></span>

6.  <span data-ttu-id="a9f75-131">بالنسبة **لاسم المستخدم**، أدخل **jemory**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-131">For **User name**, enter **jemory**.</span></span>

7.  <span data-ttu-id="a9f75-132">بالنسبة **للمستودع الافتراضي**، حدد **30**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-132">For **Default warehouse**, select **30**.</span></span>

8.  <span data-ttu-id="a9f75-133">بالنسبة **لاسم القائمة**، حدد **أساسي**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-133">For **Menu name**, select **Main**.</span></span>

9.  <span data-ttu-id="a9f75-134">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="a9f75-134">Select **Save** in the Action Pane.</span></span>

10. <span data-ttu-id="a9f75-135">بالنسبة **لكلمة المرور**، أدخل **5678**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-135">For **Password**, enter **5678**.</span></span>

11. <span data-ttu-id="a9f75-136">بالنسبة **لتأكيد كلمة المرور**، أدخل **5678**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-136">For **Confirm password**, enter **5678**.</span></span>

12. <span data-ttu-id="a9f75-137">حدد **تعيين كلمة المرور**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-137">Select **Set password**.</span></span>

13. <span data-ttu-id="a9f75-138">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9f75-138">Close the page.</span></span>


## <a name="create-a-purchase-order-receipt-by-using-the-mobile-device"></a><span data-ttu-id="a9f75-139">إنشاء إيصال أمر شراء باستخدام الجهاز المحمول</span><span class="sxs-lookup"><span data-stu-id="a9f75-139">Create a purchase order receipt by using the mobile device</span></span>

<span data-ttu-id="a9f75-140">**المتطلب الأساسي**</span><span class="sxs-lookup"><span data-stu-id="a9f75-140">**Prerequisite**</span></span>

<span data-ttu-id="a9f75-141">للتدريب العملي على استخدام الجهاز المحمول، يجب تمكين محاكي جهاز محمول في الجهاز الظاهري.</span><span class="sxs-lookup"><span data-stu-id="a9f75-141">To practice using the mobile device, you must enable a mobile device emulator in the Virtual machine.</span></span> 
<span data-ttu-id="a9f75-142">***قد تحتاج إلى توسيع الشريط الأيسر في بيئة المختبر لعرض كافة المحتويات في التعليمات.***</span><span class="sxs-lookup"><span data-stu-id="a9f75-142">***You may need to expand the right bar in the lab environment to see all content in the instructions.***</span></span>
<span data-ttu-id="a9f75-143">قم بإجراء الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="a9f75-143">Perform the following steps.</span></span>

1.  <span data-ttu-id="a9f75-144">انقر بزر الماوس الأيمن على علامة تبويب لوحة المعلومات الافتراضية الخاصة بالنظام العادي وحدد **تكرار علامة التبويب**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-144">Right-click on the tab of your normal system default dashboard and select **Duplicate tab**.</span></span>
2.  <span data-ttu-id="a9f75-145">سيكون عنوان URL الموجود علي علامة التبويب الجديدة هو: https:\//usnconeboxax1aos.cloud.onebox.dynamics.com/?cmp=USP2&mi=defaultdashboard</span><span class="sxs-lookup"><span data-stu-id="a9f75-145">The URL on your new tab will be: https:\//usnconeboxax1aos.cloud.onebox.dynamics.com/?cmp=USP2&mi=defaultdashboard</span></span>
3.  <span data-ttu-id="a9f75-146">احذف كافة الأحرف في علامة التبويب الجديدة بعد dynamics.com (مثل حذف /?cmp=USP2&mi=defaultdashboard)</span><span class="sxs-lookup"><span data-stu-id="a9f75-146">Delete all characters on the new tab after dynamics.com (i.e. delete /?cmp=USP2&mi=defaultdashboard)</span></span>
4.  <span data-ttu-id="a9f75-147">استبدل تلك الأحرف بـ /?mi=action%3awhsWorkExecute&cmp=USP2</span><span class="sxs-lookup"><span data-stu-id="a9f75-147">Replace those characters with /?mi=action%3awhsWorkExecute&cmp=USP2</span></span>

<span data-ttu-id="a9f75-148">سيتم الآن تشغيل المحاكي، ويمكنك تسجيل الدخول إلى محاكي الجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="a9f75-148">The emulator will now launch, and you can sign in to the mobile device emulator.</span></span>


1.  <span data-ttu-id="a9f75-149">تسجيل الدخول إلى الجهاز المحمول مستخدماً اسم المستخدم الذي قمت بتمكينه.</span><span class="sxs-lookup"><span data-stu-id="a9f75-149">Sign in to the mobile device with the user that you have enabled.</span></span>

2.  <span data-ttu-id="a9f75-150">حدد **الوارد**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-150">Select **Inbound**.</span></span>

3.  <span data-ttu-id="a9f75-151">حدد **تلقي الشراء**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-151">Select **Purchase receive**.</span></span>

4.  <span data-ttu-id="a9f75-152">أدخل رقم أمر الشراء في حقل **PONum**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-152">Enter the purchase order number in the **PONum** field.</span></span>

5.  <span data-ttu-id="a9f75-153">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-153">Select **OK**.</span></span>

6.  <span data-ttu-id="a9f75-154">في حقل **الصنف**، أدخل **P9500**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-154">In the **Item** field, enter **P9500**.</span></span> 

7.  <span data-ttu-id="a9f75-155">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-155">Select **OK**.</span></span>

8.  <span data-ttu-id="a9f75-156">أدخل الكمية **1** في حقل **الكمية**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-156">Enter a quantity of **1** in the **Qty** field.</span></span>

9.  <span data-ttu-id="a9f75-157">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-157">Select **OK**.</span></span>

10. <span data-ttu-id="a9f75-158">حدد **موافق** مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="a9f75-158">Select **OK** again.</span></span>

11. <span data-ttu-id="a9f75-159">أدخل رقم LP **LP951**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-159">Enter LP number **LP951**.</span></span>

12. <span data-ttu-id="a9f75-160">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-160">Select **OK**.</span></span>

13. <span data-ttu-id="a9f75-161">أدخل تاريخ اليوم **كتاريخ دفعة المورد**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-161">Enter today's date as the **Vendor batch date**.</span></span>

14. <span data-ttu-id="a9f75-162">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-162">Select **OK**.</span></span>

15. <span data-ttu-id="a9f75-163">أدخل تاريخ بعد ستة أشهر من التاريخ الحالي **كتاريخ انتهاء صلاحية المورد**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-163">Enter a date six months from the current date as the **Vendor expiry date**.</span></span>

16. <span data-ttu-id="a9f75-164">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-164">Select **OK**.</span></span>

17. <span data-ttu-id="a9f75-165">حدد سهم **الاستخدام كتاريخ انتهاء الصلاحية**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-165">Select the **Use as expiration date** arrow.</span></span>

18. <span data-ttu-id="a9f75-166">حدد **لا** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-166">Select **No** and select **OK**.</span></span>

19. <span data-ttu-id="a9f75-167">بالنسبة **لبلد/منطقة المنشأ 1**، أدخل **الولايات الأمريكية**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-167">For **Country/Region of Origin 1**, enter **USA**.</span></span>

20. <span data-ttu-id="a9f75-168">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-168">Select **OK**.</span></span>

21. <span data-ttu-id="a9f75-169">حدد **موافق** مرة أخرى لتجاوز الإدخال الثاني **للبلد/المنطقة**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-169">Select **OK** again to bypass the second **Country/region** entry.</span></span>

22. <span data-ttu-id="a9f75-170">لاحظ إشعار **اكتمال العمل**.</span><span class="sxs-lookup"><span data-stu-id="a9f75-170">Notice the **Work completed** notification.</span></span> 
