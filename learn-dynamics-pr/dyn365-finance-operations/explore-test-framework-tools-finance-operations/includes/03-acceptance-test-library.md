---
ms.openlocfilehash: 9fa17cffbd1806574e18ad60e3f8be0c1af0cb6f
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072272"
---

<span data-ttu-id="b6f6c-101">مكتبة اختبار القبول (ATL) هي مكتبة اختبار X++‎ التي تسمح للمطورين بإنشاء بيانات اختبار متسقة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-101">The Acceptance test library (ATL) is an X++ test library that allows developers to create consistent test data.</span></span> <span data-ttu-id="b6f6c-102">فهي تجعل كود الاختبار أكثر قابلية للقراءة، ويصبح اكتشاف الطرق التي تنشئ بيانات الاختبار أكثر سهولة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-102">It makes test code more readable, and methods that create test data become more easily discovered.</span></span> <span data-ttu-id="b6f6c-103">تدعم ATL أيضاً الأداء العالي لحالات الاختبار.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-103">ATL also supports high performance of test cases.</span></span> <span data-ttu-id="b6f6c-104">يمكنك استخدام الفئات داخل ATL لإنشاء اختبارات قابلة للتكرار من شأنها كتابة بيانات الاختبار وتشغيل العمليات باستخدام تلك البيانات.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-104">You can use the classes within the ATL to create repeatable tests that will write test data and run processes by using that data.</span></span> <span data-ttu-id="b6f6c-105">يمكن لهذه الميزة تبسيط بعض عمليات إعداد البيانات الأكثر تعقيداً والعمليات التي ستكون مطلوبة للاختبار من خلال واجهة المستخدم (UI).</span><span class="sxs-lookup"><span data-stu-id="b6f6c-105">This feature can simplify some of the more complicated data setup and processes that would be required testing through the user interface (UI).</span></span>

<span data-ttu-id="b6f6c-106">عند إنشاء الفئات والطرق في ATL، يتعين عليك اتباع هيكلة وتسمية صارمة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-106">When creating classes and methods in ATL, you must follow rigid structuring and naming.</span></span> <span data-ttu-id="b6f6c-107">يتم تجميع الفئات في المفاهيم التالية:</span><span class="sxs-lookup"><span data-stu-id="b6f6c-107">Classes are grouped into the following concepts:</span></span>

-   <span data-ttu-id="b6f6c-108">**التنقل** - اكتشاف الكيانات و‏‫أساليب بيانات الاختبار‬.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-108">**Navigation** - Discover entities and test data methods.</span></span>
-   <span data-ttu-id="b6f6c-109">**أساليب بيانات الاختبار** - تُستخدم هذه الطرق لإعداد بيانات الاختبار.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-109">**Test data methods** - These methods are used to set up test data.</span></span>
-   <span data-ttu-id="b6f6c-110">**الكيانات** - تمثيل البيانات والسلوك المرتبط بها والذي يُنظر إليه على أنه وحدة واحدة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-110">**Entities** - Represent data and associated behavior that is perceived as a single unit.</span></span>
-   <span data-ttu-id="b6f6c-111">**المنشئون** - يتيحون لك إنشاء بيانات اختبار محددة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-111">**Creators** - Let you create specific test data.</span></span>
-   <span data-ttu-id="b6f6c-112">**الأوامر** - تشغيل عمليات الأعمال.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-112">**Commands** - Run business operations.</span></span>
-   <span data-ttu-id="b6f6c-113">**الاستعلامات** - البحث عن الكيانات.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-113">**Queries** - Find entities.</span></span>
-   <span data-ttu-id="b6f6c-114">**المواصفات** - وصف الكيانات المتوقعة في نهاية الاختبار.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-114">**Specifications** - Describe expected entities at the end of the test.</span></span>
 
<span data-ttu-id="b6f6c-115">يقوم منشئ أكواد ATL بإنشاء وتحديث كيانات واستعلامات ومواصفات ATL جديدة سريعاً استناداً إلى الجداول وكيانات البيانات.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-115">The ATL code generator quickly creates and updates new ATL entities, queries, and specifications based on tables and data entities.</span></span>


![لقطة شاشة لصفحة إنشاء الكيان البديل.](../media/alt.png)

