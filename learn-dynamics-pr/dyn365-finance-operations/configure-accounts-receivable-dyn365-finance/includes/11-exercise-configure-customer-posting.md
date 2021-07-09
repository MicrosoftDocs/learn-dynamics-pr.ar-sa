---
ms.openlocfilehash: f4d14782e0cdc40da86210155c18ac8171ba3f91
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070623"
---
## <a name="scenario"></a><span data-ttu-id="a9d38-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="a9d38-101">Scenario</span></span>

<span data-ttu-id="a9d38-102">قام مدير الحسابات في Contoso بطلب موظف الحسابات المدينة لإعداد ملف تعريف ترحيل جديد لمجموعة من عملاء البيع بالتجزئة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-102">The Accounting Manager at Contoso has asked the Accounts receivable clerk to set up a new posting profile for a group of retail customers.</span></span>

<span data-ttu-id="a9d38-103">حدد الخيارات المناسبة لضمان ما يلي:</span><span class="sxs-lookup"><span data-stu-id="a9d38-103">Select the appropriate options to ensure the following:</span></span>

-   <span data-ttu-id="a9d38-104">سيتم إنشاء الإدخالات باستخدام ملف التعريف هذا للتسوية التلقائية.</span><span class="sxs-lookup"><span data-stu-id="a9d38-104">Entries will be created using this profile for automatic settlement.</span></span>
-   <span data-ttu-id="a9d38-105">سيقوم التطبيق بحساب الفائدة على الأرصدة المعلقة للعملاء الذين لديهم ملف التعريف هذا.</span><span class="sxs-lookup"><span data-stu-id="a9d38-105">The application will calculate interest on outstanding balances for customers who have this profile.</span></span>
-   <span data-ttu-id="a9d38-106">قد يتم إصدار خطاب تحصيل للعملاء الذين لديهم ملف التعريف هذا.</span><span class="sxs-lookup"><span data-stu-id="a9d38-106">A collection letter might be issued for customers who have this profile.</span></span>
-   <span data-ttu-id="a9d38-107">عند تسوية الحركات بالكامل، يجب ألا تتغير الحركات إلى ملف تعريف ترحيل آخر.</span><span class="sxs-lookup"><span data-stu-id="a9d38-107">When transactions are settled in full, the transactions should not change to another posting profile.</span></span>
-   <span data-ttu-id="a9d38-108">سيتم ترحيل حركات مجموعة عملاء البيع بالتجزئة إلى الحساب الملخص 130100 وحساب التسوية 110110.</span><span class="sxs-lookup"><span data-stu-id="a9d38-108">Transactions for the retail customers group will post to summary account 130100 and settle account 110110.</span></span>


## <a name="set-up-a-customer-posting-profile"></a><span data-ttu-id="a9d38-109">إعداد ملف تعريف ترحيل العميل</span><span class="sxs-lookup"><span data-stu-id="a9d38-109">Set up a customer posting profile</span></span>

