---
ms.openlocfilehash: 7b3a4ef2d7e0e00bd61316a0f70578f130e69785
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072380"
---
<span data-ttu-id="af9b2-101">لإجراء اختبارات قبول المستخدم، ستحتاج إلى إنشاء خطة اختبار ومجموعة اختبارات في Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="af9b2-101">To run your user acceptance tests, you will need to create a test plan and test suite in Azure DevOps.</span></span> <span data-ttu-id="af9b2-102">وسيسمح لك هذا بإجراء مجموعة منظمة من حالات الاختبار وإدارة النتائج والاستقصاء عنها وتعقبها بسهولة.</span><span class="sxs-lookup"><span data-stu-id="af9b2-102">This will allow you to run an ordered suite of test cases and easily manage, investigate, and track the results.</span></span>

1.  <span data-ttu-id="af9b2-103">سجِّل الدخول إلى Azure DevOps وحدد المشروع وخطة الاختبار التي تود اتباعها لإجراء الاختبار.</span><span class="sxs-lookup"><span data-stu-id="af9b2-103">Sign in to Azure DevOps and select the project and test plan that you want to test in.</span></span>

2.  <span data-ttu-id="af9b2-104">في شريط الأدوات، حدد **الاختبار> خطط الاختبارات**.</span><span class="sxs-lookup"><span data-stu-id="af9b2-104">On the toolbar, select **Test > Test Plans**.</span></span>

3.  <span data-ttu-id="af9b2-105">في الجزء الأيسر، حدد القائمة المنسدلة بجوار علامة زائد الخضراء **+** ثم حدد **مجموعة ثابتة**.</span><span class="sxs-lookup"><span data-stu-id="af9b2-105">On the left pane, select the drop-down next to the green plus **+** sign and then select **Static suite**.</span></span>

4.  <span data-ttu-id="af9b2-106">أدخل اسماً للمجموعة.</span><span class="sxs-lookup"><span data-stu-id="af9b2-106">Enter a name for the suite.</span></span>

5.  <span data-ttu-id="af9b2-107">حدد **إضافة الحالي** وقم بالاستعلام عن العلامة **LCS: حالات الاختبار**.</span><span class="sxs-lookup"><span data-stu-id="af9b2-107">Select **Add existing** and query the tag **LCS:Test Cases**.</span></span>

6.  <span data-ttu-id="af9b2-108">حدد **إجراء > إضافة حالات اختبار**.</span><span class="sxs-lookup"><span data-stu-id="af9b2-108">Select **Run > Add test cases**.</span></span>

7.  <span data-ttu-id="af9b2-109">حدد حالة الاختبار لعرض التفاصيل وملف XML المرفق.</span><span class="sxs-lookup"><span data-stu-id="af9b2-109">Select the test case to view details and the attached XML file.</span></span>

<span data-ttu-id="af9b2-110">أنشئ مجموعات اختبارات متنوعة ضمن خطة الاختبار نفسها ثم استخدم الاستعلامات المخصصة لإضافة حالات اختبار معينة إلى مجموعة الاختبارات.</span><span class="sxs-lookup"><span data-stu-id="af9b2-110">Create various test suites under the same test plan and then use custom queries to add specific test cases to a test suite.</span></span> <span data-ttu-id="af9b2-111">يمكن أن تنتمي حالة الاختبار إلى أكثر من مجموعة اختبارات واحدة.</span><span class="sxs-lookup"><span data-stu-id="af9b2-111">A test case can belong to more than one test suite.</span></span>

### <a name="run-manual-test-cases"></a><span data-ttu-id="af9b2-112">إجراء حالات الاختبارات اليدوية</span><span class="sxs-lookup"><span data-stu-id="af9b2-112">Run manual test cases</span></span>

