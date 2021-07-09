---
ms.openlocfilehash: f1f4836651e61c891ababfbe1e488ee1db503df1
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072440"
---
<span data-ttu-id="1579a-101">بعد إنشاء مكتبة أداة تكوين عمليات الأعمال (BPM)، ستحتاج إلى استخدام مسجل المهام لإنشاء حالات الاختبار ومن ثمَّ قم بتحميل الحالات إلى مكتبة BPM.</span><span class="sxs-lookup"><span data-stu-id="1579a-101">After you have created a Business Process Modeler (BPM) library, you'll need to use Task recorder to create your test cases and then upload the cases to BPM.</span></span>

<span data-ttu-id="1579a-102">بعد ذلك، ستحتاج إلى إنشاء خطة اختبار ومجموعة اختبارات في Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="1579a-102">Next, you will need to create a test plan and test suite in Azure DevOps.</span></span> <span data-ttu-id="1579a-103">وسيسمح لك هذا بإجراء مجموعة منظمة من حالات الاختبار وإدارة النتائج والاستقصاء عنها وتعقبها بسهولة.</span><span class="sxs-lookup"><span data-stu-id="1579a-103">This will allow you to run an ordered suite of test cases and easily manage, investigate, and track the results.</span></span>

### <a name="before-you-begin"></a><span data-ttu-id="1579a-104">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="1579a-104">Before you begin</span></span>

<span data-ttu-id="1579a-105">للحصول على أقصى استفادة من هذا التدريب، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في تطبيقات Finance and Operations والتي يتم تثبيتها باستخدام Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="1579a-105">To get the most benefit from this exercise, we recommend that you have the standard sample data available in Finance and Operations apps installed by using Lifecycle Services (LCS).</span></span>

### <a name="create-a-bpm-library"></a><span data-ttu-id="1579a-106">إنشاء مكتبة BPM</span><span class="sxs-lookup"><span data-stu-id="1579a-106">Create a BPM library</span></span>

1.  <span data-ttu-id="1579a-107">في Lifecycle Service (LCS)، انتقل إلى مشروعك.</span><span class="sxs-lookup"><span data-stu-id="1579a-107">In LCS, navigate to your project.</span></span> <span data-ttu-id="1579a-108">في الإطارات المتجانبة الموجودة على اليمين، حدد **أداة تكوين عمليات الأعمال**.</span><span class="sxs-lookup"><span data-stu-id="1579a-108">In the tiles on the right, select **Business process modeler**.</span></span> 
1.  <span data-ttu-id="1579a-109">في صفحة **مكتبات عمليات الأعمال**، حدد **مكتبة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="1579a-109">On the **Business process libraries** page, select **New library**.</span></span>
1.  <span data-ttu-id="1579a-110">أدخل اسماً.</span><span class="sxs-lookup"><span data-stu-id="1579a-110">Enter a name.</span></span> <span data-ttu-id="1579a-111">وكمثال على ذلك، يمكنك إدخال **التدريب الأول** كاسم للمكتبة الجديدة، ثم حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="1579a-111">for example **Training First** for the new library, and then select  **Create**.</span></span> 

### <a name="add-a-new-process"></a><span data-ttu-id="1579a-112">إضافة عملية جديدة</span><span class="sxs-lookup"><span data-stu-id="1579a-112">Add a new process</span></span>

1.  <span data-ttu-id="1579a-113">في مكتبة BPM، حدد **التدريب الأول**.</span><span class="sxs-lookup"><span data-stu-id="1579a-113">In the BPM library, select **Training First**.</span></span>
1.  <span data-ttu-id="1579a-114">قم بتمييز العملية **عملية الأعمال الأساسية النموذجية** ثم حدد **إضافة عملية**.</span><span class="sxs-lookup"><span data-stu-id="1579a-114">Highlight the process **Sample Core Business Process** and then select **Add process**.</span></span> 
1.  <span data-ttu-id="1579a-115">يمكنك تحديد إضافة العملية كتابعة أو فرعية لعقدة العملية المحددة.</span><span class="sxs-lookup"><span data-stu-id="1579a-115">You can select to add the process as a child or a sibling of the selected process node.</span></span> <span data-ttu-id="1579a-116">وبهذه الطريقة، يمكنك إنشاء تدرج هرمي دلالي لعمليات الأعمال.</span><span class="sxs-lookup"><span data-stu-id="1579a-116">In this way, you can create a semantic hierarchy of business processes.</span></span> <span data-ttu-id="1579a-117">حدد **كتابعة**.</span><span class="sxs-lookup"><span data-stu-id="1579a-117">Select **As child**.</span></span>

