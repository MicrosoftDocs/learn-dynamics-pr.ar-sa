---
ms.openlocfilehash: f8d555c65a727181fb0d9551243546165a66368d
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072273"
---
<span data-ttu-id="71e0c-101">يُستخدم Application Object Server‏ (AOS) لتطبيقات Finance and Operations لمشاركة كائنات التطبيق والمعلومات كأداة فعالة لزيادة أداء التطبيق.</span><span class="sxs-lookup"><span data-stu-id="71e0c-101">The Finance and Operations apps Application Object Server (AOS) is used for sharing application objects and information as an effective tool to increase application performance.</span></span>

<span data-ttu-id="71e0c-102">يتصل تطبيق الأجهزة المحمولة بـ AOS للحصول على البيانات الوصفية لمساحات العمل المحمولة (والصفحات والحقول التي تظهر على الصفحة)، وللحصول على بيانات للحقول الموجودة على الصفحات.</span><span class="sxs-lookup"><span data-stu-id="71e0c-102">The mobile app communicates with the AOS to get metadata for the mobile workspaces (and the pages and fields that appear on the page), and to get data for the fields on the pages.</span></span> 
 
![رسم تخطيطي يوضح كيفية اتصال تطبيق الأجهزة المحمولة بـ AOS للحصول على البيانات.](../media/aos.png) 

<span data-ttu-id="71e0c-104">في كل مرة يطلب فيها تطبيق الأجهزة المحمولة بيانات لصفحة ما، تُنشئ AOS جلسة جديدة تستخدم سياق الشخص الذي يستخدم تطبيق الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="71e0c-104">Each time that the mobile app requests data for a page, AOS creates a new session that uses the context of the person who is using the mobile app.</span></span> <span data-ttu-id="71e0c-105">ويستخدم AOS بعد ذلك سياق هذا الشخص لفتح النماذج المقابلة (باستخدام عناصر القائمة المقابلة).</span><span class="sxs-lookup"><span data-stu-id="71e0c-105">AOS then uses that person’s context to open the corresponding forms (by using the corresponding menu items).</span></span> 

<span data-ttu-id="71e0c-106">يمكن لـ AOS فتح نماذج متعددة في تتابع سريع وتنفيذ إجراءات على تلك النماذج (على سبيل المثال، التصفية وفتح **مربعات الحقائق**، وتغيير صفحات علامات التبويب والنقر فوق الأزرار).</span><span class="sxs-lookup"><span data-stu-id="71e0c-106">AOS can open multiple forms in quick succession and perform actions on those forms (for example, filtering, opening **Fact Boxes**, changing tab pages, and clicking buttons).</span></span> <span data-ttu-id="71e0c-107">يتم أيضاً تشغيل أي منطق أعمال في النماذج كالمعتاد.</span><span class="sxs-lookup"><span data-stu-id="71e0c-107">Any business logic on the forms is also run as usual.</span></span> <span data-ttu-id="71e0c-108">من خلال هذه العملية، يجمع AOS قيم البيانات من الحقول المطلوبة ثم يرسل تلك البيانات مرة أخرى إلى تطبيق الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="71e0c-108">Through that process, AOS collects the data values from the requested fields and then sends that data back to the mobile app.</span></span>

## <a name="navigate-the-mobile-app"></a><span data-ttu-id="71e0c-109">التنقل في تطبيق الأجهزة المحمولة</span><span class="sxs-lookup"><span data-stu-id="71e0c-109">Navigate the mobile app</span></span>

<span data-ttu-id="71e0c-110">لبدء العمل مع إطار عمل تطبيق الأجهزة المحمولة، انتقل إلى **الإعدادات > تطبيق الأجهزه المحمولة**.</span><span class="sxs-lookup"><span data-stu-id="71e0c-110">To start working with the mobile app framework, go to **Settings > Mobile app**.</span></span>
 

