---
ms.openlocfilehash: 78d4cb58ada5a4f219741c8c92756f10538bceaa
ms.sourcegitcommit: c332416640d93a9a9f8ba875c22bdb8e2eb64c3e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "6073855"
---
## <a name="scenario"></a><span data-ttu-id="4dbec-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="4dbec-101">Scenario</span></span>

<span data-ttu-id="4dbec-102">أنت مدير حسابات تقوم بالاطلاع على أمر يتم شحنه إلى مصنع Acme.</span><span class="sxs-lookup"><span data-stu-id="4dbec-102">You are an accounting manager overseeing an order that is being shipped to the Acme Factory.</span></span> <span data-ttu-id="4dbec-103">للقيام بهذا الهدف، يجب تعديل تفاصيل صنف اختبار FIFO، ويجب إنشاء أمر الشراء، وكذلك إنشاء سعر صنف تم تحديثه، كما يجب إنشاء فاتورة.</span><span class="sxs-lookup"><span data-stu-id="4dbec-103">To accomplish this goal, details of the FIFO test item must be modified, the purchase order must be created, an item price updated, and an invoice must be generated.</span></span>

## <a name="modify-details-of-the-fifo-test-item"></a><span data-ttu-id="4dbec-104">تعديل تفاصيل صنف اختبار FIFO</span><span class="sxs-lookup"><span data-stu-id="4dbec-104">Modify details of the FIFO test item</span></span>  ##

1.  <span data-ttu-id="4dbec-105">انتقل إلى صفحة **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-105">Go to the **Product information management > Products > Released products** page.</span></span> 
1.  <span data-ttu-id="4dbec-106">حدد المنتج **A0001** وقم بفتح التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="4dbec-106">Select product **A0001** and open details.</span></span>  
1.  <span data-ttu-id="4dbec-107">حدد **تحرير** لتعديل التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="4dbec-107">Select **Edit** to modify details.</span></span> 
1.  <span data-ttu-id="4dbec-108">انتقل إلى علامة التبويب السريعة **شراء**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-108">Go to the **Purchase** FastTab.</span></span> <span data-ttu-id="4dbec-109">(علامة التبويب السريعة هي منطقة قابلة للتوسيع وقابلة للطي في الصفحة، لذلك تظهر علامة التبويب السريعة **شراء** في منتصف الشاشة.</span><span class="sxs-lookup"><span data-stu-id="4dbec-109">(The FastTab is an expandable and collapsible area of a page, so  the **Purchase** FastTab appears in the middle of your screen.</span></span>  <span data-ttu-id="4dbec-110">لا تخلط بين هذا مع زر **شراء** الذي يظهر في جزء الإجراءات وهو شريط الأزرار عبر الجزء العلوي من الشاشة.)</span><span class="sxs-lookup"><span data-stu-id="4dbec-110">Do not confuse this with the  **Purchase** button which appears in the Action Pane which is the strip of buttons across the top of the screen.)</span></span>
1.  <span data-ttu-id="4dbec-111">تحديث السعر من 12.00 إلى 16.49 في الحقل **السعر**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-111">Update the price from 12.00 to 16.49 in the **Price** field.</span></span>
1.  <span data-ttu-id="4dbec-112">قم بتعيين شريط التمرير **آخر سعر شراء** إلى **نعم** ضمن القسم **تحديث السعر**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-112">Set the **Latest purchase price** slider to **Yes** under the **Price update** section.</span></span>
1.  <span data-ttu-id="4dbec-113">لتحديث سعر المبيعات، قم بتوسيع علامة التبويب السريعة **البيع**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-113">To update the sales price, expand the **Sell** FastTab.</span></span>
1.  <span data-ttu-id="4dbec-114">أدخل **19.99** في حقل **السعر** ضمن **سعر المبيعات الأساسي**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-114">Enter **19.99** in the **Price** field under **Base sales price**.</span></span> 
1.  <span data-ttu-id="4dbec-115">حدد **نسبة المساهمة** في **نموذج سعر المبيعات** ضمن **تحديث السعر**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-115">Select **Contribution ratio** in **Sales price model** under **Price update**.</span></span> 
1.  <span data-ttu-id="4dbec-116">في حقل **نسبة المساهمة**، أدخل **50.00**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-116">Enter **50.00** in the **Contribution ratio** field.</span></span> 
1.  <span data-ttu-id="4dbec-117">حدد **سعر الشراء** في القائمة المنسدلة **السعر الأساسي**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-117">Select **Purchase price** in the **Base price** drop-down menu.</span></span>
1.  <span data-ttu-id="4dbec-118">لإدارة سعر التكلفة الأخير للصنف، انتقل إلى علامة التبويب السريعة **إدارة التكاليف**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-118">To manage the latest cost price for the item, go to the **Manage costs** FastTab.</span></span> 
1.  <span data-ttu-id="4dbec-119">بالنسبة **لآخر سعر تكلفة**، قم بتعيين شريط التمرير إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-119">For **Latest cost price**, set the slider to **Yes**.</span></span> 
1.  <span data-ttu-id="4dbec-120">قم بتعيين السعر إلى **16.49** في الحقل **السعر**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-120">Set the price to **16.49** in the **Price** field.</span></span> 
1.  <span data-ttu-id="4dbec-121">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="4dbec-121">Select **Save**</span></span>
1.  <span data-ttu-id="4dbec-122">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="4dbec-122">Close the page.</span></span>

## <a name="create-a-purchase-order-and-update-the-item-price"></a><span data-ttu-id="4dbec-123">إنشاء أمر شراء وتحديث سعر الصنف</span><span class="sxs-lookup"><span data-stu-id="4dbec-123">Create a purchase order and update the item price</span></span> 
 