### <a name="edit-the-properties-of-the-process"></a><span data-ttu-id="1579a-118">تحرير خصائص العملية</span><span class="sxs-lookup"><span data-stu-id="1579a-118">Edit the properties of the process</span></span>

1.  <span data-ttu-id="1579a-119">في مكتبة BPM، حدد عقدة العملية لتحرير **عملية أعمال جديدة**.</span><span class="sxs-lookup"><span data-stu-id="1579a-119">In the BPM library, select the process node to edit **New business process**.</span></span>
1.  <span data-ttu-id="1579a-120">في الجزء الأيمن، في علامة التبويب **نظرة عامة**، حدد وضع **التحرير**.</span><span class="sxs-lookup"><span data-stu-id="1579a-120">On the right-pane, on the **Overview** tab, select **Edit mode**.</span></span>
1.  <span data-ttu-id="1579a-121">أدخل اسماً ووصفاً لعقدة العملية.</span><span class="sxs-lookup"><span data-stu-id="1579a-121">Enter a name and description for the process node:</span></span>
    -   <span data-ttu-id="1579a-122">**الاسم**: إنشاء أمر مبيعات</span><span class="sxs-lookup"><span data-stu-id="1579a-122">**Name**: Create a sales order</span></span>
    -   <span data-ttu-id="1579a-123">**الوصف**: هذه العملية توثّق إنشاء أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="1579a-123">**Description**: This process documents the creation of a sales order.</span></span>
1.  <span data-ttu-id="1579a-124">بشكلٍ اختياري، حدد المجالات والبلدان أو المناطق التي تنطبق عليها العملية.</span><span class="sxs-lookup"><span data-stu-id="1579a-124">Optionally, select the industries and the countries or regions that the process applies to.</span></span> <span data-ttu-id="1579a-125">يمكنك كذلك إضافة كلمات أساسية وارتباطات.</span><span class="sxs-lookup"><span data-stu-id="1579a-125">You can also add keywords and links.</span></span> <span data-ttu-id="1579a-126">تمكنك الكلمات الأساسية من تحديد الفئات أو عمليات دفق العمل أو بيانات تعريف أخرى.</span><span class="sxs-lookup"><span data-stu-id="1579a-126">Keywords let you define categories, work streams, or other metadata.</span></span> <span data-ttu-id="1579a-127">تتيح لك الارتباطات (عناوين URL) الرجوع إلى المواقع الخارجية أو الوثائق.</span><span class="sxs-lookup"><span data-stu-id="1579a-127">Links (URLs) let you reference external sites or documentation.</span></span>
1.  <span data-ttu-id="1579a-128">عند الانتهاء من تحرير الخصائص، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="1579a-128">When you've finished editing the properties, select **Save**.</span></span>

### <a name="copy-a-library"></a><span data-ttu-id="1579a-129">نسخ مكتبة</span><span class="sxs-lookup"><span data-stu-id="1579a-129">Copy a library</span></span>

<span data-ttu-id="1579a-130">قد تحتاج إلى نسخ مكتبة، لأحد التباينات مثلاً.</span><span class="sxs-lookup"><span data-stu-id="1579a-130">You may have the need to copy a library, for example, for a variation.</span></span> <span data-ttu-id="1579a-131">توضح هذه المهمة كيفية تنفيذ ذلك.</span><span class="sxs-lookup"><span data-stu-id="1579a-131">This task illustrates how it’s done.</span></span>

