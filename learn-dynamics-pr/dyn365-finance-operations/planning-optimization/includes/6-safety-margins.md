---
ms.openlocfilehash: 841e0c3044102c3586d4faed31e96381e51a2926
ms.sourcegitcommit: 01f8d224bf1e548ba0cbe53b3e2150c43302c125
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "6072087"
---
<span data-ttu-id="47d1b-101">توفر هوامش الأمان وقتاً في المخزن المؤقت بعد الحد الأدنى لوقت الإنتاج العادي.</span><span class="sxs-lookup"><span data-stu-id="47d1b-101">Safety margins provide buffer time beyond the normal lead time.</span></span> 

<span data-ttu-id="47d1b-102">على سبيل المثال، إذا تطلب المنتج المستلم فحصاً أو معالجة أو تم تأخيره ولم يكن جاهزاً للاستهلاك الفوري، فباستخدام هامش أمان، لن تحتاج إلى إضافة زمن وصول البضاعة مع المورد لأن ذلك سيعطي للمورد ذلك الوقت المتوقع الإضافي.</span><span class="sxs-lookup"><span data-stu-id="47d1b-102">For example, if a received product requires inspection, handling, or is otherwise delayed and not ready for immediate consumption, with a safety margin, you don’t need to add to the purchase lead time with the vendor because that would give that extra lead time to the vendor.</span></span> 

<span data-ttu-id="47d1b-103">يتم استخدام هوامش الأمان في العمليات الحسابية لثلاث خدمات:</span><span class="sxs-lookup"><span data-stu-id="47d1b-103">Safety margins are used in calculations for three services:</span></span>

- <span data-ttu-id="47d1b-104">**هامش الاستلام** – وقت المخزن المؤقت لمعالجة أمر وارد.</span><span class="sxs-lookup"><span data-stu-id="47d1b-104">**Receipt margin** – The buffer time for handling an incoming order.</span></span>
- <span data-ttu-id="47d1b-105">**هامش إعادة الطلب** – وقت المخزن المؤقت لوضع أمر.</span><span class="sxs-lookup"><span data-stu-id="47d1b-105">**Reorder margin** – The buffer time for placing an order.</span></span>
- <span data-ttu-id="47d1b-106">**هامش الإصدار** – وقت المخزن المؤقت لمعالجة الشحنات الصادرة.</span><span class="sxs-lookup"><span data-stu-id="47d1b-106">**Issue margin** – The buffer time for handling outgoing shipments.</span></span>

> [!NOTE]
> <span data-ttu-id="47d1b-107">لم يتم دعم إعادة ترتيب الهامش وهامش الإصدار، المُشار إليهما في الجدول بخط مائل، من أجل تحسين التخطيط.</span><span class="sxs-lookup"><span data-stu-id="47d1b-107">Reorder margin and Issue margin, which are indicated in the table in italic font, are not yet supported for Planning Optimization.</span></span> <span data-ttu-id="47d1b-108">وحتى الآن، يتم التعامل مع جميع القيم التي تم إدخالها على أنها صفر.</span><span class="sxs-lookup"><span data-stu-id="47d1b-108">Until then, all values that are entered are treated as zero.</span></span>

<span data-ttu-id="47d1b-109">يعرض الجدول التالي مثال على الهوامش المستخدمة في العمليات الحسابية.</span><span class="sxs-lookup"><span data-stu-id="47d1b-109">An example of the margins that are used in calculations are shown in the following table.</span></span>

| <span data-ttu-id="47d1b-110">**الحدث**</span><span class="sxs-lookup"><span data-stu-id="47d1b-110">**Event**</span></span> | <span data-ttu-id="47d1b-111">**عدد الأيام**</span><span class="sxs-lookup"><span data-stu-id="47d1b-111">**# Days**</span></span> | <span data-ttu-id="47d1b-112">**التواريخ**</span><span class="sxs-lookup"><span data-stu-id="47d1b-112">**Dates**</span></span> |
 | ------------- | ------------- |------------- |
 | <span data-ttu-id="47d1b-113">**تاريخ الأمر**</span><span class="sxs-lookup"><span data-stu-id="47d1b-113">**Order date**</span></span> |   | <span data-ttu-id="47d1b-114">1 يوليو</span><span class="sxs-lookup"><span data-stu-id="47d1b-114">July 1</span></span>|
 | <span data-ttu-id="47d1b-115">\**_هامش إعادة الطلب_* _</span><span class="sxs-lookup"><span data-stu-id="47d1b-115">\**_Reorder margin_* _</span></span> | <span data-ttu-id="47d1b-116">2</span><span class="sxs-lookup"><span data-stu-id="47d1b-116">2</span></span> | <span data-ttu-id="47d1b-117">_July 3 – تاريخ بدء التوريد\*</span><span class="sxs-lookup"><span data-stu-id="47d1b-117">_July 3 – Supply start date\*</span></span> |