1.  <span data-ttu-id="a9d38-110">في الشركة **USMF**، انتقل إلى **الحسابات المدينة > إعداد > ملفات تعريف ترحيل العميل**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-110">In the **USMF** company, go to **Accounts receivable > Setup > Customer posting profiles**.</span></span>
2.  <span data-ttu-id="a9d38-111">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-111">Select **New**.</span></span>
3.  <span data-ttu-id="a9d38-112">في الحقل **ملف تعريف الترحيل**، اكتب **عرض**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-112">In the **Posting Profile** field, type **Prom**.</span></span>
4.  <span data-ttu-id="a9d38-113">في حقل **الوصف**، اكتب **عرض ترويجي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-113">In the **Description** field, type **Promotion**.</span></span>
5.  <span data-ttu-id="a9d38-114">في علامة التبويب السريعة **قيود الجدول**، تأكد من تعيين الخيار التالي **السماح بالتسوية التلقائية** إلى **نعم.**</span><span class="sxs-lookup"><span data-stu-id="a9d38-114">On the **Table restrictions** FastTab, make sure that the following option has **Allow automatic settlement** set to **Yes.**</span></span>
6.  <span data-ttu-id="a9d38-115">قم بتعيين خيارات **الفائدة** و **خطاب التحصيل** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-115">Set the **Interest** and **Collection letter** options to **Yes**.</span></span>
7.  <span data-ttu-id="a9d38-116">تحقق من أن حقل **الإغلاق** فارغ.</span><span class="sxs-lookup"><span data-stu-id="a9d38-116">Verify that the **Close** field is blank.</span></span>
8.  <span data-ttu-id="a9d38-117">في علامة التبويب السريعة **الإعداد**، حدد **إضافة** لإنشاء حساب جديد وإعداده.</span><span class="sxs-lookup"><span data-stu-id="a9d38-117">In the **Setup** FastTab, select **Add** to create and set up a new Account.</span></span>
9.  <span data-ttu-id="a9d38-118">في الحقل **كود الحساب**، حدد **مجموعة**</span><span class="sxs-lookup"><span data-stu-id="a9d38-118">In the **Account code** field, select **Group**.</span></span>
10. <span data-ttu-id="a9d38-119">في الحقل **رقم الحساب/المجموعة**، حدد **30 عميل بيع بالتجزئة**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-119">In the **Account/Group Number** field, select **30 Retail customers**.</span></span>
11. <span data-ttu-id="a9d38-120">في الحقل **حساب الملخص**، حدد **130100**</span><span class="sxs-lookup"><span data-stu-id="a9d38-120">In the  **Summary account** field, select **130100**.</span></span>
12. <span data-ttu-id="a9d38-121">في الحقل **حساب السيولة للمدفوعات**، حدد **110110**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-121">In the **Liquidity account for payments** field, select **110110**.</span></span>
13. <span data-ttu-id="a9d38-122">في الحقل **تسلسل خطاب التحصيل**، حدد **عالي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-122">In the **Collection letter sequence** field, select **High**.</span></span>
14. <span data-ttu-id="a9d38-123">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-123">Select **Save**.</span></span>
15. <span data-ttu-id="a9d38-124">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-124">Close the page.</span></span>

## <a name="establish-customer-payment-terms"></a><span data-ttu-id="a9d38-125">‏‫وضع شروط دفع العميل‬</span><span class="sxs-lookup"><span data-stu-id="a9d38-125">Establish customer payment terms</span></span>

