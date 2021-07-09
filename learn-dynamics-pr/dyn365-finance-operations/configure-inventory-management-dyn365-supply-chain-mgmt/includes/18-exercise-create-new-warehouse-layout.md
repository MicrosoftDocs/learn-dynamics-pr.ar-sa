---
ms.openlocfilehash: 15930c02d3842ad1ba234e671db69878999ce8ae
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073236"
---
## <a name="scenario"></a><span data-ttu-id="79d5f-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="79d5f-101">Scenario</span></span>

<span data-ttu-id="79d5f-102">في هذا التدريب، تحتاج إلى إنشاء مستودع في شركة **USMF**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-102">For this exercise, you need to create a warehouse in company **USMF**.</span></span> 

<span data-ttu-id="79d5f-103">يحتوي هذا المستودع على التنسيق التالي لموقعه: ممر-حامل-رف، والذي سيتم تمثيله بقيم عددية مثل **001-01-01**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-103">This warehouse has the following format for its location: Aisle-Rack-Shelf, which will be represented with numerical values such as **001-01-01**.</span></span> 

<span data-ttu-id="79d5f-104">الموقع الافتراضي هو 450‎ × 250 × 200 كالعرض والعمق والارتفاع.</span><span class="sxs-lookup"><span data-stu-id="79d5f-104">The default location is 450 X 250 X 200 as width, depth, and height.</span></span> 

## <a name="set-the-default-location-capacity"></a><span data-ttu-id="79d5f-105">تعيين قدرة الموقع الافتراضي الإنتاجية</span><span class="sxs-lookup"><span data-stu-id="79d5f-105">Set the default location capacity</span></span> 

1.  <span data-ttu-id="79d5f-106">افتح شركة **USMF**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-106">Open company **USMF**.</span></span>
2.  <span data-ttu-id="79d5f-107">انتقل إلى **إدارة المخزون > الإعداد > معلمات إدارة المستودع والمخزون**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-107">Go to **Inventory management > Setup > Inventory and warehouse management parameters**.</span></span>
3.  <span data-ttu-id="79d5f-108">حدد علامة التبويب **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-108">Select the **Locations** tab.</span></span>
4.  <span data-ttu-id="79d5f-109">في الحقل **عرض قياسي**، أدخل **450**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-109">In the **Standard width** field, enter **450**.</span></span>
5.  <span data-ttu-id="79d5f-110">في الحقل **عمق قياسي**، أدخل **250**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-110">In the **Standard depth** field, enter **250**.</span></span>
6.  <span data-ttu-id="79d5f-111">في الحقل **ارتفاع قياسي**، أدخل **200**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-111">In the **Standard height** field, enter **200**.</span></span>
7.  <span data-ttu-id="79d5f-112">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-112">Select **Save**.</span></span>
8.  <span data-ttu-id="79d5f-113">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="79d5f-113">Close the page.</span></span>

## <a name="define-the-location-name-format"></a><span data-ttu-id="79d5f-114">تحديد تنسيق اسم الموقع</span><span class="sxs-lookup"><span data-stu-id="79d5f-114">Define the location name format</span></span> 