| <span data-ttu-id="47d1b-118">**الحد الأدنى لوقت الإنتاج**</span><span class="sxs-lookup"><span data-stu-id="47d1b-118">**Lead Time**</span></span> | <span data-ttu-id="47d1b-119">5</span><span class="sxs-lookup"><span data-stu-id="47d1b-119">5</span></span> | <span data-ttu-id="47d1b-120">_July 8 – تاريخ تسليم التوريد</span><span class="sxs-lookup"><span data-stu-id="47d1b-120">July 8 – Supply delivery date</span></span> |
| <span data-ttu-id="47d1b-121">**هامش الاستلام**</span><span class="sxs-lookup"><span data-stu-id="47d1b-121">**Receipt margin**</span></span> | <span data-ttu-id="47d1b-122">2</span><span class="sxs-lookup"><span data-stu-id="47d1b-122">2</span></span> | <span data-ttu-id="47d1b-123">_July 10 – تاريخ متطلبات التوريد</span><span class="sxs-lookup"><span data-stu-id="47d1b-123">July 10 – Supply requirement date</span></span> |
| <span data-ttu-id="47d1b-124">\**_هامش الإصدار_* _</span><span class="sxs-lookup"><span data-stu-id="47d1b-124">\**_Issue margin_* _</span></span> | <span data-ttu-id="47d1b-125">3</span><span class="sxs-lookup"><span data-stu-id="47d1b-125">3</span></span> | <span data-ttu-id="47d1b-126">_July 13 – تاريخ متطلبات الطلب\*</span><span class="sxs-lookup"><span data-stu-id="47d1b-126">_July 13 – Demand requirement date\*</span></span> |



<span data-ttu-id="47d1b-127">عندما يتم تمكين هامش الإصدار وإعادة الترتيب لتحسين التخطيط، ستكون التواريخ الممثلة كما هي مدرجة في الرسم التخطيطي التالي.</span><span class="sxs-lookup"><span data-stu-id="47d1b-127">When the reorder and issue margin are enabled for Planning Optimization, the represented dates will be as listed in the following diagram.</span></span> 

![الرسم التخطيطي للمخطط الزمني من تاريخ الأمر إلى تاريخ الطلب.](../media/safety-margins-c.png)


> [!NOTE]
> <span data-ttu-id="47d1b-129">يمثل هذا الرسم سيناريو يتم فيه تعيين أيام الهوامش في الإعداد على **لا**.</span><span class="sxs-lookup"><span data-stu-id="47d1b-129">This graphic represents a scenario where margins in the setup have working days set to **No**.</span></span> <span data-ttu-id="47d1b-130">إذا تم تعيين أيام العمل على **نعم**، فسيعرض حساب الأيام تقويم أيام العمل ويستبعد تلك الأيام بخلاف أيام العمل.</span><span class="sxs-lookup"><span data-stu-id="47d1b-130">If working days is set to **Yes**, the days calculation would look at the working days calendar and exclude those days that are not working days.</span></span> <span data-ttu-id="47d1b-131">في السيناريو الذي لا يتم فيه تعيين يومي السبت والأحد كأيام عمل ويتم تعيين الهوامش لتضمين أيام العمل، سيكون تاريخ الطلب الفعلي في هذا التقويم لعام 2020 هو 17 يوليو لأن عطلات نهاية الأسبوع ستكون إجمالاً 12 يوماً.</span><span class="sxs-lookup"><span data-stu-id="47d1b-131">In a scenario where Saturday and Sunday are not set as working days and setup on margins are set to include working days, the actual demand date in this calendar for 2020 would be July 17 because two weekends are in the total of 12 days.</span></span> 

<span data-ttu-id="47d1b-132">قبل أن تتمكن من استخدام هذه الوظيفة، يجب عليك تمكين ميزة **الهوامش لتحسين التخطيط** في مساحة عمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="47d1b-132">Before you can use this functionality, you must enable the **Margins for Planning optimization** feature in the **Feature management** workspace.</span></span>

![ <span data-ttu-id="47d1b-133">لقطة شاشة لصفحة إدارة الميزات.</span><span class="sxs-lookup"><span data-stu-id="47d1b-133">Screenshot of the Feature management page.</span></span>](../media/safety-margins-feature-ssm.png)


<span data-ttu-id="47d1b-134">عند التمكين، ستصبح الهوامش جزءاً من حساب الحد الأدنى لوقت الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="47d1b-134">When enabled, the margins will become a part of lead time calculation.</span></span> 

<span data-ttu-id="47d1b-135">يمكن إعداد هوامش الأمان في مجموعة التغطية والخطة الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="47d1b-135">Safety margins can be set up on the Coverage group and the Master plan.</span></span> <span data-ttu-id="47d1b-136">إذا تم إدخال هوامش الأمان في كليهما، فستتم إضافتهما فوق بعضهما البعض.</span><span class="sxs-lookup"><span data-stu-id="47d1b-136">If safety margins are entered in both, they are added on top of each other.</span></span> <span data-ttu-id="47d1b-137">وبالتالي، إذا أدخلت يومين في مجموعة التغطية ويومين في الخطة الرئيسية، فسيكون هذا هامشاً لمدة أربعة أيام.</span><span class="sxs-lookup"><span data-stu-id="47d1b-137">Thus, if you enter two days in the Coverage group and two days on the Master plan, it will be a four-day margin.</span></span>


<span data-ttu-id="47d1b-138">شاهد الفيديو التالي للتعرف على هوامش الأمان.</span><span class="sxs-lookup"><span data-stu-id="47d1b-138">Watch the following video to learn about safety margins.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4IsWa]

