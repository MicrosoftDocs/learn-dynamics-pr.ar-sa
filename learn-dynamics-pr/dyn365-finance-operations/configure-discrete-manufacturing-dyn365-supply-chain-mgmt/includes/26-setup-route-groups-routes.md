---
ms.openlocfilehash: 948b7d43bcaa5c914c573372dd97600c5d2062dd
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073012"
---
<span data-ttu-id="c1259-101">المسارات هي المسارات التي يسلكها الصنف من عملية إلى عملية، بدءاً من بداية عملية الإنتاج وحتى النهاية.</span><span class="sxs-lookup"><span data-stu-id="c1259-101">Routes are the paths that the item takes from operation to operation, starting with the beginning of the production process and continuing to the end.</span></span> <span data-ttu-id="c1259-102">إنها مجموعة من العمليات أو المهام المتسلسلة المطلوبة لإنتاج أحد الأصناف.</span><span class="sxs-lookup"><span data-stu-id="c1259-102">It is a set of sequential operations, or tasks, that are required to produce an item.</span></span> <span data-ttu-id="c1259-103">يتضمن الموارد والوقت القياسي الذي يستغرقه إعداد العمليات وتشغيلها.</span><span class="sxs-lookup"><span data-stu-id="c1259-103">It includes the resources and the standard time it takes to set up and run the operations.</span></span> <span data-ttu-id="c1259-104">تحدد العمليات على المسار المهام المتضمنة في تصنيع أحد الأصناف، وتشمل التفاصيل اللازمة لجدولة الإنتاج بكفاءة.</span><span class="sxs-lookup"><span data-stu-id="c1259-104">The operations on the route specify the tasks that are involved in manufacturing an item, and include the detail necessary to efficiently schedule production.</span></span>

<span data-ttu-id="c1259-105">يتضمن كل مسار ما يلي:</span><span class="sxs-lookup"><span data-stu-id="c1259-105">Each route includes:</span></span>

-   <span data-ttu-id="c1259-106">العمليات المطلوب تنفيذها</span><span class="sxs-lookup"><span data-stu-id="c1259-106">Operations to be performed</span></span>

-   <span data-ttu-id="c1259-107">تسلسل العمليات</span><span class="sxs-lookup"><span data-stu-id="c1259-107">Sequence of the operations</span></span>

-   <span data-ttu-id="c1259-108">متطلبات الموارد المشاركة في استكمال العمليات</span><span class="sxs-lookup"><span data-stu-id="c1259-108">Resource requirements involved in completing the operations</span></span>

-   <span data-ttu-id="c1259-109">الأوقات القياسية لإعداد وتشغيل الإنتاج</span><span class="sxs-lookup"><span data-stu-id="c1259-109">Standard times for the setup and run of the production</span></span>

<span data-ttu-id="c1259-110">يمكن تعيين مسار مختلف لكل منتج، اعتماداً على المنتج والعملية.</span><span class="sxs-lookup"><span data-stu-id="c1259-110">A different route can be mapped for each product, depending on the product and the process.</span></span> <span data-ttu-id="c1259-111">يمكنك إنشاء مسار جديد تماماً، أو يمكنك إنشاء مسار جديد استناداً إلى معلومات المسار الحالية، ثم تعديل المعلومات أو تحديثها لمطابقة عملية الإنتاج الجديدة.</span><span class="sxs-lookup"><span data-stu-id="c1259-111">You can create an entirely new route, or you can base a new route on existing route information, and then adjust or update the information to match the new production process.</span></span>


## <a name="set-up-route-groups"></a><span data-ttu-id="c1259-112">إعداد مجموعات المسارات</span><span class="sxs-lookup"><span data-stu-id="c1259-112">Set up route groups</span></span>

<span data-ttu-id="c1259-113">تتعلق المحددات المحددة في مجموعة المسار بجميع المسارات في تلك المجموعة.</span><span class="sxs-lookup"><span data-stu-id="c1259-113">The parameters defined on a route group pertain to all routes in that group.</span></span> <span data-ttu-id="c1259-114">تحتاج إلى إعداد مجموعات المسارات قبل إنشاء مسارات الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="c1259-114">You need to set up route groups before creating production routes.</span></span> <span data-ttu-id="c1259-115">يمكن إعداد مجموعات المسار لتحديد:</span><span class="sxs-lookup"><span data-stu-id="c1259-115">Route groups can be set up to define:</span></span>

-   <span data-ttu-id="c1259-116">كيف تحسب التكاليف.</span><span class="sxs-lookup"><span data-stu-id="c1259-116">How costs are calculated.</span></span>

-   <span data-ttu-id="c1259-117">كيف سيتم التخطيط.</span><span class="sxs-lookup"><span data-stu-id="c1259-117">How planning will take place.</span></span>

-   <span data-ttu-id="c1259-118">نوع التعليقات التي تريدها للمجموعة.</span><span class="sxs-lookup"><span data-stu-id="c1259-118">The kind of feedback that you want for the group.</span></span>

-   <span data-ttu-id="c1259-119">كيف يمكن معالجة أنواع الوظائف المختلفة مثل الإعداد والعملية وقائمة الانتظار عند تشغيل جدولة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="c1259-119">How the various job types such as setup, process, and queue can be handled when production scheduling is run.</span></span>

-   <span data-ttu-id="c1259-120">كيف يمكن إدارة الوظائف.</span><span class="sxs-lookup"><span data-stu-id="c1259-120">How jobs can be managed.</span></span>

-   <span data-ttu-id="c1259-121">كيف يجب تطبيق تقويم وقت العمل والتفاصيل المتعلقة بحجز القدرة الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="c1259-121">How the working time calendar and details regarding capacity reservation must be applied.</span></span>


