---
ms.openlocfilehash: f6de731881ca0585a2f52ee359e20ceb2091cd6a
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073205"
---
## <a name="scenario"></a><span data-ttu-id="ec236-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="ec236-101">Scenario</span></span>
<span data-ttu-id="ec236-102">تحتاج إلى إنشاء تدرج هرمي جديد للحجز لمساعدتك في إدارة البرتقال.</span><span class="sxs-lookup"><span data-stu-id="ec236-102">You need to create a new reservation hierarchy to help you manage oranges.</span></span> <span data-ttu-id="ec236-103">سيتم تعقب البرتقال باستخدام الموقع والمستودع والموقع وأرقام الدُفعات.</span><span class="sxs-lookup"><span data-stu-id="ec236-103">The oranges will be tracked by using site, warehouse, location, and batch numbers.</span></span> <span data-ttu-id="ec236-104">استخدم المعلومات المتوفرة لإنشاء تدرج هرمي جديد للحجز.</span><span class="sxs-lookup"><span data-stu-id="ec236-104">Use the information provided to create a new reservation hierarchy.</span></span> 

## <a name="create-a-reservation-hierarchy"></a><span data-ttu-id="ec236-105">إنشاء تدرج هرمي للحجز</span><span class="sxs-lookup"><span data-stu-id="ec236-105">Create a reservation hierarchy</span></span>

1.  <span data-ttu-id="ec236-106">في شركة **USMF**، انتقل إلى **إدراة المستودعات > الإعداد > المخزون > التدرج الهرمي للحجز**.</span><span class="sxs-lookup"><span data-stu-id="ec236-106">In company **USMF**, go to **Warehouse management > Setup > Inventory > Reservation hierarchy**.</span></span>
2.  <span data-ttu-id="ec236-107">حدد **جديد** في جزء الإجراءات لإنشاء تدرج هرمي جديد للحجز.</span><span class="sxs-lookup"><span data-stu-id="ec236-107">Select **New** on the Action Pane to create a new reservation hierarchy.</span></span>
3.  <span data-ttu-id="ec236-108">أدخل **USMF** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="ec236-108">Enter **USMF** in the **Name** field.</span></span>
4.  <span data-ttu-id="ec236-109">أدخل **USMF افتراضي** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="ec236-109">Enter **USMF Default** in the **Description** field.</span></span>

## <a name="select-dimensions-for-the-reservation-hierarchy"></a><span data-ttu-id="ec236-110">تحديد أبعاد التدرج الهرمي للحجز</span><span class="sxs-lookup"><span data-stu-id="ec236-110">Select dimensions for the reservation hierarchy</span></span>

1.  <span data-ttu-id="ec236-111">في الجزء **المحدد**، حدد خانة الاختيار **الرقم التسلسلي**.</span><span class="sxs-lookup"><span data-stu-id="ec236-111">In the **Selected** pane, select the **Serial number** check box.</span></span>
2.  <span data-ttu-id="ec236-112">حدد زر الاتجاه الأيسر لنقل الأبعاد إلى الجزء **المتوفر**.</span><span class="sxs-lookup"><span data-stu-id="ec236-112">Select the left directional button to move the dimensions to the **Available** pane.</span></span>
3.  <span data-ttu-id="ec236-113">كرر الخطوتين 1 و2 لـ **المالك**.</span><span class="sxs-lookup"><span data-stu-id="ec236-113">Repeat steps 1-2 for **Owner**.</span></span>
4.  <span data-ttu-id="ec236-114">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ec236-114">Select **OK**.</span></span>
5.  <span data-ttu-id="ec236-115">تم إنشاء تسلسل هرمي جديد للحجز.</span><span class="sxs-lookup"><span data-stu-id="ec236-115">A new reservation hierarchy has been created.</span></span> 

## <a name="apply-the-reservation-hierarchy-to-a-new-product"></a><span data-ttu-id="ec236-116">تطبيق التدرج الهرمي للحجز على منتج جديد</span><span class="sxs-lookup"><span data-stu-id="ec236-116">Apply the reservation hierarchy to a new product</span></span> 

