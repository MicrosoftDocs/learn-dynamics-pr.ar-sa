---
ms.openlocfilehash: 7afbdb973a991fb9496e090c9134193a5e0386b3
ms.sourcegitcommit: ca87deefdcd512d3b8e382cd49adf8a15d5995fc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/02/2021
ms.locfileid: "6070447"
---
<span data-ttu-id="1da00-101">لإنشاء تسجيل باستخدام ميزة "مسجل الاختبارات"، تحتاج أولاً إلى تمكين التسجيل التجريبي في نقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="1da00-101">To create a recording by using the Test recorder feature, you first need to enable test recording in point of sale (POS).</span></span> <span data-ttu-id="1da00-102">لتشغيل وظيفة التسجيل التجريبي في نقطة البيع، اتبع هذه الخطوات في Commerce:</span><span class="sxs-lookup"><span data-stu-id="1da00-102">To turn on the test recording functionality in POS, follow these steps in Commerce:</span></span>

1.  <span data-ttu-id="1da00-103">انتقل إلى **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع > السجلات**.</span><span class="sxs-lookup"><span data-stu-id="1da00-103">Go to **Retail and Commerce > Channel Setup > POS Setup > Registers**.</span></span>
2.  <span data-ttu-id="1da00-104">حدد السجل الذي ينبغي تشغيل وظيفة التسجيل التجريبي فيه.</span><span class="sxs-lookup"><span data-stu-id="1da00-104">Select the register where the test recording functionality should be turned on.</span></span>
3.  <span data-ttu-id="1da00-105">في علامة التبويب **السجل** في علامة التبويب السريعة **عام**، قم بتعيين الخيار **تمكين مسجل الاختبار والمهمة** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="1da00-105">On the **Register** tab, on the **General** FastTab, set the **Enable task and test recorder** option to **Yes**.</span></span>
4.  <span data-ttu-id="1da00-106">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="1da00-106">Select **Save**.</span></span>
5.  <span data-ttu-id="1da00-107">انتقل إلى **البيع بالتجزئة والتجارة > تكنولوجيا معلومات البيع بالتجزئة والتجارة > جدول التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="1da00-107">Go to **Retail and Commerce > Retail and Commerce IT > Distribution schedule**.</span></span>
6.  <span data-ttu-id="1da00-108">حدد المهمة **السجلات (1090)**، ثم حدد **تشغيل الآن**.</span><span class="sxs-lookup"><span data-stu-id="1da00-108">Select the **Registers (1090)** job, and then select **Run now**.</span></span>

<span data-ttu-id="1da00-109">شاهد الفيديو التالي للحصول على عرض توضيحي حول كيفية استخدام مسجل المهام مع تطبيقات Finance and Operations بحيث يمكنك إنشاء حالات اختبار لاستخدامها مع RSAT.</span><span class="sxs-lookup"><span data-stu-id="1da00-109">Watch the following video for a demonstration on how to use the Task recorder with Finance and Operations apps so that you can create test cases to use with RSAT.</span></span> <span data-ttu-id="1da00-110">وهذه هي الطريقة نفسها المتبعة في Commerce.</span><span class="sxs-lookup"><span data-stu-id="1da00-110">The method is the same as it is with Commerce.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4uM5U]


<span data-ttu-id="1da00-111">اتبع الخطوات التالية لإنشاء تسجيل جديد باستخدام مسجل الاختبار:</span><span class="sxs-lookup"><span data-stu-id="1da00-111">Follow these steps to create a new recording by using the test recorder:</span></span>

1.  <span data-ttu-id="1da00-112">قم بتشغيل نقطة بيع المجموعة.</span><span class="sxs-lookup"><span data-stu-id="1da00-112">Launch Cloud POS.</span></span>
2.  <span data-ttu-id="1da00-113">حدد رمز الهامبرغر في الجزء الأيمن، ثم حدد **الإعدادات**.</span><span class="sxs-lookup"><span data-stu-id="1da00-113">Select the hamburger icon on the left pane and then select **Settings**.</span></span> <span data-ttu-id="1da00-114">لا تقم بتسجيل الدخول إلى نقطة بيع المجموعة.</span><span class="sxs-lookup"><span data-stu-id="1da00-114">Don't sign in to Cloud POS.</span></span> <span data-ttu-id="1da00-115">يجب تسجيل خطوة تسجيل الدخول كجزء من تدفق التسجيل التجريبي، لذلك تحتاج إلى تشغيل المُسجل قبل تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="1da00-115">The sign-in step must be recorded as part of the test recording flow, so you need to launch the recorder before you sign in.</span></span>
3.  <span data-ttu-id="1da00-116">في صفحة **الإعدادات**، في القسم **مسجلات الاختبار والمهمة**، حدد **فتح مسجل الاختبار**.</span><span class="sxs-lookup"><span data-stu-id="1da00-116">On the **Settings** page, in the **Task and Test recorders** section, select **Open test recorder**.</span></span>
    <span data-ttu-id="1da00-117">![لقطة شاشة لمسجلات الاختبار والمهمة تُظهر الخيار "فتح مسجل الاختبار".](../media/open-test-recorder-ss.jpg)</span><span class="sxs-lookup"><span data-stu-id="1da00-117">![Screenshot of the Task and Test recorders page showing the Open test recorder option.](../media/open-test-recorder-ss.jpg)</span></span>