1.  <span data-ttu-id="4dbec-124">انتقل إلى صفحة **التدبير والتوريد > أوامر الشراء > جميع أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-124">Go to the **Procurement and sourcing > Purchase orders > All purchase orders** page.</span></span> 
1.  <span data-ttu-id="4dbec-125">حدد **جديد** لإنشاء أمر شراء جديد.</span><span class="sxs-lookup"><span data-stu-id="4dbec-125">To create a new purchase order, select **New**.</span></span> 
1.  <span data-ttu-id="4dbec-126">حدد **حساب المورد** **1001**</span><span class="sxs-lookup"><span data-stu-id="4dbec-126">Select **Vendor account** **1001**</span></span> 
1.  <span data-ttu-id="4dbec-127">في علامة التبويب السريعة **عام**، حدد **الموقع 1** و **المستودع 13** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-127">On the **General** FastTab, select **Site 1** and **Warehouse 13** and then select **OK**.</span></span> 
1.  <span data-ttu-id="4dbec-128">حدد **إضافة بند** ضمن علامة التبويب السريعة **بنود أمر الشراء** لإضافة بند إلى أمر الشراء **A0001**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-128">Select **Add line** under the **Purchase order lines** FastTab to add a line to the purchase order for **A0001**.</span></span>
1.  <span data-ttu-id="4dbec-129">حدد **رقم الصنف A0001**، ثم أدخل **5** في الحقل **الكمية**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-129">Select the **Item number A0001**, then enter **5** in the **Quantity** field.</span></span> 
1.  <span data-ttu-id="4dbec-130">تحديث **سعر الوحدة** إلى **21.00**</span><span class="sxs-lookup"><span data-stu-id="4dbec-130">Update the **Unit price** to **21.00**</span></span> 
1.  <span data-ttu-id="4dbec-131">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-131">Select **Save**.</span></span> 
1.  <span data-ttu-id="4dbec-132">لتأكيد أمر الشراء، انتقل إلى علامة التبويب **شراء** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="4dbec-132">To confirm the purchase order, go to the **Purchase** tab in the Action Pane.</span></span> 
1.  <span data-ttu-id="4dbec-133">حدد **تأكيد** في قسم **الإجراءات**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-133">Select **Confirm** in the **Actions** section.</span></span> 

## <a name="generate-an-invoice"></a><span data-ttu-id="4dbec-134">إنشاء فاتورة</span><span class="sxs-lookup"><span data-stu-id="4dbec-134">Generate an invoice</span></span> 

1.  <span data-ttu-id="4dbec-135">انتقل إلى **الفاتورة** في جزء الإجراء، ضمن القسم **إنشاء**، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-135">Go to **Invoice** in the Action Pane and select **Invoice** under the **Generate** section.</span></span>
1.  <span data-ttu-id="4dbec-136">في أعلى الشاشة، حدد **الافتراضي من: الكمية المطلوبة**</span><span class="sxs-lookup"><span data-stu-id="4dbec-136">At the top of the screen, select **Default from: Ordered quantity**</span></span> 
1.  <span data-ttu-id="4dbec-137">في الصفحة **فاتورة المورد**، حدد الرقم 1217ABC في الحقل **الرقم**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-137">On the **Vendor invoice** page, specify number 1217ABC in the **Number** field.</span></span>
1.  <span data-ttu-id="4dbec-138">حدد تاريخ اليوم في الحقل **تاريخ الترحيل**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-138">Put today’s date in the **Posting date** field.</span></span> 
1.  <span data-ttu-id="4dbec-139">قم بالتمرير لأسفل للتحقق من سعر الوحدة ومعلومات الكمية في علامة التبويب السريعة **البنود**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-139">Scroll down to verify the unit price and quantity info on the **Lines** FastTab.</span></span> 
1.  <span data-ttu-id="4dbec-140">حدد **حالة مطابقة التحديث** في أعلى الشاشة</span><span class="sxs-lookup"><span data-stu-id="4dbec-140">Select, at the top, **Update match status**</span></span>
1.  <span data-ttu-id="4dbec-141">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-141">Select **Post**.</span></span> 
1.  <span data-ttu-id="4dbec-142">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="4dbec-142">Close the page.</span></span> 
1.  <span data-ttu-id="4dbec-143">انتقل إلى **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-143">Go to **Product Information Management > Products > Released products**.</span></span> 
1.  <span data-ttu-id="4dbec-144">افتح الصنف **A0001** وانتقل إلى علامة التبويب السريعة **الشراء**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-144">Open item **A0001** and go to the **Purchase** FastTab.</span></span>
1.  <span data-ttu-id="4dbec-145">التحقق من تحديث **السعر** إلى آخر سعر لأمر الشراء</span><span class="sxs-lookup"><span data-stu-id="4dbec-145">Verify that the **Price** has been updated to the latest purchase order price</span></span> 
1.  <span data-ttu-id="4dbec-146">انتقل إلى علامة التبويب السريعة **البيع**.</span><span class="sxs-lookup"><span data-stu-id="4dbec-146">Go to the **Sell** FastTab.</span></span>
1.  <span data-ttu-id="4dbec-147">تحقق من تحديث تاريخ السعر، ومن تحديث سعر المبيعات الأساسي.</span><span class="sxs-lookup"><span data-stu-id="4dbec-147">Verify that the date of price, and base sales price are updated.</span></span>
1.  <span data-ttu-id="4dbec-148">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="4dbec-148">Close all pages.</span></span>