1.  <span data-ttu-id="1579a-132">افتح صفحة  **مكتبات عمليات الأعمال** عبر الإطار المتجانب **‏‫أداة تكوين عمليات الأعمال‬** في صفحة المشروع في LCS.</span><span class="sxs-lookup"><span data-stu-id="1579a-132">Open the  **Business process libraries** page via the **Business process modeler** tile on the project page on LCS.</span></span>

1.  <span data-ttu-id="1579a-133">في الإطار المتجانب **التدريب الأول**، باعتبارها المكتبة التي تود نسخها، حدد زر علامة الحذف (...) ثم حدد **نسخ**.</span><span class="sxs-lookup"><span data-stu-id="1579a-133">On the tile for **Training first**, as the library that you want to copy, select the ellipsis button (...) and then select  **Copy**.</span></span> 

1.  <span data-ttu-id="1579a-134">أدخل اسماً للمكتبة **التدريب الثاني** ثم حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="1579a-134">Enter a name for the library **Training Second** and then select  **Create**.</span></span> 

### <a name="add-a-new-child-process"></a><span data-ttu-id="1579a-135">إضافة عملية تابعة جديدة</span><span class="sxs-lookup"><span data-stu-id="1579a-135">Add a new child process</span></span>

1.  <span data-ttu-id="1579a-136">في مكتبة **التدريب الثاني**، حدد العملية الموجودة **إنشاء أمر مبيعات**.</span><span class="sxs-lookup"><span data-stu-id="1579a-136">In the **Training Second** library, select the existing process **Create a sales order**.</span></span> <span data-ttu-id="1579a-137">يمكنك تنفيذ ذلك عن طريق تحديد علامة الإقحام الموجودة بجوار **عملية الأعمال الأساسية النموذجية** وتمييز سطر **إنشاء أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="1579a-137">You do this by selecting the caret next to **Sample Core Business Process** and highlighting the **Create a sales order** line.</span></span>
1.  <span data-ttu-id="1579a-138">حدد **إضافة عملية**.</span><span class="sxs-lookup"><span data-stu-id="1579a-138">Select **Add process**.</span></span> <span data-ttu-id="1579a-139">يمكنك تحديد إضافة العملية كتابعة أو فرعية لعقدة العملية المحددة.</span><span class="sxs-lookup"><span data-stu-id="1579a-139">You can select to add the process as a child or a sibling of the selected process node.</span></span> <span data-ttu-id="1579a-140">وبهذه الطريقة، يمكنك إنشاء تدرج هرمي دلالي لعمليات الأعمال.</span><span class="sxs-lookup"><span data-stu-id="1579a-140">In this way, you can create a semantic hierarchy of business processes.</span></span> <span data-ttu-id="1579a-141">حدد **كتابعة**.</span><span class="sxs-lookup"><span data-stu-id="1579a-141">Select **As child**.</span></span>

### <a name="edit-the-properties-of-the-process"></a><span data-ttu-id="1579a-142">تحرير خصائص العملية</span><span class="sxs-lookup"><span data-stu-id="1579a-142">Edit the properties of the process</span></span>

1.  <span data-ttu-id="1579a-143">في الجزء الأيمن، في علامة التبويب **نظرة عامة**، حدد وضع **التحرير**.</span><span class="sxs-lookup"><span data-stu-id="1579a-143">On the right-pane, on the **Overview** tab, select **Edit** mode.</span></span>
1.  <span data-ttu-id="1579a-144">أدخل اسماً ووصفاً لعقدة العملية.</span><span class="sxs-lookup"><span data-stu-id="1579a-144">Enter a name and description for the process node:</span></span>
    -   <span data-ttu-id="1579a-145">**الاسم**: إنشاء سطر مبيعات</span><span class="sxs-lookup"><span data-stu-id="1579a-145">**Name**: Create a sales line</span></span>
    -   <span data-ttu-id="1579a-146">**الوصف**: تعمل هذه العملية على إنشاء سطر لأمر المبيعات الأصلي.</span><span class="sxs-lookup"><span data-stu-id="1579a-146">**Description**: This process creates a line for the parent sales order.</span></span>