<span data-ttu-id="71e0c-111">يتكون التنقل في تطبيق الأجهزة المحمولة من أربعة مفاهيم بسيطة: لوحة المعلومات ومساحات العمل والصفحات والإجراءات.</span><span class="sxs-lookup"><span data-stu-id="71e0c-111">Navigation in the mobile app consists of four simple concepts: the dashboard, workspaces, pages, and actions.</span></span> 

<span data-ttu-id="71e0c-112">عند فتح إطار عمل تطبيق الأجهزة المحمولة، يمكنك عرض إدارة مصمم تطبيقات الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="71e0c-112">When the mobile app framework opens, you can view the Manage mobile app designer.</span></span> <span data-ttu-id="71e0c-113">هنا، يمكنك نشر التطبيقات وإلغاء نشرها، واستيراد التطبيقات وتصديرها، وإنشاء تطبيق أجهزة محمولة جديد.</span><span class="sxs-lookup"><span data-stu-id="71e0c-113">Here, you can publish and unpublish apps, import and export apps, and create a new mobile app.</span></span>
 
<span data-ttu-id="71e0c-114">عند بدء تشغيل التطبيق، يتم فتحه على لوحة المعلومات.</span><span class="sxs-lookup"><span data-stu-id="71e0c-114">When you start the app, it opens on the dashboard.</span></span> <span data-ttu-id="71e0c-115">في لوحة المعلومات، لاحظ أنها تحتوي على قائمة بمساحات العمل المتوفرة في بيئة تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="71e0c-115">On the dashboard, notice that it contains a list of workspaces that are available in your Finance and Operations apps environment.</span></span>
 

![لقطة شاشة لصفحة إدارة تطبيق الأجهزة المحمولة.](../media/manage-mobile-app.png) 

<span data-ttu-id="71e0c-117">في كل مساحة عمل، يمكنك عرض قائمة بالصفحات المتوفرة لمساحة العمل هذه.</span><span class="sxs-lookup"><span data-stu-id="71e0c-117">In each workspace, you can view a list of pages that are available for that workspace.</span></span> 
 

 ![لقطة شاشة لصفحة إدارة تطبيق الأجهزة المحمولة مع تمييز إضافة حقول الصفحة.](../media/page.png) 

<span data-ttu-id="71e0c-119">في إحدى الصفحات، يمكنك عرض البيانات التي تم تجميعها من صفحة أو أكثر من صفحات تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="71e0c-119">On a page, you can view data that is collected from one or more Finance and Operations apps pages.</span></span>
 
 ![لقطة شاشة لصفحة إدارة تطبيق الأجهزة المحمولة مع تمييز إضافة حقول التحديد.](../media/field.png)

<span data-ttu-id="71e0c-121">تقوم وظيفة خطوة الوظيفة تلقائياً بإنشاء دليل المهام لمستخدم الأعمال، كما هو موضح في الشكل التالي.</span><span class="sxs-lookup"><span data-stu-id="71e0c-121">The job-step functionality automatically generates the task guide for the business user, as shown in the following figure.</span></span>
 
 ![لقطة شاشة لدليل المهام لإنشاء عميل جديد.](../media/app-task-guide.png)

<span data-ttu-id="71e0c-123">من إحدى الصفحات، يمكنك الانتقال إلى صفحات أخرى للحصول على البيانات ذات الصلة، مثل تفاصيل أو بنود الكيان.</span><span class="sxs-lookup"><span data-stu-id="71e0c-123">From a page, you can go to other pages for related data, such as an entity details or lines.</span></span> <span data-ttu-id="71e0c-124">في الصفحة، يمكنك عرض قائمة بالإجراءات المتوفرة لهذه الصفحة.</span><span class="sxs-lookup"><span data-stu-id="71e0c-124">On a page, you can view a list of actions that are available for that page.</span></span> <span data-ttu-id="71e0c-125">تتيح لك الإجراءات إنشاء بيانات موجودة أو تحريرها.</span><span class="sxs-lookup"><span data-stu-id="71e0c-125">Actions let you create or edit existing data.</span></span>
 

 ![لقطة شاشة لصفحة إدارة تطبيق الأجهزة المحمولة تعرض قائمة الإجراءات المتاحة.](../media/action.png)

