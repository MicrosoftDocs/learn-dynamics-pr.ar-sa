---
ms.openlocfilehash: 9d21bafd6004be556dd49159098ccfb7225a8699
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073689"
---
<span data-ttu-id="771ea-101">فيما يلي سيناريوهين لإنشاء أمر مبيعات: واحد بسيط وآخر يتضمن تباينات.</span><span class="sxs-lookup"><span data-stu-id="771ea-101">Here are two scenarios for creating a sales order: a simple one and one with variances.</span></span>

<span data-ttu-id="771ea-102">تستخدم السيناريوهات شركة البيانات التجريبية USMF لـSupply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="771ea-102">The scenarios use the demo data company USMF for Supply Chain Management.</span></span>

## <a name="scenario---sales-order-entry-to-cash-process---simple"></a><span data-ttu-id="771ea-103">السيناريو - إدخال أمر المبيعات لعملية نقدية - بسيط</span><span class="sxs-lookup"><span data-stu-id="771ea-103">Scenario - Sales order entry to cash process - simple</span></span>

<span data-ttu-id="771ea-104">في هذا السيناريو، يؤدي معالج الأمر في USMF، دور العديد من الأشخاص في هذا العرض التوضيحي الشامل.</span><span class="sxs-lookup"><span data-stu-id="771ea-104">In this scenario, the Order processor in USMF, plays the role of multiple persons in this end-to-end demonstration.</span></span> <span data-ttu-id="771ea-105">وتقوم الشركة التي يعمل بها معالج الأمر ببيع منتجات قياسية، والتي عادة ما تكون مصنعة أو مشتراة للمخزون.</span><span class="sxs-lookup"><span data-stu-id="771ea-105">The company that the Order processor works for sells standard products, typically either manufactured, or procured to stock.</span></span> <span data-ttu-id="771ea-106">يساعد بيع المنتجات القياسية في ضمان وقت تسليم قصير خاص بالإنتاج.</span><span class="sxs-lookup"><span data-stu-id="771ea-106">The sale of standard products helps ensure a short delivery lead time.</span></span> <span data-ttu-id="771ea-107">في بعض الحالات، تشتري الشركة حسب الطلب.</span><span class="sxs-lookup"><span data-stu-id="771ea-107">In some cases, the company procures to order.</span></span> <span data-ttu-id="771ea-108">في هذا السيناريو، يطلب العميل (تجار الجملة) تزويد ثلاثة أصناف بنود، وجهاز عرض وتلفزيونات LCD.</span><span class="sxs-lookup"><span data-stu-id="771ea-108">In this scenario, the customer (a wholesaler) orders replenishment of three line items, a projector, and LCD TVs.</span></span>
<span data-ttu-id="771ea-109">طلب العميل US-013 شحن كافة بنود الأمر في أقرب وقت ممكن، وإكماله؛ بالتالي لن تكون أي طلبات جزئية مقبولة.</span><span class="sxs-lookup"><span data-stu-id="771ea-109">Customer US-013 requests that all order lines be shipped as early as possible, and be complete; so no partial orders will be accepted.</span></span>

### <a name="instructions"></a><span data-ttu-id="771ea-110">الإرشادات</span><span class="sxs-lookup"><span data-stu-id="771ea-110">Instructions</span></span>

1.  <span data-ttu-id="771ea-111">انتقل إلى **المبيعات والتسويق > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="771ea-111">Go to **Sales and marketing > Customers > All customers**.</span></span>

2.  <span data-ttu-id="771ea-112">حدد العميل **US-013**.</span><span class="sxs-lookup"><span data-stu-id="771ea-112">Select customer **US-013**.</span></span>

3.  <span data-ttu-id="771ea-113">في علامة التبويب السريعة **البيع**، تحت القائمة الفرعية **جديد**، حدد **أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-113">On the **Sell** FastTab, under the **New** sub-menu, select **Sales order**.</span></span>

4.  <span data-ttu-id="771ea-114">تحت علامة التبويب السريعة **بنود أمر المبيعات**، في حقل **رقم الصنف**، حدد **T0002**.</span><span class="sxs-lookup"><span data-stu-id="771ea-114">Under the **Sales order lines** FastTab, in the **Item number** field, select **T0002**.</span></span>

5.  <span data-ttu-id="771ea-115">في حقل **الكمية**، أدخِل **10**.</span><span class="sxs-lookup"><span data-stu-id="771ea-115">In the **Quantity** field, enter **10**.</span></span> <span data-ttu-id="771ea-116">في علامة التبويب السريعة **أوامر المبيعات**، تكون القيمة الافتراضية لـ **تاريخ الشحن المطلوب** و **تاريخ الاستلام المطلوب** هو التاريخ الحالي.</span><span class="sxs-lookup"><span data-stu-id="771ea-116">In the **Sales order** FastTab, the **Requested ship date** and the **Requested receive date** default to the current date.</span></span>  

6.  <span data-ttu-id="771ea-117">قم بتوسيع علامة التبويب السريعة **تفاصيل البند**، ثم حدد علامة التبويب السريعة **التسليم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-117">Expand the **Line details** FastTab, and then select the **Delivery** FastTab.</span></span>

7.  <span data-ttu-id="771ea-118">حدد ارتباط **محاكاة تواريخ تاريخ التسليم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-118">Select the **Simulate delivery dates** link.</span></span>

8.  <span data-ttu-id="771ea-119">في مربع حوار **تواريخ الشحن والاستلام المتاحة**، لاحظ **أيام النقل** (على سبيل المثال: خمسة أيام).</span><span class="sxs-lookup"><span data-stu-id="771ea-119">In the **Available ship and receipt dates** dialog, observe the **Transport days** (Example: five days).</span></span> <span data-ttu-id="771ea-120">لاحظ أنه يمكنك شحن البضائع غداً، وأن العميل سيستلم صنف البند بعد خمسة أيام العمل.</span><span class="sxs-lookup"><span data-stu-id="771ea-120">Observe that you can ship the goods tomorrow, and that the customer will receive the line item in five business days.</span></span>

10. <span data-ttu-id="771ea-121">حدد **إلغاء الأمر** للخروج من الصفحة.</span><span class="sxs-lookup"><span data-stu-id="771ea-121">Select **Cancel** to exit the page.</span></span>

    > [!NOTE]
    > <span data-ttu-id="771ea-122">لن تقوم بتأكيد التواريخ لكل بند؛ بدلاً من ذلك، ستقوم بتأكيد التواريخ عبر كافة البنود فيما بعد حتى يمكنك ضمان انسجام تاريخ الشحن للحصول على التسليم الكامل.</span><span class="sxs-lookup"><span data-stu-id="771ea-122">You will not confirm dates on a line-by-line basis; instead, you will confirm dates across all lines later so that you can ensure ship date alignment for complete delivery.</span></span>

11. <span data-ttu-id="771ea-123">بالرجوع إلى التبويب السريعة **بنود أمر المبيعات**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="771ea-123">Back in the **Sales order lines** FastTab, select **Add line**.</span></span>

12. <span data-ttu-id="771ea-124">في الحقل **رقم الصنف**، حدد **T0004**.</span><span class="sxs-lookup"><span data-stu-id="771ea-124">In the **Item number** field, select **T0004**.</span></span>

13. <span data-ttu-id="771ea-125">في حقل **الكمية**، أدخِل **8**.</span><span class="sxs-lookup"><span data-stu-id="771ea-125">In the **Quantity** field, enter **8**.</span></span>

14. <span data-ttu-id="771ea-126">في علامة التبويب السريعة **تفاصيل البند**، حدد علامة التبويب **المنتج**.</span><span class="sxs-lookup"><span data-stu-id="771ea-126">In **Line details** FastTab, select the **Product** tab.</span></span>

15. <span data-ttu-id="771ea-127">في حقل **اللون**، أدخِل **فضي**.</span><span class="sxs-lookup"><span data-stu-id="771ea-127">In the **Color** field, enter **Silver**.</span></span>

16. <span data-ttu-id="771ea-128">بالرجوع إلى التبويب السريعة **بنود أمر المبيعات**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-128">Back in the **Sales order lines** FastTab, Select **Add**.</span></span>

