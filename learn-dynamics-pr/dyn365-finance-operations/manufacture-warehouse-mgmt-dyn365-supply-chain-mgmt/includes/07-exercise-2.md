---
ms.openlocfilehash: 54b81dfbc5aefbc3c047db9b8a6a8d0aa5f456b8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073290"
---
## <a name="scenario"></a><span data-ttu-id="6029e-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="6029e-101">Scenario</span></span>
<span data-ttu-id="6029e-102">سوف تستخدم الشركة **USMF** لإعداد النظام لتوزيع البضائع المخطط له.</span><span class="sxs-lookup"><span data-stu-id="6029e-102">You will use the company **USMF** to set up the system for planned cross docking.</span></span> 

## <a name="create-a-work-class"></a><span data-ttu-id="6029e-103">إنشاء درجة عمل</span><span class="sxs-lookup"><span data-stu-id="6029e-103">Create a work class</span></span>

1. <span data-ttu-id="6029e-104">انتقل إلى **إدارة المستودعات > إعداد > العمل > فئات العمل**.</span><span class="sxs-lookup"><span data-stu-id="6029e-104">Go to **Warehouse management > Setup > Work > Work classes**.</span></span>
2. <span data-ttu-id="6029e-105">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="6029e-105">Select **New**.</span></span>
3. <span data-ttu-id="6029e-106">في الحقل **معرف فئة العمل**، أدخل **CrossDock**.</span><span class="sxs-lookup"><span data-stu-id="6029e-106">In the **Work class ID** field, enter **CrossDock**.</span></span>
4. <span data-ttu-id="6029e-107">في الحقل **الوصف**، أدخل **توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-107">In the **Description** field, enter **Cross-docking**.</span></span>
5. <span data-ttu-id="6029e-108">في الحقل **نوع أمر العمل**، حدد **توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-108">In the **Work order type** field, select  **Cross docking**.</span></span>
6. <span data-ttu-id="6029e-109">حدد **حفظ** و **أغلق** الصفحة.</span><span class="sxs-lookup"><span data-stu-id="6029e-109">**Save** and **Close** the page.</span></span>

## <a name="create-a-work-template"></a><span data-ttu-id="6029e-110">إنشاء قالب عمل</span><span class="sxs-lookup"><span data-stu-id="6029e-110">Create a work template</span></span>
1. <span data-ttu-id="6029e-111">انتقل إلى **إدارة المستودعات > إعداد > العمل > قوالب العمل**</span><span class="sxs-lookup"><span data-stu-id="6029e-111">Go to **Warehouse management > Setup > Work > Work templates**.</span></span>
2. <span data-ttu-id="6029e-112">في الحقل **نوع أمر العمل**، حدد **توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-112">In the **Work order type** field, select **Cross docking**.</span></span>
3. <span data-ttu-id="6029e-113">حدد **جديد** في جزء الإجراءات</span><span class="sxs-lookup"><span data-stu-id="6029e-113">Select **New** in the Action Pane</span></span>
4. <span data-ttu-id="6029e-114">في علامة التبويب **نظرة عامة**، في الحقل **قالب العمل**، أدخل **توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-114">In the **Overview** tab, in the  **Work template** field, enter **Cross docking**.</span></span>
5. <span data-ttu-id="6029e-115">في الحقل **وصف قالب العمل**، أدخل **توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-115">In the  **Work template description** field, enter **Cross docking**.</span></span>
6. <span data-ttu-id="6029e-116">في علامة التبويب **تفاصيل قالب العمل**، حدد **جديد** (قد تحتاج إلى تحديث الشاشة قبل تمكين الخيار "جديد".)</span><span class="sxs-lookup"><span data-stu-id="6029e-116">In the **Work Template Details** tab, select **New** (you may need to refresh the screen before New becomes enabled).</span></span>
7. <span data-ttu-id="6029e-117">في السطر رقم 1، حدد **انتقاء** في الحقل **نوع العمل**.</span><span class="sxs-lookup"><span data-stu-id="6029e-117">In Line number 1, select **Pick** in the **Work type** field.</span></span>
8. <span data-ttu-id="6029e-118">في الحقل **معرف فئة العمل**، حدد **CrossDock**.</span><span class="sxs-lookup"><span data-stu-id="6029e-118">In the **Work class ID** field select **CrossDock**.</span></span>
9. <span data-ttu-id="6029e-119">في علامة التبويب **تفاصيل قالب العمل**، حدد **جديد** (قد تحتاج إلى تحديث الشاشة قبل تمكين الخيار "جديد".)</span><span class="sxs-lookup"><span data-stu-id="6029e-119">In the **Work Template Details** tab, select **New** (you may need to refresh the screen before New becomes enabled).</span></span>
10. <span data-ttu-id="6029e-120">في السطر رقم 2، حدد **وضع** في الحقل **نوع العمل**.</span><span class="sxs-lookup"><span data-stu-id="6029e-120">In Line number 2, select **Put** in the **Work type** field.</span></span>
11. <span data-ttu-id="6029e-121">في الحقل **معرف فئة العمل**، حدد **CrossDock**.</span><span class="sxs-lookup"><span data-stu-id="6029e-121">In the **Work class ID** field, select **CrossDock**.</span></span>
12. <span data-ttu-id="6029e-122">حدد **حفظ** و **أغلق** الصفحة.</span><span class="sxs-lookup"><span data-stu-id="6029e-122">**Save** and **Close** the page.</span></span>