1.  <span data-ttu-id="a9d38-126">في **USMF**، انتقل إلى **الحسابات المدينة > إعداد المدفوعات > أيام الدفع**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-126">In **USMF**, go to **Accounts receivable > Payments setup > Payment days**.</span></span>
2.  <span data-ttu-id="a9d38-127">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-127">Select **New**.</span></span>
3.  <span data-ttu-id="a9d38-128">في الحقل **يوم الدفع**، أدخل **17**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-128">In the **Payment day** field, enter **17**.</span></span>
4.  <span data-ttu-id="a9d38-129">في الحقل **الوصف**، أدخل **17 من الشهر**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-129">In the **Description** field, enter **17th of the month**.</span></span>
5.  <span data-ttu-id="a9d38-130">في الحقل **أسبوع/شهر**، حدد **شهر**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-130">In the **Week/Month** field, select **Month**.</span></span>
6.  <span data-ttu-id="a9d38-131">في الحقل **يوم الشهر**، أدخل **17**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-131">In the **Day of month** field, enter **17**.</span></span>
7.  <span data-ttu-id="a9d38-132">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-132">Select **Save**.</span></span>
8.  <span data-ttu-id="a9d38-133">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-133">Close the page.</span></span>
9.  <span data-ttu-id="a9d38-134">انتقل إلى **الحسابات المدينة > إعداد المدفوعات > أيام الدفع**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-134">Go to **Accounts receivable > Payments setup > Terms of payment**.</span></span>
10. <span data-ttu-id="a9d38-135">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-135">Select **New**.</span></span> 
11. <span data-ttu-id="a9d38-136">في الحقل **شروط الدفع**، أدخل **GTL-45**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-136">In the **Terms of payment** field, enter **GTL-45**.</span></span>
12. <span data-ttu-id="a9d38-137">في حقل **الوصف**، أدخل **صافي 45 يوماً**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-137">In the **Description** field, enter **Net 45 days**.</span></span>
13. <span data-ttu-id="a9d38-138">في الحقل **طريقة الدفع**، حدد **الشهر الحالي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-138">In the **Payment method** field, select **Current month**.</span></span> 
14. <span data-ttu-id="a9d38-139">في الحقل **يوم الدفع**، أدخل **17**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-139">In the **Payment day** field, enter **17**.</span></span> 
15. <span data-ttu-id="a9d38-140">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-140">Select **Save**.</span></span>
16. <span data-ttu-id="a9d38-141">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-141">Close the page.</span></span>
17. <span data-ttu-id="a9d38-142">انتقل إلى **الحسابات المدينة > إعداد المدفوعات > خصومات نقدية**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-142">Go to **Accounts receivable > Payments setup > Cash discounts**.</span></span>
18. <span data-ttu-id="a9d38-143">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-143">Select **New**.</span></span>
19. <span data-ttu-id="a9d38-144">في حقل **الخصم النقدي**، أدخل **GLS-15D5%**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-144">In the **Cash discount** field, enter **GLS-15D5%**.</span></span>
20. <span data-ttu-id="a9d38-145">في الحقل **الوصف**، أدخل **عرض 5% إذا تم الدفع خلال 15 يوماً**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-145">In the **Description** field, enter **Offer 5% if paid within 15 days**.</span></span>
21. <span data-ttu-id="a9d38-146">أدخل عدد الأيام المستخدمة لحساب تاريخ الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="a9d38-146">Enter the number of days used to calculate the cash discount date.</span></span> <span data-ttu-id="a9d38-147">في حقل **الأيام**، أدخل **15**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-147">In the **Days** field, enter **15**.</span></span> 
22. <span data-ttu-id="a9d38-148">في حقل **نسبة الخصم**، أدخل **5**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-148">In the **Discount percentage** field, enter **5**.</span></span>
23. <span data-ttu-id="a9d38-149">في الحقل **الحساب الرئيسي لخصومات العميل**، حدد **403300**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-149">In the **Main account for customer discounts** field, select **403300**.</span></span>
24. <span data-ttu-id="a9d38-150">في حقل **حسابات مقابلة الخصم**، حدد **استخدام الحساب الرئيسي لخصومات المورد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-150">In the **Discount offset accounts** field, select **Use main account for Vendor discounts**.</span></span>
25. <span data-ttu-id="a9d38-151">في الحقل **الحساب الرئيسي لخصومات المورد**، حدد **.212160**</span><span class="sxs-lookup"><span data-stu-id="a9d38-151">In the **Main account for vendor discounts**, select **212160.**</span></span> 
26. <span data-ttu-id="a9d38-152">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-152">Select **Save**.</span></span>
27. <span data-ttu-id="a9d38-153">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-153">Close the page.</span></span>

## <a name="create-a-method-of-payment-for-customer-payments"></a><span data-ttu-id="a9d38-154">إنشاء طريقة دفع لمدفوعات العميل</span><span class="sxs-lookup"><span data-stu-id="a9d38-154">Create a method of payment for customer payments</span></span>

