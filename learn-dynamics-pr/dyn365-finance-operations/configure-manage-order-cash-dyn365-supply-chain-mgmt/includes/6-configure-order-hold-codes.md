---
ms.openlocfilehash: 5032605b1fbe287cb94aaeb690ec6d1465b777ce
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073223"
---
<span data-ttu-id="55cac-101">أثناء إدخال الأمر، ولكن قبل إرسال الطلب وتأكيده، قد يرغب البائعون في تعليق أمر يدوياً لمنع إصداره إلى المستودع لمزيد من المعالجة.</span><span class="sxs-lookup"><span data-stu-id="55cac-101">During order entry, but before order submission and confirmation, salespersons might want to manually put an order on hold to prevent it from being released to the warehouse for further processing.</span></span> <span data-ttu-id="55cac-102">على سبيل المثال، قد لا يكون العميل الذي يقدم الطلب جاهزاً للالتزام به، أو قد تكون البيانات المهمة المطلوبة لمعالجة الأمر مفقودة.</span><span class="sxs-lookup"><span data-stu-id="55cac-102">For example, the customer who is placing the order might not be ready to commit to it, or critical data that is required to process the order might be missing.</span></span> 

<span data-ttu-id="55cac-103">عندما يكون الطلب معلقاً، لا يمكن للمستودع معالجته للشحن.</span><span class="sxs-lookup"><span data-stu-id="55cac-103">While the order is on hold, it cannot be processed by the warehouse for shipping.</span></span>

<span data-ttu-id="55cac-104">من خلال تعليق عرض أسعار أو أمر مبيعات، يمكنك إيقاف الأمر أو الإرجاع أو بند الأمر أو بند الإرجاع.</span><span class="sxs-lookup"><span data-stu-id="55cac-104">By placing a quotation or sales order on hold, you can stop an order, return, order line, or return line.</span></span> <span data-ttu-id="55cac-105">يمكنك تطبيق عمليات تعليق الطلبات يدوياً أو تلقائياً بناءً على مجموعة من المعايير التي تحددها، مثل فحص ائتمان العميل.</span><span class="sxs-lookup"><span data-stu-id="55cac-105">You can apply order holds manually or automatically based on a set of criteria that you define, like a customer credit check.</span></span>

<span data-ttu-id="55cac-106">يمكنك تحديد العديد من الحجوزات المختلفة حسب حاجتك لإدارة أعمالك.</span><span class="sxs-lookup"><span data-stu-id="55cac-106">You can define as many different holds as you need to manage your business.</span></span> <span data-ttu-id="55cac-107">يمكن أن تكون الطلبات المعلقة قابلة للتطبيق في خطوات محددة في دورة حياة أمرك أو يتم تطبيقها على عميل أو صنف بغض النظر عن مكان الأوامر في دورة الأوامر الحالية، مع استثناء واحد.</span><span class="sxs-lookup"><span data-stu-id="55cac-107">The order holds can be applicable at specific steps in your order's life cycle or applied to a customer or item no matter where the orders are in the current order cycle, with one exception.</span></span> <span data-ttu-id="55cac-108">لا يمكنك تطبيق تعليق إذا تم إصدار أمرك للانتقاء.</span><span class="sxs-lookup"><span data-stu-id="55cac-108">You cannot apply a hold if your order has been pick released.</span></span>

<span data-ttu-id="55cac-109">شاهد هذا الفيديو لترى العميل يعلق العمليات في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="55cac-109">Watch this video to see the customer holds processes in Supply Chain Management.</span></span> 

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3ZqRY]


<span data-ttu-id="55cac-110">توضح الإجراءات التالية كيفية تعليق أوامر مبيعات العملاء، وكيفية التعامل مع عمليات تسجيل الخروج من تعليقات الأوامر، وكيفية إزالة الأوامر المعلقة.</span><span class="sxs-lookup"><span data-stu-id="55cac-110">The following procedures show how to place customer sales orders on hold, how to work with order hold checkouts, and how to remove order holds.</span></span>

<span data-ttu-id="55cac-111">يمكنك تشغيل هذا الإجراء في شركة بيانات العرض التوضيحي USMF في Supply Chain Management، أو يمكنك تشغيل الإجراء على بياناتك الخاصة.</span><span class="sxs-lookup"><span data-stu-id="55cac-111">You can run this procedure in the demo data company USMF in Supply Chain Management, or you can run the procedure on your own data.</span></span>