1.  <span data-ttu-id="1579a-147">عند الانتهاء من تحرير الخصائص، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="1579a-147">When you've finished editing the properties, select **Save**.</span></span>

### <a name="record-test-cases-and-save-to-bpm"></a><span data-ttu-id="1579a-148">تسجيل حالات الاختبار والحفظ في مكتبة BPM</span><span class="sxs-lookup"><span data-stu-id="1579a-148">Record test cases and save to BPM</span></span>

1.  <span data-ttu-id="1579a-149">افتح عميل تطبيقات Finance and Operations وقم بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="1579a-149">Open the Finance and Operations apps client and sign in.</span></span>

1.  <span data-ttu-id="1579a-150">حدد الشركة التي تود استخدامها في أثناء التسجيل، في هذه الحالة تكون الشركة **USMF‎**.</span><span class="sxs-lookup"><span data-stu-id="1579a-150">Select the company that you want to use while recording, in this case **USMF**.</span></span>

1.  <span data-ttu-id="1579a-151">انتقل إلى **الإعدادات > مسجل المهام**.</span><span class="sxs-lookup"><span data-stu-id="1579a-151">Go to **Settings > Task recorder**.</span></span>

    > ![لقطة شاشة لميزة "مسجل المهام" في قائمة "الإعدادات".](../media/task-recorder.png)

1.  <span data-ttu-id="1579a-153">حدد **إنشاء تسجيل جديد**.</span><span class="sxs-lookup"><span data-stu-id="1579a-153">Select **Create a new recording**.</span></span>

1.  <span data-ttu-id="1579a-154">أدخل اسماً للتسجيل: **إنشاء أمر مبيعات**، ثم حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="1579a-154">Enter a name for the recording: **Sales order creation**, and then select  **Start**.</span></span> <span data-ttu-id="1579a-155">يبدأ التسجيل لحظة تحديدك **بدء**.</span><span class="sxs-lookup"><span data-stu-id="1579a-155">Recording begins the moment that you select **Start**.</span></span>
    
1.    <span data-ttu-id="1579a-156">انتقل إلى **الوحدات > الحسابات المدينة > الأوامر > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="1579a-156">Navigate to **Modules > Accounts receivable > Orders > All sales orders**.</span></span>
1. <span data-ttu-id="1579a-157">انقر على **جديد**</span><span class="sxs-lookup"><span data-stu-id="1579a-157">Click **New**.</span></span>
1.  <span data-ttu-id="1579a-158">أدخل **US-001** في حقل **العميل**.</span><span class="sxs-lookup"><span data-stu-id="1579a-158">Enter **US-001** in the **Customer** field.</span></span>
1.  <span data-ttu-id="1579a-159">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="1579a-159">Select **OK**.</span></span>
1.  <span data-ttu-id="1579a-160">في سطر أمر المبيعات، أدخل **A0001** في حقل **الصنف**.</span><span class="sxs-lookup"><span data-stu-id="1579a-160">In the sales order line, enter **A0001** in the **Item** field.</span></span>
1.  <span data-ttu-id="1579a-161">في حقل **الموقع**، أدخل *1*.</span><span class="sxs-lookup"><span data-stu-id="1579a-161">In the **Site** field, enter *1*.</span></span>
1.  <span data-ttu-id="1579a-162">السماح بتعيين القيم المتبقية إلى الإعداد الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="1579a-162">Allow the remaining values to default.</span></span>
1.  <span data-ttu-id="1579a-163">حدد **حفظ** وإغلاق باستخدام زر **X**.</span><span class="sxs-lookup"><span data-stu-id="1579a-163">Select **Save**, and close with the **X** button.</span></span>
 
1.  <span data-ttu-id="1579a-164">عند اكتمال المهمة، في جزء مسجل المهام، حدد **إيقاف**.</span><span class="sxs-lookup"><span data-stu-id="1579a-164">When the task is complete, on the Task recorder pane, select **Stop**.</span></span>

