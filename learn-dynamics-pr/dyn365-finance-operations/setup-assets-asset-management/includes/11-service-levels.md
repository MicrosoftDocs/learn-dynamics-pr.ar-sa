---
ms.openlocfilehash: cd8af82aaf8014b72d46378c2d0847ff6d499225
ms.sourcegitcommit: 13594cb3c8f0b1478f14aac7e239bc20317f480c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/15/2021
ms.locfileid: "6072496"
---
<span data-ttu-id="7fed3-101">يتم استخدام مستويات خدمة الأصل، المرتبطة بالأصول، في طلبات الصيانة وأوامر العمل لتحديد أولوية أوامر العمل أثناء جدولة أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="7fed3-101">Asset service levels that are associated with assets are used on maintenance requests and work orders and determine the priority of work orders during work order scheduling.</span></span> 

<span data-ttu-id="7fed3-102">يتم تحديد مستويات خدمة الأصل عن طريق إقران العناصر التالية:</span><span class="sxs-lookup"><span data-stu-id="7fed3-102">The asset service levels are defined by associating the following elements:</span></span>

- <span data-ttu-id="7fed3-103">موقع العمل</span><span class="sxs-lookup"><span data-stu-id="7fed3-103">Functional location</span></span>
- <span data-ttu-id="7fed3-104">نوع الأصل</span><span class="sxs-lookup"><span data-stu-id="7fed3-104">Asset type</span></span>
- <span data-ttu-id="7fed3-105">الشركة المصنعة</span><span class="sxs-lookup"><span data-stu-id="7fed3-105">Manufacturer</span></span>
- <span data-ttu-id="7fed3-106">النموذج</span><span class="sxs-lookup"><span data-stu-id="7fed3-106">Model</span></span>
- <span data-ttu-id="7fed3-107">الأصل</span><span class="sxs-lookup"><span data-stu-id="7fed3-107">Asset</span></span>
- <span data-ttu-id="7fed3-108">نوع أمر العمل</span><span class="sxs-lookup"><span data-stu-id="7fed3-108">Work order type</span></span>
- <span data-ttu-id="7fed3-109">مستوى الخدمة (الإعداد في **إدارة الأصول > إعداد > مستويات خدمة الأصل**)</span><span class="sxs-lookup"><span data-stu-id="7fed3-109">Service level (set up in **Asset Management > Setup > Asset service levels**)</span></span>
    - <span data-ttu-id="7fed3-110">1 = هام</span><span class="sxs-lookup"><span data-stu-id="7fed3-110">1=Critical</span></span>
    - <span data-ttu-id="7fed3-111">2 = عاجل</span><span class="sxs-lookup"><span data-stu-id="7fed3-111">2=Urgent</span></span>
    - <span data-ttu-id="7fed3-112">3 = مرتفع</span><span class="sxs-lookup"><span data-stu-id="7fed3-112">3=High</span></span>
    - <span data-ttu-id="7fed3-113">4 = متوسط</span><span class="sxs-lookup"><span data-stu-id="7fed3-113">4=Medium</span></span>
    - <span data-ttu-id="7fed3-114">5 = منخفض</span><span class="sxs-lookup"><span data-stu-id="7fed3-114">5=Low</span></span>

<span data-ttu-id="7fed3-115">لمزيد من المعلومات حول إعداد حساب نقاط التصنيف لجدولة أمر العمل، راجع وحدة **إدارة معلمات الأصول** في هذه الوحدة النمطية.</span><span class="sxs-lookup"><span data-stu-id="7fed3-115">For more information about how calculation of rating scores is set up for work order scheduling, refer to the **Set up asset management parameters** unit in this module.</span></span>

> [!NOTE]
> <span data-ttu-id="7fed3-116">يجب إعداد سجل افتراضي واحد على الأقل لمستوى خدمة الأصل.</span><span class="sxs-lookup"><span data-stu-id="7fed3-116">You must set up at least one default record for the asset service level.</span></span> <span data-ttu-id="7fed3-117">يتم استخدام هذا السجل الافتراضي في حالة عدم العثور على أية مطابقة أخرى أثناء جدولة أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="7fed3-117">This default record is used when no other match is found during work order scheduling.</span></span>

## <a name="set-up-asset-service-levels"></a><span data-ttu-id="7fed3-118">إعداد مستويات خدمة الأصول</span><span class="sxs-lookup"><span data-stu-id="7fed3-118">Set up asset service levels</span></span>


1. <span data-ttu-id="7fed3-119">لإعداد مستويات خدمة الأصل، انتقل إلى **إدارة الأصول > إعداد > مستويات خدمة الأصل** وحدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7fed3-119">To set up asset service levels, go to **Asset management > Setup > Asset service levels** and select **New**.</span></span>

