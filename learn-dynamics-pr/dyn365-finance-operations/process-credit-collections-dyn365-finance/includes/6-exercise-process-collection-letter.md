---
ms.openlocfilehash: c4eb1ce536491b8b1d336f5b0a738d4d396d952e
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070722"
---
## <a name="scenario"></a><span data-ttu-id="2c7ce-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="2c7ce-101">Scenario</span></span>

<span data-ttu-id="2c7ce-102">يجب أن يقوم مدير الائتمان والتحصيلات بشركة Contoso المعروفة بـ **USMF** بمعالجة وإرسال خطاب تحصيل للعميل Forest Wholesales (US-003).</span><span class="sxs-lookup"><span data-stu-id="2c7ce-102">The Credit and Collections Manager at Contoso company **USMF**, must process and post a collection letter for customer Forest Wholesales (US-003).</span></span> <span data-ttu-id="2c7ce-103">في الملخص، هذه هي الإجراءات التي تحتاجها للقيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-103">In summary, these are the actions you need to do this.</span></span>

1. <span data-ttu-id="2c7ce-104">قم بتشغيل وظيفة خطاب تحصيل لخطاب التحصيل.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-104">Run a collection letter job for the collection letter.</span></span>
2. <span data-ttu-id="2c7ce-105">استخدم الأول من أبريل 2020 كتاريخ.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-105">Use 1st April 2020 as the date.</span></span> 
3. <span data-ttu-id="2c7ce-106">اطبع الخطاب.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-106">Print the letter.</span></span>
4. <span data-ttu-id="2c7ce-107">قم بترحيل خطاب التحصيل.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-107">Post the collection letter.</span></span>

### <a name="to-run-a-collection-letter-job"></a><span data-ttu-id="2c7ce-108">لتشغيل وظيفة خطاب التحصيل:</span><span class="sxs-lookup"><span data-stu-id="2c7ce-108">To run a Collection letter job:</span></span>

1. <span data-ttu-id="2c7ce-109">في شركة **USMF** انتقل إلى **الائتمان والتحصيلات** > **خطاب التحصيل >** **إنشاء خطابات تحصيل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-109">In company **USMF** go to **Credit and collections** > **Collection letter >** **Create Collection letters**.</span></span>
1. <span data-ttu-id="2c7ce-110">قم بتعيين حقل **فاتورة** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-110">Set the **Invoice** field to **Yes**.</span></span>
3. <span data-ttu-id="2c7ce-111">حدد القائمة المنسدلة **خطاب التحصيل**، ثم حدد **الكل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-111">Select the **Collection letter** drop-down, and then select **All**.</span></span>
4. <span data-ttu-id="2c7ce-112">في حقل **تاريخ خطاب التحصيل**، أدخل **الأول من أبريل 2020**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-112">In the **Collection letter date** field, enter **1st April 2020**.</span></span> 
5. <span data-ttu-id="2c7ce-113">حدد القائمة المنسدلة **استخدام ملف تعريف الترحيل من** ثم انقر على **تحديد**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-113">Select the **Use posting profile from** drop-down, and then click **Select**.</span></span>
6. <span data-ttu-id="2c7ce-114">حدد القائمة المنسدلة **ملف تعريف الترحيل** ثم انقر على **GEN‎**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-114">Select the **Posting profile** drop-down, and then select **GEN**.</span></span>
8. <span data-ttu-id="2c7ce-115">قم بتوسيع علامة التبويب السريعة **السجلات المطلوب تضمينها**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-115">Expand the **Records to include** FastTab.</span></span>
9. <span data-ttu-id="2c7ce-116">حدد الرمز **عامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-116">Select the **Filter** icon.</span></span>
10. <span data-ttu-id="2c7ce-117">أدخل **US-003** في عمود **المعايير** في الصف **حساب العميل** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-117">Enter **US-003** in the **Criteria** column on the **Customer account** row, and then select **OK**.</span></span>
11. <span data-ttu-id="2c7ce-118">حدد **موافق** لمعالجة الوظيفة **إنشاء خطاب التحصيل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-118">Select **OK** to process the **Creation of collection letter** job.</span></span> <span data-ttu-id="2c7ce-119">ستظهر رسالة في مركز الإجراء تفيد بأن عملية إنشاء خطاب التحصيل قد اكتملت.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-119">A message will appear in the Action center that the Collection letter creation process is complete.</span></span>
12. <span data-ttu-id="2c7ce-120">أغلق مركز الإجراء.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-120">Close the Action center.</span></span>

