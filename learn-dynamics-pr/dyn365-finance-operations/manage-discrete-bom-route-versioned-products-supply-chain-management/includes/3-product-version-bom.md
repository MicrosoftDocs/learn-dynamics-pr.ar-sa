---
ms.openlocfilehash: e5fd7c2b0c460ccfdbbf17a548fbd45b417bdbd7
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074828"
---
<span data-ttu-id="73e10-101">يمكن للشركة الهندسية المالكة إرفاق قائمة مكونات الصنف بإصدار منتج هندسي.</span><span class="sxs-lookup"><span data-stu-id="73e10-101">The owning engineering company can attach a BOM to an engineering product version.</span></span>

<span data-ttu-id="73e10-102">على سبيل المثال، إذا قامت الكيانات القانونية العاملة بتصنيع منتج تم إنشاؤه في شركة هندسية، فيجب أن يتكون المنتج من نفس بنود قائمة مكونات الصنف خلال التطبيق.</span><span class="sxs-lookup"><span data-stu-id="73e10-102">For example, if operating legal entities have manufactured a product that is created in the engineering company, the product should be composed of the same BOM lines throughout the application.</span></span> <span data-ttu-id="73e10-103">لإنجاز هذه المهمة، يمكنك إنشاء قائمة مكونات الصنف عند إنشاء المنتج الهندسي.</span><span class="sxs-lookup"><span data-stu-id="73e10-103">To accomplish this task, you can create the BOM when creating the engineering product.</span></span>

<span data-ttu-id="73e10-104">عند إصدارها للكيانات القانونية (التشغيلية) الأخرى، فإن التغييرات التي يمكن إجراؤها على قائمة مكونات الصنف لها قيود:</span><span class="sxs-lookup"><span data-stu-id="73e10-104">When released to other (operational) legal entities, the changes that can be made to the BOM have limitations:</span></span>

-   <span data-ttu-id="73e10-105">لا يمكن للشركة التشغيلية إزالة بنود قائمة مكونات الصنف التي تم إصدارها.</span><span class="sxs-lookup"><span data-stu-id="73e10-105">The operational company can't remove released BOM lines.</span></span>

-   <span data-ttu-id="73e10-106">الحقول الهندسية في قائمة مكونات الصنف للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="73e10-106">Engineering fields on the BOM are read-only.</span></span> <span data-ttu-id="73e10-107">يمكن للشركة التشغيلية تحرير جميع حقول التنفيذ اللوجستية الأخرى.</span><span class="sxs-lookup"><span data-stu-id="73e10-107">The operational company can edit all other logistical implementation fields.</span></span>

-   <span data-ttu-id="73e10-108">يمكن للشركة التشغيلية إضافة بنود إلى قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="73e10-108">The operational company can add lines to the BOM.</span></span>

-   <span data-ttu-id="73e10-109">يمكن للشركة التشغيلية إضافة قائمة مكونات صنف محلية وجديدة.</span><span class="sxs-lookup"><span data-stu-id="73e10-109">The operational company can add a new, local BOM.</span></span>

-   <span data-ttu-id="73e10-110">يتم الاحتفاظ بجميع قوائم مكونات الأصناف التي تم إنشاؤها محلياً وبنود قائمة قائمة مكونات الصنف عندما تقوم الشركة الهندسية بتحديث قائمة مكونات الصنف الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="73e10-110">All locally created BOMs and BOM lines are preserved when the engineering company updates its BOM.</span></span>

<span data-ttu-id="73e10-111">لإضافة قائمة مكونات الصنف إلى المنتج الهندسي، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="73e10-111">To add a BOM to the engineering product, follow these steps:</span></span>

1.  <span data-ttu-id="73e10-112">في جزء الإجراء، حدد **المهندس > إدارة التغيير الهندسي > الإصدارات الهندسية**.</span><span class="sxs-lookup"><span data-stu-id="73e10-112">In the Action Pane, select **Engineer > Engineering change management > Engineering versions**.</span></span>

1.  <span data-ttu-id="73e10-113">حدد الارتباط التشعبي **الإصدار** الحالي.</span><span class="sxs-lookup"><span data-stu-id="73e10-113">Select the current **Version** hyperlink.</span></span>

