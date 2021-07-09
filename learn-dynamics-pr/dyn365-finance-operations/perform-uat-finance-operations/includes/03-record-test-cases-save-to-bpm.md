---
ms.openlocfilehash: c82f016ea4c550ef209486e1e57fd66d998b669b
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072387"
---
<span data-ttu-id="46241-101">بعد إنشاء مكتبة BPM، ستحتاج إلى استخدام مسجل المهام لإنشاء حالات الاختبار ومن ثمَّ تحميل الحالات إلى مكتبة BPM.</span><span class="sxs-lookup"><span data-stu-id="46241-101">After you have created a BPM library, you'll need to use the task recorder to create your test cases and then upload the cases to BPM.</span></span>
<span data-ttu-id="46241-102">هناك طرق عديدة للقيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="46241-102">There are several ways to do this.</span></span>

<span data-ttu-id="46241-103">إذا كنت تستخدم مكتبة BPM تحتوي بالفعل على جميع تسجيلات المهام الضرورية (حالات الاختبار) المرفقة، يمكنك تخطي هذه الخطوة.</span><span class="sxs-lookup"><span data-stu-id="46241-103">If you're using a BPM library that already has all the necessary task recordings (test cases) attached, you can skip this step.</span></span> <span data-ttu-id="46241-104">بخلاف ذلك، اتبع التعليمات اللاحقة لإنشاء تسجيلات مهام جديدة.</span><span class="sxs-lookup"><span data-stu-id="46241-104">Otherwise, follow the subsequent instructions to create new task recordings.</span></span>

<span data-ttu-id="46241-105">لتمكين التشغيل الفعال لاختباراتك باستخدام أدوات التشغيل التلقائي، تأكد من أن جميع تسجيلات المهام الخاصة بك تبدأ على لوحة المعلومات الرئيسية لتطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="46241-105">To enable the effective running of your tests by using automation tools, make sure that all your task recordings start on the main dashboard of Finance and Operations apps.</span></span>

<span data-ttu-id="46241-106">بالنسبة للعمليات الشاملة التي يقوم بها أكثر من مستخدم واحد، نوصي بتقسيم تسجيلات المهام الخاصة بك إلى مهام خاصة بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="46241-106">For end-to-end processes that are performed by more than one user, we recommend that you divide your task recordings into user-specific tasks.</span></span>
<span data-ttu-id="46241-107">يؤدي هذا إلى تبسيط صيانة حالات الاختبار ويسمح لك بتشغيل حالات الاختبار في سياق أدوار الأمان، وهي أفضل ممارسة.</span><span class="sxs-lookup"><span data-stu-id="46241-107">This simplifies the maintenance of test cases and allows you to run test cases in the context of security roles, which is a best practice.</span></span>

<span data-ttu-id="46241-108">شاهد هذا الفيديو للحصول على عرض توضيحي لكيفية استخدام مسجل المهام لإنشاء حالة اختبار لأداة Regression suite automation tool‏ (RSAT).</span><span class="sxs-lookup"><span data-stu-id="46241-108">Watch this video for a demonstration of how to use the task recorder to create a test case for the Regression suite automation tool (RSAT).</span></span> 
 
 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4uM5U]

### <a name="create-and-save-a-new-task-recording"></a><span data-ttu-id="46241-109">إنشاء وحفظ تسجيل مهام جديد</span><span class="sxs-lookup"><span data-stu-id="46241-109">Create and save a new task recording</span></span>

1.  <span data-ttu-id="46241-110">انتقل إلى **الإعدادات > مسجل المهام**.</span><span class="sxs-lookup"><span data-stu-id="46241-110">Go to **Settings > Task recorder**.</span></span>

    ![لقطة شاشة لخيار "مسجل المهام" في قائمة "الإعدادات".](../media/task-recorder.png)

2.  <span data-ttu-id="46241-112">حدد **إنشاء تسجيل**.</span><span class="sxs-lookup"><span data-stu-id="46241-112">Select **Create recording**.</span></span>

    ![لقطة شاشة لإنشاء تسجيل في قائمة "مسجل المهام".](../media/create-new-recording.png)