17. <span data-ttu-id="771ea-129">في حقل **رقم البند**، أدخِل **T0005**.</span><span class="sxs-lookup"><span data-stu-id="771ea-129">In the **Item number** field, enter **T0005**.</span></span>

18. <span data-ttu-id="771ea-130">في حقل **الكمية**، أدخِل **10**.</span><span class="sxs-lookup"><span data-stu-id="771ea-130">In the **Quantity** field, enter **10**.</span></span>

19. <span data-ttu-id="771ea-131">في علامة التبويب السريعة **تفاصيل البند**، في حقل **اللون**، حدد **أبيض**.</span><span class="sxs-lookup"><span data-stu-id="771ea-131">In **Line details** FastTab, in the **Color** field, select **White**.</span></span> <span data-ttu-id="771ea-132">لديك الآن ثلاثة بنود أمر للعميل.</span><span class="sxs-lookup"><span data-stu-id="771ea-132">You now have three order lines for the customer.</span></span>

20. <span data-ttu-id="771ea-133">انقر على **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="771ea-133">Click **Save**.</span></span>

21. <span data-ttu-id="771ea-134">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="771ea-134">Close the page.</span></span>

<span data-ttu-id="771ea-135">قد تتلقى تحذيراً بأنه تم تجاوز الحد الائتماني للعميل.</span><span class="sxs-lookup"><span data-stu-id="771ea-135">You might receive a warning that the customer credit limit has been exceeded.</span></span> <span data-ttu-id="771ea-136">والسبب هو أن موظف اللحسابات المدينة لديه اجتماع خارج الموقع ولم يقم بتسجيل المدفوعات التي تم استلامها مؤخراً من العميل.</span><span class="sxs-lookup"><span data-stu-id="771ea-136">The reason is because the Accounts receivable clerks have had an off-site meeting and have not registered the payments that have been recently received from the customer.</span></span> <span data-ttu-id="771ea-137">بالتالي، تعتبر هذه الرسالة تحذيراً فقط، لذا يمكنك المتابعة.</span><span class="sxs-lookup"><span data-stu-id="771ea-137">Therefore, this message is only a warning, so you may proceed.</span></span>

## <a name="scenario---sales-order-entry-to-cash-process---reserve-inventory"></a><span data-ttu-id="771ea-138">السيناريو - إدخال أمر المبيعات لعملية نقدية - حجز المخزون</span><span class="sxs-lookup"><span data-stu-id="771ea-138">Scenario - Sales order entry to cash process - reserve inventory</span></span>

<span data-ttu-id="771ea-139">نظراً لأن US-013 هو أحد العملاء الذين يحظون بالأولوية، فقد تلقيت طلباً لإجراء حجز مقابل المخزون لضمان عدم قيام أوامر لاحقة بحجز الكمية المتاحة المطلوبة لأمر العميل صاحب الأولوية.</span><span class="sxs-lookup"><span data-stu-id="771ea-139">Because US-013 is a high priority customer, you have received a request to make a reservation against inventory to ensure that no subsequent orders reserve the required on-hand for this high priority customer order.</span></span>

### <a name="instructions"></a><span data-ttu-id="771ea-140">الإرشادات</span><span class="sxs-lookup"><span data-stu-id="771ea-140">Instructions</span></span>

1. <span data-ttu-id="771ea-141">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-141">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>

23. <span data-ttu-id="771ea-142">في صفحة القائمة، ابحث عن أمر المبيعات الذي قمت بإنشائه.</span><span class="sxs-lookup"><span data-stu-id="771ea-142">On the list page, find the sales order that you just created.</span></span> <span data-ttu-id="771ea-143">ستجد أمر المبيعات هذا موجوداً في الغالب في أسفل الشبكة.</span><span class="sxs-lookup"><span data-stu-id="771ea-143">This sales order is most likely at the bottom of the grid.</span></span>

24. <span data-ttu-id="771ea-144">حدد **رقم أمر المبيعات**، والذي يعد ارتباطاً يفتح أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="771ea-144">Select the **Sales order** number, which is a link that will open the sales order.</span></span>

25. <span data-ttu-id="771ea-145">حدد **تحرير** في جزء الإجراءات في أعلى الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-145">Select **Edit** in the Action Pane at the top of the screen.</span></span>

25. <span data-ttu-id="771ea-146">تحت علامة التبويب السريعة **بنود أمر المبيعات**، حدد الصنف **T0002**.</span><span class="sxs-lookup"><span data-stu-id="771ea-146">Under the **Sales order lines** FastTab, select line item **T0002**.</span></span> <span data-ttu-id="771ea-147">تظهر علامة اختيار على البند المحدد.</span><span class="sxs-lookup"><span data-stu-id="771ea-147">A check mark appears on the line selected.</span></span>

26. <span data-ttu-id="771ea-148">قم بتوسيع علامة التبويب السريعة **تفاصيل البند** ثم حدد علامة التبويب **إعداد**.</span><span class="sxs-lookup"><span data-stu-id="771ea-148">Expand the **Line details** FastTab and then select the **Setup** tab.</span></span>

26. <span data-ttu-id="771ea-149">قم بتعيين حقل **الحجز** إلى **تلقائي**.</span><span class="sxs-lookup"><span data-stu-id="771ea-149">Set the **Reservation** field to **Automatic**.</span></span> <span data-ttu-id="771ea-150">يعمل هذا الإعداد على إنشاء حجز في المخزون لطلب بند أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="771ea-150">This setting creates a reservation in inventory for the sales order line demand.</span></span>

27. <span data-ttu-id="771ea-151">قم بالتمرير لأعلى إلى **بنود أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-151">Scroll up to the **Sales order lines**.</span></span> <span data-ttu-id="771ea-152">في الشبكة، حدد صنف البند **T0004**.</span><span class="sxs-lookup"><span data-stu-id="771ea-152">In the grid, select line item **T0004**.</span></span>

28. <span data-ttu-id="771ea-153">في علامة التبويب السريعة **تفاصيل البند** حدد **إعداد**. وقم بتعيين حقل **الحجز** الحجز إلى **تلقائي**.</span><span class="sxs-lookup"><span data-stu-id="771ea-153">In the **Line details** FastTab select the **Setup** tab. Set the **Reservation** field to **Automatic**.</span></span>

29. <span data-ttu-id="771ea-154">قم بالتمرير مرة أخرى لأعلى إلى **بنود أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-154">Scroll back up to the **Sales order lines**.</span></span> <span data-ttu-id="771ea-155">في الشبكة، حدد صنف البند **T0005**.</span><span class="sxs-lookup"><span data-stu-id="771ea-155">In the grid, select line item **T0005**.</span></span>

30. <span data-ttu-id="771ea-156">قم بتعيين حقل **الحجز** إلى **تلقائي**.</span><span class="sxs-lookup"><span data-stu-id="771ea-156">Set the **Reservation** field to **Automatic**.</span></span> <span data-ttu-id="771ea-157">والآن، تم حجز كافة أصناف البند.</span><span class="sxs-lookup"><span data-stu-id="771ea-157">Now, all line items have been reserved.</span></span>

31. <span data-ttu-id="771ea-158">انقر على **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="771ea-158">Click **Save**.</span></span>

32. <span data-ttu-id="771ea-159">في جزء الإجراء، حدد علامة التبويب **إدارة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-159">In the Action Pane, select the **Manage** tab.</span></span>  

33. <span data-ttu-id="771ea-160">في القائمة الفرعية **العميل**، حدد **البحث عن الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="771ea-160">In the **Customer** submenu, select **Find prices**.</span></span> <span data-ttu-id="771ea-161">يتم فتح صفحة **الأسعار والخصومات الحالية**.</span><span class="sxs-lookup"><span data-stu-id="771ea-161">The **Current prices and discounts** page opens.</span></span> <span data-ttu-id="771ea-162">قم بإغلاق رسالة التحذير "تم تجاوز الحد الائتماني للعميل" في حالة ظهوره.</span><span class="sxs-lookup"><span data-stu-id="771ea-162">Close the "customer credit limit is exceeded" warning if it appears.</span></span>