### <a name="follow-these-steps-to-review-print-and-post-the-collection-letter"></a><span data-ttu-id="2c7ce-121">اتبع الخطوات التالية لمراجعة خطاب التحصيل وطباعته وترحيله:</span><span class="sxs-lookup"><span data-stu-id="2c7ce-121">Follow these steps to review, print, and post the collection letter:</span></span>

1. <span data-ttu-id="2c7ce-122">انتقل إلى **‎الائتمان والتحصيلات** > **خطاب تحصيل** >
    **مراجعة خطابات التحصيل ومعالجتها**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-122">Go to **Credit and collections** > **Collection letter** >
 **Review and process collection letters**.</span></span>
1. <span data-ttu-id="2c7ce-123">حدد خطاب التحصيل الذي تم إنشاؤه مسبقاً للعميل **US-003** وافتحه (يمكنك الفرز حسب التاريخ لإحضاره إلى أعلى القائمة)</span><span class="sxs-lookup"><span data-stu-id="2c7ce-123">Select and open the collection letter previously created for customer **US-003** (you can sort by date to bring it to the top of the list).</span></span>
2. <span data-ttu-id="2c7ce-124">حدد الزر **طباعة** ثم حدد **إشعار خطاب التحصيل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-124">Select the **Print** button, and then select **Collection letter note**.</span></span>
1. <span data-ttu-id="2c7ce-125">حدد **موافق** في الصفحة **إشعار خطاب التحصيل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-125">Select **OK** in the **Collection letter note** page.</span></span>
1. <span data-ttu-id="2c7ce-126">راجع خطاب التحصيل.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-126">Review the collection letter.</span></span>
1. <span data-ttu-id="2c7ce-127">أغلق خطاب التحصيل.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-127">Close the collection letter.</span></span> <span data-ttu-id="2c7ce-128">يتم الآن تعيين الحقل **مطبوع** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-128">The **Printed** field is now set to **Yes**.</span></span>
1. <span data-ttu-id="2c7ce-129">أثناء وجودك في خطاب التحصيل الذي تم إنشاؤه مسبقاً للعميل **US-003** حدد الزر **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-129">While on the collection letter previously created for customer  **US-003**, select the **Post** button.</span></span>
1. <span data-ttu-id="2c7ce-130">حدد تاريخ اليوم في الحقل **تاريخ الترحيل**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-130">Select today's date in the **Posting date** field.</span></span>
1. <span data-ttu-id="2c7ce-131">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-131">Select **OK**.</span></span> <span data-ttu-id="2c7ce-132">يظهر شريطان أزرقان؛ منهما شريط بالرسالة **اكتملت العملية**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-132">Two blue bars appear; one with the message **Operation completed**.</span></span> <span data-ttu-id="2c7ce-133">تحتوي الرسالة الأخرى على رقم خطاب التحصيل، بالإضافة إلى رمز خطاب التحصيل والعميل الذي تمت معالجته.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-133">The other message contains the collection letter number, as well as the collection letter code and customer that was processed.</span></span>
1. <span data-ttu-id="2c7ce-134">أغلق صفحة **مراجعة خطابات التحصيل المراجعة ومعالجتها**.</span><span class="sxs-lookup"><span data-stu-id="2c7ce-134">Close the **Review and process collection letters** page.</span></span>