3.  <span data-ttu-id="46241-114">أدخل اسماً للتسجيل ثم حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="46241-114">Enter a name for the recording and then select **Start**.</span></span>

    ![لقطة شاشة لصفحة البدء مع حقول الاسم والوصف.](../media/start-1.png)

4.  <span data-ttu-id="46241-116">عند اكتمال التسجيل، في جزء مسجل المهام، حدد **إيقاف**.</span><span class="sxs-lookup"><span data-stu-id="46241-116">When the recording is complete, in the Task recorder pane, select **Stop**.</span></span>

5.  <span data-ttu-id="46241-117">لحفظ تسجيل المهمة إلى مكتبة BPM المرفقة، حدد **حفظ إلى Lifecycle Services**.</span><span class="sxs-lookup"><span data-stu-id="46241-117">To save the task recording to an attached BPM, select **Save to Lifecycle Services**.</span></span>

    ![لقطة شاشة لميزة حفظ إلى Lifecycle Services.](../media/lcs-1.png)

6.  <span data-ttu-id="46241-119">حدد المكتبة التي تريد حفظ التسجيل فيها، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="46241-119">Select the library that you want to save the recording to and then select **OK**.</span></span> <span data-ttu-id="46241-120">يؤدي هذا تلقائياً إلى حفظ التسجيل في Lifecycle Services.</span><span class="sxs-lookup"><span data-stu-id="46241-120">This automatically saves the recording into Lifecycle Services.</span></span> <span data-ttu-id="46241-121">إذا كانت لديك مكتبة أعمال بالفعل، فحدد ذلك في علامة التبويب **إدارة النظام > الإعداد > معلمات النظام > تعليمات**.</span><span class="sxs-lookup"><span data-stu-id="46241-121">If you already have a business library, then identify that in **System administration > Setup > System Parameters > Help** tab.</span></span>

7.  <span data-ttu-id="46241-122">إذا كنت تريد أيضاً حفظ التسجيل في جهاز الكمبيوتر الخاص بك، فحدد **حفظ في هذا الكمبيوتر**.</span><span class="sxs-lookup"><span data-stu-id="46241-122">If you also want to save the recording on your computer, select **Save to this PC**.</span></span> <span data-ttu-id="46241-123">ملحق ملف التسجيل هو AXTR.</span><span class="sxs-lookup"><span data-stu-id="46241-123">The extension of the recording file is AXTR.</span></span>

### <a name="upload-an-axtr-file-to-bpm"></a><span data-ttu-id="46241-124">تحميل ملف AXTR على BPM</span><span class="sxs-lookup"><span data-stu-id="46241-124">Upload an AXTR file to BPM</span></span>

<span data-ttu-id="46241-125">إذا قمت بحفظ التسجيلات الخاصة بك (ملفات AXTR) في جهاز الكمبيوتر الخاص بك، فاتبع الخطوات التالية لتحميلها على BPM.</span><span class="sxs-lookup"><span data-stu-id="46241-125">If you have saved your recordings (AXTR files) to your PC, follow these steps to upload them to BPM.</span></span>

1.  <span data-ttu-id="46241-126">في Lifecycle Services، في مشروعك، في صفحة **مكتبات عمليات الأعمال** ، حدد المكتبة التي سيتم تحميل تسجيل المهمة إليها.</span><span class="sxs-lookup"><span data-stu-id="46241-126">In Lifecycle Services, in your project, on the **Business process libraries** page, select the library to upload the task recording to.</span></span>

2.  <span data-ttu-id="46241-127">في الجزء الأيسر، حدد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="46241-127">In the right pane, select **Upload**.</span></span>

3.  <span data-ttu-id="46241-128">حدد **استعراض** للعثور على الملف المراد تحميله وتحديده، ثُم حدد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="46241-128">Select **Browse** to find and select the file to upload, and then  select **Upload**.</span></span>

