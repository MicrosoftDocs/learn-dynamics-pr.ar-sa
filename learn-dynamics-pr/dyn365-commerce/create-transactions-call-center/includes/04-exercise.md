---
ms.openlocfilehash: 3d95a3905b4be7bb8430c7c8dcf8ccd460678778
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070339"
---
<span data-ttu-id="e2101-101">لهذا التمرين، ننصحك باستخدام بيانات العرض التوضيحي في الشركة **USRT**.</span><span class="sxs-lookup"><span data-stu-id="e2101-101">For this exercise, we recommend that you use the demo data in the **USRT** company.</span></span>

## <a name="scenario---create-a-call-center-order"></a><span data-ttu-id="e2101-102">السيناريو ـ إنشاء أمر مركز الاتصال</span><span class="sxs-lookup"><span data-stu-id="e2101-102">Scenario - Create a call center order</span></span>
<span data-ttu-id="e2101-103">أنت موظف في مركز الاتصال وتتلقى مكالمة من عميل دوري، **Karen Berg**، الذي يرغب في شراء صنف **0005** عبر الهاتف وتسليمه عبر الشحن القياسي.</span><span class="sxs-lookup"><span data-stu-id="e2101-103">You are a call center associate and are taking a call from a regular customer, **Karen Berg**, who wants to purchase item **0005** over the phone and have it delivered with a standard shipment.</span></span> <span data-ttu-id="e2101-104">لهذا التمرين، سوف تستخدم طريقة الدفع **شيك**.</span><span class="sxs-lookup"><span data-stu-id="e2101-104">For this exercise, you will be using a payment method of **CHECK**.</span></span>

1.  <span data-ttu-id="e2101-105">في شركة **USRT**، انتقل إلى **البيع بالتجزئة وCommerce > العملاء > خدمة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="e2101-105">In the company **USRT**, go to **Retail and Commerce > Customers > Customer service**.</span></span>
2.  <span data-ttu-id="e2101-106">في **خدمة العملاء**، ابحث عن **Karen**.</span><span class="sxs-lookup"><span data-stu-id="e2101-106">In **Customer service**, search for **Karen**.</span></span>
3.  <span data-ttu-id="e2101-107">حدد **أمر مبيعات جديد**.</span><span class="sxs-lookup"><span data-stu-id="e2101-107">Select **New sales order**.</span></span>
4.  <span data-ttu-id="e2101-108">في مقدمة أمر المبيعات، في الحقل **طريقة التسليم**، أدخل **99**.</span><span class="sxs-lookup"><span data-stu-id="e2101-108">On the sales order header, in the **Mode of delivery** field, enter **99**.</span></span>
5.  <span data-ttu-id="e2101-109">في الحقل **رقم الصنف**، أدخل **0005**.</span><span class="sxs-lookup"><span data-stu-id="e2101-109">In the **Item number** field, enter **0005**.</span></span>
6.  <span data-ttu-id="e2101-110">في جزء الإجراء، حدد علامة تبويب **أمر مبيعات** ثم حدد **مدفوعات**.</span><span class="sxs-lookup"><span data-stu-id="e2101-110">On the Action Pane, select the **Sales order** tab and then select **Payments**.</span></span>
7.  <span data-ttu-id="e2101-111">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e2101-111">Select **New**.</span></span>
8.  <span data-ttu-id="e2101-112">في حقل **طريقة الدفع**، أدخل **2** (**شيك**).</span><span class="sxs-lookup"><span data-stu-id="e2101-112">In the **Payment method** field, enter **2** (**Check**).</span></span>
9.  <span data-ttu-id="e2101-113">في **رقم الشيك** حقل، أدخل **1234**.</span><span class="sxs-lookup"><span data-stu-id="e2101-113">In the **Check number** field, enter **1234**.</span></span>
10. <span data-ttu-id="e2101-114">في حقل **مبلغ الدفع**، أدخل **4.59**.</span><span class="sxs-lookup"><span data-stu-id="e2101-114">In the **Payment amount** field, enter **4.59**.</span></span>
11. <span data-ttu-id="e2101-115">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e2101-115">Select **OK**.</span></span>
12. <span data-ttu-id="e2101-116">أغلق صفحة **المدفوعات**.</span><span class="sxs-lookup"><span data-stu-id="e2101-116">Close the **Payments** page.</span></span>
13. <span data-ttu-id="e2101-117">في جزء الإجراء، حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="e2101-117">On the Action Pane, select **Complete**.</span></span>
14. <span data-ttu-id="e2101-118">راجع ملخص الأمر للتحقق من صحته ثم حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="e2101-118">Review the order summary for correctness and then select **Submit**.</span></span>


## <a name="scenario---create-a-hold-code"></a><span data-ttu-id="e2101-119">سيناريو ـ إنشاء كود حجز</span><span class="sxs-lookup"><span data-stu-id="e2101-119">Scenario - Create a hold code</span></span>
<span data-ttu-id="e2101-120">أنت مدير في مركز اتصالات وتريد إنشاء أمر كود حجز يسمى **شيك ائتماني** للسماح للعاملين في مركز الاتصال الذي لديهم صلاحية وصول محددة (دور **مدير تقديم الخدمات**) بوضع الأوامر قيد الانتظار بينما يتم التحقق من الرصيد الائتماني للعميل بنجاح.</span><span class="sxs-lookup"><span data-stu-id="e2101-120">You are a call center manager and want to create an order hold code named \*\*Credit check \*\* to allow call center workers with specific access (role of **Service Delivery Manager**) to place orders on hold while a customer’s credit is successfully verified.</span></span> <span data-ttu-id="e2101-121">تريد تعيين كود الحجز هذا ككود افتراضي لوضع الأوامر قيد الانتظار، ولم تكن تريد الأوامر المحجوزة لحجز المخزون.</span><span class="sxs-lookup"><span data-stu-id="e2101-121">You want to assign that hold code as a default code for placing orders on hold, and you don’t want held orders to reserve inventory.</span></span>

