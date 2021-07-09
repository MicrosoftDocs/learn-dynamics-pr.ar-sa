---
ms.openlocfilehash: 1e535d8b3b60b590709e7073af4a3dd3efac175f
ms.sourcegitcommit: 7d4cc5f2048fa309552e39da447684b1d06d0772
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/13/2021
ms.locfileid: "6072453"
---
<span data-ttu-id="eaa03-101">إذا كان لديك إصدار سابق من Finance and Operations، مثل 7.0 (RTW) أو 7.1 (1611) أو 7.2 (يوليو‬ 2017) أو 7.3، فيمكنك تطبيق ترقية الخدمة الذاتية دون تبعيات على دعم Microsoft.</span><span class="sxs-lookup"><span data-stu-id="eaa03-101">If you have a previous version of Finance and Operations, such as 7.0 (RTW), 7.1 (1611), 7.2 (July 2017), or 7.3, you can apply a self-service upgrade with no dependencies on Microsoft support.</span></span> 

<span data-ttu-id="eaa03-102">استخدم ميزة ترقية الخدمة الذاتية في LCS لترقية بيئات التطوير والاختبار المعزولة والتشغيل.</span><span class="sxs-lookup"><span data-stu-id="eaa03-102">Use the LCS upgrade self-service feature to upgrade the development, sandbox, and production environments.</span></span> 

 ![لقطة شاشة لصفحة ترقية الخدمة الذاتية في LCS.](../media/7x-code-upgrade.png)

## <a name="process-to-upgrade"></a><span data-ttu-id="eaa03-104">عملية الترقية</span><span class="sxs-lookup"><span data-stu-id="eaa03-104">Process to upgrade</span></span> 

<span data-ttu-id="eaa03-105">يمكنك تقسيم عملية الترقية إلى مراحل.</span><span class="sxs-lookup"><span data-stu-id="eaa03-105">You could divide the upgrade process into phases.</span></span> <span data-ttu-id="eaa03-106">المرحلة الأولى هي التحليل، والتي ستُكمل فيها المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="eaa03-106">The first phase is Analysis, where you will complete the following tasks:</span></span>

1.  <span data-ttu-id="eaa03-107">تجميد التعليمات البرمجية (نقل أحدث تعليمات برمجية إلى الفرع Trunk/Main).</span><span class="sxs-lookup"><span data-stu-id="eaa03-107">Freeze your code (move the latest code to the Trunk/Main branch).</span></span>
2.  <span data-ttu-id="eaa03-108">الحصول على الإصدار الأخير من تعليمات ISV البرمجية (إن أمكن).</span><span class="sxs-lookup"><span data-stu-id="eaa03-108">Obtain the latest version of ISV code (if applicable).</span></span>
3.  <span data-ttu-id="eaa03-109">تشغيل ترقية كود الإصدار الأخير في LCS.</span><span class="sxs-lookup"><span data-stu-id="eaa03-109">Run the latest version code upgrade in LCS.</span></span>
4.  <span data-ttu-id="eaa03-110">نشر الإصدار الأخير في بيئة التطوير.</span><span class="sxs-lookup"><span data-stu-id="eaa03-110">Deploy the latest version in the development environment.</span></span>
5.  <span data-ttu-id="eaa03-111">تحليل تراكب الطبقات لنقاط الملحق.</span><span class="sxs-lookup"><span data-stu-id="eaa03-111">Analyze overlayering for extension points.</span></span>
6.  <span data-ttu-id="eaa03-112">طلب نقاط الملحق المطلوبة في LCS.</span><span class="sxs-lookup"><span data-stu-id="eaa03-112">Request required extension points in LCS.</span></span> 
7.  <span data-ttu-id="eaa03-113">الحصول على نقاط الملحق الجديدة من تحديث Microsoft الشهري.</span><span class="sxs-lookup"><span data-stu-id="eaa03-113">Receive the new extension points from Microsoft’s monthly update.</span></span>
8.  <span data-ttu-id="eaa03-114">إنشاء خطة مشروع.</span><span class="sxs-lookup"><span data-stu-id="eaa03-114">Create a project plan.</span></span>

<span data-ttu-id="eaa03-115">تذكّر الاعتبارات والمهام التالية لمرحلة التحليل:</span><span class="sxs-lookup"><span data-stu-id="eaa03-115">Keep in mind the following considerations and tasks for the Analysis phase:</span></span> 

- <span data-ttu-id="eaa03-116">إذا كنت تستخدم عدة فروع، فتأكد من أن الكود النهائي لديك موجود في الفرع Trunk/Main قبل تشغيل ترقية الكود.</span><span class="sxs-lookup"><span data-stu-id="eaa03-116">If you use multiple branches, make sure that your final code is in the Trunk/Main branch before you run the code upgrade.</span></span>