<span data-ttu-id="ec236-117">تحتاج إلى إنشاء منتج جديد في شركة USMF يُسمى عصير برتقال منخفض السكر، رقم الصنف B1234.</span><span class="sxs-lookup"><span data-stu-id="ec236-117">You need to create a new product in company USMF called Low sugar orange juice, item number B1234.</span></span> <span data-ttu-id="ec236-118">سيتعقب الصنف الجديد الموقع والمستودع والموقع وأرقام الدُفعات.</span><span class="sxs-lookup"><span data-stu-id="ec236-118">The new item will track site, warehouse, location, and batch numbers.</span></span> <span data-ttu-id="ec236-119">ستستخدم تكلفة المنتج منهجية ما يرد أولاً يصرف أولاً وسيستخدم الترحيل الترحيلات القياسية.</span><span class="sxs-lookup"><span data-stu-id="ec236-119">The costing for the product will use the FIFO methodology and the posting will use the standard  postings.</span></span> <span data-ttu-id="ec236-120">استخدم المعلومات المتوفرة لإنشاء صنف جديد.</span><span class="sxs-lookup"><span data-stu-id="ec236-120">Use the information provided to create a new item.</span></span>

## <a name="create-a-product"></a><span data-ttu-id="ec236-121">إنشاء منتج</span><span class="sxs-lookup"><span data-stu-id="ec236-121">Create a product</span></span>

1.  <span data-ttu-id="ec236-122">في **USMF**، افتح **إدارة معلومات المنتج > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="ec236-122">In **USMF**, open **Product information management > Products > Released products**.</span></span>
2.  <span data-ttu-id="ec236-123">حدد **جديد** في جزء الإجراءات لإنشاء منتج جديد.</span><span class="sxs-lookup"><span data-stu-id="ec236-123">Select **New** in the Action Pane to create a new product.</span></span>
3.  <span data-ttu-id="ec236-124">أدخل المعلومات التالية في حقول الإدخال:</span><span class="sxs-lookup"><span data-stu-id="ec236-124">Enter the following information in the entry fields:</span></span>
    -  <span data-ttu-id="ec236-125">**رقم المنتج** -‏ B1234</span><span class="sxs-lookup"><span data-stu-id="ec236-125">**Product number** - B1234</span></span>
    -  <span data-ttu-id="ec236-126">**اسم المنتج** ‏- USB Hub</span><span class="sxs-lookup"><span data-stu-id="ec236-126">**Product name** - USB Hub</span></span>
    -  <span data-ttu-id="ec236-127">**مجموعة نماذج الصنف** - الوارد أولاً يُصرف أولاً‬‬</span><span class="sxs-lookup"><span data-stu-id="ec236-127">**Item model group** - FIFO</span></span>
    -  <span data-ttu-id="ec236-128">**مجموعة الأصناف** - الاستهلاك</span><span class="sxs-lookup"><span data-stu-id="ec236-128">**Item group** - Consume</span></span>
    -  <span data-ttu-id="ec236-129">**مجموعة أبعاد التخزين** - ‏أدوات</span><span class="sxs-lookup"><span data-stu-id="ec236-129">**Storage dimension group** - Ware</span></span>
    -  <span data-ttu-id="ec236-130">**مجموعة أبعاد التعقب** - الدفعة</span><span class="sxs-lookup"><span data-stu-id="ec236-130">**Tracking dimension group** - Batch-Phy</span></span>
    -  <span data-ttu-id="ec236-131">**التدرج الهرمي للحجز** - الدفعة - التدرج الهرمي لحجز الدفعات</span><span class="sxs-lookup"><span data-stu-id="ec236-131">**Reservation hierarchy** - Batch -  batch reservation hierarchy</span></span>
4.  <span data-ttu-id="ec236-132">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ec236-132">Select **OK**.</span></span>
5.  <span data-ttu-id="ec236-133">تم إنشاء منتج جديد وسيتم عرض الصفحة الرئيسية **تفاصيل المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="ec236-133">A new product is created and the **Released Product details** master page will display.</span></span>




