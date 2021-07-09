---
ms.openlocfilehash: 66b8c4636c04b15f4ad3132ae73f63c2124f14bb
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6072636"
---
## <a name="scenario"></a><span data-ttu-id="5bb01-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="5bb01-101">Scenario</span></span>
<span data-ttu-id="5bb01-102">في هذا التمرين العملي، ستقوم بتصدير البيانات من الكيان **جميع العملاء** باستخدام مساحة العمل **إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="5bb01-102">In this lab, you will export data from the **All customers** entity using the **Data management** workspace.</span></span> 

1.  <span data-ttu-id="5bb01-103">في الشركة **USMF** انتقل إلى **مساحات العمل > إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="5bb01-103">In the company **USMF** navigate to **Workspaces > Data management**.</span></span> 
2.  <span data-ttu-id="5bb01-104">ستري الرسالة **يتم الآن تحديث قائمة الكيانات.**</span><span class="sxs-lookup"><span data-stu-id="5bb01-104">You will see the message **The entity list is being refreshed.**</span></span> <span data-ttu-id="5bb01-105">ويمكنك مواصلة عملك بينما يحدث ذلك.</span><span class="sxs-lookup"><span data-stu-id="5bb01-105">You may continue your work while this happens.</span></span> <span data-ttu-id="5bb01-106">يمكن العثور على حالة الاكتمال لهذه العملية في مركز الرسائل.</span><span class="sxs-lookup"><span data-stu-id="5bb01-106">The completion status of this operation can be found in the message center.</span></span>
3.  <span data-ttu-id="5bb01-107">دع هذه الوظيفة تعمل لعدة دقائق (قد تتلقى خطأ لاحقاً إذا قمت بإغلاقها مبكراً جداً)، ثم "أغلق" نافذة المعلومات هذه.</span><span class="sxs-lookup"><span data-stu-id="5bb01-107">Let this job work for several minutes (you may receive an error later if you close it too early), then Close this information window.</span></span>
2.  <span data-ttu-id="5bb01-108">حدد المربع **تصدير** في الصفحة.</span><span class="sxs-lookup"><span data-stu-id="5bb01-108">Select the **Export** tile on the page.</span></span> 
3.  <span data-ttu-id="5bb01-109">حدد المعلومات التالية في الصفحة:</span><span class="sxs-lookup"><span data-stu-id="5bb01-109">Specify the following information on the page:</span></span>
    - <span data-ttu-id="5bb01-110">**اسم المجموعة** - تصدير العملاء</span><span class="sxs-lookup"><span data-stu-id="5bb01-110">**Group name** - Customers Export</span></span>
    - <span data-ttu-id="5bb01-111">**الوصف** - تصدير العميل</span><span class="sxs-lookup"><span data-stu-id="5bb01-111">**Description** - Customer Export</span></span>
    - <span data-ttu-id="5bb01-112">**نوع عملية مشروع البيانات** - تصدير</span><span class="sxs-lookup"><span data-stu-id="5bb01-112">**Data project operation type** - Export</span></span> 
    - <span data-ttu-id="5bb01-113">**فئة المشروع** - مشروع</span><span class="sxs-lookup"><span data-stu-id="5bb01-113">**Project category** -  Project</span></span>
    - <span data-ttu-id="5bb01-114">**إنشاء حزمة بيانات** - نعم</span><span class="sxs-lookup"><span data-stu-id="5bb01-114">**Generate data package** - Yes</span></span> 
4.  <span data-ttu-id="5bb01-115">حدد **حفظ** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="5bb01-115">Select **Save** in the Action Pane.</span></span> 
5.  <span data-ttu-id="5bb01-116">في علامة التبويب السريعة **الكيانات المحددة**، حدد **إضافة كيان**.</span><span class="sxs-lookup"><span data-stu-id="5bb01-116">In the **Selected entities** FastTab, select **Add entity**.</span></span> 
6.  <span data-ttu-id="5bb01-117">حدد المعلومات التالية في مربع الحوار **إضافة كيان**:</span><span class="sxs-lookup"><span data-stu-id="5bb01-117">Specify the following information in the **Add entity** dialog:</span></span>
    - <span data-ttu-id="5bb01-118">**اسم الكيان** - العملاء V3</span><span class="sxs-lookup"><span data-stu-id="5bb01-118">**Entity name** - Customers V3</span></span>
    - <span data-ttu-id="5bb01-119">**تنسيق البيانات الهدف** - EXCEL</span><span class="sxs-lookup"><span data-stu-id="5bb01-119">**Target data format** - EXCEL</span></span>
    - <span data-ttu-id="5bb01-120">**حدد الحقول** - الحقول القابلة للاستيراد</span><span class="sxs-lookup"><span data-stu-id="5bb01-120">**Select fields** - Importable fields</span></span>
7.  <span data-ttu-id="5bb01-121">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="5bb01-121">Select **Add**.</span></span> <span data-ttu-id="5bb01-122">سيتم إنشاء سطر جديد بمعلومات الكيان التي حددتها.</span><span class="sxs-lookup"><span data-stu-id="5bb01-122">A new line will be created with the entity information you defined.</span></span> 
9.  <span data-ttu-id="5bb01-123">راجع أي تحذيرات، ثم حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="5bb01-123">Review any warnings, and then select **Close**.</span></span> 
10. <span data-ttu-id="5bb01-124">حدد سطر الكيان، ثم حدد **تصدير** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="5bb01-124">Select the entity line, and then select **Export** in the Action Pane.</span></span> <span data-ttu-id="5bb01-125">سيتم تنفيذ مهمة البيانات.</span><span class="sxs-lookup"><span data-stu-id="5bb01-125">The data job will execute.</span></span> 
12. <span data-ttu-id="5bb01-126">حدد **تحديث** عند اكتمال المهمة.</span><span class="sxs-lookup"><span data-stu-id="5bb01-126">Select **Refresh** when the job is complete.</span></span> <span data-ttu-id="5bb01-127">ستتلقى إعلاماً بأن التصدير قد اكتمل.</span><span class="sxs-lookup"><span data-stu-id="5bb01-127">You will receive a notification that the export has completed.</span></span> 
13. <span data-ttu-id="5bb01-128">حدد **تنزيل الحزمة** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="5bb01-128">Select **Download package** in the Action Pane.</span></span> <span data-ttu-id="5bb01-129">سيتم تنزيل ملف .zip.</span><span class="sxs-lookup"><span data-stu-id="5bb01-129">A .zip file will download.</span></span> 
15. <span data-ttu-id="5bb01-130">افتح ملف .zip ثم افتح ملف Excel الموجود في ملف .zip.</span><span class="sxs-lookup"><span data-stu-id="5bb01-130">Open the .zip file and then open the Excel file that is in the .zip file.</span></span> 
16. <span data-ttu-id="5bb01-131">سترى هنا جميع البيانات التي تم تصديرها من Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="5bb01-131">Here you will see all the data that exported from Finance and Operations.</span></span>