- <span data-ttu-id="eaa03-117">مراجعة علامة التبويب **RemainingOverlayering** في تقرير **MigrationSummary.xlsx_ExcelReport** من ترقية الكود.</span><span class="sxs-lookup"><span data-stu-id="eaa03-117">Review the **RemainingOverlayering** tab in the **MigrationSummary.xlsx_ExcelReport** report from the code upgrade.</span></span> 
  
    <span data-ttu-id="eaa03-118">[![لقطة شاشة لعملية ترقية الكود في التقرير المعروض.](../media/code-upgrade.process.png)](../media/code-upgrade.process.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="eaa03-118">[![Screenshot of the Code upgrade process with the report displayed.](../media/code-upgrade.process.png)](../media/code-upgrade.process.png#lightbox)</span></span>

-   <span data-ttu-id="eaa03-119">مراجعة المستندات من أجل الإصلاحات العاجلة التي يجب عليك تثبيتها في البيئة المصدر لديك، وذلك وفقاً للإصدار الذي تتم الترقية منه.</span><span class="sxs-lookup"><span data-stu-id="eaa03-119">Review the docs for the hotfixes that you must install in your source environment, depending on the version that you're upgrading from.</span></span>
-   <span data-ttu-id="eaa03-120">تشغيل ترقية الكود في LCS والحصول على تقدير جهد ترقية الكود.</span><span class="sxs-lookup"><span data-stu-id="eaa03-120">Run the code upgrade in LCS and get the estimate for the code upgrade effort.</span></span>
-   <span data-ttu-id="eaa03-121">تعيين الإصدار الأخير من بيئة التطوير لديك إلى فرع الإصدار الذي تم إنشاؤه من خلال ترقية الكود:</span><span class="sxs-lookup"><span data-stu-id="eaa03-121">Map the latest version of your development environment to  the release branch that was created by the code upgrade:</span></span> 
    1.  <span data-ttu-id="eaa03-122">استنساخ تعريف البنية الموجود الذي تم إنشاؤه من أجل **Trunk > Main**.</span><span class="sxs-lookup"><span data-stu-id="eaa03-122">Clone the existing build definition that was created for **Trunk > Main**.</span></span> 
    2.  <span data-ttu-id="eaa03-123">تحديث الحقلين **تعيين** و **حماية** في معلمة **الحصول على مصادر** لمطابقة فرع الإصدار.</span><span class="sxs-lookup"><span data-stu-id="eaa03-123">Update **Map** and **Cloak** fields in the **Get Sources** parameter to match the release branch.</span></span> 
    3.  <span data-ttu-id="eaa03-124">نسخ **AXModulesBuild.proj** من الفرع **الرئيسي** إلى فرع **الإصدار**.</span><span class="sxs-lookup"><span data-stu-id="eaa03-124">Copy **AXModulesBuild.proj** from the **Main** branch to the **Release** branch.</span></span> 
    4.  <span data-ttu-id="eaa03-125">تحديث معلمة **المشروع** ضمن **إنشاء الحل** للإشارة إلى المشروع الذي تم نسخه.</span><span class="sxs-lookup"><span data-stu-id="eaa03-125">Update the **Project** parameter under **Build the solution** to refer to the copied project.</span></span> 
    5.  <span data-ttu-id="eaa03-126">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="eaa03-126">Select **Save**.</span></span> <span data-ttu-id="eaa03-127">والآن حان الوقت لإنشاء حزمة جديدة قابلة للنشر.</span><span class="sxs-lookup"><span data-stu-id="eaa03-127">Now, it is time to build a new deployable package.</span></span>

-   <span data-ttu-id="eaa03-128">بالنسبة إلى تراكب الطبقات، سيتعيّن عليك تسجيل طلبات قابلية التوسعة لإعلام Microsoft بما تحتاجه.</span><span class="sxs-lookup"><span data-stu-id="eaa03-128">For overlayering, you will need to log extensibility requests to inform Microsoft of what you need.</span></span> <span data-ttu-id="eaa03-129">تأكد من بيان التفاصيل عند إنشاء طلبات قابلية التوسعة الخاصة بك لأنها ستصبح تصميماً من أجل التغيير.</span><span class="sxs-lookup"><span data-stu-id="eaa03-129">Make sure that you are detailed when creating your extensibility requests because they will become a design for the changes.</span></span> <span data-ttu-id="eaa03-130">يمكنك قراءة المزيد في [تسجيل طلبات قابلية التوسعة لـ Dynamics 365 Finance and Operations (الإصدار 8)](https://community.dynamics.com/365/financeandoperations/b/mfp/posts/logging-extensibility-requests-for-dynamics-365-finance-and-operations-v8-0/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="eaa03-130">You can read more in [Logging extensibility requests for Dynamics 365 Finance and Operations (V8)](https://community.dynamics.com/365/financeandoperations/b/mfp/posts/logging-extensibility-requests-for-dynamics-365-finance-and-operations-v8-0/?azure-portal=true).</span></span>

<span data-ttu-id="eaa03-131">أما المرحلة التالية في عملية الترقية، فهي **التنفيذ**، والتي ستقوم فيها بأداء الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="eaa03-131">The next phase in the upgrade process is **Execute**, where you will perform the following steps:</span></span> 

1.  <span data-ttu-id="eaa03-132">تثبيت التحديث الشهري الذي يتضمن نقاط الملحق الجديدة.</span><span class="sxs-lookup"><span data-stu-id="eaa03-132">Install the monthly update that includes the new extension points.</span></span> 
2.  <span data-ttu-id="eaa03-133">نقل الكود المتراكب إلى الملحقات.</span><span class="sxs-lookup"><span data-stu-id="eaa03-133">Move overlayered code to extensions.</span></span> 
3.  <span data-ttu-id="eaa03-134">إجراء **تسجيل الكود النهائي** في عنصر التحكم بالمصادر.</span><span class="sxs-lookup"><span data-stu-id="eaa03-134">Perform the **Final code check-in** to source control.</span></span> 
4.  <span data-ttu-id="eaa03-135">إجراء ترقية البيانات في بيئة التطوير.</span><span class="sxs-lookup"><span data-stu-id="eaa03-135">Perform data upgrade in a development environment.</span></span> 
5.  <span data-ttu-id="eaa03-136">استخدام أحدث إصدار من بيئة الإنشاء من أجل إنشاء حزمة قابلة للنشر.</span><span class="sxs-lookup"><span data-stu-id="eaa03-136">Use a latest version build environment to generate a deployable package.</span></span> 
6.  <span data-ttu-id="eaa03-137">إجراء **ترقية بيانات** الخدمة الذاتية في بيئة الاختبار المعزولة‬.</span><span class="sxs-lookup"><span data-stu-id="eaa03-137">Perform a self-service **Data upgrade** on the sandbox.</span></span> 

<span data-ttu-id="eaa03-138">النقاط الرئيسية التي تجب مراعاتها في مرحلة التنفيذ:</span><span class="sxs-lookup"><span data-stu-id="eaa03-138">Key points to consider in the Execute phase:</span></span> 

-   <span data-ttu-id="eaa03-139">ستوفر Microsoft نقاط الملحق الجديدة في تحديث شهري.</span><span class="sxs-lookup"><span data-stu-id="eaa03-139">Microsoft will deliver the new extension points in a monthly update.</span></span>
-   <span data-ttu-id="eaa03-140">يجب عليك تثبيت التحديث الشهري الذي يتضمن جميع نقاط الملحق في بيئة التطوير.</span><span class="sxs-lookup"><span data-stu-id="eaa03-140">You should install the monthly update that includes all your extension points in the development environment.</span></span>
-   <span data-ttu-id="eaa03-141">ينبغي أن تكون الملحقات كاملة.</span><span class="sxs-lookup"><span data-stu-id="eaa03-141">Your extensions should be complete.</span></span>
-   <span data-ttu-id="eaa03-142">يجب تحديث Retail SDK.</span><span class="sxs-lookup"><span data-stu-id="eaa03-142">The Retail SDK should be updated.</span></span> 
-   <span data-ttu-id="eaa03-143">يجب استخدام أحدث إصدار من بيئة الإنشاء لديك من أجل إنشاء حزمة قابلة للنشر (إلزامي).</span><span class="sxs-lookup"><span data-stu-id="eaa03-143">The latest version of your build environment should be used to generate a deployable package (mandatory).</span></span> 
-   <span data-ttu-id="eaa03-144">يجب تشغيل ترقية البيانات في بيئة التطوير (إلزامي).</span><span class="sxs-lookup"><span data-stu-id="eaa03-144">A data upgrade should be run in a development environment (mandatory).</span></span>
-   <span data-ttu-id="eaa03-145">إذا كنت في العرض المباشر بالفعل، فاستخدم **النسخ الاحتياطي لقاعدة بيانات الإنتاج إلى التطوير** قبل إجراء الترقية.</span><span class="sxs-lookup"><span data-stu-id="eaa03-145">If you are already live, use **the prod DB backup to Dev** before performing an upgrade.</span></span> 
-   <span data-ttu-id="eaa03-146">تتوفر حزمة ترقية البيانات من مكتبة الأصول المشتركة.</span><span class="sxs-lookup"><span data-stu-id="eaa03-146">A data upgrade package is available from the Shared Asset library.</span></span>
-   <span data-ttu-id="eaa03-147">ستتم ترقية البيئة المستضافة على الشبكة السحابية من خلال دليل التشغيل.</span><span class="sxs-lookup"><span data-stu-id="eaa03-147">A cloud-hosted environment will be upgraded through a runbook.</span></span> 
-   <span data-ttu-id="eaa03-148">ستتم ترقية البيئة المستضافة من قِبل Microsoft من خلال ميزة الخدمة الذاتية في LCS.</span><span class="sxs-lookup"><span data-stu-id="eaa03-148">A Microsoft-hosted environment will be upgraded through the LCS self-service feature.</span></span> 
-   <span data-ttu-id="eaa03-149">يجب تثبيت التحديث الشهري الذي يتضمن جميع نقاط الملحق في بيئة الاختبار المعزولة.</span><span class="sxs-lookup"><span data-stu-id="eaa03-149">The monthly update that includes all your extension points should be installed in the sandbox.</span></span>
-   <span data-ttu-id="eaa03-150">ينبغي استخدام الخدمة الذاتية في LCS لتشغيل ترقية بيانات بيئة الاختبار المعزولة.</span><span class="sxs-lookup"><span data-stu-id="eaa03-150">LCS self-service should be used to run the sandbox data upgrade.</span></span> 

> [!NOTE]
> <span data-ttu-id="eaa03-151">يمكن ترقية الكود/البيانات مباشرةً إلى أحدث إصدار من الإصدار 7.x.</span><span class="sxs-lookup"><span data-stu-id="eaa03-151">Code/data can be upgraded directly to the latest version from any 7.x version.</span></span> 

<span data-ttu-id="eaa03-152">بعد اكتمال الترقية، فإن المرحلة التالية هي **التحقق** من إنجاز المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="eaa03-152">After you have completed your upgrade, the next phase is to **Validate** that the following tasks have been accomplished:</span></span> 

-   <span data-ttu-id="eaa03-153">اكتمال ترقية بيئة الاختبار المعزولة</span><span class="sxs-lookup"><span data-stu-id="eaa03-153">Completion of the sandbox upgrade</span></span> 
-   <span data-ttu-id="eaa03-154">اختبار وظيفي</span><span class="sxs-lookup"><span data-stu-id="eaa03-154">Functional testing</span></span> 
-   <span data-ttu-id="eaa03-155">إصلاح أي تراجع أو أخطاء أخرى</span><span class="sxs-lookup"><span data-stu-id="eaa03-155">Fixing of any regressions or other bugs</span></span>
-   <span data-ttu-id="eaa03-156">الموافقة على الاختبار الوظيفي</span><span class="sxs-lookup"><span data-stu-id="eaa03-156">Sign-off on the functional testing</span></span>
-   <span data-ttu-id="eaa03-157">إجراء الترقية الذاتية لبيئة التشغيل</span><span class="sxs-lookup"><span data-stu-id="eaa03-157">Production self-upgrade is performed</span></span>
-   <span data-ttu-id="eaa03-158">الانتهاء من ترقية بيئة التشغيل</span><span class="sxs-lookup"><span data-stu-id="eaa03-158">Production upgrade is complete</span></span>
-   <span data-ttu-id="eaa03-159">إجراء اختبار الدخان الخاص بالتشغيل والموافقة عليه (العرض المباشر)</span><span class="sxs-lookup"><span data-stu-id="eaa03-159">Production smoke test and sign-off (Go-Live) has been performed</span></span>
-   <span data-ttu-id="eaa03-160">يمكن لمستخدمي الوظائف المتميزين تنفيذ حالات الاختبار لديهم تلقائياً باستخدام Regression Suite Automation tool.</span><span class="sxs-lookup"><span data-stu-id="eaa03-160">Functional power users can automate the implementation of their test cases by using the Regression Suite Automation tool</span></span>
-   <span data-ttu-id="eaa03-161">اعتماد الاختبار الوظيفي من مستخدمي الأعمال</span><span class="sxs-lookup"><span data-stu-id="eaa03-161">Functional testing sign-off from business users</span></span> 
-   <span data-ttu-id="eaa03-162">ترقية بيانات تشغيل الخدمة الذاتية</span><span class="sxs-lookup"><span data-stu-id="eaa03-162">Self-service production data upgrade</span></span> 
-   <span data-ttu-id="eaa03-163">تثبيت التحديث الشهري الذي يتضمن جميع نقاط الملحق في بيئة التشغيل</span><span class="sxs-lookup"><span data-stu-id="eaa03-163">Monthly update that includes all your extension points in production is installed</span></span>
-   <span data-ttu-id="eaa03-164">إتمام اختبار الدخان الخاص بالتشغيل واعتماده من العميل</span><span class="sxs-lookup"><span data-stu-id="eaa03-164">Production smoke test and sign-off by customer is completed</span></span>