---
ms.openlocfilehash: e3b20c3aeb54fcd9f82a4daedeab6fcd66d31c4c
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074846"
---
<span data-ttu-id="7f073-101">يتم اجراء هذا التدريب في شركة **DEMF** في بيانات العرض التوضيحي القياسية لـ Dynamics 365 Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="7f073-101">This exercise is performed in the **DEMF** company in the Dynamics 365 Supply Chain Management standard demo data.</span></span> <span data-ttu-id="7f073-102">يتعين تمكين الوظيفة الإضافية لإدارة التغيير الهندسي وإعدادها.</span><span class="sxs-lookup"><span data-stu-id="7f073-102">The Engineering Change Management Add-in must be enabled and set up.</span></span> 

<span data-ttu-id="7f073-103">لمزيد من المعلومات، راجع [إعداد إدارة التغيير الهندسي لـ Dynamics 365 Supply Chain Management](/learn/paths/set-up-engineering-change-management/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="7f073-103">For more information, see [Set up engineering change management for Dynamics 365 Supply Chain Management](/learn/paths/set-up-engineering-change-management/?azure-portal=true).</span></span>

## <a name="scenario"></a><span data-ttu-id="7f073-104">السيناريو</span><span class="sxs-lookup"><span data-stu-id="7f073-104">Scenario</span></span>

<span data-ttu-id="7f073-105">لقد تم تكليفك بإنشاء منتج هندسي جديد سيتم إصداره لاحقاً لشركة **USMF** للإنتاج.</span><span class="sxs-lookup"><span data-stu-id="7f073-105">You have been tasked with creating a new engineering product that will later be released to the **USMF** company for production.</span></span>

## <a name="task-1---create-a-new-engineering-product"></a><span data-ttu-id="7f073-106">المهمة 1 - إنشاء منتج هندسي جديد</span><span class="sxs-lookup"><span data-stu-id="7f073-106">Task 1 - Create a new engineering product</span></span>

<span data-ttu-id="7f073-107">لإنشاء منتج هندسي جديد، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="7f073-107">To create a new engineering product, follow these steps:</span></span>

1.  <span data-ttu-id="7f073-108">انتقل إلى **إدارة التغيير الهندسي > عام > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="7f073-108">Go to **Engineering change management > Common > Released products**.</span></span>

1.  <span data-ttu-id="7f073-109">في جزء الإجراءات، في علامة التبويب  **المنتج** ، في المجموعة  **جديد** ، حدد  **منتج هندسي**.</span><span class="sxs-lookup"><span data-stu-id="7f073-109">On the Action Pane, on the **Product** tab, in the **New** group, select **Engineering product**.</span></span>

1.  <span data-ttu-id="7f073-110">في مربع الحوار  **منتج جديد** ، عيِّن القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="7f073-110">In the **New product** dialog box, set the following values:</span></span>

    - <span data-ttu-id="7f073-111">**فئة المنتج الهندسي** - مكونات الخزانة</span><span class="sxs-lookup"><span data-stu-id="7f073-111">**Engineering Product Category** -  Cabinet components</span></span>

    - <span data-ttu-id="7f073-112">**رقم المنتج** -‏ Z1234</span><span class="sxs-lookup"><span data-stu-id="7f073-112">**Product number** - Z1234</span></span>
 
    - <span data-ttu-id="7f073-113">**اسم المنتج** - الخزانة</span><span class="sxs-lookup"><span data-stu-id="7f073-113">**Product name** - Cabinet</span></span>

1.  <span data-ttu-id="7f073-114">حدد  **موافق**  لإنشاء المنتج وإغلاق مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="7f073-114">Select **OK** to create the product and then close the dialog box.</span></span>

1.  <span data-ttu-id="7f073-115">في جزء الإجراء، حدد **المهندس > إدارة التغيير الهندسي > الإصدارات الهندسية**.</span><span class="sxs-lookup"><span data-stu-id="7f073-115">In the Action Pane, select **Engineer > Engineering change management > Engineering versions**.</span></span>

1.  <span data-ttu-id="7f073-116">حدد الارتباط التشعبي **الإصدار** الحالي.</span><span class="sxs-lookup"><span data-stu-id="7f073-116">Select the current **Version** hyperlink.</span></span>

1.  <span data-ttu-id="7f073-117">في صفحة  **الإصدار الهندسي** ، في علامة التبويب السريعة  **‏‫قائمة مكونات الصنف‬** ، حدد  **إنشاء قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="7f073-117">On the **Engineering version** page, on the **Bill of materials** FastTab, select **Create BOM**.</span></span>

1.  <span data-ttu-id="7f073-118">في مربع الحوار  **إنشاء قائمة مكونات الصنف** ، عيِّن القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="7f073-118">In the **Create BOM** dialog box, set the following values:</span></span>

    - <span data-ttu-id="7f073-119">**الاسم** - خزانه</span><span class="sxs-lookup"><span data-stu-id="7f073-119">**Name** - Cabinet</span></span>

    - <span data-ttu-id="7f073-120">**الموقع** - ‏1</span><span class="sxs-lookup"><span data-stu-id="7f073-120">**Site** - 1</span></span>

1.  <span data-ttu-id="7f073-121">حدد  **موافق**  لإنشاء قائمة مكونات الصنف وأغلق مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="7f073-121">Select **OK** to add the BOM and close the dialog box.</span></span>

1. <span data-ttu-id="7f073-122">في علامة التبويب السريعة  **قائمة مكونات الصنف** ، حدد الارتباط التشعبي **رقم قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="7f073-122">On the  **Bill of materials** FastTab, select the **BOM number** hyperlink.</span></span>

1. <span data-ttu-id="7f073-123">في صفحة  **قائمة مكونات الصنف**، في علامة التبويب السريعة  **بنود قائمة مكونات الصنف**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="7f073-123">On the  **Bill of materials** page, on the  **Bill of materials lines** FastTab, select **New**.</span></span>

1. <span data-ttu-id="7f073-124">أضف ثلاثة أسطر لأرقام العناصر  **F00001** و  **F00010** و **J00006**.</span><span class="sxs-lookup"><span data-stu-id="7f073-124">Add three lines for item numbers  **F00001**, **F00010**, and **J00006**.</span></span>

1. <span data-ttu-id="7f073-125">حدد  **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7f073-125">Select **Save**.</span></span>

1. <span data-ttu-id="7f073-126">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7f073-126">Close the page.</span></span>

1. <span data-ttu-id="7f073-127">في صفحة  **الإصدار الهندسي** ، في علامة التبويب السريعة  **‏‫قائمة مكونات الصنف‬** ، حدد  **‏‫موافقة**.</span><span class="sxs-lookup"><span data-stu-id="7f073-127">On the **Engineering version** page, on the **Bill of materials** FastTab, select **Approve**.</span></span>

1. <span data-ttu-id="7f073-128">في مربع الحوار الذي يفتح، حدد  **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7f073-128">In the dialog box that opens, select **OK**.</span></span>

1. <span data-ttu-id="7f073-129">في صفحة  **الإصدار الهندسي** ، في علامة التبويب السريعة  **‏‫قائمة مكونات الصنف‬** ، حدد  **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="7f073-129">On the **Engineering version** page, on the **Bill of materials** FastTab, select **Activate**.</span></span> <span data-ttu-id="7f073-130">لاحظ أنه تم تحديد مربعي الاختيار  **نشط** و **تمت الموافقة عليه** لقائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="7f073-130">Notice that the **Active** and **Approved** check boxes are selected for the BOM.</span></span>

## <a name="task-2---release-the-engineering-product-and-accept-it-in-the-operational-company"></a><span data-ttu-id="7f073-131">المهمة 2 - تحرير المنتج الهندسي وقبوله في الشركة التشغيلية</span><span class="sxs-lookup"><span data-stu-id="7f073-131">Task 2 - Release the engineering product and accept it in the operational company</span></span>

<span data-ttu-id="7f073-132">والآن بعد إنشاء منتج هندسي، ستصدر المنتج إلى الشركة التشغيلية التي ستقوم بتصنيع المنتج.</span><span class="sxs-lookup"><span data-stu-id="7f073-132">Now that you have created an engineering product, you will release the product to the operational company that will manufacture the product.</span></span> <span data-ttu-id="7f073-133">لإصدار المنتج، اتبع الخطوات التالية في الشركة **DEMF**:</span><span class="sxs-lookup"><span data-stu-id="7f073-133">To release the product, follow these steps in the **DEMF** company:</span></span>

1.  <span data-ttu-id="7f073-134">انتقل إلى  **إدارة معلومات المنتجات > المنتجات > المنتجات الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="7f073-134">Go to **Product information management > Products > Released products**.</span></span>

1.  <span data-ttu-id="7f073-135">حدد المنتج  **Z1234**.</span><span class="sxs-lookup"><span data-stu-id="7f073-135">Select product **Z1234**.</span></span>

1.  <span data-ttu-id="7f073-136">في جزء الإجراءات، ضمن علامة التبويب  **المنتج** ، في مجموعة  **الصيانة** ، حدد  **بنية إصدار المنتج**  لفتح معالج  **إصدار المنتجات** .</span><span class="sxs-lookup"><span data-stu-id="7f073-136">On the Action Pane, on the **Product** tab, in the **Maintain** group, select **Release product structure** to open the **Release products** wizard.</span></span>

1.  <span data-ttu-id="7f073-137">في صفحة  **تحديد المنتجات الهندسية المراد إصدارها** ، حدد خانة الاختيار  **تحديد**  للمنتج  **Z1234**.</span><span class="sxs-lookup"><span data-stu-id="7f073-137">On the **Select engineering products to release** page, select the **Select** check box for product **Z1234**.</span></span>

1.  <span data-ttu-id="7f073-138">حدد **تفاصيل الإصدار**.</span><span class="sxs-lookup"><span data-stu-id="7f073-138">Select **Release details**.</span></span> <span data-ttu-id="7f073-139">تظهر صفحة  **تفاصيل إصدار المنتج** ، حيث يمكنك مراجعة تفاصيل المنتج الذي تم إصداره وبنيته.</span><span class="sxs-lookup"><span data-stu-id="7f073-139">The **Product release details** page opens, where you can review the details of the released product and its structure.</span></span> 

1.  <span data-ttu-id="7f073-140">قم بتعيين خيار  **إرسال قائمة مكونات الصنف**  إلى  **نعم**.</span><span class="sxs-lookup"><span data-stu-id="7f073-140">Set the **Send BOM** option to **Yes**.</span></span>

1.  <span data-ttu-id="7f073-141">أغلق الصفحة للعودة إلى معالج معالج **‏‫إصدار المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="7f073-141">Close the page to return to the **Release products** wizard.</span></span>

1.  <span data-ttu-id="7f073-142">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="7f073-142">Select **Next**.</span></span>

1.  <span data-ttu-id="7f073-143">في صفحة **تحديد الشركات**، لشركة **USMF**، قم بتعيين **موقع الاستلام** على **1**.</span><span class="sxs-lookup"><span data-stu-id="7f073-143">On the **Select companies** page, for the **USMF** company, set the **Receiving site** to **1**.</span></span>

1. <span data-ttu-id="7f073-144">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="7f073-144">Select **Next**.</span></span>

1. <span data-ttu-id="7f073-145">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="7f073-145">Select **Finish**.</span></span>


<span data-ttu-id="7f073-146">لمراجعة المنتج وتحريره إلى شركة **USMF**، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="7f073-146">To review the product and release it to **USMF**, follow these steps:</span></span>

1. <span data-ttu-id="7f073-147">قم بتغيِّر الشركة إلى  **USMF**.</span><span class="sxs-lookup"><span data-stu-id="7f073-147">Change the company to **USMF**.</span></span>

1. <span data-ttu-id="7f073-148">انتقل إلى **إدارة التغيير الهندسي > عام > إصدارات المنتج > إصدارات المنتجات المفتوحة**.</span><span class="sxs-lookup"><span data-stu-id="7f073-148">Go to **Engineering change management > Common > Product releases > Open product releases**.</span></span>

   <span data-ttu-id="7f073-149">تُظهر صفحة  **إصدارات المنتجات المفتوحة**  المنتج  **Z1234**، والذي تكون حالته هي  **موافقة معلقة**.</span><span class="sxs-lookup"><span data-stu-id="7f073-149">The **Open product releases** page shows product **Z1234**, which has a status of **Pending acceptance**.</span></span>

1. <span data-ttu-id="7f073-150">حدد القيمة في العمود **رقم المنتج** لفتح صفحة **تفاصيل إصدار المنتج**.</span><span class="sxs-lookup"><span data-stu-id="7f073-150">Select the value in the **Product number** column to open the **Product release details** page.</span></span>


<span data-ttu-id="7f073-151">عندما تنتهي من مراجعة المعلومات، فستكون على استعداد لقبول المنتج، وبهذه الطريقة، قم بتحريره لشركة  **USMF** .</span><span class="sxs-lookup"><span data-stu-id="7f073-151">When you've finished reviewing the information, you're ready to accept the product and, in this way, release it to the **USMF** company.</span></span> 

1. <span data-ttu-id="7f073-152">في جزء الاجراء، حدد **إجراءات > قبول**.</span><span class="sxs-lookup"><span data-stu-id="7f073-152">On the Action Pane, select **Actions > Accept**.</span></span> <span data-ttu-id="7f073-153">ستتلقى رسالة مفادها أن المنتج **Z1234** قد تم تحريره.</span><span class="sxs-lookup"><span data-stu-id="7f073-153">You will receive a message that product **Z1234** is released.</span></span>

1. <span data-ttu-id="7f073-154">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="7f073-154">Close the page.</span></span>