1.  <span data-ttu-id="a9d38-155">افتح **الحسابات المدينة > إعداد المدفوعات > أساليب الدفع**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-155">Open **Accounts receivable > Payments setup > Methods of payment**.</span></span>
2.  <span data-ttu-id="a9d38-156">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-156">Select **New**.</span></span>
3.  <span data-ttu-id="a9d38-157">في الحقل **شروط الدفع**، أدخل **GTL-EP**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-157">In the **Method of payment** field, enter **GTL-EP**.</span></span> <span data-ttu-id="a9d38-158">يتم عرض طريقة معرف الدفع في الفواتير والمدفوعات، التالي جعلها وصفية بشكل كافٍ لمعرفة نوع الدفع الذي يتم تسجيله وللحساب البنكي.</span><span class="sxs-lookup"><span data-stu-id="a9d38-158">The Method of payment ID is shown on invoices and payments, so make it descriptive enough to understand what type of payment is being recorded and for what bank account.</span></span>
4.  <span data-ttu-id="a9d38-159">في الحقل **الوصف**، أدخل **المدفوعات الإلكترونية**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-159">In the **Description** field, enter **Electronic payments**.</span></span>
5.  <span data-ttu-id="a9d38-160">في الحقل **حالة الدفع**، حدد **تمت الموافقة**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-160">In the **Payment status** field, select **Approved**.</span></span> 
6.  <span data-ttu-id="a9d38-161">في الحقل **الفترة**، حدد **الإجمالي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-161">In the **Period** field, select **Total**.</span></span> 
7.  <span data-ttu-id="a9d38-162">في الحقل **نوع الدفع**، حدد نوع الدفع **كدفع إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-162">In the **Payment type** field, select the type of payment as **Electronic payment**.</span></span> 
8.  <span data-ttu-id="a9d38-163">في الحقل **نوع الحساب**، حدد **البنك.**</span><span class="sxs-lookup"><span data-stu-id="a9d38-163">In the **Account type** field, select **Bank.**</span></span>
9.  <span data-ttu-id="a9d38-164">في الحقل **حساب الدفع**، حدد **USMF OPER**</span><span class="sxs-lookup"><span data-stu-id="a9d38-164">In the **Payment account** field, select **USMF OPER**.</span></span>
10. <span data-ttu-id="a9d38-165">في الحقل **نوع حركة البنك**، حدد **إيداع**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-165">In the **Bank transaction type** field, select **Deposit**.</span></span> 
11. <span data-ttu-id="a9d38-166">سيؤدي تحديد هذا الدفع إلى الترحيل إلى حساب وسيط بشكل مؤقت.</span><span class="sxs-lookup"><span data-stu-id="a9d38-166">Selecting this payment will temporarily post to a bridging account.</span></span>
    <span data-ttu-id="a9d38-167">عيّن الخيار **ترحيل وسيط** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-167">Set the **Bridging posting** option to **Yes**.</span></span> 