34. <span data-ttu-id="771ea-163">تعرض صفحة **الأسعار والخصومات الحالية** كيفية حساب الأسعار والخصومات على الأصناف الخاصة بالعميل المحدد في حقل **حساب العميل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-163">The **Current prices and discounts** page shows how prices and discounts are calculated on items for the specific customer in the **Customer account** field.</span></span>           

33. <span data-ttu-id="771ea-164">في القائمة المنسدلة **رقم الصنف**، حدد رقم الصنف **T0002**.</span><span class="sxs-lookup"><span data-stu-id="771ea-164">In the **Item number** drop-down menu, select item number **T0002**.</span></span>

34. <span data-ttu-id="771ea-165">أدخِل **كمية** مقدارها **10** ثم اضغط على tab.</span><span class="sxs-lookup"><span data-stu-id="771ea-165">Enter a **Quantity** of **10** and then press tab.</span></span>

35. <span data-ttu-id="771ea-166">اعرض التفاصيل في قسم **السعر والخصومات من الاتفاقيات** باتجاه أسفل الصفحة.</span><span class="sxs-lookup"><span data-stu-id="771ea-166">View the detail of the **Price and discounts from agreements** section towards the bottom of the page.</span></span> 

36. <span data-ttu-id="771ea-167">لاحظ كيفية استرداد الأسعار والخصومات من الاتفاقيات التجارية.</span><span class="sxs-lookup"><span data-stu-id="771ea-167">Observe how prices and discounts are retrieved from trade agreements.</span></span> <span data-ttu-id="771ea-168">لم يتم تحديد أي خصومات ولا يوجد فواصل للسعر.</span><span class="sxs-lookup"><span data-stu-id="771ea-168">No discounts have been defined and there are no price breaks.</span></span> <span data-ttu-id="771ea-169">تم تحديد سعر عام لكافة العملاء، ما يعني وجود سعر قائمة قياسي قدره 3750.00 دولار أمريكي لكافة العملاء غير المعتمدين على الكمية.</span><span class="sxs-lookup"><span data-stu-id="771ea-169">A general price for all customers has been defined, implying a standard list price of USD 3,750.00 for all customers who are quantity independent.</span></span>

38. <span data-ttu-id="771ea-170">في القائمة المنسدلة **رقم الصنف**، أدخل الكمية **15**، ثم اضغط على tab لإعادة حساب القيم.</span><span class="sxs-lookup"><span data-stu-id="771ea-170">In the **Item number** drop-down menu, enter a quantity of **15**, and then press tab to recalculate values.</span></span>

39. <span data-ttu-id="771ea-171">لاحظ، كما هو متوقع، لم يتم منح أي سعر أفضل أو خصم إضافي للكمية الأعلى التي تم طلبها.</span><span class="sxs-lookup"><span data-stu-id="771ea-171">Observe, as expected, that no better price or additional discount is granted for a higher quantity that is ordered.</span></span>

40. <span data-ttu-id="771ea-172">أغلق **صفحة الأسعار والخصومات الحالية**.</span><span class="sxs-lookup"><span data-stu-id="771ea-172">Close the **Current prices and discounts page**.</span></span>

41. <span data-ttu-id="771ea-173">في جزء الإجراءات **أمر المبيعات**، حدد علامة التبويب **البيع**.</span><span class="sxs-lookup"><span data-stu-id="771ea-173">On the **Sales order** Action Pane, select the **Sell** tab.</span></span>

42. <span data-ttu-id="771ea-174">في القائمة الفرعية **الضرائب**، حدد **ضريبة المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-174">In the **Tax** submenu, select **Sales tax**.</span></span>

43. <span data-ttu-id="771ea-175">لاحظ **مبلغ ضريبة المبيعات الفعلي** الذي تم حسابه.</span><span class="sxs-lookup"><span data-stu-id="771ea-175">Observe the **Actual sales tax amount** calculated.</span></span> <span data-ttu-id="771ea-176">وضريبة المبيعات المحتسبة ترتبط برمز ضريبة المبيعات لموقع إيصال العميل، والذي يكون في هذه الحالة ولاية نيويورك، حيث يكون رمز ضريبة المبيعات 4 بالمائة.</span><span class="sxs-lookup"><span data-stu-id="771ea-176">The sales tax calculated is for a sales tax code for the customer receipt location, which in this case is New York State, where the sales tax code is 4 percent.</span></span>

44. <span data-ttu-id="771ea-177">انقر على **موافق** لإغلاق صفحة **ضريبة المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-177">Click **OK** to close the **Sales tax** page.</span></span>

45. <span data-ttu-id="771ea-178">في جزء الإجراء، حدد علامة التبويب **أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-178">In the Action Pane, select the **Sales order** tab.</span></span>

46. <span data-ttu-id="771ea-179">في القائمة الفرعية **عرض**، حدد **الإجماليات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-179">In the **View** submenu, select **Totals**.</span></span>

47. <span data-ttu-id="771ea-180">لاحظ الحساب الإجمالي لكافة ضرائب المبيعات المرتبطة بأمر المبيعات هذا.</span><span class="sxs-lookup"><span data-stu-id="771ea-180">Observe the total computation of all sales taxes that pertain to this sales order.</span></span> <span data-ttu-id="771ea-181">الحد الائتماني للعميل هو 500000.00 دولار أمريكي.</span><span class="sxs-lookup"><span data-stu-id="771ea-181">The customer credit line is USD 500,000.00.</span></span> <span data-ttu-id="771ea-182">إذا تجاوز **المبلغ الإجمالي الفرعي** مبلغ الحد الائتماني فسوف تستلم رسالة تحذير بتجاوز الحد الائتماني.</span><span class="sxs-lookup"><span data-stu-id="771ea-182">If the **Subtotal amount** exceeds the credit line amount you will receive the credit limit exceeded warning.</span></span> <span data-ttu-id="771ea-183">بالإضافة إلى ذلك، يتضمن حقل **مبلغ الفاتورة** إجمالي أمر المبيعات المطلوب فوترته للعميل.</span><span class="sxs-lookup"><span data-stu-id="771ea-183">Additionally, the **Invoice amount** field has the sales order total to be invoiced to the customer.</span></span>

<span data-ttu-id="771ea-184">بعد إنشاء تأكيد أمر المبيعات للعميل، يكون الهدف هو التأكد من أن كافة أصناف البند منسجمة مع صنف البند الذي يقع في تاريخ الشحن الأبعد في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="771ea-184">After creating a sales order confirmation for the customer, the objective is to ensure that all line items align with the line item that has the ship date farthest in the future.</span></span> <span data-ttu-id="771ea-185">وهذا التحقق لأجل التأكد من إجراء الشحن الكامل، دون حدوث شحن جزئي.</span><span class="sxs-lookup"><span data-stu-id="771ea-185">This verification is to ensure complete shipment, no partials.</span></span> 

<span data-ttu-id="771ea-186">النتيجة هو أن كل البنود ستكون بنفس تاريخ الشحن والاستلام المؤكد، وسيتم تلقائياً تحديث تاريخ الشحن والاستلام المؤكد لرأس أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="771ea-186">Output is that all lines will get the same confirmed ship and receipt date, and the sales order header will have the confirmed ship and receipt date auto updated.</span></span>

1. <span data-ttu-id="771ea-187">في صفحة **أمر المبيعات**، مع اختيار أمر المبيعات، حدد علامة التبويب **بيع** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="771ea-187">On the **Sales order** page, with your sales order checked, select the **Sell** tab in the Action Pane.</span></span>

49. <span data-ttu-id="771ea-188">في القائمة الفرعية **حساب**، حدد **تواريخ التسليم المؤكدة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-188">In the **Calculate** submenu, select **Confirmed delivery dates**.</span></span> <span data-ttu-id="771ea-189">يتم تعيين تواريخ الشحن المؤكدة على كافة بنود الأوامر وعلى رأس أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="771ea-189">Confirmed ship dates are set on all order lines and on the sales order header.</span></span> <span data-ttu-id="771ea-190">حدد **آخر تاريخ مؤكد مقبول** باستخدام رمز التقويم.</span><span class="sxs-lookup"><span data-stu-id="771ea-190">Select the **Latest confirmed date accepted** using the calendar icon.</span></span>