<span data-ttu-id="af9b2-113">إذا كان لديك مجموعة اختبارات، فستكون جاهزاً لاستخدامها في اختبار الانحدار بعد إجراء تحديثات في استمارة تقديم تطبيقات Finance and Operations في بيئة اختبار معزولة أو بيئة اختبار.</span><span class="sxs-lookup"><span data-stu-id="af9b2-113">When you have a test suite, you are ready to use it for regression testing after updates have been made to your Finance and Operations apps application in a sandbox or test environment.</span></span> <span data-ttu-id="af9b2-114">يمكنك إجراء حالات الاختبار في مجموعة اختبارات يدوياً.</span><span class="sxs-lookup"><span data-stu-id="af9b2-114">You can run the test cases in your test suite manually.</span></span> <span data-ttu-id="af9b2-115">بدلاً من ذلك، يمكنك تشغيل تسجيلات المهام التي تعد جزءاً من مجموعة الاختبارات واستخدام Azure DevOps لتوضيح حالات الاختبار على أنها "تم الاجتياز" أو "تم الرسوب".</span><span class="sxs-lookup"><span data-stu-id="af9b2-115">Alternatively, you can play the task recordings that are part of the test suite and use Azure DevOps to denote the test cases as passed or failed.</span></span>

![لقطة شاشة لحقل نتائج الاختبارات اليدوية.](../media/manual-tests.png)