12. <span data-ttu-id="a9d38-168">في الحقل **حساب الوسيط**، حدد **130730.**</span><span class="sxs-lookup"><span data-stu-id="a9d38-168">In the **Bridging account** field, select **130730.**</span></span> <span data-ttu-id="a9d38-169">هذا هو الحساب الرئيسي الذي سيتم ترحيل الدفع إليه بشكل مؤقت إذا كنت تستخدم وسيط.</span><span class="sxs-lookup"><span data-stu-id="a9d38-169">This is the main account to which the payment will temporarily post if you are using bridging.</span></span>
13. <span data-ttu-id="a9d38-170">استخدم علامة التبويب السريعة **تنسيقات الملف** لتحديد إعداد المدفوعات الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="a9d38-170">Use the **File formats** Fast tab to define the  setting for electronic payments.</span></span> 
14. <span data-ttu-id="a9d38-171">حدد الزر **إعداد**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-171">Select the **Setup** button.</span></span>
14. <span data-ttu-id="a9d38-172">من علامة التبويب **تصدير**، في القائمة **متوفر**، حدد **NACHA (US)** واستخدم السهم لتحريكه إلى المجموعة **المحددة**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-172">On the **Export** tab, in the **AVAILABLE** list, select **NACHA (US)** and use the arrow to move it to the **SELECTED** group.</span></span> 
15. <span data-ttu-id="a9d38-173">في علامة التبويب **استيراد**، حدد **JBA(JP)- Format A** وقم بنقله إلى المجموعة **المحددة**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-173">On the **Import** tab, select **JBA(JP)- Format A** and move it to the **SELECTED** group.</span></span>
16. <span data-ttu-id="a9d38-174">من علامة التبويب **إعادة**، في القائمة **متوفر**، حدد **ملف تخطيط قابل للتكوين** وحرِّكه إلى المجموعة **المحددة**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-174">On the **Return** tab, in the **AVAILABLE** list, select the **Configurable layout file** and move it to the **SELECTED** group.</span></span> 
17. <span data-ttu-id="a9d38-175">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-175">Select **Save**.</span></span>
18. <span data-ttu-id="a9d38-176">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-176">Close the page.</span></span>
19. <span data-ttu-id="a9d38-177">في علامة التبويب السريعة **تنسيقات الملفات** في مجموعة **تحديث الفاتورة**، قم بتعيين شريط التمرير إلى **نعم** **لإنشاء دفتر يومية السحب وترحيله تلقائياً عند ترحيل الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-177">On the **File formats** Fast tab in the **INVOICE UPDATE** group, set the slider to **Yes** for **Create and post draw journal automatically when posting invoices**.</span></span>
20. <span data-ttu-id="a9d38-178">في الحقل **الاسم**، حدد **CustPay**</span><span class="sxs-lookup"><span data-stu-id="a9d38-178">In the **Name** field, select **CustPay**.</span></span>
21. <span data-ttu-id="a9d38-179">في المجموعة **تنسيقات الملفات**، **لتنسيق التصدير** حدد **NACHA (US)**</span><span class="sxs-lookup"><span data-stu-id="a9d38-179">In the **FILE FORMATS** group, for **Export format** select **NACHA (US)**</span></span>
22. <span data-ttu-id="a9d38-180">في **تنسيق الاستيراد**، حدد **JBA(JP) – Format A**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-180">In the **Import format**, select **JBA(JP) – Format A**.</span></span>
23. <span data-ttu-id="a9d38-181">في **تنسيق الإرجاع**، حدد **ملف تخطيط قابل للتكوين**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-181">In the **Return format**, select **Configurable layout file**.</span></span> 
24. <span data-ttu-id="a9d38-182">استخدم علامة التبويب السريعة **التحكم في الدفع** لتحديد الحقول الإلزامية.</span><span class="sxs-lookup"><span data-stu-id="a9d38-182">Use the **Payment control** Fast tab to define mandatory fields.</span></span> <span data-ttu-id="a9d38-183">حدد كافة الحقول الموجودة في العمود **ممكن**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-183">Select all fields in the **Enabled** column.</span></span>
25. <span data-ttu-id="a9d38-184">استخدم علامة التبويب السريعة **سمات الدفع** لتحديد سمات الدفع التي ترغب في استخدامها لطريقة الدفع هذه.</span><span class="sxs-lookup"><span data-stu-id="a9d38-184">Use the **Payment attributes** Fast tab to define which payment     attributes you want to use for this method of payment.</span></span> <span data-ttu-id="a9d38-185">حدد **حساب الدفع** و **معرف الدفع** في العمود **ممكن**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-185">Select **Payment account** and **Payment ID** in the **Enabled** column.</span></span>
26. <span data-ttu-id="a9d38-186">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-186">Select **Save**.</span></span>
27. <span data-ttu-id="a9d38-187">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a9d38-187">Close the page.</span></span>

## <a name="create-payment-fees-for-customer-payments"></a><span data-ttu-id="a9d38-188">قم بإنشاء رسوم الدفع لمدفوعات العميل.</span><span class="sxs-lookup"><span data-stu-id="a9d38-188">Create payment fees for customer payments.</span></span>