50. <span data-ttu-id="771ea-191">انقر على **موافق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-191">Click **OK**.</span></span> <span data-ttu-id="771ea-192">سيتم إرجاعك بعد ذلك إلى صفحة **تفاصيل أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-192">You are then returned to the **Sales order details** page.</span></span> 

51. <span data-ttu-id="771ea-193">حدد **أمر المبيعات** الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="771ea-193">Select your **Sales order**.</span></span> <span data-ttu-id="771ea-194">وهذا يضع علامة اختيار بجانب الأمر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="771ea-194">This places a check mark next to your order.</span></span>

52. <span data-ttu-id="771ea-195">في جزء الإجراء، في القائمة الفرعية **إنشاء**، حدد **تأكيد أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-195">On the Action Pane, in the **Generate** submenu, select **Confirm sales order**.</span></span>

53. <span data-ttu-id="771ea-196">في مربع الحوار **تأكيد أمر المبيعات**، قم بتعيين شريط التبديل **تأكيد الطباعة** إلى **نعم**، ثم حدد **موافق** لإنشاء طباعة على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-196">In the **Confirm sales order** dialog, set the **Print confirmation** toggle bar to **Yes**, and then select **OK** to generate print-to-screen.</span></span> <span data-ttu-id="771ea-197">قد تتلقى تحذيراً بشأن نشر التأكيد والطباعة إلى الشاشة فقط.</span><span class="sxs-lookup"><span data-stu-id="771ea-197">You may receive a warning about posting the confirmation and printing to screen only.</span></span> <span data-ttu-id="771ea-198">انقر على **نعم** للمتابعة.</span><span class="sxs-lookup"><span data-stu-id="771ea-198">Click **Yes** to continue.</span></span>

54. <span data-ttu-id="771ea-199">ستتلقى شاشة تعرض التقرير.</span><span class="sxs-lookup"><span data-stu-id="771ea-199">You will receive a screen displaying the report.</span></span> <span data-ttu-id="771ea-200">قم بمراجعة التقرير ثم إغلاقه.</span><span class="sxs-lookup"><span data-stu-id="771ea-200">Review and then close the report.</span></span> <span data-ttu-id="771ea-201">قد تتلقى تحذيراً إذا تم تجاوز الحد الائتماني.</span><span class="sxs-lookup"><span data-stu-id="771ea-201">You may receive a warning if the credit limit is exceeded.</span></span> <span data-ttu-id="771ea-202">أغلق رسالة التحذير.</span><span class="sxs-lookup"><span data-stu-id="771ea-202">Close the warning.</span></span>

55. <span data-ttu-id="771ea-203">في جزء الإجراءات **أمر المبيعات**، حدد علامة تبويب **التعبئة والتغليف**.</span><span class="sxs-lookup"><span data-stu-id="771ea-203">On the **Sales order** Action Pane, select the **Pick and Pack** tab.</span></span>

56. <span data-ttu-id="771ea-204">في القائمة الفرعية **إنشاء**، حدد **إنشاء قائمة انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="771ea-204">In the **Generate** submenu, select **Generate picking list**.</span></span>

57. <span data-ttu-id="771ea-205">في صفحة **نشر قائمة الانتقاء**، يمكنك التمرير للاطلاع على **نظرة عامة على قائمة الانتقاء** و **بنود أمر المبيعات** المرتبطة.</span><span class="sxs-lookup"><span data-stu-id="771ea-205">In the **Posting picking list** page, you can scroll to see the **Picking list overview**, and the associated **Sales order lines**.</span></span> <span data-ttu-id="771ea-206">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-206">Select **OK**.</span></span> <span data-ttu-id="771ea-207">ستتلقى رسالة تأكيد تفيد أنك على وشك نشر المستند دون طباعته.</span><span class="sxs-lookup"><span data-stu-id="771ea-207">You will receive a confirmation message noting you are about to post the document without printing it.</span></span> 

58. <span data-ttu-id="771ea-208">انقر على **موافق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-208">Click **OK**.</span></span> <span data-ttu-id="771ea-209">لا تطبع.</span><span class="sxs-lookup"><span data-stu-id="771ea-209">Do not print.</span></span> <span data-ttu-id="771ea-210">تم الآن إصدار قائمة الانتقاء ويمكن بدء الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="771ea-210">The picking list has now been issued and picking can commence.</span></span> <span data-ttu-id="771ea-211">يمكن بدء الانتقاء من مناطق متعددة في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="771ea-211">Picking can be started from multiple areas in Supply Chain Management.</span></span> <span data-ttu-id="771ea-212">حتى الآن، قمت بإجراء انتقاء باستخدام أبسط طريقة، من خلال صفحة **أمر المبيعات** مباشرة.</span><span class="sxs-lookup"><span data-stu-id="771ea-212">So far, you have performed picking in the simplest way, which is directly from the **Sales order** page.</span></span>

    > [!NOTE] 
    > <span data-ttu-id="771ea-213">ثمة طريقة بديلة وأكثر تخصيصاً لإصدار البنود للانتقاء وذلك باستخدام **إصدار انتقاء أمر المبيعات**، مما يتيح عرضاً مركزياً وموحداً لطلبات بنود أمر المبيعات التي تنتظر أن يتم إصدارها للانتقاء.</span><span class="sxs-lookup"><span data-stu-id="771ea-213">An alternative and more specialized way to release lines for picking is to use **Release sales order picking**, allowing a centralized and consolidated view on sales order line demands that are waiting to be released to pick.</span></span> <span data-ttu-id="771ea-214">ومن بين الأساليب الأخرى الإصدار في دفعة، وذلك بناء على معايير استعلام محددة.</span><span class="sxs-lookup"><span data-stu-id="771ea-214">Yet another approach would be to release in a batch, depending on specific query criteria.</span></span>

59. <span data-ttu-id="771ea-215">في جزء الإجراءات **أمر المبيعات**، حدد علامة تبويب **التعبئة والتغليف**.</span><span class="sxs-lookup"><span data-stu-id="771ea-215">On the **Sales order** Action Pane, select the **Pick and Pack** tab.</span></span>

60. <span data-ttu-id="771ea-216">في القائمة الفرعية **إنشاء**، حدد **تسجيل قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="771ea-216">In the **Generate** submenu, select **Picking List Registration**.</span></span>

61. <span data-ttu-id="771ea-217">في جزء الإجراء، حدد **التحديثات > تحديث الكل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-217">In the Action Pane, select **Updates > Update All**.</span></span> <span data-ttu-id="771ea-218">ستظهر **حالة المعالجة** تحت علامة التبويب السريعة **التعريف** الآن على أنها **مكتملة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-218">The **Handling status** under the **Identification** FastTab now shows **Completed**.</span></span>

62. <span data-ttu-id="771ea-219">انقر على **حفظ** ثم **أغلق** النافذة.</span><span class="sxs-lookup"><span data-stu-id="771ea-219">Click **Save** and then **Close** the window.</span></span>

63. <span data-ttu-id="771ea-220">في جزء الإجراءات **أمر المبيعات**، حدد علامة تبويب **التعبئة والتغليف**.</span><span class="sxs-lookup"><span data-stu-id="771ea-220">On the **Sales order** Action Pane, select the **Pick and Pack** tab.</span></span>

64. <span data-ttu-id="771ea-221">في القائمة الفرعية **إنشاء**، حدد **نشر إيصال التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-221">In the **Generate** submenu, select **Post Packing Slip**.</span></span>

65. <span data-ttu-id="771ea-222">في صفحة **نشر إيصال التعبئة**، قم بتعيين شريط تبديل **طباعة إيصال التعبئة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-222">On the **Packing slip posting** page, set the **Print packing slip** toggle bar to **Yes**.</span></span>

