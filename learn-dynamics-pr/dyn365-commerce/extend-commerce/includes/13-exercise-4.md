---
ms.openlocfilehash: 822a925a287bca5540e6a9b01c7a8ee73f4f52d8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070075"
---
<span data-ttu-id="fcada-101">وباعتبارك مطوراً في التجارة الإلكترونية، فقد تمت مطالبتك بإنشاء حل مخصص في إحدى ملحقات التجارة الإلكترونية ثم نشر الحزمة إلى الموقع عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="fcada-101">As an e-Commerce developer, you have been asked to build a customized solution in an e-Commerce extension and then deploy the package to the online site.</span></span> 

<span data-ttu-id="fcada-102">ستقوم بتنفيذ المهام التالية في هذا التدريب:</span><span class="sxs-lookup"><span data-stu-id="fcada-102">In this exercise, you will perform the following tasks:</span></span>

1. <span data-ttu-id="fcada-103">قم بإنشاء الحزمة في رمز Visual Studio ثم قم بتحميلها خلال خدمات Lifecycle Services من Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="fcada-103">Build the package in Visual Studio Code and then upload it through Dynamics 365 Lifecycle Services.</span></span>
2. <span data-ttu-id="fcada-104">نشر تكوين الحزمة من خلال خدمات Lifecycle Services من Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="fcada-104">Deploy the package configuration through Dynamics 365 Lifecycle Services.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="fcada-105">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="fcada-105">Before you begin</span></span>

<span data-ttu-id="fcada-106">ستحتاج إلى بيئة اختبار معزولة للمطورين وترخيص تجريبي أو دائم باستخدام Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="fcada-106">You will need a developer sandbox environment and a trial or permanent license for using Visual Studio Code.</span></span> <span data-ttu-id="fcada-107">ستحتاج أيضاً إلى الاشتراك في خدمات Lifecycle Services من Dynamics 365 ومشروع تم إنشاؤه لـ CSU وموقع تجارة الخدمات الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="fcada-107">Also, you will need a subscription to Dynamics 365 Lifecycle Services and a created project for CSU and an e-Commerce site.</span></span>

## <a name="build-and-upload-the-package"></a><span data-ttu-id="fcada-108">إنشاء الحزمة وتنزيلها</span><span class="sxs-lookup"><span data-stu-id="fcada-108">Build and upload the package</span></span> 

<span data-ttu-id="fcada-109">لإنشاء الحزمة وتحميلها، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="fcada-109">To build and upload the package, follow these steps:</span></span>

