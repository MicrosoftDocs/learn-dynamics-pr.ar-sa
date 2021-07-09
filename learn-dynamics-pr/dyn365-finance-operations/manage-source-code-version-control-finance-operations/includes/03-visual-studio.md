---
ms.openlocfilehash: 17aca98fbc3ca1b01826d144fb3528f41a7ae36b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071834"
---
<span data-ttu-id="62bee-101">تشرح هذه الوحدة كيفية إيداع الكود، ودمج الكود، وحل التعارضات، والتراجع عن التغييرات في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="62bee-101">This unit explains how to check in code, merge code, resolve conflicts, and roll back changes in Visual Studio.</span></span>

## <a name="get-the-latest-version-and-check-in-code"></a><span data-ttu-id="62bee-102">الحصول على أحدث إصدار وإيداع الكود</span><span class="sxs-lookup"><span data-stu-id="62bee-102">Get the latest version and check in code</span></span> 

 
<span data-ttu-id="62bee-103">عند العمل مع عدة مطورين أو مشاريع، يجب أن تتحقق من أن الكود يتضمن أحدث إصدار للتحكم في المصادر.</span><span class="sxs-lookup"><span data-stu-id="62bee-103">When working with multiple developers or projects, you should validate that your code includes the latest source control's version.</span></span> <span data-ttu-id="62bee-104">لتجنب التعارض والتأكد من تطوير الكود بشكل صحيح، يعد التحقق من المصدر أمراً إلزامياً.</span><span class="sxs-lookup"><span data-stu-id="62bee-104">To avoid conflicts and ensure that the code is developed correctly, checking the source is mandatory.</span></span>

<span data-ttu-id="62bee-105">مستكشف التحكم في المصادر هو عرض لجميع الأكواد والكائنات التي تم التحقق منها في التحكم في المصادر.</span><span class="sxs-lookup"><span data-stu-id="62bee-105">The Source Control Explorer is your go-to view for all the code and objects that have been checked into source control.</span></span> 
 