1.  <span data-ttu-id="1579a-165">لحفظ تسجيل المهمة إلى مكتبة BPM المرفقة، حدد **حفظ إلى Lifecycle Services**.</span><span class="sxs-lookup"><span data-stu-id="1579a-165">To save the task recording to an attached BPM, select **Save to Lifecycle Services**.</span></span>

    -   <span data-ttu-id="1579a-166">إذا لم تكن متصلاً بـ Lifecycle Services بعد، فقد حان الوقت الآن للاتصال.</span><span class="sxs-lookup"><span data-stu-id="1579a-166">If you haven’t connected to Lifecycle Services yet, now is the time to establish a connection.</span></span> <span data-ttu-id="1579a-167">حدد زر **انقر هنا للاتصال بـ Lifecycle Services**.</span><span class="sxs-lookup"><span data-stu-id="1579a-167">Select the **Click here to connect to Lifecycle Services** button.</span></span>
    -   <span data-ttu-id="1579a-168">يجب أن يتم توجيهك إلى علامة تبويب "مستعرض" التي توضح تنفيذك الناجح.</span><span class="sxs-lookup"><span data-stu-id="1579a-168">You should be sent to a browser tab saying that you were successful.</span></span> <span data-ttu-id="1579a-169">يمكنك إغلاق علامة التبويب.</span><span class="sxs-lookup"><span data-stu-id="1579a-169">You can close the tab.</span></span>
    -   <span data-ttu-id="1579a-170">قم بالرجوع إلى شاشة Finance and Operations وحدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="1579a-170">Return to your Finance and Operations screen and select **OK**.</span></span>
1.  <span data-ttu-id="1579a-171">حدد المكتبة التي تود حفظ التسجيل فيها، والتي سيكون اسمها **التدريب الثاني** والعملية **إنشاء أمر مبيعات** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="1579a-171">Select the library that you want to save the recording to, which will have the name **Training Second**, and the process **Create a sales order**, then select **OK**.</span></span>

### <a name="alternate-method--save-locally-then-upload"></a><span data-ttu-id="1579a-172">طريقة بديلة – قم بالحفظ محلياً، ثم قم بتحميلها</span><span class="sxs-lookup"><span data-stu-id="1579a-172">Alternate method – save locally, then upload</span></span>

1.  <span data-ttu-id="1579a-173">وبدلاً من ذلك، يمكنك تحديد **حفظ إلى هذا الكمبيوتر الشخصي**.</span><span class="sxs-lookup"><span data-stu-id="1579a-173">Alternatively, you can select **Save to this PC**.</span></span><span data-ttu-id="1579a-174">أكمل عملية حفظ ملف .axtr.</span><span class="sxs-lookup"><span data-stu-id="1579a-174"> Complete the save process of the .axtr.</span></span>

1. <span data-ttu-id="1579a-175">افتح أو ارجع إلى LCS، في مشروعك، في صفحة **مكتبات عمليات الأعمال**، حدد المكتبة التي سيتم تحميل تسجيل المهمة إليها.</span><span class="sxs-lookup"><span data-stu-id="1579a-175">Open or return to LCS, in your project, on the **Business process libraries** page, select the library to upload the task recording to.</span></span>
1.  <span data-ttu-id="1579a-176">حدد موقع العملية وحددها (**إنشاء أمر مبيعات** ضمن **التدريب الثاني**) لتحميل تسجيل المهمة إليها.</span><span class="sxs-lookup"><span data-stu-id="1579a-176">Locate and select the process (**Create a sales order** under **Training Second**) to upload the task recording to.</span></span>
1.  <span data-ttu-id="1579a-177">في الجزء الأيمن، حدد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="1579a-177">On the right-pane, select **Upload**.</span></span>
1.  <span data-ttu-id="1579a-178">حدد **استعراض** للعثور على ملف .axtr وتحديده، ثُم حدد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="1579a-178">Select **Browse** to find and select the .axtr file to upload, and then select **Upload**.</span></span>