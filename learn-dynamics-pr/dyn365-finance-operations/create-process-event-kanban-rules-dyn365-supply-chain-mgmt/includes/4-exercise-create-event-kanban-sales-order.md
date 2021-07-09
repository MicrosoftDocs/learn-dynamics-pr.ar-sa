---
ms.openlocfilehash: 9514828c7b3ab3e0e0a0841a702281e61929faad
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073503"
---
## <a name="before-you-begin"></a><span data-ttu-id="ad5f6-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="ad5f6-101">Before you begin</span></span>
<span data-ttu-id="ad5f6-102">لتحقيق الاستفادة القصوى من التمارين في هذه الوحدة النمطية، ننصحك بأن تكون عينة البيانات القياسية متوفرة في Supply Chain Management التي يتم تثبيتها باستخدام Lifecycle Services ‏(LCS).‬</span><span class="sxs-lookup"><span data-stu-id="ad5f6-102">To get the most benefit from the exercises in this module, we recommend that you have the standard sample data available in Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

<span data-ttu-id="ad5f6-103">تم استلام أمر مبيعات لمجموعات مكبرات صوت باللون الأخضر، يؤدي إلى تشغيل وظائف كانبان للأحداث لمجموعة مكبرات صوت في خلية عمل التغليف والتعبئة ومجموعات أدوات مكبرات الصوت في خلية عمل تجميع مكبرات الصوت.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-103">A sales order has been received for a green speaker set, which triggers event kanbans for the speaker set on the packaging work cell and the speaker kits on the speaker assembly work cell.</span></span> <span data-ttu-id="ad5f6-104">عليك إنتاج مجموعات مواد مكبر الصوت وأجهزة مكبرات الصوت لتنفيذ أمر مبيعات العميل.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-104">Produce the speaker kits and speaker set to fulfill the customer sales order.</span></span>

## <a name="crete-a-kanban-line-event"></a><span data-ttu-id="ad5f6-105">إنشاء حدث بند كانبان‬</span><span class="sxs-lookup"><span data-stu-id="ad5f6-105">Crete a kanban line event</span></span>

1.  <span data-ttu-id="ad5f6-106">انتقل إلى **المبيعات والتسويق > أوامر المبيعات > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-106">Go to **Sales and marketing > Sales orders > All sales orders**.</span></span>

2.  <span data-ttu-id="ad5f6-107">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-107">Select **New**.</span></span>

3.  <span data-ttu-id="ad5f6-108">حدد **حساب العميل**، **US-016**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-108">Select the **Customer account** as **US-016**.</span></span>

4.  <span data-ttu-id="ad5f6-109">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-109">Select **OK**.</span></span>

5.  <span data-ttu-id="ad5f6-110">أدخل **رقم الصنف**، **L0026**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-110">Enter an **Item number** of **L0026**.</span></span>

6.  <span data-ttu-id="ad5f6-111">حدد متغيراً مثل **VN-000130**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-111">Select a variant such as **VN-000130**.</span></span>

7.  <span data-ttu-id="ad5f6-112">أدخل **الكمية** **12.00**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-112">Enter a **Quantity** of **12.00**.</span></span>

8.  <span data-ttu-id="ad5f6-113">حدد **1** لخيار **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-113">Select **1** for the **Site**.</span></span>

9.  <span data-ttu-id="ad5f6-114">حدد **13** لخيار **المستودع**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-114">Select **13** for the **Warehouse**.</span></span>

10. <span data-ttu-id="ad5f6-115">حدد **13** لخيار **الموقع**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-115">Select **13** for the **Location**.</span></span>

11. <span data-ttu-id="ad5f6-116">إذا لم يتم تعيين **الموقع** على أمر المبيعات، فحدد الزر **بند أمر المبيعات > عرض > الأبعاد**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-116">If **Location** is not set on the sales order, select the **Sales order line > Display > Dimensions** button.</span></span>

12. <span data-ttu-id="ad5f6-117">حدد زر القائمة **المنتج والتوريد‬‏‫ > المتطلبات > عرض شجرة تثبيت السعر‬‏‫** لعرض وظائف كانبان للأحداث المُنشأة لأمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-117">Select the **Product and supply > Requirements > View pegging tree** menu button to view the event kanbans that are created for the sales order.</span></span>

## <a name="plan-the-kanbans"></a><span data-ttu-id="ad5f6-118">تخطيط كانبان</span><span class="sxs-lookup"><span data-stu-id="ad5f6-118">Plan the kanbans</span></span>