<span data-ttu-id="62bee-106">[ ![لقطة شاشة لصفحة مستكشف التحكم في المصادر](../media/source-control.png) ](../media/source-control.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="62bee-106">[ ![Screenshot of Source Control explorer page](../media/source-control.png) ](../media/source-control.png#lightbox)</span></span>

<span data-ttu-id="62bee-107">للوصول إلى "مستكشف التحكم في المصادر"، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="62bee-107">To reach the Source Control Explorer, follow these steps:</span></span>

1.  <span data-ttu-id="62bee-108">حدد **عرض** علي شريط القائمة في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="62bee-108">Select **View** on the menu bar of Visual Studio.</span></span>
2.  <span data-ttu-id="62bee-109">في القائمة المنسدلة، حدد **نوافذ أخرى**.</span><span class="sxs-lookup"><span data-stu-id="62bee-109">In the drop-down menu, select **Other Windows**.</span></span>
3.  <span data-ttu-id="62bee-110">من الخيارات المتوفرة، حدد **مستكشف التحكم في المصادر**.</span><span class="sxs-lookup"><span data-stu-id="62bee-110">From the available options, select **Source Control Explorer**.</span></span>

<span data-ttu-id="62bee-111">للتأكد من أنك تبحث عن أحدث إصدار تم إيداعه من الكائنات في مستكشف التحكم في المصادر، انقر بزر الماوس الأيمن فوق الكائنات وحدد **الحصول على أحدث إصدار**.</span><span class="sxs-lookup"><span data-stu-id="62bee-111">To make sure that you are looking at the most recent checked-in version of objects in the Source Control Explorer, right-click on the objects and select **Get Latest Version**.</span></span> <span data-ttu-id="62bee-112">بدلاً من ذلك، يمكنك القيام بذلك على مستوى المجلد للحصول على جميع التحديثات.</span><span class="sxs-lookup"><span data-stu-id="62bee-112">Alternatively, you can do this at the folder level to get all the updates.</span></span>

<span data-ttu-id="62bee-113">يجب أن تحصل دائماً على أحدث الملفات من الفرع الذي تعمل فيه قبل إيداع التغييرات الجديدة.</span><span class="sxs-lookup"><span data-stu-id="62bee-113">You should always get the latest files from the branch that you are working in before checking in new changes.</span></span> <span data-ttu-id="62bee-114">إذا قام شخص آخر أيضاً بدفع التغييرات إلى الملف الذي كنت تقوم بتحريره، فإن ذلك يمنحك فرصة لتسوية تغييراتك مع تغييراته والتأكد من عمل جميع الميزات قبل إيداع التغييرات الناتجة.</span><span class="sxs-lookup"><span data-stu-id="62bee-114">If someone else has also pushed changes to the file that you were editing, this will give you an opportunity to reconcile your changes with theirs and make sure that all the features are working before the resulting changes are checked in.</span></span>

<span data-ttu-id="62bee-115">لإجراء عملية الإيداع، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="62bee-115">To perform the check-in process, follow these steps:</span></span>

1.  <span data-ttu-id="62bee-116">حدد **التغييرات المعلقة** من نافذة **مستكشف الفريق**.</span><span class="sxs-lookup"><span data-stu-id="62bee-116">Select **Pending Changes** from the **Team Explorer** window.</span></span>
2.  <span data-ttu-id="62bee-117">أدخل تعليقاً على الإيداع.</span><span class="sxs-lookup"><span data-stu-id="62bee-117">Enter a check-in comment.</span></span>
3.  <span data-ttu-id="62bee-118">حدد **إيداع**.</span><span class="sxs-lookup"><span data-stu-id="62bee-118">Select **Check In**.</span></span>

## <a name="merging-code-and-resolving-code-conflicts"></a><span data-ttu-id="62bee-119">دمج الكود وحل تعارضات الأكواد</span><span class="sxs-lookup"><span data-stu-id="62bee-119">Merging code and resolving code conflicts</span></span>

<span data-ttu-id="62bee-120">أحياناً، عند الحصول علي أحدث كود من فرع في Visual Studio، سيكون للكود المخزن في الخادم تغييرات مختلفة عن التغييرات التي أجريتها محلياً.</span><span class="sxs-lookup"><span data-stu-id="62bee-120">Sometimes, when you get the latest code from a branch into Visual Studio, the code stored on the server will have changes that are different from the changes that you made locally.</span></span> <span data-ttu-id="62bee-121">هذا تعارض في الدمج.</span><span class="sxs-lookup"><span data-stu-id="62bee-121">This is a merge conflict.</span></span>

<span data-ttu-id="62bee-122">عندما يواجه Visual Studio تعارضاً في الدمج، سيحاول حله تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="62bee-122">When Visual Studio encounters a merge conflict, it will attempt to resolve it automatically.</span></span> <span data-ttu-id="62bee-123">وتوجد أمثلة هذا الحل في سجل المخرجات.</span><span class="sxs-lookup"><span data-stu-id="62bee-123">Any such resolution is in the output log.</span></span> <span data-ttu-id="62bee-124">إذا فشل حل أي تعارضات تلقائياً، فستظهر في نافذة جديدة تطالبك بإخبار Visual Studio بما يجب أن يفعله لكل ملف متعارض.</span><span class="sxs-lookup"><span data-stu-id="62bee-124">If any conflicts fail to resolve automatically, they will appear in a new window that prompts you to tell Visual Studio what it should do for each conflicting file.</span></span>

<span data-ttu-id="62bee-125">تمنحك نافذة **حل التعارضات** الخيارات التالية لكل ملف:</span><span class="sxs-lookup"><span data-stu-id="62bee-125">The **Resolve Conflicts** window gives you the following options for each file:</span></span>

-   <span data-ttu-id="62bee-126">**الحصول على المصدر** - استخدام الملف الذي قمت بسحبه من التحكم في المصادر، ومحو جميع التغييرات المحلية.</span><span class="sxs-lookup"><span data-stu-id="62bee-126">**Take Source** - Use the file that you pulled from source control, erasing all your local changes.</span></span>
-   <span data-ttu-id="62bee-127">**الاحتفاظ بالملف المحلي** - الاحتفاظ بملفك المحلي، وفقد أي تغييرات موجودة في التحكم في المصادر.</span><span class="sxs-lookup"><span data-stu-id="62bee-127">**Keep Local** - Keep your local file, losing any changes that are present in source control.</span></span>
-   <span data-ttu-id="62bee-128">**الدمج باستخدام أداة الدمج** - عرض كلا الإصدارين من الملف جنباً إلى جنب، واختيار الاحتفاظ بكل تغيير في أي إصدار أو تجاهله، واحداً تلو الآخر.</span><span class="sxs-lookup"><span data-stu-id="62bee-128">**Merge using Merge Tool** - View both versions of the file side by side, choosing to keep or discard each change in either version, one at a time.</span></span>

<span data-ttu-id="62bee-129">لن تتمكن من التحقق من مجموعة التغييرات حتى لا توجد تعارضات دمج لم يتم حلها، لذا فإن إتقان هذه الأدوات هو مفتاح نجاحك كعضو في فريق التطوير.</span><span class="sxs-lookup"><span data-stu-id="62bee-129">You will not be able to check in a changeset until there are no unresolved merge conflicts, so mastering these tools is key to your success as a member of a development team.</span></span>

## <a name="roll-back-changes-in-visual-studio"></a><span data-ttu-id="62bee-130">التراجع عن التغييرات في Visual Studio</span><span class="sxs-lookup"><span data-stu-id="62bee-130">Roll back changes in Visual Studio</span></span>


<span data-ttu-id="62bee-131">يرتكب الجميع أخطاء، وفي بعض الأحيان تحتاج إلى التراجع عن التغييرات التي تم التحقق منها في فرع التحكم في المصادر.</span><span class="sxs-lookup"><span data-stu-id="62bee-131">Everybody makes mistakes, and sometimes you need to roll back changes that were checked into a source control branch.</span></span>

<span data-ttu-id="62bee-132">يسهل تنفيذ ذلك في Visual Studio من مستكشف التحكم في المصادر.</span><span class="sxs-lookup"><span data-stu-id="62bee-132">In Visual Studio, this is simple to accomplish from the Source Control Explorer.</span></span> <span data-ttu-id="62bee-133">انقر بزر الماوس الأيمن فوق الفرع الذي تريد التراجع عن التغييرات منه وحدد **عرض المحفوظات**.</span><span class="sxs-lookup"><span data-stu-id="62bee-133">Right-click the branch that you want to roll back changes from and select **View History**.</span></span> <span data-ttu-id="62bee-134">يفتح هذا التحديد نافذة جديدة، حيث يمكنك مشاهدة جميع مجموعات التغييرات التي تم إيداعها في هذا الفرع.</span><span class="sxs-lookup"><span data-stu-id="62bee-134">This selection opens a new window, where you can see all the changesets that have been checked in to this branch.</span></span> <span data-ttu-id="62bee-135">لاسترجاع مجموعة التغييرات، انقر بزر الماوس الأيمن فوق مجموعه التغييرات وحدد **العودة بأكملها إلى مجموعة التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="62bee-135">To roll back a changeset, right-click the changeset and select **Rollback Entire Changeset**.</span></span>