1.  <span data-ttu-id="a9d38-189">في **USMF**، انتقل إلى **الحسابات المدينة > إعداد المدفوعات > رسوم الدفع**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-189">In **USMF**, go to **Accounts receivable > Payments setup > Payment fee**.</span></span>
2.  <span data-ttu-id="a9d38-190">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-190">Select **New**.</span></span>
3.  <span data-ttu-id="a9d38-191">في الحقل **معرف الرسوم**، أدخل **W01**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-191">In the **Fee ID** field, enter **W01**.</span></span> <span data-ttu-id="a9d38-192">يتم عرض **معرف الرسوم** على دفاتر يومية المدفوعات، لذلك اجعلها وصفية بما يكفي لفهم الرسوم التي يتم تقييمها.</span><span class="sxs-lookup"><span data-stu-id="a9d38-192">The **Fee ID** displays on payment journals, so make it descriptive enough to understand what fee is being assessed.</span></span>
4.  <span data-ttu-id="a9d38-193">في حقل **الاسم**، أدخِل **بنكي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-193">In the **Name** field, enter **Wire**.</span></span>
5.  <span data-ttu-id="a9d38-194">في الحقل **وصف الرسوم**، أدخل **رسوم بنكية للتحويل البنكي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-194">In the **Fee description** field, enter **Bank fee for wire transfer**.</span></span>
6.  <span data-ttu-id="a9d38-195">في الحقل **التكلفة**، حدد **العميل**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-195">In the **Charge** field, select **Customer**.</span></span>
7.  <span data-ttu-id="a9d38-196">في الحقل **نوع دفتر اليومية**، حدد **دفع العميل**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-196">In the **Journal type** field, select **Customer payment**.</span></span>
8.  <span data-ttu-id="a9d38-197">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-197">Select **Save**.</span></span>
9. <span data-ttu-id="a9d38-198">حدد **إعداد رسوم الدفع**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-198">Select **Payment fee setup**.</span></span> <span data-ttu-id="a9d38-199">يتم استخدام إعداد رسوم الدفع لتحديد المعايير الخاصة بوقت تقييم رسوم الدفع.</span><span class="sxs-lookup"><span data-stu-id="a9d38-199">The Payment fee setup is used to define the criteria for when the payment fee will be assessed.</span></span> <span data-ttu-id="a9d38-200">على سبيل المثال، يمكنك تحديد حساب الرسوم إذا كان الحساب البنكي هو **USMF OPER**، وكانت طريقة الدفع هي **شيك**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-200">For example, you can define that the fee will be calculated if the bank account is **USMF OPER**, and the method of payment is **check**.</span></span>
10. <span data-ttu-id="a9d38-201">في حقل **عمليات التجميع**، حدد **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-201">In the **Groupings** field, select **Table**.</span></span> 
11. <span data-ttu-id="a9d38-202">في الحقل **علاقة البنك**، حدد **USMF OPER**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-202">In the **Bank relation** field, select **USMF OPER**.</span></span>
12. <span data-ttu-id="a9d38-203">في الحقل **طريقة الدفع**، حدد **المدفوعات الإلكترونية GTL-EP**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-203">In the **Method of payment** field, select **GTL-EP Electronic payments**.</span></span>
13. <span data-ttu-id="a9d38-204">في الحقل **عملة الدفع**، أدخل **دولار أمريكي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-204">In the **Payment currency** field, enter **USD**.</span></span> 
14. <span data-ttu-id="a9d38-205">في حقل **النسبة المئوية/المبلغ** حدد **نسبه مئوية**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-205">In the **Percentage/Amount** field select **Percent**.</span></span>  
15. <span data-ttu-id="a9d38-206">في حقل **عملة الرسوم**، حدد **دولار أمريكي**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-206">In the **Fee currency** field, select **USD**.</span></span>
16. <span data-ttu-id="a9d38-207">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a9d38-207">Select **Save**.</span></span>
17. <span data-ttu-id="a9d38-208">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="a9d38-208">Close all pages.</span></span>

## <a name="go-to-the-next-lab-instructions"></a><span data-ttu-id="a9d38-209">الانتقال إلى إرشادات المعمل التالية</span><span class="sxs-lookup"><span data-stu-id="a9d38-209">Go to the next lab instructions</span></span> 
 
<span data-ttu-id="a9d38-210">حدد الزر **التالي** في الركن الأيسر السفلي من الشريط الجانبي.</span><span class="sxs-lookup"><span data-stu-id="a9d38-210">Select the **Next** button in the bottom-right corner of the side bar.</span></span> 
