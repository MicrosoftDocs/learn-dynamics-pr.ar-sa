---
ms.openlocfilehash: 76015fdff95a649c37e5108f3ef87e67b4d15ee8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071636"
---
## <a name="scenario"></a><span data-ttu-id="a6421-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="a6421-101">Scenario</span></span>

<span data-ttu-id="a6421-102">تمت مطالبتك بالعمل مع بعض وظائف الدُفعات والتنبيهات.</span><span class="sxs-lookup"><span data-stu-id="a6421-102">You have been asked to work with some batch jobs and alerts.</span></span> <span data-ttu-id="a6421-103">للقيام بذلك، يجب أولاً القيام بالمهام التالية:</span><span class="sxs-lookup"><span data-stu-id="a6421-103">To do this, you must perform the following tasks:</span></span>

1. <span data-ttu-id="a6421-104">إنشاء وظيفة دفعية</span><span class="sxs-lookup"><span data-stu-id="a6421-104">Create a batch job</span></span>
1. <span data-ttu-id="a6421-105">إنشاء تكرار</span><span class="sxs-lookup"><span data-stu-id="a6421-105">Create a recurrence</span></span>
1. <span data-ttu-id="a6421-106">إضافة تنبيهات</span><span class="sxs-lookup"><span data-stu-id="a6421-106">Add alerts</span></span>
1. <span data-ttu-id="a6421-107">نسخ وظيفة دفعية</span><span class="sxs-lookup"><span data-stu-id="a6421-107">Copy a batch job</span></span>
1. <span data-ttu-id="a6421-108">تمكين الوظيفة الدفعية</span><span class="sxs-lookup"><span data-stu-id="a6421-108">Enable the batch job</span></span>
1. <span data-ttu-id="a6421-109">تعيين دور مدير الدُفعات إلى مستخدم</span><span class="sxs-lookup"><span data-stu-id="a6421-109">Assign the Batch manager role to a user</span></span>


## <a name="create-a-batch-job"></a><span data-ttu-id="a6421-110">إنشاء وظيفة دفعية</span><span class="sxs-lookup"><span data-stu-id="a6421-110">Create a batch job</span></span>

1. <span data-ttu-id="a6421-111">انتقل إلى **إدارة النظام > استعلامات > وظائف الدُفعة**.</span><span class="sxs-lookup"><span data-stu-id="a6421-111">Go to **System administration > Inquiries > Batch jobs**.</span></span>
2. <span data-ttu-id="a6421-112">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="a6421-112">Select **New**.</span></span>
3. <span data-ttu-id="a6421-113">في الحقل **وصف الوظيفة**، أدخل قيمة، مثل **دُفعة تحديث التخزين المؤقت للبيانات**.</span><span class="sxs-lookup"><span data-stu-id="a6421-113">In the **Job description** field, enter a value, such as **Data cache refresh batch**.</span></span>
4. <span data-ttu-id="a6421-114">في الحقل **وقت/ تاريخ البدء المجدول**، أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="a6421-114">In the **Scheduled start date/time** field, enter a date and time.</span></span>
5. <span data-ttu-id="a6421-115">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a6421-115">Select **Save**.</span></span>

## <a name="create-a-recurrence"></a><span data-ttu-id="a6421-116">إنشاء تكرار</span><span class="sxs-lookup"><span data-stu-id="a6421-116">Create a recurrence</span></span>

1. <span data-ttu-id="a6421-117">في **جزء الإجراءات**، حدد **الوظيفة الدفعية**.</span><span class="sxs-lookup"><span data-stu-id="a6421-117">On the **Action Pane**, select **Batch job**.</span></span>
2. <span data-ttu-id="a6421-118">حدد **التكرار** واستخدم الخيارات لإدخال نطاق ونمط التكرار.</span><span class="sxs-lookup"><span data-stu-id="a6421-118">Select **Recurrence** and use the options to enter a range and pattern for the recurrence.</span></span>
3. <span data-ttu-id="a6421-119">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a6421-119">Select **OK**.</span></span>

## <a name="add-alerts"></a><span data-ttu-id="a6421-120">إضافة تنبيهات</span><span class="sxs-lookup"><span data-stu-id="a6421-120">Add alerts</span></span> 

1. <span data-ttu-id="a6421-121">في **جزء الإجراءات**، حدد **الوظيفة الدفعية**.</span><span class="sxs-lookup"><span data-stu-id="a6421-121">On the **Action Pane**, select **Batch job**.</span></span>
2. <span data-ttu-id="a6421-122">حدد **التنبيهات**.</span><span class="sxs-lookup"><span data-stu-id="a6421-122">Select **Alerts**.</span></span>
3. <span data-ttu-id="a6421-123">قم بالإشارة إلى ما إذا كنت تريد إرسال رسائل التنبيه عند انتهاء الوظيفة الدفعية أم وقوع خطأ بها أو عند إلغائها.</span><span class="sxs-lookup"><span data-stu-id="a6421-123">Indicate if you want alert messages sent when the batch job ends, has an error, or is canceled.</span></span> <span data-ttu-id="a6421-124">بعد ذلك حدد ما إذا كنت تريد عرض التنبيهات كرسائل منبثقة.</span><span class="sxs-lookup"><span data-stu-id="a6421-124">Then specify if you want the alerts to be displayed as pop-up messages.</span></span>
4. <span data-ttu-id="a6421-125">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a6421-125">Select **OK**.</span></span>