<span data-ttu-id="b6f6c-117">تساعدك الخطوات التالية في إنشاء فئة كيان ATL باستخدام إنشاء الكود:</span><span class="sxs-lookup"><span data-stu-id="b6f6c-117">The following steps help you create an ATL entity class by using the code generation:</span></span>

1.  <span data-ttu-id="b6f6c-118">في Visual Studio، افتح الجدول الذي تريد استخدامه في نافذة المصمم.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-118">In Visual Studio, open the table you want to use in the Designer window.</span></span>
2.  <span data-ttu-id="b6f6c-119">في قائمة **الوظائف الإضافية**، حدد **إنشاء كيان ATL**.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-119">On the **Addins** menu, select **Generate ATL Entity**.</span></span>
3.  <span data-ttu-id="b6f6c-120">حدد الحقول التي يجب تضمينها في فئة كيان ATL.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-120">Select the fields that should be included in the ATL Entity class.</span></span>
4.  <span data-ttu-id="b6f6c-121">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-121">Select **Add**.</span></span>
5.  <span data-ttu-id="b6f6c-122">أعد تسمية الكيان والحقول حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-122">Rename the entity and fields as needed.</span></span>
6.  <span data-ttu-id="b6f6c-123">حدد **إنشاء** لإنشاء الفئة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-123">Select **Generate** to create the class.</span></span>

<span data-ttu-id="b6f6c-124">لإنشاء فئة استعلام ATL باستخدام المعالج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b6f6c-124">To create an ATL query class by using the wizard, follow these steps:</span></span>

1.  <span data-ttu-id="b6f6c-125">في Visual Studio، افتح الجدول الذي تريد استخدامه في نافذة المصمم.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-125">In Visual Studio, open the table you want to use in the Designer window.</span></span>
2.  <span data-ttu-id="b6f6c-126">في قائمة **الوظائف الإضافية**، حدد **إنشاء استعلام ATL**.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-126">On the **Addins** menu, select **Generate ATL Query**.</span></span>
3.  <span data-ttu-id="b6f6c-127">حدد الحقول والعلاقات التي يجب تضمينها في فئة استعلام ATL.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-127">Select the fields and relations that should be included in the ATL Query class.</span></span>
4.  <span data-ttu-id="b6f6c-128">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-128">Select **Add**.</span></span>
5.  <span data-ttu-id="b6f6c-129">أعد تسمية الكيان والحقول والعلاقات حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-129">Rename the entity, fields, and the relations as needed.</span></span>
6.  <span data-ttu-id="b6f6c-130">حدد **إنشاء** لإنشاء الفئة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-130">Select **Generate** to create the class.</span></span>

<span data-ttu-id="b6f6c-131">لإنشاء فئة مواصفات ATL باستخدام المعالج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b6f6c-131">To create an ATL Specification class by using the wizard, follow these steps:</span></span>

1.  <span data-ttu-id="b6f6c-132">في Visual Studio، افتح الجدول الذي تريد استخدامه في نافذة المصمم.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-132">In Visual Studio, open the table you want to use in the Designer window.</span></span>
2.  <span data-ttu-id="b6f6c-133">في قائمة **الوظائف الإضافية**، حدد **إنشاء مواصفات ATL**.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-133">On the **Addins** menu, select **Generate ATL Specification**.</span></span>
3.  <span data-ttu-id="b6f6c-134">حدد الحقول التي يجب تضمينها في فئة مواصفات ATL.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-134">Select the fields that should be included in the ATL Specification class.</span></span>
4.  <span data-ttu-id="b6f6c-135">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-135">Select **Add**.</span></span>
5.  <span data-ttu-id="b6f6c-136">أعد تسمية الكيان والمواصفات حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-136">Rename the specification and fields as needed.</span></span>
6.  <span data-ttu-id="b6f6c-137">حدد **إنشاء** لإنشاء الفئة.</span><span class="sxs-lookup"><span data-stu-id="b6f6c-137">Select **Generate** to create the class.</span></span>


<span data-ttu-id="b6f6c-138">لمعرفة المزيد حول مكتبة اختبار القبول (ATL)، انتقل إلى [موارد مكتبة اختبار القبول](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/perf-test/acceptance-test-library/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="b6f6c-138">To learn more about the Acceptance test library (ATL), go to  [Acceptance test library resources](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/perf-test/acceptance-test-library/?azure-portal=true).</span></span>