<span data-ttu-id="ad5f6-119">استخدم الخطوات التالية لتخطيط وظائف كانبان على خلايا التغليف والتعبئة وتجميع مكبرات الصوت.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-119">Use the following steps to plan the kanbans on the packaging and speaker assembly work cells.</span></span> <span data-ttu-id="ad5f6-120">يستمر هذا الجزء من التمرين من الخطوات السابقة.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-120">This part of the exercise continues from the previous steps.</span></span>

1.  <span data-ttu-id="ad5f6-121">انتقل إلى **التحكم بالإنتاج > كانبان > جدولة وظيفة كانبان**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-121">Go to **Production control > Kanban > Kanban job scheduling**.</span></span>

2.  <span data-ttu-id="ad5f6-122">حدد القائمة المنسدلة **خلية العمل**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-122">Select the **Work cell** drop-down menu.</span></span>

3.  <span data-ttu-id="ad5f6-123">حدّث **خلية العمل** إلى **1275**، واطّلع على وظائف كانبان المخطط لها.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-123">Update the **Work cell** to **1275**, and see planned kanbans.</span></span>

4.  <span data-ttu-id="ad5f6-124">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-124">Close all pages.</span></span>

5.  <span data-ttu-id="ad5f6-125">انتقل إلى **التحكم بالإنتاج > كانبان > لوحة كانبان لوظائف المعالجة**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-125">Go to **Production control > Kanban > Kanban board for process jobs**.</span></span>

6.  <span data-ttu-id="ad5f6-126">حدد الزر **تغيير الخلية**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-126">Select the **Change cell** button.</span></span>

7.  <span data-ttu-id="ad5f6-127">حدّث **خلية العمل** إلى **1250**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-127">Update the **Work cell** to **1250**.</span></span>

8.  <span data-ttu-id="ad5f6-128">ميّز وظائف كانبان المطلوبة، ثم حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-128">Highlight the desired kanbans and then select **Start**.</span></span>

9.  <span data-ttu-id="ad5f6-129">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-129">Select **Complete**.</span></span>

12. <span data-ttu-id="ad5f6-130">ميّز وظيفة كانبان، وانتقل إلى علامة تبويب **تثبيت السعر** في صفحة خلية عمل **لوحة كانبان لوظائف المعالجة‬**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-130">Highlight a kanban and switch to the **Pegging** tab on the **Kanban board for process jobs** work cell page.</span></span> <span data-ttu-id="ad5f6-131">استعرض وظائف كانبان لمجموعة مكبرات صوت ذات مستوى أدنى على شجرة تثبيت السعر.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-131">View the complete lower-level speaker set kanbans on the pegging tree.</span></span>

13. <span data-ttu-id="ad5f6-132">حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-132">Select **Start**.</span></span>

14. <span data-ttu-id="ad5f6-133">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-133">Select **Complete**.</span></span>

## <a name="transfer-the-speaker-set"></a><span data-ttu-id="ad5f6-134">تحويل مجموعة مكبرات الصوت</span><span class="sxs-lookup"><span data-stu-id="ad5f6-134">Transfer the speaker set</span></span>

<span data-ttu-id="ad5f6-135">اتبع الخطوات التالية لتحويل مجموعة مكبرات الصوت إلى المستودع:</span><span class="sxs-lookup"><span data-stu-id="ad5f6-135">Follow these steps to transfer the speaker set to the warehouse:</span></span>

1.  <span data-ttu-id="ad5f6-136">انتقل إلى **التحكم بالإنتاج > كانبان > لوحة كانبان لمهام التحويل**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-136">Go to **Production control > Kanban > Kanban board for transfer jobs**.</span></span>

2.  <span data-ttu-id="ad5f6-137">قم بتوسيع علامة التبويب السريعة **عوامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-137">Expand the **Filters** FastTab.</span></span>

3.  <span data-ttu-id="ad5f6-138">حدد **تدفق إنتاج**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-138">Select a **Production Flow**.</span></span>

4.  <span data-ttu-id="ad5f6-139">حدد **تحويل** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-139">Select **TRANSFER** on the Action Pane.</span></span>

5.  <span data-ttu-id="ad5f6-140">حدد **تحديث قائمة الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-140">Select **Update picking list**.</span></span>

5.  <span data-ttu-id="ad5f6-141">حدد **إضافة بند الانتقاء**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-141">Select **Add picking line**.</span></span>

6.  <span data-ttu-id="ad5f6-142">حدد **تأكيد انتقاء الكل**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-142">Select **Confirm pick all**.</span></span>

7.  <span data-ttu-id="ad5f6-143">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-143">Close the page.</span></span>

8.  <span data-ttu-id="ad5f6-144">حدد **بدء**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-144">Select **Start**.</span></span>

9.  <span data-ttu-id="ad5f6-145">حدد **إكمال**.</span><span class="sxs-lookup"><span data-stu-id="ad5f6-145">Select **Complete**.</span></span> 