66. <span data-ttu-id="771ea-223">حدد **موافق** لإنشاء طباعة إلى الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-223">Select **OK** to generate print-to-screen.</span></span> <span data-ttu-id="771ea-224">لقد تم الآن إنشاء إيصال تعبئة وتم شحن البضائع.</span><span class="sxs-lookup"><span data-stu-id="771ea-224">A packing slip has now been generated and goods have been shipped.</span></span> <span data-ttu-id="771ea-225">ستتلقى تحذيراً بأنك تقوم بنشر إيصال التعبئة والطباعة على الشاشة فقط.</span><span class="sxs-lookup"><span data-stu-id="771ea-225">You will receive a warning that you are posting the packing slip and printing to the screen only.</span></span> <span data-ttu-id="771ea-226">انقر على **نعم** للمتابعة.</span><span class="sxs-lookup"><span data-stu-id="771ea-226">Click **Yes** to continue.</span></span>

68. <span data-ttu-id="771ea-227">عند مراجعة التقرير، قم بإغلاق التقرير.</span><span class="sxs-lookup"><span data-stu-id="771ea-227">When you have reviewed the report, close the report.</span></span>

69. <span data-ttu-id="771ea-228">في رأس **أمر المبيعات**، حدد علامة التبويب **الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-228">On the **Sales order** header, select the **Invoice** tab.</span></span>

70. <span data-ttu-id="771ea-229">في القائمة الفرعية **إنشاء**، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-229">In the **Generate** submenu, select **Invoice**.</span></span>

71. <span data-ttu-id="771ea-230">في صفحة **نشر الفاتورة**، قم بتعيين شريط تبديل **طباعة الفاتورة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-230">On the **Posting Invoice** page, set the **Print invoice** toggle bar to **Yes**.</span></span> <span data-ttu-id="771ea-231">يمكنك أيضاً التمرير لأسفل لعرض **نظرة عامة على الفاتورة** بالإضافة إلى **البنود**.</span><span class="sxs-lookup"><span data-stu-id="771ea-231">You can also scroll down to view the **Invoice overview** as well as the **Lines**.</span></span>

72. <span data-ttu-id="771ea-232">حدد **موافق** لإنشاء طباعة إلى الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-232">Select **OK** to generate print-to-screen.</span></span> <span data-ttu-id="771ea-233">لاحظ رقم فاتورة العميل؛ ستحتاج إلى هذا الرقم لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="771ea-233">Note the customer invoice number; you will need this number later.</span></span> <span data-ttu-id="771ea-234">ستتلقى تحذيراً بأنك تقوم بنشر الفاتورة والطباعة على الشاشة فقط.</span><span class="sxs-lookup"><span data-stu-id="771ea-234">You will receive a warning that you are posting the invoice and printing to screen only.</span></span> 

73. <span data-ttu-id="771ea-235">انقر على **نعم.**</span><span class="sxs-lookup"><span data-stu-id="771ea-235">Click **Yes.**</span></span> 

### <a name="create-a-new-payment-journal"></a><span data-ttu-id="771ea-236">قم بإنشاء دفتر يومية مدفوعات جديد.</span><span class="sxs-lookup"><span data-stu-id="771ea-236">Create a new payment journal.</span></span> 

<span data-ttu-id="771ea-237">ثمة المزيد من الطرق لاستلام مدفوعات العميل وتسوية الدفع مقابل واحد أو أكثر من ديون العميل.</span><span class="sxs-lookup"><span data-stu-id="771ea-237">There are more ways to receive a customer payment and settle the payment against one or more customer debits.</span></span> <span data-ttu-id="771ea-238">الأسلوب المختار الموضح هنا هو الأسرع ويقوم بتسجيل الدفع وتسويته في نفس المهمة.</span><span class="sxs-lookup"><span data-stu-id="771ea-238">The chosen method shown here is fast and performs the payment registration and settlement in the same task.</span></span> <span data-ttu-id="771ea-239">مع ذلك، يمكن أولاً استلام دفع العميل ثم تسويته لاحقاً مقابل واحد أو أكثر من ديون العملاء، إذا اقتضت متطلبات الأعمال ذلك.</span><span class="sxs-lookup"><span data-stu-id="771ea-239">However, if business requirements dictate, a customer payment can first be received and then later settled against one or more customer debits.</span></span>

1. <span data-ttu-id="771ea-240">انتقل إلى **الحسابات المدينة > المدفوعات > دفتر يومية المدفوعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-240">Go to **Accounts receivable > Payments > Customer payment journal**.</span></span>

75. <span data-ttu-id="771ea-241">في جزء الإجراءات في أعلى الصفحة، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="771ea-241">In the Action Pane at the top of the page, select **New**.</span></span>

76. <span data-ttu-id="771ea-242">في حقل **الاسم**، أدخِل **CustPay**.</span><span class="sxs-lookup"><span data-stu-id="771ea-242">In the **Name** field, enter **CustPay**.</span></span> <span data-ttu-id="771ea-243">يقوم النظام افتراضياً بتعيين **الوصف** إلى **مدفوعات العميل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-243">The system defaults the **Description** to **Customer payment**.</span></span>

77. <span data-ttu-id="771ea-244">في جزء الإجراءات في الأعلى الشاشة، حدد علامة التبويب **إدخال مدفوعات العميل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-244">In the Action Pane at the top, select the **Enter customer payments" tab**.</span></span>

78. <span data-ttu-id="771ea-245">حدد **العميل** **US-013**.</span><span class="sxs-lookup"><span data-stu-id="771ea-245">Select the **Customer** **US-013**.</span></span>

79. <span data-ttu-id="771ea-246">أدخل مرجع دفع مناسب من اختيارك، مثال: **مدفوعات العميل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-246">Enter an appropriate payment reference of your choice, example: **Customer Payment**.</span></span>

80. <span data-ttu-id="771ea-247">أدخل **مبلغ** الدفع.</span><span class="sxs-lookup"><span data-stu-id="771ea-247">Enter the **Amount** of the payment.</span></span> <span data-ttu-id="771ea-248">مثال: 74092.80 دولار أمريكي.</span><span class="sxs-lookup"><span data-stu-id="771ea-248">Example: $74,092.80.</span></span> <span data-ttu-id="771ea-249">بالنسبة للمرجع، يظهر مبلغ الفاتورة المستحق في أسفل الصفحة، ويتم عرضه ضمن عمود **المبلغ المطلوب دفعه**.</span><span class="sxs-lookup"><span data-stu-id="771ea-249">For reference, the invoice amount that is due appears at the bottom of the page, displayed under the **Amount to pay** column.</span></span> <span data-ttu-id="771ea-250">هذا هو المبلغ الصافي المستحق بعد الخصومات.</span><span class="sxs-lookup"><span data-stu-id="771ea-250">This is the net amount due after discounts.</span></span> <span data-ttu-id="771ea-251">تأكد من أن مبلغ الدفع مساوياً للمبلغ المقيد كمدين للعميل في الفاتورة السابقة.</span><span class="sxs-lookup"><span data-stu-id="771ea-251">Ensure that the amount of payment is equal to the amount debited to the customer for the previous invoice.</span></span> 

81. <span data-ttu-id="771ea-252">حدد **العملة** إذا كانت مختلفة عن الدولار الأمريكي.</span><span class="sxs-lookup"><span data-stu-id="771ea-252">Select the **Currency** if different than USD.</span></span> 

82. <span data-ttu-id="771ea-253">في الشبكة **تحديد للدفع**، حدد الفاتورة التي تم إنشاؤها سابقاً.</span><span class="sxs-lookup"><span data-stu-id="771ea-253">In the **Select to Pay** grid, select the invoice that was previously created.</span></span>

83. <span data-ttu-id="771ea-254">في حقل **المبلغ**، أدخل المبلغ الذي يساوي **المبلغ المتبقي**.</span><span class="sxs-lookup"><span data-stu-id="771ea-254">In the **Amount** field, enter the amount equal to the **Remaining amount**.</span></span> <span data-ttu-id="771ea-255">لاحظ أن حقل **تمت تسويته** يقوم تلقائياً بحساب مبلغ الدفع الذي تم تقديمه.</span><span class="sxs-lookup"><span data-stu-id="771ea-255">Note that the **Settled** field automatically calculates the payment amount being made.</span></span>