1.  <span data-ttu-id="73e10-114">في صفحة  **الإصدار الهندسي** ، في علامة التبويب السريعة  **‏‫قائمة مكونات الصنف‬** ، حدد  **إنشاء قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="73e10-114">On the **Engineering version** page, on the **Bill of materials** FastTab, select **Create BOM**.</span></span>

1.  <span data-ttu-id="73e10-115">في مربع الحوار  **إنشاء قائمة مكونات الصنف** ، عيِّن القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="73e10-115">In the **Create BOM** dialog box, set the following values:</span></span>

    - <span data-ttu-id="73e10-116">**الاسم** - حدد كيفية تحديد اسم قائمة مكونات الصنف (BOM) عند استلام المنتج (إصداره) في كيان قانوني.</span><span class="sxs-lookup"><span data-stu-id="73e10-116">**Name** - Select how the name of the bill of materials (BOM) is defined when the product is received (released) in a legal entity.</span></span>
    
    - <span data-ttu-id="73e10-117">**الموقع** - حدد موقع قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="73e10-117">**Site** - Select the site for the BOM.</span></span>

1.  <span data-ttu-id="73e10-118">حدد  **موافق**  لإضافة قائمة مكونات الصنف وأغلق مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="73e10-118">Select **OK** to add the BOM and then close the dialog box.</span></span>

1.  <span data-ttu-id="73e10-119">في علامة التبويب السريعة  **قائمة مكونات الصنف** ، حدد الارتباط التشعبي **رقم قائمة مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="73e10-119">On the  **Bill of materials** FastTab, select the **BOM number** hyperlink.</span></span>

1.  <span data-ttu-id="73e10-120">في صفحة  **قائمة مكونات الصنف** ، في علامة التبويب السريعة  **بنود قائمة مكونات الصنف** ، أضف الأصناف التي تشكل قائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="73e10-120">On the **Bill of materials** page, on the **Bill of materials lines** FastTab, add the items that make up the BOM.</span></span> <span data-ttu-id="73e10-121">حدد  **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="73e10-121">Select **Save**.</span></span>

1.  <span data-ttu-id="73e10-122">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="73e10-122">Close the page.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="73e10-123">[![لقطة شاشة لصفحة قائمة مكونات الصنف التي تفتح عند تحديد إنشاء قائمة مكونات الصنف. في هذه الصفحة، ستضيف العناصر التي ستشكل قائمة مكونات الصنف.](../media/create-bom.png)](../media/create-bom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="73e10-123">[![Screenshot of the Bill of materials page that opens when you select Create BOM. On this page, you will add the items that will make up the BOM.](../media/create-bom.png)](../media/create-bom.png#lightbox)</span></span>

1. <span data-ttu-id="73e10-124">في صفحة  **الإصدار الهندسي** ، في علامة التبويب السريعة  **‏‫قائمة مكونات الصنف‬** ، حدد  **‏‫موافقة**.</span><span class="sxs-lookup"><span data-stu-id="73e10-124">On the **Engineering version** page, on the **Bill of materials** FastTab, select **Approve**.</span></span>

1. <span data-ttu-id="73e10-125">في مربع الحوار الذي يظهر، حدد  **موافق**.</span><span class="sxs-lookup"><span data-stu-id="73e10-125">In the dialog box that appears, select **OK**.</span></span>

1. <span data-ttu-id="73e10-126">في صفحة  **الإصدار الهندسي** ، في علامة التبويب السريعة  **‏‫قائمة مكونات الصنف‬** ، حدد  **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="73e10-126">On the **Engineering version** page, on the **Bill of materials** FastTab, select **Activate**.</span></span>

1. <span data-ttu-id="73e10-127">لاحظ أنه تم تحديد مربعي الاختيار  **نشط** و **تمت الموافقة عليه** لقائمة مكونات الصنف.</span><span class="sxs-lookup"><span data-stu-id="73e10-127">Notice that the **Active** and **Approved** check boxes are selected for the BOM.</span></span>