### <a name="download-a-task-recording"></a><span data-ttu-id="46241-129">تنزيل تسجيل المهام</span><span class="sxs-lookup"><span data-stu-id="46241-129">Download a task recording</span></span>
<span data-ttu-id="46241-130">يمكنك تنزيل تسجيل مهام (ملف AXTR) تم تحميله إلى عملية BPM.</span><span class="sxs-lookup"><span data-stu-id="46241-130">You can download a task recording (AXTR file) that has been uploaded to a BPM process.</span></span>

1. <span data-ttu-id="46241-131">في Lifecycle Services، في مشروعك، في صفحة **مكتبات عمليات الأعمال**، حدد المكتبة لتنزيل تسجيل المهام.</span><span class="sxs-lookup"><span data-stu-id="46241-131">In Lifecycle Services, in your project, on the **Business process libraries** page, select the library to download the task recording.</span></span>
2. <span data-ttu-id="46241-132">حدد عملية تم تحميل تسجيل مهام إليها.</span><span class="sxs-lookup"><span data-stu-id="46241-132">Select a process that has task recording uploaded.</span></span>
3. <span data-ttu-id="46241-133">في الجزء **نظرة عامة**، حدد **تنزيل** لحفظ تسجيل المهام (AXTR).</span><span class="sxs-lookup"><span data-stu-id="46241-133">On the **Overview** pane, select **Download** to save the task recording (AXTR).</span></span>

### <a name="save-an-existing-task-recording-to-bpm"></a><span data-ttu-id="46241-134">حفظ تسجيل المهام الموجود في BPM</span><span class="sxs-lookup"><span data-stu-id="46241-134">Save an existing task recording to BPM</span></span>

1.  <span data-ttu-id="46241-135">لإرفاق تسجيل مهام موجود، سجّل الدخول إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="46241-135">To attach an existing task recording, sign in to the client.</span></span>

2.  <span data-ttu-id="46241-136">انتقل إلى **الإعدادات > مسجل المهام**.</span><span class="sxs-lookup"><span data-stu-id="46241-136">Go to **Settings > Task recorder**.</span></span>

3.  <span data-ttu-id="46241-137">حدد **تحرير التسجيل** وأرفق الملف إما من خلال الحفظ مباشرة في LCS أو تنزيل AXTR، ثم التحميل إلى BPM.</span><span class="sxs-lookup"><span data-stu-id="46241-137">Select **Edit Recording** and attach the file by either saving directly to LCS or downloading the AXTR and then uploading to BPM.</span></span>

    ![لقطة شاشة لميزة تحرير التسجيل.](../media/edit-recording.png)

### <a name="guidelines-for-recording-test-cases"></a><span data-ttu-id="46241-139">إرشادات تسجيل حالات الاختبار</span><span class="sxs-lookup"><span data-stu-id="46241-139">Guidelines for recording test cases</span></span>

<span data-ttu-id="46241-140">اتبع هذه الإرشادات عند كتابة حالات الاختبار الخاصة بك وتسجيلها، خاصة إذا كنت تخطط لأتمتة تشغيل اختبار.</span><span class="sxs-lookup"><span data-stu-id="46241-140">Follow these guidelines when writing and recording your test cases, especially if you are planning to automate a test run.</span></span> <span data-ttu-id="46241-141">تنطبق العملية والأدوات الموضحة في هذه المقالة على اختبارات قبول عمليات الأعمال؛ حيث لا يُقصد منها أن تحل محل اختبار المكونات والوحدات التي يمتلكها المطورون عادةً.</span><span class="sxs-lookup"><span data-stu-id="46241-141">The process and tools that are described in this article apply to business process acceptance tests; they are not meant to replace component and unit testing that is typically owned by developers.</span></span>

-   <span data-ttu-id="46241-142">اكتب عدداً محدوداً من حالات الاختبار التي، عند دمجها، تغطي العمليات الشاملة.</span><span class="sxs-lookup"><span data-stu-id="46241-142">Write a limited number of test cases that, when combined, cover complete end-to-end processes.</span></span>