1.  <span data-ttu-id="79d5f-115">انتقل إلى **إدارة المخزون> إعداد> تصنيف المخزون> مستودعات**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-115">Go to **Inventory management > Setup > Inventory breakdown > Warehouses**.</span></span>
2.  <span data-ttu-id="79d5f-116">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-116">Select **New**.</span></span>
3.  <span data-ttu-id="79d5f-117">في الحقل **مستودع**، اكتب **17**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-117">In the **Warehouse** field, type **17**.</span></span>
4.  <span data-ttu-id="79d5f-118">في الحقل **اسم**، اكتب **المواد الخام**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-118">In the **Name** field, type **Raw materials**.</span></span>
5.  <span data-ttu-id="79d5f-119">في الحقل **الموقع**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="79d5f-119">In the **Site** field, select the drop-down button to open the lookup.</span></span>
6.  <span data-ttu-id="79d5f-120">في القائمة، ابحث عن الموقع **1** وحدده.</span><span class="sxs-lookup"><span data-stu-id="79d5f-120">In the list, find and select site **1**.</span></span>
7.  <span data-ttu-id="79d5f-121">قم بتوسيع قسم **أسماء المواقع**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-121">Expand the **Location names** section.</span></span> <span data-ttu-id="79d5f-122">تحدد الخيارات الموجودة في هذا القسم التنسيق الافتراضي لأسماء المواقع.</span><span class="sxs-lookup"><span data-stu-id="79d5f-122">The options in this section define the default format for location names.</span></span> <span data-ttu-id="79d5f-123">في هذا المثال، ستقوم بتضمين رقم الممر ورقم الحامل ورقم الرف.</span><span class="sxs-lookup"><span data-stu-id="79d5f-123">For this example, you'll include the aisle number, rack number, and shelf number.</span></span>
8.  <span data-ttu-id="79d5f-124">عيّن الخيار **تضمين الممر** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-124">Set the **Include aisle** option to **Yes**.</span></span>
9.  <span data-ttu-id="79d5f-125">عيّن الخيار **تضمين الحامل** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-125">Set the **Include rack** option to **Yes**.</span></span>
10. <span data-ttu-id="79d5f-126">في الحقل **تنسيق**، للحامل، اكتب **-##**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-126">In the **Format** field, for the rack, type **-##**.</span></span>
11. <span data-ttu-id="79d5f-127">عيّن الخيار **تضمين الرف** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-127">Set the **Include shelf** option to **Yes**.</span></span>
12. <span data-ttu-id="79d5f-128">في حقل **تنسيق**، للرف، اكتب **-##**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-128">In the **Format** field, for the shelf, type **-##**.</span></span>
13. <span data-ttu-id="79d5f-129">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-129">Select **Save**.</span></span>

## <a name="define-warehouse-locations"></a><span data-ttu-id="79d5f-130">تحديد مواقع المستودعات</span><span class="sxs-lookup"><span data-stu-id="79d5f-130">Define warehouse locations</span></span> ##

1.  <span data-ttu-id="79d5f-131">في جزء الإجراء، حدد **مستودع**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-131">On the Action Pane, select **Warehouse**.</span></span>
2.  <span data-ttu-id="79d5f-132">حدد **معالج المواقع**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-132">Select **Location wizard**.</span></span>
3.  <span data-ttu-id="79d5f-133">حدد **التالي**</span><span class="sxs-lookup"><span data-stu-id="79d5f-133">Select **Next**</span></span>
4.  <span data-ttu-id="79d5f-134">إذا تعذر عليك إلغاء تحديد الخيارات، فيرجى تحديد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-134">If you are unable to de-select options, please select **Next**.</span></span> <span data-ttu-id="79d5f-135">إذا كان بإمكانك إلغاء تحديد الخيارات، فقم بإلغاء تحديد **أرصف داخلية**، و **مواقع الانتقاء**، و **مواقع مجمعة**</span><span class="sxs-lookup"><span data-stu-id="79d5f-135">If you are able to de-select options, de-select **Inbound docks**, **Picking locations**, and **Bulk locations**</span></span> 
6.  <span data-ttu-id="79d5f-136">حدد **التالي** حتى يظهر الزر **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-136">Select **Next** until the **Finish** button appears.</span></span> <span data-ttu-id="79d5f-137">هذا يعني قبول جميع المواقع التي يقترحها النظام.</span><span class="sxs-lookup"><span data-stu-id="79d5f-137">This is accepting all the locations the system is suggesting.</span></span> 
14. <span data-ttu-id="79d5f-138">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="79d5f-138">Select **Finish**.</span></span>
15. <span data-ttu-id="79d5f-139">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="79d5f-139">Close all pages.</span></span>

 