84. <span data-ttu-id="771ea-256">تحقق من عدم وجود أي مبلغ **متبقي** للتسوية الناتجة عن الدفع.</span><span class="sxs-lookup"><span data-stu-id="771ea-256">Check that there is no **Remaining** amount for settlement that has resulted from the payment.</span></span>

85. <span data-ttu-id="771ea-257">حدد **حفظ في دفتر اليومية** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="771ea-257">Select **Save in Journal** in the Action Pane.</span></span>

86. <span data-ttu-id="771ea-258">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-258">Select **Close**.</span></span> <span data-ttu-id="771ea-259">لقد قمت الآن بتسجيل دفع العميل واستلمته وقمت بتسويته مقابل فاتورة العميل.</span><span class="sxs-lookup"><span data-stu-id="771ea-259">You have now recorded the customer payment and have received and settled it against the customer invoice.</span></span> <span data-ttu-id="771ea-260">ومع ذلك، لم يتم ترحيله في دفتر الأستاذ بعد.</span><span class="sxs-lookup"><span data-stu-id="771ea-260">However, it has not been posted in the ledger yet.</span></span>

87. <span data-ttu-id="771ea-261">في صفحة **دفتر يومية مدفوعات العميل**، انقر لتحديد **رقم مجموعة دفتر اليومية** الخاص بدفتر يومية المدفوعات الذي قمت بإنشائه لتوك.</span><span class="sxs-lookup"><span data-stu-id="771ea-261">In the **Customer payment journal** page, click to select the **Journal batch number** for the payment journal that you just created.</span></span> <span data-ttu-id="771ea-262">ستظهر علامة اختيار بجوار دفتر يومية المدفوعات.</span><span class="sxs-lookup"><span data-stu-id="771ea-262">A check mark will appear next to the payment journal.</span></span>

88. <span data-ttu-id="771ea-263">حدد **ترحيل** ثم حدد خيار **الترحيل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-263">Select **Post** and then select the **Post** option.</span></span> <span data-ttu-id="771ea-264">في صفحة **دفتر يومية المدفوعات للعميل**، ضمن عمود **تاريخ الترحيل**، سيظهر تاريخ ووقت ترحيل عملية الدفع.</span><span class="sxs-lookup"><span data-stu-id="771ea-264">On the **Customer payment journal** page, under the **Posted on** column, you will see the date and time the payment was posted.</span></span>

89. <span data-ttu-id="771ea-265">إذا ظهر سجل المعلومات، فحدد لإغلاقه.</span><span class="sxs-lookup"><span data-stu-id="771ea-265">If the Infolog appears, select to close it.</span></span>

90. <span data-ttu-id="771ea-266">في الصفحة، حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-266">On the page, select **Close**.</span></span>

## <a name="scenario---sales-order-entry-to-cash-process---with-variances"></a><span data-ttu-id="771ea-267">السيناريو - إدخال أمر المبيعات لعملية نقدية - مع تباينات</span><span class="sxs-lookup"><span data-stu-id="771ea-267">Scenario - Sales order entry to cash process - with variances</span></span> 

<span data-ttu-id="771ea-268">في هذا السيناريو، يطلب العميل (تاجر جملة) تزويد صنفي بنود.</span><span class="sxs-lookup"><span data-stu-id="771ea-268">In this scenario, the customer (a wholesaler) orders replenishment of two line items.</span></span> <span data-ttu-id="771ea-269">ومع ذلك، لا يكون المخزون كافياً لأحد أصناف البند، ويجب أن يقوم معالج الأمر بتشغيل توريد لهذا الطلب الخاص.</span><span class="sxs-lookup"><span data-stu-id="771ea-269">However, stock is insufficient on one of the line items, and the Order processor must trigger supply for this specific demand.</span></span> <span data-ttu-id="771ea-270">يمكن اعتبار هذا السيناريو انحرافاً عن السيناريو السابق وهو أكثر تعقيداً قليلاً.</span><span class="sxs-lookup"><span data-stu-id="771ea-270">This scenario can be considered a deviation of the previous scenario and is slightly more complex.</span></span>

1.  <span data-ttu-id="771ea-271">انتقل إلى **المبيعات والتسويق > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="771ea-271">Go to **Sales and marketing > Customers > All customers**.</span></span>

2.  <span data-ttu-id="771ea-272">في صفحه القائمة، حدد العميل **US-027**.</span><span class="sxs-lookup"><span data-stu-id="771ea-272">On the list page, select customer **US-027**.</span></span>

3.  <span data-ttu-id="771ea-273">في علامة التبويب **البيع**، تحت القائمة الفرعية **جديد**، حدد **أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-273">On the **Sell** tab, under the **New** submenu, select **Sales order**.</span></span>

4.  <span data-ttu-id="771ea-274">في صفحة **تفاصيل أمر المبيعات**، قم بتوسيع علامة التبويب السريعة **تفاصيل البند**.</span><span class="sxs-lookup"><span data-stu-id="771ea-274">On the **Sales order details** page, expand the **Line details** FastTab.</span></span>

5.  <span data-ttu-id="771ea-275">حدد علامة التبويب **التسليم**. تكون القيمة الافتراضية لـ **تاريخ الشحن المطلوب** وتواريخ الاستلام هي اليوم، والتي يتم افتراضها من رأس الأمر.</span><span class="sxs-lookup"><span data-stu-id="771ea-275">Select the **Delivery** tab. The **Requested ship date** and receipt dates default to today, which is defaulted from the order header.</span></span> <span data-ttu-id="771ea-276">نظراً لعدم تحديد موقع شحن حالياً، يكون **تاريخ الشحن المطلوب** و **تاريخ الاستلام المطلوب** في موقع العميل هو نفسه (لذا لا يوجد وقت شحن).</span><span class="sxs-lookup"><span data-stu-id="771ea-276">Because a shipping location is not defined currently, the **Requested ship date** and **Requested receipt date** at the customer location are the same (so no transport time).</span></span>
<span data-ttu-id="771ea-277">يريد العميل 10 أجهزة تليفزيون جهاز عرض، و8 مستقبلات صوت، و10 كبلات قياس كل واحد منها 10 أمتار، و4 كابلات قياس كل واحد منها 4 أمتار.</span><span class="sxs-lookup"><span data-stu-id="771ea-277">The customer wants 10 projector televisions, 8 sound receivers, 10 cables that measure 10 meters each, and 4 cables that measure 2 meters each.</span></span>

6.  <span data-ttu-id="771ea-278">في علامة التبويب السريعة **بنود أمر المبيعات**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="771ea-278">In the **Sales order lines** FastTab, select **Add line.**</span></span>
 
8.  <span data-ttu-id="771ea-279">في الحقل **رقم الصنف**، أدخل وحدد **T0002**.</span><span class="sxs-lookup"><span data-stu-id="771ea-279">In the **Item number** field, enter and select **T0002**.</span></span>

9.  <span data-ttu-id="771ea-280">في حقل **الكمية**، أدخِل **10**.</span><span class="sxs-lookup"><span data-stu-id="771ea-280">In the **Quantity** field, enter **10**.</span></span> <span data-ttu-id="771ea-281">في علامة التبويب السريعة **تفاصيل البند**، ضمن علامة تبويب **التسليم**، لاحظ تاريخ الاستلام المطلوب عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="771ea-281">In the **Line details** FastTab, under the **Delivery** tab, observe the requested receipt date online.</span></span> <span data-ttu-id="771ea-282">تم عرض هذا التاريخ بعدد الأيام من تاريخ الشحن المطلوب، لذلك سيتعين عليك الاستقصاء.</span><span class="sxs-lookup"><span data-stu-id="771ea-282">This date has been projected in the number of days from the requested ship date, so you will need to investigate.</span></span>

10.  <span data-ttu-id="771ea-283">حدد ارتباط **محاكاة تاريخ التسليم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-283">Select the **Simulate delivery date** link.</span></span>

