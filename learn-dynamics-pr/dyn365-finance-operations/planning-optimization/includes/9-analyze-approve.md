---
ms.openlocfilehash: b705ebb85b1410ff90243d08ea3f5d3c21dd72d5
ms.sourcegitcommit: 7d4cc5f2048fa309552e39da447684b1d06d0772
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/13/2021
ms.locfileid: "6072467"
---
<span data-ttu-id="fe53b-101">بعد تشغيل "تحسين التخطيط" لأمر مخطط محدد، يمكنك تحليل الأمر والموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="fe53b-101">After Planning Optimization has run for a specific planned order, you can analyze and approve the order.</span></span>

1.  <span data-ttu-id="fe53b-102">افتح **التخطيط الرئيسي > التخطيط الرئيسي > الأوامر المخططة**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-102">Go to **Master planning > Master planning > Planned orders**.</span></span>
2.  <span data-ttu-id="fe53b-103">حدد **الإنتاج المخطط**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-103">Select a **Planned production**.</span></span> 
3.  <span data-ttu-id="fe53b-104">في جزء الإجراءات، في علامة التبويب **طريقة عرض** في مجموعة **المتطلبات**، حدد **تحديد إجمالي المكونات المطلوبة**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-104">In the Action Pane, on the **View** tab in the **Requirements** group, select **Explosion**.</span></span>
4.  <span data-ttu-id="fe53b-105">راجع إجمالي المكونات المطلوبة في هذا الأمر، مما يدل على أنه سيحتاج إلى ثلاثة أوامر شراء للحصول على مواد كافية لتجميع العنصر **P0001**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-105">Review the explosion of this order, which shows that it will need three purchase orders to have enough materials to assemble item **P0001**.</span></span>

    <span data-ttu-id="fe53b-106">[ ![لقطة شاشة لصفحة تحديد إجمالي المكونات المطلوبة للأمر.](../media/explosion-ss.png) ](../media/explosion-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fe53b-106">[ ![Screenshot of the Explosion page for the order.](../media/explosion-ss.png) ](../media/explosion-ss.png#lightbox)</span></span>

5.  <span data-ttu-id="fe53b-107">أغلق صفحة **تحديد إجمالي المكونات المطلوبة**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-107">Close the **Explosion** page.</span></span>
6.  <span data-ttu-id="fe53b-108">في صفحة **الطلبات المخططة**، حدد **مخطط Gantt** في مجموعة **عرض** في علامة التبويب **عرض**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-108">On the **Planned orders** page, select **Gantt chart** in the **View** group on the **View** tab.</span></span> 

    <span data-ttu-id="fe53b-109">[ ![لقطة شاشة لصفحة مخطط Gantt من علامة التبويب عرض.](../media/gantt-chart-ss.png) ](../media/gantt-chart-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fe53b-109">[ ![Screenshot of the Gantt chart page from the view tab.](../media/gantt-chart-ss.png) ](../media/gantt-chart-ss.png#lightbox)</span></span>

7.  <span data-ttu-id="fe53b-110">قم بتحديث الكمية من 123 إلى 250 ثم قم بالموافقة على الأمر.</span><span class="sxs-lookup"><span data-stu-id="fe53b-110">Update the quantity from 123 to 250 and then approve the order.</span></span>
    - <span data-ttu-id="fe53b-111">أغلق صفحة **مخطط Gantt**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-111">Close the **Gantt chart** page.</span></span> 
    - <span data-ttu-id="fe53b-112">ارجع إلى صفحة **الأوامر المخططة**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-112">Return to the **Planned orders** page.</span></span> 
    - <span data-ttu-id="fe53b-113">قم بتغيير **الكمية المطلوبة** إلى **‎‎250.00**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-113">Change the **Requirement quantity** to **250.00**.</span></span>
    - <span data-ttu-id="fe53b-114">في جزء الإجراء، حدد **موافقة**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-114">In the Action Pane, select **Approve**.</span></span> 
    - <span data-ttu-id="fe53b-115">في مربع الحوار، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="fe53b-115">Select **OK** in the dialog box.</span></span>

    <span data-ttu-id="fe53b-116">[ ![لقطة شاشة توضح الأمر المخطط المعتمد.](../media/approved-planned-order-ssm.png) ](../media/approved-planned-order-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fe53b-116">[ ![Screenshot showing the approved planned order.](../media/approved-planned-order-ssm.png) ](../media/approved-planned-order-ssm.png#lightbox)</span></span>

8.  <span data-ttu-id="fe53b-117">لا تؤدي الموافقة على الأمر إلى تغيير أوامر الشراء المخططة أو مخطط Gantt.</span><span class="sxs-lookup"><span data-stu-id="fe53b-117">Approving the order does not change the planned purchase orders or the Gantt chart.</span></span> <span data-ttu-id="fe53b-118">لإكمال هذا الإجراء، تحتاج إلى تشغيل "تحسين التخطيط" مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="fe53b-118">To complete this action, you need to run Planning Optimization again.</span></span> <span data-ttu-id="fe53b-119">تقوم الموافقة بحفظ كمية الأمر التي تم تغييرها وعند تشغيلها مرة أخرى، فإنها تحافظ على الأمر كما كان ولكنه يقوم بمراجعة المتطلبات.</span><span class="sxs-lookup"><span data-stu-id="fe53b-119">The approval saves the changed order quantity and when run again, it maintains the order as it was but revises the requirements.</span></span> 

    ![لقطة شاشة لأمر إنتاج معتمد مع تمييز الحالة.](../media/approved-production-1-ssm.png)

    ![لقطة شاشة لعرض إجمالي المكونات المطلوبة لأمر الإنتاج المخطط.](../media/production-order-explosion-ss.png)

    ![لقطة شاشة لملاحظة أن التغييرات اليدوية تنعكس أولاً في تشغيل التخطيط الرئيسي التالي.](../media/manual-change-ss.png)

<span data-ttu-id="fe53b-123">شاهد الفيديو التالي لمشاهدة العملية بأكملها من البداية إلى النهاية.</span><span class="sxs-lookup"><span data-stu-id="fe53b-123">Watch the following video to see the entire process from beginning to end.</span></span> 

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4IquI]