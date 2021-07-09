---
ms.openlocfilehash: 0087e0e976295e3a112bf2984ab8d0fd9c3d161a
ms.sourcegitcommit: 01f8d224bf1e548ba0cbe53b3e2150c43302c125
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "6072086"
---
<span data-ttu-id="0f810-101">التأكيد التلقائي هو عملية إصدار أمر مخطط وتحويله إلى أمر شراء أو أمر تحويل أو أمر تشغيل.</span><span class="sxs-lookup"><span data-stu-id="0f810-101">Auto-firming is the process of releasing a planned order and converting it into a purchase order, transfer order, or a production order.</span></span> <span data-ttu-id="0f810-102">باستخدام "تحسين التخطيط"، يمكن تأكيد الأوامر المخططة أثناء تشغيل الخطة عندما يكون التاريخ ضمن نطاق الحد الزمني للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="0f810-102">With Planning Optimization, planned orders can be firmed during a plan run when the date is within the time fence for firming.</span></span> 

<span data-ttu-id="0f810-103">ولتمكين "التأكيد التلقائي"، يجب تمكين ميزة **التأكيد التلقائي لتحسين التخطيط** في مساحة العمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="0f810-103">To enable auto-firming, you must enable the **Auto-firming for Planning Optimization** feature in the **Feature management** workspace.</span></span>

![ <span data-ttu-id="0f810-104">لقطة شاشة تُظهر التأكيد التلقائي لخيار "تحسين التخطيط".</span><span class="sxs-lookup"><span data-stu-id="0f810-104">Screenshot showing Auto-firming for Planning Optimization option.</span></span>](../media/feature-auto-firming-ssm.png)


## <a name="differences-in-firming-an-order-between-built-in-master-planning-and-planning-optimization"></a><span data-ttu-id="0f810-105">الاختلافات في تأكيد الأمر بين التخطيط الرئيسي المدمج و"تحسين التخطيط"</span><span class="sxs-lookup"><span data-stu-id="0f810-105">Differences in firming an order between built-in master planning and Planning Optimization</span></span>

<span data-ttu-id="0f810-106">في "تحسين التخطيط":</span><span class="sxs-lookup"><span data-stu-id="0f810-106">With Planning Optimization:</span></span>

- <span data-ttu-id="0f810-107">يعتمد التأكيد التلقائي على تاريخ الأمر (تاريخ البدء).</span><span class="sxs-lookup"><span data-stu-id="0f810-107">Auto-firming is based on the order date (start date).</span></span>
- <span data-ttu-id="0f810-108">ولأن تاريخ الأمر (تاريخ البدء) يقوم بتشغيل التأكيد، فلن تكون بحاجة إلى التفكير في وقت الإنتاج كجزء من الحد الزمني للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="0f810-108">Because the order date (start date) triggers the firming, you don't have to consider the lead time as part of the firming time fence.</span></span>
- <span data-ttu-id="0f810-109">إذا كنت ترغب في تأكيد جميع الأوامر التي يجب أن تبدأ خلال الأسبوع الحالي، فيجب أن يكون الحد الزمني للتأكيد أسبوعاً واحداً.</span><span class="sxs-lookup"><span data-stu-id="0f810-109">If you want to firm all orders that must start during the current week, the firming time fence must be one week.</span></span>

<span data-ttu-id="0f810-110">في التخطيط الرئيسي المدمج:</span><span class="sxs-lookup"><span data-stu-id="0f810-110">With built-in master planning:</span></span>

- <span data-ttu-id="0f810-111">يعتمد التأكيد التلقائي على تاريخ المتطلبات (تاريخ الانتهاء).</span><span class="sxs-lookup"><span data-stu-id="0f810-111">Auto-firming is based on the requirement date (end date).</span></span>
- <span data-ttu-id="0f810-112">للمساعدة على ضمان تأكيد الأوامر في الوقت المناسب، يجب أن يكون الحد الزمني للتأكيد أطول من وقت الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="0f810-112">To help guarantee that orders are firmed in due time, the firming time fence must be longer than the lead time.</span></span>
- <span data-ttu-id="0f810-113">إذا كنت ترغب في تأكيد جميع الأوامر التي يجب أن تبدأ خلال الأسبوع الحالي، فيجب أن يكون الحد الزمني للتأكيد وقت الإنتاج بالإضافة إلى أسبوع واحد.</span><span class="sxs-lookup"><span data-stu-id="0f810-113">If you want to firm all orders that must start during the current week, the firming time fence must be the lead time plus one week.</span></span>


## <a name="set-up-the-firming-time-fence"></a><span data-ttu-id="0f810-114">إعداد الحد الزمني للتأكيد</span><span class="sxs-lookup"><span data-stu-id="0f810-114">Set up the firming time fence</span></span>

<span data-ttu-id="0f810-115">يتم حساب الحد الزمني للتأكيد بداية من تاريخ تشغيل الخطة.</span><span class="sxs-lookup"><span data-stu-id="0f810-115">The firming time fence is calculated forward from the run date of the plan.</span></span> <span data-ttu-id="0f810-116">ويتم تحديده بعدد الأيام التي تم إدخالها.</span><span class="sxs-lookup"><span data-stu-id="0f810-116">It’s defined by the number of days that are entered.</span></span>