11.  <span data-ttu-id="771ea-284">في **محاكاة تاريخ التسليم**، لاحظ **أيام النقل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-284">In the **Delivery date simulation**, observe the **Transport days**.</span></span> <span data-ttu-id="771ea-285">لاحظ أنه يمكنك شحن البضائع اليوم وأن العميل سيستلم صنف البند خلال عدد الأيام المشار إليها من اليوم.</span><span class="sxs-lookup"><span data-stu-id="771ea-285">Notice that you can ship the goods today and that the customer will receive the line item in the number of days noted from today.</span></span> <span data-ttu-id="771ea-286">على سبيل المثال: إذا كان حقل **أيام النقل** يعرض 3 أيام، فسوف يتلقى العميل البضائع بعد ثلاثة أيام.</span><span class="sxs-lookup"><span data-stu-id="771ea-286">Example: If the **Transport days** field shows 3 days, the customer will receive the goods in three days.</span></span>

12. <span data-ttu-id="771ea-287">حدد **إلغاء الأمر** للخروج من الصفحة.</span><span class="sxs-lookup"><span data-stu-id="771ea-287">Select **Cancel** to exit the page.</span></span> <span data-ttu-id="771ea-288">لن تقوم بتأكيد التواريخ لكل بند؛ بدلاً من ذلك، ستقوم بتأكيد التواريخ عبر كافة البنود فيما بعد حتى يمكنك ضمان انسجام تاريخ الشحن للحصول على التسليم الكامل.</span><span class="sxs-lookup"><span data-stu-id="771ea-288">You will not confirm dates on a line-by-line basis; instead, you will confirm dates across all lines later so that you can ensure ship date alignment for complete delivery.</span></span>

13. <span data-ttu-id="771ea-289">في علامة التبويب السريعة **بنود أمر المبيعات**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="771ea-289">In the **Sales order lines** FastTab, select **Add line**.</span></span>

14. <span data-ttu-id="771ea-290">في الحقل **رقم الصنف**، أدخل وحدد **T0001**.</span><span class="sxs-lookup"><span data-stu-id="771ea-290">In the **Item number** field, enter and select **T0001**.</span></span>

15. <span data-ttu-id="771ea-291">في حقل **الكمية**، أدخِل **8**.</span><span class="sxs-lookup"><span data-stu-id="771ea-291">In the **Quantity** field, enter **8**.</span></span>

16. <span data-ttu-id="771ea-292">في علامة التبويب السريعة **تفاصيل البند**، حدد علامة التبويب **المنتج**.</span><span class="sxs-lookup"><span data-stu-id="771ea-292">In the **Line details** FastTab, select the **Product** tab.</span></span>

17. <span data-ttu-id="771ea-293">في القائمة المنسدلة **الحجم**، حدد **10**.</span><span class="sxs-lookup"><span data-stu-id="771ea-293">In the **Size** drop-down menu, select **10**.</span></span>

18. <span data-ttu-id="771ea-294">في شبكة **بنود أمر المبيعات**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="771ea-294">In the **Sales order lines** grid, select **Add line**.</span></span>

19. <span data-ttu-id="771ea-295">في حقل **رقم البند**، أدخِل **T0003**.</span><span class="sxs-lookup"><span data-stu-id="771ea-295">In the **Item number** field, enter **T0003**.</span></span>

20. <span data-ttu-id="771ea-296">في حقل **الكمية**، أدخِل **16**.</span><span class="sxs-lookup"><span data-stu-id="771ea-296">In the **Quantity** field, enter **16**.</span></span>

    <span data-ttu-id="771ea-297">تبعاً لبياناتك، عند إدخال صنف البند **T0003**، ربما تلاحظ أن **تاريخ الشحن المطلوب** الذي تم تعيينه بواسطة حساب **متوفر حسب التعهد (ATP)** يقع في المستقبل قليلا.</span><span class="sxs-lookup"><span data-stu-id="771ea-297">Depending on your data, when you entered the **T0003** line item, you might have noticed that the **Requested ship date** that was set by the **Available to Promise (ATP)** calculation was slightly into the future.</span></span> <span data-ttu-id="771ea-298">والسبب في ذلك أنه قد يكون لديك بالفعل الكثير من الطلب الموزع على الوقت للتوريد المرتقب الموزع الوقت والتوريد لفترة قصيرة.</span><span class="sxs-lookup"><span data-stu-id="771ea-298">The reason is because you might already have too much time-phased demand for your projected and time-phased supply and shorter-term supply.</span></span>

21. <span data-ttu-id="771ea-299">في أثناء وضع المؤشر على صنف البند **T0003**، وفي علامة التبويب السريعة **بنود أمر المبيعات**، حدد **المنتج والتوريد > معلومات ATP**.</span><span class="sxs-lookup"><span data-stu-id="771ea-299">With the cursor still positioned on line item **T0003**, on the **Sales order lines** FastTab, select **Product and supply > ATP information**.</span></span>

22. <span data-ttu-id="771ea-300">انتقل إلى جدول **كمية ATP**.</span><span class="sxs-lookup"><span data-stu-id="771ea-300">Go to the **ATP quantity** table.</span></span>

23. <span data-ttu-id="771ea-301">قم بالتمرير إلى السطر الأول الذي لا يحتوي على علامة تعجب.</span><span class="sxs-lookup"><span data-stu-id="771ea-301">Scroll to the first line that does not have an exclamation mark.</span></span>
<span data-ttu-id="771ea-302">هذه النقطة من الوقت هي التي تتواجد فيها، واستنادا إلى الإيصالات الحالية المتوقعة والإصدارات والكميات الفعلية المرتقبة، يمكن التعهد بشحن كمية مقدارها 16.</span><span class="sxs-lookup"><span data-stu-id="771ea-302">This point in time is where you, based on current expected receipts, issues, and projected on-hand, can promise a shipment of a quantity of 16.</span></span>

24. <span data-ttu-id="771ea-303">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-303">Select **Close**.</span></span> <span data-ttu-id="771ea-304">يكون الهدف هو التأكد من أن كافة أصناف البند منسجمة مع صنف البند الذي يقع في تاريخ الشحن الأبعد في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="771ea-304">The objective is to ensure that all line items align with the line item that has the ship date farthest in the future.</span></span> <span data-ttu-id="771ea-305">وهذا يساعد في ضمان الشحن الكامل وبدون تسليم جزئي.</span><span class="sxs-lookup"><span data-stu-id="771ea-305">This helps to ensure complete shipment and no partial delivery.</span></span> <span data-ttu-id="771ea-306">النتيجة هو أن كل البنود ستكون بنفس تاريخ الشحن والاستلام المؤكد، وسيتم تلقائياً تحديث تاريخ الشحن والاستلام المؤكد لرأس أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="771ea-306">Output is that all lines will get the same confirmed ship and receipt date, and the sales order header will have the confirmed ship and receipt date auto updated.</span></span>

25. <span data-ttu-id="771ea-307">في رأس **أمر المبيعات**،  حدد علامة التبويب **البيع**.</span><span class="sxs-lookup"><span data-stu-id="771ea-307">On the **Sales order** header, select the **Sell** tab.</span></span>

27. <span data-ttu-id="771ea-308">في رأس **أمر المبيعات**، في المجموعة **إنشاء**، حدد **تأكيد أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-308">On the **Sales order** header, in the **Generate** group, select **Confirm sales order**.</span></span>

28. <span data-ttu-id="771ea-309">في مربع الحوار **تأكيد أمر المبيعات**، قم بتعيين شريط التبديل **تأكيد الطباعة** إلى **نعم**، ثم حدد **موافق** لإنشاء طباعة على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-309">In the **Confirm sales order** dialog, set the **Print confirmation** toggle bar to **Yes**, and then select **OK** to generate print-to-screen.</span></span>

28. <span data-ttu-id="771ea-310">ستتلقى تحذيراً بأنك تقوم بنشر التأكيد والطباعة على الشاشة فقط.</span><span class="sxs-lookup"><span data-stu-id="771ea-310">You will receive a warning that you are posting the confirmation and printing to screen only.</span></span> <span data-ttu-id="771ea-311">انقر على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-311">Click **Yes**.</span></span>

29. <span data-ttu-id="771ea-312">قم بمراجعة التقرير ثم إغلاقه.</span><span class="sxs-lookup"><span data-stu-id="771ea-312">Review and then close the report.</span></span>