1.  <span data-ttu-id="e2101-122">في شركة **USRT**، انتقل إلى **البيع بالتجزئة وCommerce > إعداد القناة >إعداد مركز اتصال > أمر كود الحجز**.</span><span class="sxs-lookup"><span data-stu-id="e2101-122">In the company **USRT**, go to **Retail and Commerce > Channel Setup > Call center setup > Order hold codes**.</span></span> 
2.  <span data-ttu-id="e2101-123">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e2101-123">Select **New**.</span></span>  
3.  <span data-ttu-id="e2101-124">أدخل **ائتمان** في حقل **كود الحجز**.</span><span class="sxs-lookup"><span data-stu-id="e2101-124">Enter **Credit** in the **Hold code** field.</span></span> 
4.  <span data-ttu-id="e2101-125">في حقل **الوصف**، أدخل **شيك ائتماني**.</span><span class="sxs-lookup"><span data-stu-id="e2101-125">In the **Description** field, enter **Credit check**.</span></span> 
5.  <span data-ttu-id="e2101-126">قم بتعيين لدور أمان **مدير تقديم الخدمات** للاستخدام الحصري لأمر كود الحجز.</span><span class="sxs-lookup"><span data-stu-id="e2101-126">Assign the **Service Delivery Manager** security role for the exclusive use of an order hold code.</span></span> 
6.  <span data-ttu-id="e2101-127">قم بتعيين خيار **الإعداد الافتراضي لأمر المبيعات** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e2101-127">Set the **Default for sales order** option to **Yes**.</span></span>  
7.  <span data-ttu-id="e2101-128">قم بتعيين خيار **إلغاء حجوزات المخزون** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="e2101-128">Set the **Remove inventory reservations** option to **Yes**.</span></span>
8.  <span data-ttu-id="e2101-129">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e2101-129">Select **Save**.</span></span>

## <a name="scenario---put-an-order-on-hold-and-release-it-from-hold"></a><span data-ttu-id="e2101-130">سيناريو ـ وضع أمر قيد الانتظار وتحريره من الانتظار</span><span class="sxs-lookup"><span data-stu-id="e2101-130">Scenario - Put an order on hold and release it from hold</span></span>
<span data-ttu-id="e2101-131">أنت موظف في مركز الاتصالات وقد طلب منك مديرك وضع الأمر **012517** قيد الانتظار لمراجعته قبل مواصلة معالجة الأمر.</span><span class="sxs-lookup"><span data-stu-id="e2101-131">You are a call center employee and have been asked by your manager to place order **012517** on hold for review before the order is further processed.</span></span> <span data-ttu-id="e2101-132">في وقت لاحق، يطلب منك مديرك تحرير الأمر من الانتظار لأن الفحوصات الداخلية قد اكتملت بنجاح.</span><span class="sxs-lookup"><span data-stu-id="e2101-132">Later, your manager asks you to release the order from hold because the internal checks have been successfully completed.</span></span>

1.  <span data-ttu-id="e2101-133">في شركة **USRT**، انتقل إلى **البيع بالتجزئة وCommerce > العملاء > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="e2101-133">In the company **USRT**, go to **Retail and Commerce > Customers > All sales orders**.</span></span>
2.  <span data-ttu-id="e2101-134">حدد الأمر **012517**.</span><span class="sxs-lookup"><span data-stu-id="e2101-134">Select order **012517**.</span></span>
3.  <span data-ttu-id="e2101-135">في جزء الإجراء، حدد **أمر المبيعات > الوظائف > حجوزات الأوامر**.</span><span class="sxs-lookup"><span data-stu-id="e2101-135">In the Action Pane, select **Sales order > Functions > Order holds**.</span></span>
4.  <span data-ttu-id="e2101-136">في صفحة **حجوزات الأوامر**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="e2101-136">On the **Order holds** page, select **New**.</span></span>
5.  <span data-ttu-id="e2101-137">في حقل **كود الحجز**، أدخل **MGRREV**.</span><span class="sxs-lookup"><span data-stu-id="e2101-137">In the **Hold code** field, enter **MGRREV**.</span></span>
6.  <span data-ttu-id="e2101-138">في علامة التبويب **الملاحظات**، أدخل **هذه الملاحظة بشأن مراجعة المدير لكود الحجز** في حقل **ملاحظات الحجز**.</span><span class="sxs-lookup"><span data-stu-id="e2101-138">On the **Notes** tab, enter **This is a note for hold code Manager review** in the **Hold notes** field.</span></span>
7.  <span data-ttu-id="e2101-139">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e2101-139">Select **Save**.</span></span>
8.  <span data-ttu-id="e2101-140">انتقل إلى **البيع بالتجزئة وCommerce > العملاء > حجوزات الأوامر**.</span><span class="sxs-lookup"><span data-stu-id="e2101-140">Go to **Retail and Commerce > Customers > Order holds**.</span></span>
9.  <span data-ttu-id="e2101-141">في جزء الإجراء، حدد علامة التبويب **مسح الحجز** ثم حدد **مسح الحجوزات**.</span><span class="sxs-lookup"><span data-stu-id="e2101-141">On the Action Pane, select the **Clear hold** tab and then select **Clear holds**.</span></span>