<span data-ttu-id="af9b2-117">كما يوفر Azure DevOps أداة، تسمى "Test Runner"، لإدارة عمليات تشغيل حالات الاختبارات اليدوية.</span><span class="sxs-lookup"><span data-stu-id="af9b2-117">Azure DevOps also provides a tool, named Test Runner, to manage manual test case runs.</span></span> <span data-ttu-id="af9b2-118">للحصول علي مزيد من المعلومات حول استخدام أداة "Test Runner"، راجع [تشغيل الاختبارات اليدوية](https://docs.microsoft.com/azure/devops/test/run-manual-tests?view=azure-devops/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="af9b2-118">For more information about using Test Runner, see [Run manual tests](https://docs.microsoft.com/azure/devops/test/run-manual-tests?view=azure-devops/?azure-portal=true).</span></span>

<span data-ttu-id="af9b2-119">نوصيك بالاستفادة من Azure DevOps لأنه يوفر مجموعة ثرية من ميزات الإدارة التي ليست للاختبار فقط ولكن لإدارة النتائج وتخفيف المخاطر أيضاً .</span><span class="sxs-lookup"><span data-stu-id="af9b2-119">We recommend that you take advantage of Azure DevOps because it provides a rich set of management features that are not only for testing but also for result management and mitigation.</span></span>

### <a name="run-automated-test-cases"></a><span data-ttu-id="af9b2-120">إجراء حالات الاختبارات اليدوية</span><span class="sxs-lookup"><span data-stu-id="af9b2-120">Run automated test cases</span></span>

<span data-ttu-id="af9b2-121">يوفر النظام الأساسي Dynamics 365 Unified Operations للمطورين أدوات لكتابة حالات اختبار استناداً إلى تسجيلات المهام واستخدام Azure DevOps لإدارة التشغيل التلقائي لحالات الاختبارات هذه.</span><span class="sxs-lookup"><span data-stu-id="af9b2-121">The Dynamics 365 Unified Operations platform provides developers with tools to write test cases based on task recordings and use Azure DevOps to manage the automated running of these test cases.</span></span>

<span data-ttu-id="af9b2-122">ويمكن للمطورين استخدام إمكانات البناء وأتمتة الاختبارات لبيئات البناء والاختبارات.</span><span class="sxs-lookup"><span data-stu-id="af9b2-122">Developers can use the build and test automation capabilities of build and test environments.</span></span> <span data-ttu-id="af9b2-123">لمزيد من المعلومات، راجع [الصفحة الرئيسية "التسليم المستمر"](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/continuous-delivery-home-page/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="af9b2-123">For more information, see [Continuous delivery home page](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/continuous-delivery-home-page/?azure-portal=true).</span></span>

<span data-ttu-id="af9b2-124">تعمل Regression Suite Automation Tool (RSAT) على خفض الوقت والتكلفة لاختبارات قبول المستخدم (UAT) بشكلٍ ملحوظ.</span><span class="sxs-lookup"><span data-stu-id="af9b2-124">The Regression Suite Automation Tool (RSAT)significantly reduces the time and cost of user acceptance testing (UAT).</span></span> <span data-ttu-id="af9b2-125">كما تتيح RSAT لمستخدمي الطاقة الوظيفية تسجيل مهام العمل باستخدام "مسجل المهام" ثم تحويل التسجيلات إلى مجموعة من الاختبارات المؤتمتة دون الحاجة إلى كتابة كود مصدر.</span><span class="sxs-lookup"><span data-stu-id="af9b2-125">RSAT lets functional power users record business tasks by using Task recorder and then convert the recordings into a suite of automated tests, without having to write source code.</span></span> <span data-ttu-id="af9b2-126">تعد RSAT متكاملة تماماً مع Microsoft Azure DevOps لتنفيذ الاختبارات وإعداد التقارير والتحقق.</span><span class="sxs-lookup"><span data-stu-id="af9b2-126">RSAT is fully integrated with Microsoft Azure DevOps for test execution, reporting, and investigation.</span></span> <span data-ttu-id="af9b2-127">يتم إلغاء إقران معلمات الاختبارات من خطوات الاختبارات وتخزينها في ملفات بتنسيق Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="af9b2-127">Test parameters are decoupled from test steps and stored in Microsoft Excel files.</span></span>

<span data-ttu-id="af9b2-128">تنزيل الأداة ودليل المستخدم من تطبيقات [Finance and Operations، Regression Suite Automation Tool](https://www.microsoft.com/download/details.aspx?id=57357).</span><span class="sxs-lookup"><span data-stu-id="af9b2-128">Download the tool and user manual from [Finance and Operations apps, Regression Suite Automation Tool](https://www.microsoft.com/download/details.aspx?id=57357).</span></span>

<span data-ttu-id="af9b2-129">لمعرفة كيفية إنشاء خطة اختبار في Azure DevOps لاستخدامها مع الأداة "RSAT"، شاهد هذا الفيديو.</span><span class="sxs-lookup"><span data-stu-id="af9b2-129">To see how to create a test plan in Azure DevOps to use with RSAT, watch this video.</span></span>
 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4vx0I]

<span data-ttu-id="af9b2-130">لمعرفة كيفية استخدام الأداة "RSAT"، شاهد هذا الفيديو:</span><span class="sxs-lookup"><span data-stu-id="af9b2-130">To see how to use RSAT, watch this video:</span></span>
 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4vl8Z]

### <a name="investigate-test-runs"></a><span data-ttu-id="af9b2-131">التحقق من عمليات تشغيل الاختبارات</span><span class="sxs-lookup"><span data-stu-id="af9b2-131">Investigate test runs</span></span>

<span data-ttu-id="af9b2-132">عند اكتمال التشغيل المؤتمت، في شريط أدوات Azure DevOps، حدد **اختبار > عمليات التشغيل** (أو **خطط الاختبارات > عمليات التشغيل**) للتحقق من تشغيل الاختبار.</span><span class="sxs-lookup"><span data-stu-id="af9b2-132">When an automated run is complete, on the Azure DevOps toolbar, select **Test > Runs** (or **Test Plans > Runs**) to investigate your test run.</span></span> <span data-ttu-id="af9b2-133">حدد تشغيل الاختبار المطلوب للتحقق من حالات فشل حالات الاختبار وأخطائها.</span><span class="sxs-lookup"><span data-stu-id="af9b2-133">Select the desired test run to investigate test case failures and errors.</span></span>

<span data-ttu-id="af9b2-134">يمكنك أيضاً الانتقال إلى مجموعة الاختبارات في Azure DevOps للاطلاع على أحدث النتائج المقترنة مع حالات الاختبار لديك.</span><span class="sxs-lookup"><span data-stu-id="af9b2-134">You can also go to your test suite in Azure DevOps to see the latest results that are associated with your test cases.</span></span>

<span data-ttu-id="af9b2-135">لمزيد من المعلومات حول الاختبارات وإدارتها في Azure DevOps، راجع مستندات [Azure DevOps](https://docs.microsoft.com/azure/devops/?view=azure-devops/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="af9b2-135">For more information on testing and test management in Azure DevOps, see [Azure DevOps documentation](https://docs.microsoft.com/azure/devops/?view=azure-devops/?azure-portal=true).</span></span>