## <a name="set-up-routes"></a><span data-ttu-id="c1259-122">إعداد المسارات</span><span class="sxs-lookup"><span data-stu-id="c1259-122">Set up routes</span></span>

<span data-ttu-id="c1259-123">عند إعداد معلومات التوجيه الخاصة بالعميل، حدد كيفية إدارة المسارات والعمليات مع مراعاة الاعتبارات التالية:</span><span class="sxs-lookup"><span data-stu-id="c1259-123">When you set up a customer's routing information, determine how to manage the routes and operations with the following considerations:</span></span>

-   <span data-ttu-id="c1259-124">إذا كان تصنيع العميل يتكون من عدد محدود فقط من المسارات العامة.</span><span class="sxs-lookup"><span data-stu-id="c1259-124">If the customer's manufacturing consists of only a limited number of generic routes.</span></span>

-   <span data-ttu-id="c1259-125">ما إذا كانت مجموعة بسيطة من المسارات تفي باحتياجات العميل.</span><span class="sxs-lookup"><span data-stu-id="c1259-125">Whether a simple set of routes satisfy the customer's needs.</span></span>

-   <span data-ttu-id="c1259-126">ضرورة استخدام شبكات المسارات أو غيرها من المسارات المعقدة.</span><span class="sxs-lookup"><span data-stu-id="c1259-126">The necessity of using route networks or other complex routing.</span></span>

-   <span data-ttu-id="c1259-127">إذا كانت هناك منتجات متعددة تشترك في المسارات عن طريق مجموعات الأصناف.</span><span class="sxs-lookup"><span data-stu-id="c1259-127">If multiple products share the routes by way of item groups.</span></span>

-   <span data-ttu-id="c1259-128">إذا كان العميل سيستفيد من استخدام مفهوم إصدار المسار.</span><span class="sxs-lookup"><span data-stu-id="c1259-128">If the customer will benefit from using the route version concept.</span></span>

-   <span data-ttu-id="c1259-129">إذا طلب العميل مسارات متعددة لنفس الصنف.</span><span class="sxs-lookup"><span data-stu-id="c1259-129">If the customer requires multiple routes for the same item.</span></span>

-   <span data-ttu-id="c1259-130">التحكم في أن إصدار المسار النشط بناءً على "إلى تاريخ" وكذلك "من تاريخ" يعمل بالنسبة للعميل.</span><span class="sxs-lookup"><span data-stu-id="c1259-130">Controlling that the active route version based on the To date and From date works for the customer.</span></span>


<span data-ttu-id="c1259-131">يعني إنشاء مجموعات المسار أنه تم إعداد المحددات للمجموعة بأكملها بدلاً من كل مسار فردي.</span><span class="sxs-lookup"><span data-stu-id="c1259-131">The creation of route groups means that parameters are set up for the entire group rather than for each individual route.</span></span> <span data-ttu-id="c1259-132">يمكنك تحديد تعليقات تلقائية حول العمليات الحسابية والمحددات الأخرى في مجموعة مسار، أو تحديد أنواع الوظائف المرتبطة بالجدولة وإدارة الوظائف ووقت التشغيل والقدرة.</span><span class="sxs-lookup"><span data-stu-id="c1259-132">You can specify automatic feedback on calculations and other parameters in a route group, or define job types that are related to scheduling, job management, operation time, and capacity.</span></span>

<span data-ttu-id="c1259-133">يمكنك أن تحدد في مجموعة المسارات أنه يجب استيفاء الشروط التالية عند تشغيل جدول الوظيفة:</span><span class="sxs-lookup"><span data-stu-id="c1259-133">You can specify on the route group that the following conditions must be met when a job schedule is run:</span></span>

-   <span data-ttu-id="c1259-134">تأخذ جدولة الوظائف في الاعتبار نوع الوظيفة الحالية.</span><span class="sxs-lookup"><span data-stu-id="c1259-134">Job scheduling considers the current job type.</span></span>

-   <span data-ttu-id="c1259-135">تستخدم إدارة الوظائف نوع الوظيفة الحالي.</span><span class="sxs-lookup"><span data-stu-id="c1259-135">Job management uses the current job type.</span></span>
-   <span data-ttu-id="c1259-136">يتم احتساب وقت العملية على أساس التقويم الميلادي.</span><span class="sxs-lookup"><span data-stu-id="c1259-136">Operation time is calculated based on the Gregorian calendar.</span></span>

-   <span data-ttu-id="c1259-137">نوع الوظيفة يحتفظ بالقدرة فيما يتعلق بجدولة الوظيفة.</span><span class="sxs-lookup"><span data-stu-id="c1259-137">The job type reserves capacity in connection with job scheduling.</span></span>

-   <span data-ttu-id="c1259-138">يجب تحديد مجموعات التوجيه وفئات التكلفة والعمليات كمتطلبات أساسية لإنشاء المسارات.</span><span class="sxs-lookup"><span data-stu-id="c1259-138">You must define routing groups, cost categories, and operations as prerequisites to the creation of routes.</span></span>

-   <span data-ttu-id="c1259-139">يجب عليك إعداد المحددات قبل استخدام شبكة معقدة.</span><span class="sxs-lookup"><span data-stu-id="c1259-139">You should set up parameters before you use a complex network.</span></span>

-   <span data-ttu-id="c1259-140">إذا كان المسار يحتوي على أنواع مختلفة من العمليات، فيمكن تعيينه لأكثر من مجموعة توجيه واحدة في نفس الوقت.</span><span class="sxs-lookup"><span data-stu-id="c1259-140">If a route contains different kinds of operations, it can be assigned to more than one routing group at the same time.</span></span>