4.  <span data-ttu-id="1da00-118">حدد **إنشاء تسجيل جديد**.</span><span class="sxs-lookup"><span data-stu-id="1da00-118">Select **Create a new recording**.</span></span>
5.  <span data-ttu-id="1da00-119">أدخل **الاسم** و **الوصف** للتسجيل، ثم حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="1da00-119">Enter a **Name** and **Description** for the recording, and then select **Start**.</span></span> <span data-ttu-id="1da00-120">يدخل مسجل الاختبار في وضع التسجيل، وتبدأ جلسة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="1da00-120">The test recorder enters recording mode, and the recording session begins.</span></span> <span data-ttu-id="1da00-121">تعرض الصفحة **مسجل الاختبار** المعلومات وعناصر التحكم المتعلقة بجلسة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="1da00-121">The **Test Recorder** page shows information and controls that are related to the recording session.</span></span>

    ![لقطة شاشة لصفحة مسجل الاختبار تعرض المعلومات وعناصر التحكم الخاصة بالتسجيل.](../media/test-recorder-ss.jpg)
    
    <span data-ttu-id="1da00-123">يجب أن يبدأ كل تسجيل تجريبي من صفحة تسجيل الدخول إلى نقطة بيع المجموعة.</span><span class="sxs-lookup"><span data-stu-id="1da00-123">All test recording must begin from the Cloud POS sign-in page.</span></span> <span data-ttu-id="1da00-124">إذا تم بدء التسجيل من الصفحة الرئيسية، فستفشل أي حركة أو تشغيل آخر للصفحة، وستحتاج إلى بدء التسجيل مرة أخرى من صفحة تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="1da00-124">If the recording is started from the home page, any transaction or other page playback will fail, and you will need to start the recording again from the sign-in page.</span></span>


6.  <span data-ttu-id="1da00-125">قم بإجراء التسجيل في واجهة مستخدم نقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="1da00-125">Perform the recording in the POS user interface.</span></span>
7.  <span data-ttu-id="1da00-126">بعد إنهاء جلسة التسجيل، يمكنك تحميل التسجيل عن طريق تحديد **حفظ إلى هذا الكمبيوتر**.</span><span class="sxs-lookup"><span data-stu-id="1da00-126">After you end a recording session, you can download the recording by selecting **Save to this PC**.</span></span>
    <span data-ttu-id="1da00-127">![لقطة شاشة لصفحة مسجل الاختبار تُظهر الخيار "حفظ إلى هذا الكمبيوتر".](../media/save-recording-ss.jpg)</span><span class="sxs-lookup"><span data-stu-id="1da00-127">![Screenshot of the Test recorder page showing the Save to this PC option.](../media/save-recording-ss.jpg)</span></span>

<span data-ttu-id="1da00-128">يتم حفظ ملف ‎.axtr في نظام الملفات المحلي.</span><span class="sxs-lookup"><span data-stu-id="1da00-128">The .axtr file is saved to the local file system.</span></span> <span data-ttu-id="1da00-129">يجب تحميل هذا الملف يدوياً إلى LCS أو Azure DevOps ثم حذفه من نظام الملفات أو تأمينه.</span><span class="sxs-lookup"><span data-stu-id="1da00-129">You must manually upload this file to LCS or Azure DevOps and then either delete it from the file system or secure it.</span></span>

<span data-ttu-id="1da00-130">للتحميل إلى Azure DevOps مباشرةً:</span><span class="sxs-lookup"><span data-stu-id="1da00-130">To upload to Azure DevOps directly:</span></span>

1.  <span data-ttu-id="1da00-131">قم بتغيير امتداد الملف ‎.axtr إلى ‎.zip.</span><span class="sxs-lookup"><span data-stu-id="1da00-131">Change the .axtr file extension to .zip.</span></span>
2.  <span data-ttu-id="1da00-132">افتح حزمة ‎.zip.</span><span class="sxs-lookup"><span data-stu-id="1da00-132">Open the .zip package.</span></span>
3.  <span data-ttu-id="1da00-133">سيكون داخل الحزمة ملف باسم Recording.xml.</span><span class="sxs-lookup"><span data-stu-id="1da00-133">Inside the package will be a file with the name Recording.xml.</span></span> <span data-ttu-id="1da00-134">تحميل ملف Recording.xml إلى حالة الاختبار في Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="1da00-134">Upload the Recording.xml file to the test case in Azure DevOps.</span></span> <span data-ttu-id="1da00-135">لا تقم بتحميل حزمة ‎.zip</span><span class="sxs-lookup"><span data-stu-id="1da00-135">Don’t upload the entire .zip or.</span></span> <span data-ttu-id="1da00-136">أو ‎.axtr بالكامل.</span><span class="sxs-lookup"><span data-stu-id="1da00-136">axtr package.</span></span>