-   <span data-ttu-id="46241-143">ركّز على عمليات الأعمال التي تم تخصيصها.</span><span class="sxs-lookup"><span data-stu-id="46241-143">Focus on business processes that have been customized.</span></span>

-   <span data-ttu-id="46241-144">يجب أن تغطي حالة الاختبار الفردية (التسجيل) مهمة عمل واحدة أو مهمتين فقط، يتم إجراؤها عادةً بواسطة شخص واحد.</span><span class="sxs-lookup"><span data-stu-id="46241-144">An individual test case (recording) should cover one or two business tasks only, typically run by one person.</span></span> <span data-ttu-id="46241-145">ويؤدي هذا إلى تبسيط صيانة تسجيل المهام.</span><span class="sxs-lookup"><span data-stu-id="46241-145">This simplifies task recording maintenance.</span></span> <span data-ttu-id="46241-146">لا تقم بضم عملية تجارية كاملة من البداية إلى النهاية، مثل عملية الشراء إلى الدفع أو من الأمر إلى التحصيل، في تسجيل مهمة واحدة كبيرة.</span><span class="sxs-lookup"><span data-stu-id="46241-146">Do not combine a complete end-to-end business process, such as procure-to-pay or order-to-cash, into one large task recording.</span></span> 
    -   <span data-ttu-id="46241-147">على سبيل المثال، بدلاً من وجود **طلب عرض الأسعار > أمر الشراء > إيصال استلام المنتجات > فاتورة المورد > دفع المورد** كحالة اختبار واحدة، قم بتقسيم العملية إلى ثلاث أو أربع حالات اختبار.</span><span class="sxs-lookup"><span data-stu-id="46241-147">For example, instead of having **RFQ > Purchase Order > Product Receipt > Vendor Invoice > Vendor Payment** as one test case, divide the process into three or four test cases.</span></span> <span data-ttu-id="46241-148">ستكون لديك الفرصة لدمج هذه الاختبارات في مجموعة اختبار مرتبة لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="46241-148">You will have the opportunity to combine these tests into an ordered test suite later.</span></span>

-   <span data-ttu-id="46241-149">يجب أن تحتوي حالة الاختبار على تحقق من الصحة واحد على الأقل.</span><span class="sxs-lookup"><span data-stu-id="46241-149">A test case should have at least one validation.</span></span> <span data-ttu-id="46241-150">حاول التحقق من صحة الحقول بالغة الأهمية التي تغطي تأثير الحقول الأخرى.</span><span class="sxs-lookup"><span data-stu-id="46241-150">Try to validate critical fields that cover the impact of other fields.</span></span> 
    -   <span data-ttu-id="46241-151">على سبيل المثال، يغطي التحقق من صحة الإجماليات في أوامر الشراء أو المبيعات سعر الوحدة/الكمية/الخصم/الضريبة.</span><span class="sxs-lookup"><span data-stu-id="46241-151">For example, validation of totals on sales or purchase orders cover the unit price/quantity/discount/tax.</span></span>

-   <span data-ttu-id="46241-152">تجنب طباعة تقرير في حالة اختبار.</span><span class="sxs-lookup"><span data-stu-id="46241-152">Avoid printing a report in a test case.</span></span> <span data-ttu-id="46241-153">إذا احتاجت حالة اختبار إلى طباعة تقرير، فيجب تحديده على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="46241-153">If a test case needs to print a report, it should be selected on screen.</span></span>

-   <span data-ttu-id="46241-154">يجب أن تكون أكثر من 80 في المئة من حالات الاختبار للمعاملات أو المستندات المصدر.</span><span class="sxs-lookup"><span data-stu-id="46241-154">80+ percent of test cases should be of transactions or source documents.</span></span> <span data-ttu-id="46241-155">يجب أن تقتصر البيانات الرئيسية على ما يصل إلى 20 في المئة من حالات الاختبار فقط.</span><span class="sxs-lookup"><span data-stu-id="46241-155">Master data should be limited to up to 20 percent of test cases only.</span></span>