1. <span data-ttu-id="7fed3-120">استخدم الحقول المتنوعة لإنشاء مستوى خدمة الأصل كما تم تلخيصه مسبقا.</span><span class="sxs-lookup"><span data-stu-id="7fed3-120">Use the various fields to create the asset service level as previously summarized.</span></span>
    - <span data-ttu-id="7fed3-121">سيكون لمستوى خدمة الأصل الافتراضي كافة الحقول فارغة فيما عدا مستوى الخدمة.</span><span class="sxs-lookup"><span data-stu-id="7fed3-121">The default asset service level will have all the fields blank except for the service level.</span></span> 
    - <span data-ttu-id="7fed3-122">نظراً لأن سير الناقلة المقطوعة عبارة عن مشكله، فإنه يتم تصنيفها كمستوى خدمة عالي.</span><span class="sxs-lookup"><span data-stu-id="7fed3-122">Because a broken conveyor belt is a problem, it rates as a high service level.</span></span> <span data-ttu-id="7fed3-123">حدد **سير ناقلة** في الحقل **نوع الأصل**، ثم حدد **3** في الحقل **مستوى الخدمة**.</span><span class="sxs-lookup"><span data-stu-id="7fed3-123">Select **Conveyor belt** in the **Asset type** field, and then select **3** in the **Service level** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="7fed3-124">عند استخدام مستوى خدمة أصل لطلبات الصيانة وأوامر العمل، تبحث إدارة الأصول عن وجود تطابق محتمل.</span><span class="sxs-lookup"><span data-stu-id="7fed3-124">When an asset service level is used for maintenance requests and work orders, Asset Management searches for a possible match.</span></span> 


1. <span data-ttu-id="7fed3-125">تقوم إدارة الأصول دائماً بفحص المجموعة الأكثر تحديداً.</span><span class="sxs-lookup"><span data-stu-id="7fed3-125">Asset Management always checks the most specific combination first.</span></span> <span data-ttu-id="7fed3-126">بدءاً من الحقل **نوع أمر العمل**، إذا لم يتم العثور على أي تطابق، سيقوم بالتحقق من التطابق الخاص بحقل **الأصل** ثم يستمر في البحث خلال كل حقل مستوى خدمة من اليمين إلى اليسار.</span><span class="sxs-lookup"><span data-stu-id="7fed3-126">Starting in the **Work order type** field, if no match is found, it checks for a match for the **Asset** field and then continues to search through each service level field from right to left.</span></span> 

1. <span data-ttu-id="7fed3-127">في حالة عدم العثور على أي تطابق، يتم استخدام السجل الافتراضي الذي لا يحتوي على تحديدات في هذه الحقول.</span><span class="sxs-lookup"><span data-stu-id="7fed3-127">If no match is found, the default record that has no selections in those fields is used.</span></span>

<span data-ttu-id="7fed3-128">تعرض الصورة التالية مثالاً لصفحة **مستويات خدمة الأصل**.</span><span class="sxs-lookup"><span data-stu-id="7fed3-128">The following image shows an example of the **Asset service levels** page.</span></span>

<span data-ttu-id="7fed3-129">**إدارة الأصول > إعداد > مستويات خدمة الأصل**.</span><span class="sxs-lookup"><span data-stu-id="7fed3-129">**Asset management > Setup > Asset service levels**</span></span>

<span data-ttu-id="7fed3-130">[![لقطة شاشة لصفحة مستويات خدمة الأصل.](../media/service-levels-ss.png)](../media/service-levels-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7fed3-130">[![Screenshot of the Asset service levels page.](../media/service-levels-ss.png)](../media/service-levels-ss.png#lightbox)</span></span>


> [!NOTE]
> <span data-ttu-id="7fed3-131">يمكن تغيير مستويات خدمات الأصول إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="7fed3-131">Asset services levels can be changed if needed.</span></span> <span data-ttu-id="7fed3-132">ومع ذلك، إذا قمت بتغيير سجل مستوى خدمة الأصل في الصفحة **مستويات خدمة الأصل** وكان المستوى الأصلي قيد الاستخدام بالفعل، فلن يتم تحديث مستوى الخدمة الجديد في طلبات الصيانة الموجودة وأوامر العمل.</span><span class="sxs-lookup"><span data-stu-id="7fed3-132">However, if you change an asset service level record on the **Asset service levels** page and the original level is already in use, the new service level is not updated on existing maintenance requests and work orders.</span></span>

<span data-ttu-id="7fed3-133">يوضح الفيديو التالي كيفية إنشاء مستويات خدمة الأصل في إدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="7fed3-133">The following video shows you how to create asset service levels in Asset Management.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4oErt]