1. <span data-ttu-id="fcada-110">افتح **رمز  Visual Studio** وحدد نافذة **الوحدة الطرفية > وحدة طرفية جديدة** (تأكد من أن النافذة موجه أوامر وليست PowerShell).</span><span class="sxs-lookup"><span data-stu-id="fcada-110">Open **Visual Studio Code** and select **Terminal > New Terminal** window (ensure that the window is a Command Prompt and not a PowerShell).</span></span>
2. <span data-ttu-id="fcada-111">في النافذة **وحدة طرفية جديدة**، ثم نفذ الأمر التالي وحدد **إدخال** لتشغيل الأمر.</span><span class="sxs-lookup"><span data-stu-id="fcada-111">In the **New terminal** window, run the following command and then select **Enter** to run the command.</span></span> 
`c:\repos\D365.Commerce.Fabrikam>yarn msdyn365 pack`
3. <span data-ttu-id="fcada-112">انتقل إلى [https://lcs.dynamics.com/](https://lcs.dynamics.com//?azure-portal=true)، حيث يجب أن تظهر أمامك صفحة تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="fcada-112">Go to [https://lcs.dynamics.com/](https://lcs.dynamics.com//?azure-portal=true), where you should see a sign-in page.</span></span> 
4. <span data-ttu-id="fcada-113">حدد **تسجيل الدخول** ثم أدخل بيانات اعتماد الحساب المقدمة من خدمات Lifecycle Services من Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="fcada-113">Select **Sign in** and then enter your Dynamics 365 Lifecycle Services-provided account credentials.</span></span>
5. <span data-ttu-id="fcada-114">حدد مشروع التجارة الإلكترونية الذي ستقوم باستخدامه.</span><span class="sxs-lookup"><span data-stu-id="fcada-114">Select the e-Commerce project that you will be using.</span></span> <span data-ttu-id="fcada-115">قم بالتمرير إلى اليمين لعرض مزيد من الخيارات.</span><span class="sxs-lookup"><span data-stu-id="fcada-115">Scroll to the right to see more options.</span></span>
6. <span data-ttu-id="fcada-116">لتحميل الحزمة، في القسم **‏‫مزيد من الأدوات‬**، حدد لوحة **مكتبة الأصول**.</span><span class="sxs-lookup"><span data-stu-id="fcada-116">To upload the package, in the **More tools** section, select the **Asset Library** tile.</span></span>  
7. <span data-ttu-id="fcada-117">في الصفحة **مكتبة الأصول**، حدد علامة التبويب **حزمة التجارة الإلكترونية** من الجزء الأيسر. إذا لم تظهر علامة التبويب **حزمة التجارة الإلكترونية**، فيجب عليك تمكين ميزات التجارة الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="fcada-117">On the **Asset Library** page, in the left pane, select the **e-Commerce package** tab. If you don't see the **e-Commerce package** tab, you must enable e-Commerce features.</span></span> <span data-ttu-id="fcada-118">حدد علامة الجمع (**+**).</span><span class="sxs-lookup"><span data-stu-id="fcada-118">Select the plus sign (**+**).</span></span>
8. <span data-ttu-id="fcada-119">في مربع الحوار **تحميل ملف حزمة التجارة الإلكترونية**، أدخل اسماً ووصفاً للحزمة، ثم حدد **إضافة ملف**.</span><span class="sxs-lookup"><span data-stu-id="fcada-119">In the **Upload e-Commerce package file** dialog box, enter a name and description for the package, and then select **Add a file**.</span></span>
9. <span data-ttu-id="fcada-120">في مربع الحوار **تحميل أصل الملف**، حدد **استعراض** ثم استعرض بحثاً عن موقع ملف الحزمة المضغوطة الذي قمت بإنشائه سابقاً.</span><span class="sxs-lookup"><span data-stu-id="fcada-120">In the **Upload file asset** dialog box, select **Browse** and then browse to the location of the package zip file that you created previously.</span></span> <span data-ttu-id="fcada-121">حدد الملف، ثم قم بتحديد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="fcada-121">Select the file and then select **Upload**.</span></span>
10. <span data-ttu-id="fcada-122">عند اكتمال التحميل، سيتم إرجاعك إلى مربع الحوار **تحميل ملف حزمة التجارة الإلكترونية**.</span><span class="sxs-lookup"><span data-stu-id="fcada-122">When the upload is complete, you will be returned to the **Upload e-Commerce package file** dialog box.</span></span> <span data-ttu-id="fcada-123">حدد **تأكيد** لمعالجة التحميل.</span><span class="sxs-lookup"><span data-stu-id="fcada-123">Select **Confirm** to process the upload.</span></span>
11. <span data-ttu-id="fcada-124">في حالة اكتمال المعالجة بنجاح، ستظهر علامة اختيار في العمود **صالح**.</span><span class="sxs-lookup"><span data-stu-id="fcada-124">If processing has completed successfully, a check mark will appear in the **Valid** column.</span></span> <span data-ttu-id="fcada-125">(قد تستغرق هذه العملية 40 إلى 50 دقيقة).</span><span class="sxs-lookup"><span data-stu-id="fcada-125">(This process can take 40 to 50 minutes.)</span></span>

## <a name="deploy-a-package"></a><span data-ttu-id="fcada-126">نشر حزمة</span><span class="sxs-lookup"><span data-stu-id="fcada-126">Deploy a package</span></span> 

<span data-ttu-id="fcada-127">لنشر حزمة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="fcada-127">To deploy a package, follow these steps:</span></span>

1. <span data-ttu-id="fcada-128">في خدمات Lifecycle Services من Dynamics 365، انتقل إلى لوحة المعلومات **المشروع** وحدد البيئة التي تريد نشر حزمة فيها.</span><span class="sxs-lookup"><span data-stu-id="fcada-128">In Dynamics 365 Lifecycle Services, go to the **Project** dashboard and select the environment that you want to deploy a package to.</span></span>
2. <span data-ttu-id="fcada-129">في القسم **ميزات البيئة** على الجانب الأيسر من الصفحة، حدد **إدارة**.</span><span class="sxs-lookup"><span data-stu-id="fcada-129">In the **Environment features** section on the right side of the page, select **Manage**.</span></span>
3. <span data-ttu-id="fcada-130">حدد علامة التبويب **التجارة الإلكترونية**.</span><span class="sxs-lookup"><span data-stu-id="fcada-130">Select the **E-Commerce** tab.</span></span>
4. <span data-ttu-id="fcada-131">حدد **تطبيق الملحق** لتحديد الحزمة المطلوب نشرها.</span><span class="sxs-lookup"><span data-stu-id="fcada-131">Select **Apply extension** to select the package to deploy.</span></span>
5. <span data-ttu-id="fcada-132">في مربع الحوار **تحديث التجارة الإلكترونية**، حدد الحزمة التي قمت بتحميلها سابقاً، ثم حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="fcada-132">In the **Update e-Commerce** dialog box, select the package that you uploaded earlier, and then select **Update**.</span></span>

<span data-ttu-id="fcada-133">يمكنك الآن تعقب حالة النشر في قسم **التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="fcada-133">You can now track the deployment status in the **Details** section.</span></span> <span data-ttu-id="fcada-134">بعد اكتمال النشر، يجب رؤية التغييرات التي قمت بها في أدوات التأليف أو على الصفحات التي يتم تقديمها.</span><span class="sxs-lookup"><span data-stu-id="fcada-134">After the deployment has completed, you should see your changes in the authoring tools or on pages that are rendered.</span></span>