## <a name="copy-a-batch-job"></a><span data-ttu-id="a6421-126">نسخ وظيفة دفعية</span><span class="sxs-lookup"><span data-stu-id="a6421-126">Copy a batch job</span></span>

1.  <span data-ttu-id="a6421-127">حدد **إدارة النظام** > **استعلامات** > **وظائف الدفعة**.</span><span class="sxs-lookup"><span data-stu-id="a6421-127">Select **System administration** > **Inquiries** > **Batch jobs**.</span></span>
2.  <span data-ttu-id="a6421-128">حدد الوظيفة التي ترغب في نسخها، وفي **جزء الإجراء**، حدد **الوظيفة الدفعية** > **نسخ الوظيفة الدفعية**.</span><span class="sxs-lookup"><span data-stu-id="a6421-128">Select the job that you want to copy, and on the **Action Pane**, select **Batch Job** > **Copy batch job**.</span></span>
3.  <span data-ttu-id="a6421-129">قم بإدخال أية تغييرات أو إضافتها.</span><span class="sxs-lookup"><span data-stu-id="a6421-129">Enter or add any changes.</span></span> <span data-ttu-id="a6421-130">في حالة تعيين **عرض المهام لوظيفة الدفعة الجديدة** إلى **نعم**، فعند تحديد **موافق** ستنتقل مباشرةً إلى صفحة **مهام الدفعات** الخاصة بالمهمة المنسوخة.</span><span class="sxs-lookup"><span data-stu-id="a6421-130">If you set **View tasks for the new batch job** to **Yes**, when you select **OK** you will go directly to the **Batch tasks** page for the copied job.</span></span>


<span data-ttu-id="a6421-131">سيتم إنشاء الوظيفة الدفعية المنسوخة بالحالة **اقتطاع**، لذا ستحتاج إلى تمكينها.</span><span class="sxs-lookup"><span data-stu-id="a6421-131">The copied batch job will be created with a **Withhold** status, so you will need to enable it.</span></span> <span data-ttu-id="a6421-132">كما يمكن تعيين مستخدم **التشغيل بواسطة** لمنح هذا المستخدم الامتيازات المطلوبة لتشغيل الوظيفة من دون كونه مسؤول نظام.</span><span class="sxs-lookup"><span data-stu-id="a6421-132">The **Run by** user can also be set to give this user the privilege to run the job without being a Sys Admin.</span></span>

4. <span data-ttu-id="a6421-133">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a6421-133">Close the page.</span></span>

## <a name="enable-the-batch-job"></a><span data-ttu-id="a6421-134">تمكين الوظيفة الدفعية</span><span class="sxs-lookup"><span data-stu-id="a6421-134">Enable the batch job</span></span>

1.  <span data-ttu-id="a6421-135">في الصفحة **وظائف الدفعة**، في جزء الإجراء، حدد **الوظيفة الدفعية** > **تغييرالحالة**.</span><span class="sxs-lookup"><span data-stu-id="a6421-135">On the **Batch jobs** page, on the Action Pane, select **Batch job** > **Change status**.</span></span>
2.  <span data-ttu-id="a6421-136">حدد حالة **الانتظار**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a6421-136">Select the **Waiting** status, and then select **OK**.</span></span>


## <a name="assign-the-batch-job-manager-role-to-a-user"></a><span data-ttu-id="a6421-137">تعيين دور مدير الوظيفة الدفعية إلى مستخدم</span><span class="sxs-lookup"><span data-stu-id="a6421-137">Assign the Batch job manager role to a user</span></span>

1. <span data-ttu-id="a6421-138">حدد **إدارة النظام** > **الأمان** > **تعيين مستخدمين للأدوار**.</span><span class="sxs-lookup"><span data-stu-id="a6421-138">Select **System administration** > **Security** > **Assign users to roles**.</span></span>
2. <span data-ttu-id="a6421-139">حدد **مدير الوظيفة الدفعية**، وفي الجزء الأيمن، حدد **تعيين/استبعاد المستخدمين يدوياً**.</span><span class="sxs-lookup"><span data-stu-id="a6421-139">Select **Batch Job Manager**, and on the left pane, select **Manually assign/exclude users**.</span></span> 
3. <span data-ttu-id="a6421-140">حدد مستخدماً من القائمة، ثم حدد **تعيين إلى دور**.</span><span class="sxs-lookup"><span data-stu-id="a6421-140">Select a user from the list, and then select **Assign to role**.</span></span> 
4. <span data-ttu-id="a6421-141">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a6421-141">Close the page.</span></span>