## <a name="set-up-order-holds"></a><span data-ttu-id="55cac-112">إعداد الأوامر المعلقة</span><span class="sxs-lookup"><span data-stu-id="55cac-112">Set up order holds</span></span>
<span data-ttu-id="55cac-113">لإعداد الأوامر المعلقة، اتبع هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="55cac-113">To set up order holds, follow these steps.</span></span>

1.  <span data-ttu-id="55cac-114">انتقل إلى **المبيعات والتسويق > الإعداد > أوامر المبيعات > رموز تعليق الأوامر**.</span><span class="sxs-lookup"><span data-stu-id="55cac-114">Go to **Sales and marketing > Setup > Sales orders > Order hold codes**.</span></span>

2.  <span data-ttu-id="55cac-115">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="55cac-115">Select **New**.</span></span>

3.  <span data-ttu-id="55cac-116">في حقل **رمز التعليق**، أدخل **رد الاتصال**.</span><span class="sxs-lookup"><span data-stu-id="55cac-116">In the **Hold code** field, enter **Call back**.</span></span>

4.  <span data-ttu-id="55cac-117">في حقل **الوصف**، أدخل **تم تعليق الأمر في انتظار رد اتصال العميل**.</span><span class="sxs-lookup"><span data-stu-id="55cac-117">In the **Description** field, enter **Order held waiting for customer callback**.</span></span>

5.  <span data-ttu-id="55cac-118">بشكل اختياري، حدد مربع الاختيار **إزالة حجوزات المخزون** لإزالة أي حجوزات فعلية من الأمر عند إضافة رمز التعليق هذا.</span><span class="sxs-lookup"><span data-stu-id="55cac-118">Optionally, select the **Remove inventory reservations** check box to remove any physical reservations from the order when this hold code is added.</span></span>

6.  <span data-ttu-id="55cac-119">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="55cac-119">Select **Save**.</span></span>

## <a name="place-an-order-on-hold"></a><span data-ttu-id="55cac-120">تعليق أمر</span><span class="sxs-lookup"><span data-stu-id="55cac-120">Place an order on hold</span></span>
<span data-ttu-id="55cac-121">لتعليق أمر، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="55cac-121">To place an order on hold, follow these steps.</span></span>

1.  <span data-ttu-id="55cac-122">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="55cac-122">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>

2.  <span data-ttu-id="55cac-123">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="55cac-123">Select **New**.</span></span>

3.  <span data-ttu-id="55cac-124">في الحقل **حساب العميل**، أدخل أو حدد **US-013**.</span><span class="sxs-lookup"><span data-stu-id="55cac-124">In the **Customer account** field, enter or select **US-013**.</span></span>

4.  <span data-ttu-id="55cac-125">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="55cac-125">Select **OK**.</span></span>

5.  <span data-ttu-id="55cac-126">في الحقل **رقم الصنف**، أدخل أو حدد **D0001**.</span><span class="sxs-lookup"><span data-stu-id="55cac-126">In the **Item number** field, enter or select **D0001**.</span></span>

6.  <span data-ttu-id="55cac-127">في حقل **الكمية**، أدخِل **1**.</span><span class="sxs-lookup"><span data-stu-id="55cac-127">In the **Quantity** field, enter **1**.</span></span>

7.  <span data-ttu-id="55cac-128">في جزء الإجراء، حدد **أمر مبيعات**.</span><span class="sxs-lookup"><span data-stu-id="55cac-128">On the Action Pane, select **Sales order**.</span></span>

8.  <span data-ttu-id="55cac-129">حدد **عمليات تعليق الأوامر**.</span><span class="sxs-lookup"><span data-stu-id="55cac-129">Select **Order holds**.</span></span>

9.  <span data-ttu-id="55cac-130">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="55cac-130">Select **New**.</span></span>

10. <span data-ttu-id="55cac-131">في حقل **رمز التعليق**، حدد **رد الاتصال**.</span><span class="sxs-lookup"><span data-stu-id="55cac-131">In the **Hold code** field, select **Call back**.</span></span>