30. <span data-ttu-id="771ea-313">في رأس **أمر المبيعات**، حدد علامة تبويب **التعبئة والتغليف**.</span><span class="sxs-lookup"><span data-stu-id="771ea-313">On **Sales order** header, select the **Pick and Pack** tab.</span></span>

31. <span data-ttu-id="771ea-314">في المجموعة **إنشاء**، حدد **إنشاء قائمة انتقاء**.</span><span class="sxs-lookup"><span data-stu-id="771ea-314">In the **Generate** group, select **Generate Picking List**.</span></span>

32. <span data-ttu-id="771ea-315">في صفحة **نشر قائمة الانتقاء**، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-315">On the **Posting picking List** page, select **OK**.</span></span>

33. <span data-ttu-id="771ea-316">في رأس **أمر المبيعات**، حدد علامة تبويب **التعبئة والتغليف**.</span><span class="sxs-lookup"><span data-stu-id="771ea-316">On the **Sales order** header, select the **Pick and Pack** tab.</span></span>

34. <span data-ttu-id="771ea-317">في المجموعة **إنشاء**، حدد **تسجيل قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="771ea-317">In the **Generate** group, select **Picking List Registration**.</span></span>

35. <span data-ttu-id="771ea-318">اختر **التحديثات**، ثم اختر **تحديث الكل**.</span><span class="sxs-lookup"><span data-stu-id="771ea-318">Select **Updates** and then select **Update All**.</span></span>

36. <span data-ttu-id="771ea-319">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-319">Select **Close**.</span></span>

37. <span data-ttu-id="771ea-320">في جزء الإجراءات **أمر المبيعات**، حدد علامة تبويب **التعبئة والتغليف**.</span><span class="sxs-lookup"><span data-stu-id="771ea-320">On the **Sales order** Action Pane, select the **Pick and Pack** tab.</span></span>

38. <span data-ttu-id="771ea-321">في المجموعة **إنشاء**، حدد **نشر إيصال التعبئة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-321">In the **Generate** group, select the **Post Packing Slip** action.</span></span>

39. <span data-ttu-id="771ea-322">في صفحة **إيصال التعبئة**، قم بتعيين شريط التبديل لتحديد **طباعة إيصال التعبئة** إلى **نعم** ثم حدد **موافق** لإنشاء طباعة على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-322">In the **Packing slip** page, set the **Print packing slip** select the toggle bar to **Yes** and then select **OK** to generate print-to-screen.</span></span>

40. <span data-ttu-id="771ea-323">ستتلقى تحذيراً يبلغك بأنك تقوم بنشر إيصال التعبئة والطباعة على الشاشة فقط.</span><span class="sxs-lookup"><span data-stu-id="771ea-323">You will receive a warning communicating you are posting the packing slip and printing to screen only.</span></span> <span data-ttu-id="771ea-324">انقر على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-324">Click **Yes**.</span></span> <span data-ttu-id="771ea-325">لاحظ أن **حالة أمر المبيعات** تعرض الآن **مستلم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-325">Note the **Sales order status** now shows as **Delivered**.</span></span>

41. <span data-ttu-id="771ea-326">في جزء إجراءات **أمر المبيعات**، حدد علامة تبويب **الفاتورة**. وفي القائمة الفرعية **إنشاء**، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="771ea-326">On the **Sales order** Action Pane, select the **Invoice** tab. In the **Generate** submenu, select **Invoice**.</span></span>

41. <span data-ttu-id="771ea-327">في صفحة **ترحيل الفاتورة**، قم بتعيين شريط التبديل **طباعة الفاتورة** إلى **نعم** ثم حدد **موافق** لإنشاء طباعة على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="771ea-327">On the **Posting invoice** page, set the **Print invoice** toggle bar to **Yes** and then select **OK** to generate print-to-screen.</span></span>

42. <span data-ttu-id="771ea-328">ستتلقى تحذيراً يفيد بأنك تقوم بنشر الفاتورة والطباعة على الشاشة فقط.</span><span class="sxs-lookup"><span data-stu-id="771ea-328">You will receive a warning stating you are posting the invoice and printing to screen only.</span></span> <span data-ttu-id="771ea-329">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="771ea-329">Select **Yes**.</span></span>

42. <span data-ttu-id="771ea-330">قم بمراجعة التقرير ثم إغلاقه.</span><span class="sxs-lookup"><span data-stu-id="771ea-330">Review and then close the report.</span></span> <span data-ttu-id="771ea-331">قم بتدوير رقم فاتورة العميل لأنك ستحتاج إلى هذا الرقم لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="771ea-331">Note down the Customer invoice number as you will need this number later.</span></span>

43. <span data-ttu-id="771ea-332">انتقل إلى **اللحسابات المدينة > دفاتر اليومية > المدفوعات > دفتر يومية المدفوعات**.</span><span class="sxs-lookup"><span data-stu-id="771ea-332">Go to **Accounts receivables > Journals > Payments > Payment Journal**.</span></span>

44. <span data-ttu-id="771ea-333">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="771ea-333">Select **New** in the Action Pane.</span></span>

45. <span data-ttu-id="771ea-334">في حقل **الاسم**، أدخل **CustPay** ثم اضغط خارج الحقل.</span><span class="sxs-lookup"><span data-stu-id="771ea-334">In the **Name** field, enter **CustPay** and then tab off the field.</span></span>

46. <span data-ttu-id="771ea-335">مع الاستمرار في تحديد دفتر اليومية الجديد، حدد **إدخال مدفوعات العميل** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="771ea-335">With the new journal still selected, select **Enter Customer Payments** in the Action Pane.</span></span>

47. <span data-ttu-id="771ea-336">حدد العميل **US-027**.</span><span class="sxs-lookup"><span data-stu-id="771ea-336">Select customer **US-027**.</span></span>

48. <span data-ttu-id="771ea-337">تأكد من أن مبلغ الدفع مساوياً للمبلغ المقيد كمدين للعميل في الفاتورة السابقة.</span><span class="sxs-lookup"><span data-stu-id="771ea-337">Make sure that the amount of payment is equal to the amount debited to the customer for the previous invoice.</span></span>

48. <span data-ttu-id="771ea-338">في الشبكة **تحديد للدفع**، حدد الفاتورة التي تم إنشاؤها سابقاً.</span><span class="sxs-lookup"><span data-stu-id="771ea-338">In the **Select to Pay** grid, select the invoice that was previously created.</span></span>

49. <span data-ttu-id="771ea-339">في حقل **المبلغ**، أدخل المبلغ الذي يساوي **المبلغ المتبقي**.</span><span class="sxs-lookup"><span data-stu-id="771ea-339">In the **Amount** field, enter the amount equal to the **Remaining Amount**.</span></span>

50. <span data-ttu-id="771ea-340">تحقق من عدم وجود أي مبلغ متبقي للتسوية الناتجة عن الدفع.</span><span class="sxs-lookup"><span data-stu-id="771ea-340">Check that there is no remaining amount for settlement that has resulted from the payment.</span></span>

51. <span data-ttu-id="771ea-341">حدد **حفظ في دفتر اليومية** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="771ea-341">Select **Save in Journal** in the Action Pane.</span></span>

52. <span data-ttu-id="771ea-342">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-342">Select **Close**.</span></span>

53. <span data-ttu-id="771ea-343">حدد **رقم مجموعو دفتر اليومية** الذي قمت بإنشائه، ثم حدد **ترحيل**، ثم حدد خيار **النشر**.</span><span class="sxs-lookup"><span data-stu-id="771ea-343">Select the **Journal batch number** that you created, select **Post**, and then select the **Post** option.</span></span> <span data-ttu-id="771ea-344">يمكنك الآن رؤية أن **تاريخ النشر** يعرض التاريخ والوقت الذي تم فيه ترحيل دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="771ea-344">You can now see the **Posted on** date displays the date and time the journal was posted.</span></span>

54. <span data-ttu-id="771ea-345">إذا ظهر سجل المعلومات، فأغلقه.</span><span class="sxs-lookup"><span data-stu-id="771ea-345">If the Infolog appears, close it.</span></span>

55. <span data-ttu-id="771ea-346">في الصفحة، حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="771ea-346">In the page, select **Close**.</span></span>