<span data-ttu-id="71e0c-127">بعد الانتهاء من تصميم التطبيق الخاص بك، انشره لإتاحته في تطبيق Dynamics 365 for Unified Operations للأجهزة المحمولة‬ على جهازك.</span><span class="sxs-lookup"><span data-stu-id="71e0c-127">After you finish designing your application, publish it to make it available on Dynamics 365 for Unified operations mobile app on your device.</span></span> <span data-ttu-id="71e0c-128">لعرض التطبيق المنشور على جهازك الذكي، مثل الهاتف أو الكمبيوتر اللوحي، يمكنك إما لمس الشاشة بإصبعك أو استخدام جهاز تأشير للضغط على زر، وسحب الشاشة لأسفل، ثم تحريرها.</span><span class="sxs-lookup"><span data-stu-id="71e0c-128">To view the published application on your smart device, such as phone or tablet, you can either touch the screen with a finger or use a pointing device to press a button, drag the screen downward, and then release it.</span></span> <span data-ttu-id="71e0c-129">تشير هذه الإجراءات إلى التطبيق، مثل الصفحة الرئيسية (لوحة المعلومات) للتطبيق، حيث يمكنك عرض قائمة مساحات العمل لتحديث محتويات الشاشة.</span><span class="sxs-lookup"><span data-stu-id="71e0c-129">These actions signal to the application, such as the main landing page (dashboard) of the app, where you can view the list of workspaces to refresh the contents of the screen.</span></span> <span data-ttu-id="71e0c-130">يسمى هذا *السحب للتحديث*.</span><span class="sxs-lookup"><span data-stu-id="71e0c-130">This is called *pull-to-refresh*.</span></span> 

<span data-ttu-id="71e0c-131">يمكنك السحب للتحديث في تطبيق الأجهزة المحمولة لجعل تطبيق الأجهزة المحمولة يقوم بتحديث بياناته أو بيانات التعريف الخاصة به في أي وقت.</span><span class="sxs-lookup"><span data-stu-id="71e0c-131">You can pull-to-refresh in the mobile app to make the mobile app update its data or metadata at any time.</span></span> <span data-ttu-id="71e0c-132">بعد تحرير مساحة عمل موجودة أو نشر مساحة عمل، تأكد من السحب للتحديث في تطبيق الأجهزة المحمولة، إما في قائمة مساحات العمل (إذا أضفت مساحة عمل أو منطق عمل) أو قائمة الصفحات (إذا قمت بتعديل صفحة أو إجراء).</span><span class="sxs-lookup"><span data-stu-id="71e0c-132">After editing an existing workspace or publishing a workspace, be sure to pull-to-refresh in the mobile app, in either the list of workspaces (if you added a workspace or business logic) or the list of pages (if you modified a page or an action).</span></span> <span data-ttu-id="71e0c-133">تكون مساحات العمل التي تم نشرها في تطبيقات Finance and Operations مرئية لجميع المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="71e0c-133">Workspaces that have been published to Finance and Operations apps are visible to all users.</span></span> 

<span data-ttu-id="71e0c-134">في تطبيقات Finance and Operations، يقوم أمان عنصر القائمة بإخفاء الصفحات التي لا يمتلك المستخدم حق الوصول إليها تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="71e0c-134">In Finance and Operations apps, menu item security automatically hides pages that the user doesn’t have access to.</span></span> <span data-ttu-id="71e0c-135">إذا لم يكن لدى المستخدم حق الوصول إلى أي صفحات في مساحة العمل، فسيتم إخفاء مساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="71e0c-135">If a user doesn’t have access to any pages in a workspace, the workspace is hidden.</span></span>
<span data-ttu-id="71e0c-136">يتيح لك مصمم تطبيقات الأجهزة المحمولة تحديد حقول البيانات المحددة من النماذج التي يجب أن تظهر في تطبيق الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="71e0c-136">The mobile app designer lets you select the specific data fields from forms that should appear in the mobile app.</span></span>

 