11. <span data-ttu-id="55cac-132">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="55cac-132">Select **Save**.</span></span>

12. <span data-ttu-id="55cac-133">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="55cac-133">Close the page.</span></span>

13. <span data-ttu-id="55cac-134">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="55cac-134">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>

14. <span data-ttu-id="55cac-135">في القائمة، اعرض الطلبات المعلقة حالياً وتم تحديد حقلي **عدم المعالجة** و **التعليق** لها.</span><span class="sxs-lookup"><span data-stu-id="55cac-135">In the list, view the orders that are currently on hold and have the **Do not process** and **Hold** fields selected.</span></span>

15. <span data-ttu-id="55cac-136">في القائمة، حدد أمر المبيعات الذي قمت بإنشائه في الخطوات من 1 إلى 6.</span><span class="sxs-lookup"><span data-stu-id="55cac-136">In the list, select the sales order that you created in steps 1 to 6.</span></span>

## <a name="manage-order-holds"></a><span data-ttu-id="55cac-137">إدارة عمليات تعليق الأمر</span><span class="sxs-lookup"><span data-stu-id="55cac-137">Manage order holds</span></span>
<span data-ttu-id="55cac-138">لإدارة تعليق أمر، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="55cac-138">To manage an order hold, follow these steps.</span></span>

1.  <span data-ttu-id="55cac-139">في جزء الإجراء، حدد علامة التبويب **تسجيل الخروج من التعليق**.</span><span class="sxs-lookup"><span data-stu-id="55cac-139">On the Action Pane, select **Hold checkout**.</span></span>

2.  <span data-ttu-id="55cac-140">حدد **تسجيل الخروج**. يعرض حقل **تسجيل الخروج إلى** الآن معرف المستخدم الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="55cac-140">Select **Check out**. The **Checkout to** field now shows your user ID.</span></span>

3.  <span data-ttu-id="55cac-141">حدد **مسح تسجيل الخروج**.</span><span class="sxs-lookup"><span data-stu-id="55cac-141">Select **Clear checkout**.</span></span>

4.  <span data-ttu-id="55cac-142">في جزء الإجراء، حدد **مسح التعليق**.</span><span class="sxs-lookup"><span data-stu-id="55cac-142">On the Action Pane, select **Clear hold**.</span></span>

<span data-ttu-id="55cac-143">عندما تكون مستعداً لإزالة التعليق والسماح للأمر بالمتابعة إلى خطوة التنفيذ التالية، يجب عليك مسح التعليق.</span><span class="sxs-lookup"><span data-stu-id="55cac-143">When you are ready to remove the hold and allow the order to proceed to the next fulfillment step, you must clear the hold.</span></span> <span data-ttu-id="55cac-144">إذا لم يتطلب الأمر أي تغييرات، فيمكنك تشغيل إجراء **مسح التعليقات**.</span><span class="sxs-lookup"><span data-stu-id="55cac-144">If the order requires no changes, then you can run the **Clear holds** action.</span></span> <span data-ttu-id="55cac-145">ومع ذلك، يمكنك استخدام إجراء **المسح والتعديل** إذا كان عند مسح التعليق يجب تحديث الأمر.</span><span class="sxs-lookup"><span data-stu-id="55cac-145">However, you can use the **Clear and modify** action if, when clearing a hold, the order must be updated.</span></span>

<span data-ttu-id="55cac-146">ينطبق إجراء **المسح والإرسال** فقط عند استخدام وظيفة مركز الاتصال.</span><span class="sxs-lookup"><span data-stu-id="55cac-146">The **Clear and submit** action is only applicable when you use Call center functionality.</span></span>

<span data-ttu-id="55cac-147">تم الآن مسح التعليق من الأمر وإزالته من قائمة التعليقات **النشطة**.</span><span class="sxs-lookup"><span data-stu-id="55cac-147">The hold has now been cleared from the order and removed from the list of **Active** holds.</span></span> <span data-ttu-id="55cac-148">لمشاهدة كل التعليقات أو مجموعاتها الفرعية وفقاً لحالة معينة، قم بتغيير القيمة في الحقل **إظهار**.</span><span class="sxs-lookup"><span data-stu-id="55cac-148">To see all the holds or their subset according to a specific status, change the value in the **Show** field.</span></span>