## <a name="create-a-location-directive"></a><span data-ttu-id="6029e-123">إنشاء توجيه خاص بالموقع</span><span class="sxs-lookup"><span data-stu-id="6029e-123">Create a location directive</span></span>

1. <span data-ttu-id="6029e-124">انتقل إلى **إدارة المستودعات > الإعداد > توجيهات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-124">Go to **Warehouse management > Setup > Location directives**.</span></span>
2. <span data-ttu-id="6029e-125">في الحقل **نوع أمر العمل**، حدد **توزيع البضائع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-125">In the **Work order type** field, select **Cross docking**.</span></span>
3. <span data-ttu-id="6029e-126">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="6029e-126">Select **New**.</span></span>
4. <span data-ttu-id="6029e-127">تجب تعبئة الرقم التسلسلي 1 بشكل مسبق.</span><span class="sxs-lookup"><span data-stu-id="6029e-127">Sequence number 1 should pre-populate.</span></span> <span data-ttu-id="6029e-128">في الحقل **الاسم**، أدخل **توزيع البضائع ووضعها في المستودع 51**.</span><span class="sxs-lookup"><span data-stu-id="6029e-128">In the  **Name** field, enter **Cross docking WH 51 Put**.</span></span>
5. <span data-ttu-id="6029e-129">في حقل **نوع العمل**، حدد **وضع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-129">In the **Work type** field, select **Put**.</span></span>
6. <span data-ttu-id="6029e-130">في الحقلين **الموقع** و **المستودع**، حدد **5** و **51**.</span><span class="sxs-lookup"><span data-stu-id="6029e-130">In the **Site** and **Warehouse** fields, select **5** and **51**.</span></span>
7. <span data-ttu-id="6029e-131">قم بتحديث الشاشة، وفي علامة التبويب **السطور**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="6029e-131">Refresh your screen and on the **Lines** tab, select **New**.</span></span>
8. <span data-ttu-id="6029e-132">في الحقلين **من الكمية** و **إلى الكمية**، أدخل 1-100,000.</span><span class="sxs-lookup"><span data-stu-id="6029e-132">In the **From quantity** and **To quantity** fields enter 1-100,000.</span></span>
9. <span data-ttu-id="6029e-133">حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="6029e-133">Select **Refresh**.</span></span>
10. <span data-ttu-id="6029e-134">في **إجراءات توجيه الموقع**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="6029e-134">On the **Location directive actions**, select **New**.</span></span>
11. <span data-ttu-id="6029e-135">في الحقل **الاسم**، أدخل **Cross Dock 51**.</span><span class="sxs-lookup"><span data-stu-id="6029e-135">In the **Name** field, enter **Cross Dock 51**.</span></span>
12. <span data-ttu-id="6029e-136">**قم بتحديث** الشاشة.</span><span class="sxs-lookup"><span data-stu-id="6029e-136">**Refresh** the screen.</span></span>
13. <span data-ttu-id="6029e-137">حدد **تحرير الاستعلام**.</span><span class="sxs-lookup"><span data-stu-id="6029e-137">Select **Edit query**.</span></span>
14. <span data-ttu-id="6029e-138">في السطر الذي يعرض فيه **الحقل** **الموقع**، استخدم القائمة المنسدلة لتغييره إلى **معرف ملف تعريف الموقع**.</span><span class="sxs-lookup"><span data-stu-id="6029e-138">On the line where the **Field** shows **Location**, use the dropdown menu to change it to **Location profile ID**.</span></span>
15. <span data-ttu-id="6029e-139">في الحقل **المعايير**، حدد **Baydoor**.</span><span class="sxs-lookup"><span data-stu-id="6029e-139">In the **Criteria** field, select **Baydoor**.</span></span> <span data-ttu-id="6029e-140">وهذا يعني أنه عندما تكون حركة توزيع البضائع مطلوبة، فإن الانتقاء يمكن أن يكون فقط من موقع له ملف تعريف الموقع Baydoor.</span><span class="sxs-lookup"><span data-stu-id="6029e-140">This means that when a cross docking transaction is required, the pick can only be from a location with the Baydoor location profile.</span></span>
16. <span data-ttu-id="6029e-141">حدد **موافق** ثم حدد **حفظ** توجيه الموقع.</span><span class="sxs-lookup"><span data-stu-id="6029e-141">Select **OK** and then **Save** the Location directive.</span></span>