<span data-ttu-id="0f810-117">يتم تحديد الحد الزمني للتأكيد أولاً بواسطة مجموعة التغطية في **التخطيط الرئيسي > الإعداد > التغطية > مجموعات التغطية**، في علامة التبويب السريعة **غير ذلك** في الحقل **الحد الزمني للتأكيد التلقائي (الأيام)**.</span><span class="sxs-lookup"><span data-stu-id="0f810-117">The firming time fence is first defined by the coverage group in **Master planning > Setup > Coverage > Coverage groups**, on the **Other** FastTab in the **Automatic firming time fence (days)** field.</span></span>


![ <span data-ttu-id="0f810-118">لقطة شاشة للحقل "الحد الزمني للتأكيد التلقائي (الأيام)".</span><span class="sxs-lookup"><span data-stu-id="0f810-118">Screenshot of Automatic firming time fence (days) field.</span></span> ](../media/auto-firm-time-fence-ssm.png)
 


<span data-ttu-id="0f810-119">يمكن تجاوز عدد الأيام التي تم إدخالها في مجموعة التغطية من خلال تعديل **تغطية الصنف** في الصنف، ثم تحديد **تجاوز الحدود الزمنية**.</span><span class="sxs-lookup"><span data-stu-id="0f810-119">The number of days that are entered in the coverage group can be overridden by modifying the **Item coverage** in the item and then selecting **Override time fences**.</span></span>

![ <span data-ttu-id="0f810-120">لقطة شاشة للحقل "تجاوز الحدود الزمنية".</span><span class="sxs-lookup"><span data-stu-id="0f810-120">Screenshot of the Override time fences field.</span></span>](../media/override-time-fence-ssm.png)



<span data-ttu-id="0f810-121">يمكنك أيضاً تجاوز التغطية الفردية أو تغطية المجموعة بالانتقال إلى الخطة الرئيسية، والانتقال إلى علامة التبويب السريعة **الحدود الزمنية بالأيام** وتعيين **التأكيد** على **نعم**، ثم إدخال الوقت بالأيام.</span><span class="sxs-lookup"><span data-stu-id="0f810-121">You can also override the individual or group coverage by going to the master plan, going to the **Time fences in days** FastTab, setting **Firming** to **Yes**, and then entering the time in days.</span></span> 

![ <span data-ttu-id="0f810-122">لقطة شاشة لعلامة التبويب السريعة "الحدود الزمنية بالأيام".</span><span class="sxs-lookup"><span data-stu-id="0f810-122">Screenshot of the Time fences in days FastTab.</span></span>](../media/firming-time-fence-ssm.png)


<span data-ttu-id="0f810-123">عند تشغيل خطة رئيسية تستخدم "تحسين التخطيط"، يتم تشغيل عملية التأكيد التلقائي وفقاً للإعداد الذي تم تعيينه.</span><span class="sxs-lookup"><span data-stu-id="0f810-123">When a master plan is run that uses Planning Optimization, the auto-firming process is run according to the setup that has been done.</span></span> <span data-ttu-id="0f810-124">وإذا لم يتم تشغيلها، يتم تخطي عملية التأكيد التلقائي.</span><span class="sxs-lookup"><span data-stu-id="0f810-124">If it isn’t turned on, the auto-firming process is skipped.</span></span>

## <a name="run-planning-optimization-with-auto-firming"></a><span data-ttu-id="0f810-125">تشغيل "تحسين التخطيط" مع التأكيد التلقائي</span><span class="sxs-lookup"><span data-stu-id="0f810-125">Run Planning Optimization with auto-firming</span></span>

<span data-ttu-id="0f810-126">لتشغيل "تحسين التخطيط" مع التأكيد التلقائي، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="0f810-126">To run Planning Optimization with auto-firming, follow these steps:</span></span>

1.  <span data-ttu-id="0f810-127">انتقل إلى مساحة عمل **التخطيط الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="0f810-127">Go to the **Master planning** workspace.</span></span>
2.  <span data-ttu-id="0f810-128">في القسم **ملخص الخطة الحالية**، حدد **تشغيل** في الإطار المتجانب **التخطيط الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="0f810-128">In the **Summary of the current plan** section, select **Run** in the **Master planning** tile.</span></span>
3.  <span data-ttu-id="0f810-129">في مربع الحوار **تحسين التخطيط**، عيِّن شريط التمرير الخاص بـ **تمكين التأكيد التلقائي** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="0f810-129">In the **Planning Optimization** dialog box, set the slider for **Enable auto-firming** to **Yes**.</span></span>
4.  <span data-ttu-id="0f810-130">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0f810-130">Select **OK**.</span></span>

    ![ <span data-ttu-id="0f810-131">لقطة شاشة لمربع الحوار "تحسين التخطيط".</span><span class="sxs-lookup"><span data-stu-id="0f810-131">Screenshot of the Planning Optimization dialog box.</span></span>](../media/enable-autofirming-ssm.png)


<span data-ttu-id="0f810-132">شاهد الفيديو الآتي للحصول على عرض توضيحي حول كيفية استخدام التأكيد التلقائي في الأمر المخطط.</span><span class="sxs-lookup"><span data-stu-id="0f810-132">Watch the following video for a demonstration of how to use auto-firming on a planned order.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4Iy7X]

