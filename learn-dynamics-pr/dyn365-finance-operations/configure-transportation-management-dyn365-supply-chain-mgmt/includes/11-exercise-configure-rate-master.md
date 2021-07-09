---
ms.openlocfilehash: 9668500dda9b7e96189bd5bdb321cb2985cbedeb
ms.sourcegitcommit: b21044c60b6081c58bda95313d2790aeed26d48d
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/20/2020
ms.locfileid: "6073566"
---
## <a name="scenario"></a><span data-ttu-id="bcc29-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="bcc29-101">Scenario</span></span>
<span data-ttu-id="bcc29-102">تخطط شركة **USRT** لشحن النباتات الحية إلى عميل جديد في بوثيل، واشنطن، الولايات المتحدة، حيث الرمز البريدي هو</span><span class="sxs-lookup"><span data-stu-id="bcc29-102">The **USRT** company is planning to ship some live plants to a new customer in Bothell, Washington, United States, where the zip code is</span></span>
98021. <span data-ttu-id="bcc29-103">ستقوم الشركة بالشحن من مستودعها في كارمل، إنديانا، الولايات المتحدة، حيث الرمز البريدي هو 46032.</span><span class="sxs-lookup"><span data-stu-id="bcc29-103">The company will be shipping from their warehouse in Carmel, Indiana, United States, where the zip code is 46032.</span></span>

<span data-ttu-id="bcc29-104">يحتاج مدير النقل إلى تكوين سعر نقل **أزهار** رئيسي جديد وتكوين مهمة لمواقع المصدر والوجهة باستخدام محدد عدد الأميال.</span><span class="sxs-lookup"><span data-stu-id="bcc29-104">The Transportation manager needs to configure a new **Flower** moving rate master and configure an assignment for the source and destination locations by using the mileage engine.</span></span>


## <a name="create-a-rate-master"></a><span data-ttu-id="bcc29-105">إنشاء سعر رئيسي</span><span class="sxs-lookup"><span data-stu-id="bcc29-105">Create a rate master</span></span> 

1.  <span data-ttu-id="bcc29-106">في شركة USRT، افتح **إدارة النقل > إعداد > التسعير > السعر الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-106">In the USRT company, open **Transportation management > Setup > Rating > Rate master**.</span></span>
2.  <span data-ttu-id="bcc29-107">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-107">Select **New**.</span></span>
3.  <span data-ttu-id="bcc29-108">في حقل **السعر الرئيسي**، أدخل **FlowerMovingMaster**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-108">In the **Rate master** field, enter **FlowerMovingMaster**.</span></span>
4.  <span data-ttu-id="bcc29-109">في حقل **الاسم**، أدخل **FlowerMovingMaster**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-109">In the **Name** field, enter **FlowerMovingMaster**.</span></span>
5.  <span data-ttu-id="bcc29-110">في الحقل **معرّف بيانات تعريف التقييم**، حدد **عدد الأميال**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-110">In the **Rating metadata ID** field, select **Milage**.</span></span>

## <a name="assign-the-rate-base-assignments"></a><span data-ttu-id="bcc29-111">تعيين مهمات أساس التسعير</span><span class="sxs-lookup"><span data-stu-id="bcc29-111">Assign the rate base assignments</span></span> 

1.  <span data-ttu-id="bcc29-112">في صفحة **الأسعار الرئيسية**، حدد **أساس التسعير** في القائمة العلوية</span><span class="sxs-lookup"><span data-stu-id="bcc29-112">On the **Rate masters** page, select **Rate base** on the top menu</span></span>
1.  <span data-ttu-id="bcc29-113">حدد **جديد**</span><span class="sxs-lookup"><span data-stu-id="bcc29-113">Select **New**</span></span>
1.  <span data-ttu-id="bcc29-114">في حقل **أساس التسعير**، أدخل **FlowerMovingBase**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-114">In the **Rate base** field, enter **FlowerMovingBase**</span></span>
1.  <span data-ttu-id="bcc29-115">في حقل **الاسم**، أدخل **سعر نقل الأزهار الأساسي**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-115">In the **Name** field, enter **Flower Moving Base**</span></span>
1.  <span data-ttu-id="bcc29-116">في حقل **السعر الرئيسي**، حدد **FlowerMovingMaster**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-116">In the **Rate master** field, select **FlowerMovingMaster**.</span></span>
1.  <span data-ttu-id="bcc29-117">في حقل **الفاصل الرئيسي**، حدد **عدد الأميال**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-117">In the **Break master** field, select **Milage**</span></span>
1.  <span data-ttu-id="bcc29-118">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="bcc29-118">Close the page.</span></span> 
1.  <span data-ttu-id="bcc29-119">في صفحة **الأسعار الرئيسية**، حدد علامة التبويب السريعة **مهمات أساس التسعير** ثم حدد **جديد**</span><span class="sxs-lookup"><span data-stu-id="bcc29-119">In the **Rate masters** page, select the **Rate base assignments** FastTab and then select **New**</span></span>
1.  <span data-ttu-id="bcc29-120">في الحقل **الاسم**، أدخل **LTL**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-120">In the **Name** field, enter **LTL**.</span></span>
1.  <span data-ttu-id="bcc29-121">في علامة التبويب السريعة **مهمات أساس التسعير**، حدد **FlowerMovingBase** في القائمة المنسدلة **أساس التسعير**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-121">On the **Rate base assignments** FastTab, select **FlowerMovingBase** in the **Rate base** drop-down list.</span></span>
1.  <span data-ttu-id="bcc29-122">في حقل **الخدمة**، حدد **شاحنة**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-122">In the **Service** field, select **Truck**.</span></span>
1.  <span data-ttu-id="bcc29-123">في حقل **جهاز الكمبيوتر الشخصي الأصلي**، أدخل **46032**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-123">In the **Origin PC** field, enter **46032**.</span></span>
1.  <span data-ttu-id="bcc29-124">في حقل **DestStartPC**، أدخل **98021**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-124">In the **DestStartPC** field, enter **98021**.</span></span>
1.  <span data-ttu-id="bcc29-125">في حقل **DestEndPC**، أدخل **98021**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-125">In the **DestEndPC** field, enter **98021**.</span></span>
1.  <span data-ttu-id="bcc29-126">في الحقل **البلد الوجهة**، أدخل **الولايات المتحدة الأمريكية**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-126">In the **DestCountry** field, enter **USA**.</span></span>
1.  <span data-ttu-id="bcc29-127">في حقل **تاريخ ووقت البدء الفعلي**، حدد **الانتقال إلى اليوم**.</span><span class="sxs-lookup"><span data-stu-id="bcc29-127">In the **Effective start date and time** field, select **Go to today**.</span></span>
1.  <span data-ttu-id="bcc29-128">حدد **حفظ** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="bcc29-128">Select **Save** on the Action Pane.</span></span>
1. <span data-ttu-id="bcc29-129">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="bcc29-129">Close the page.</span></span>
