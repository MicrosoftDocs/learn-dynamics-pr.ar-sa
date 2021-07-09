---
ms.openlocfilehash: bd5933d6bddd0add13be9b3eb7bdf1ea85b47c9d
ms.sourcegitcommit: de79d56e760ae35a1ea1549067da2fba04de7088
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/01/2021
ms.locfileid: "6072164"
---
<span data-ttu-id="70c29-101">شاهد هذا الفيديو للتعرف على كيفية إنشاء مساحة عمل مخصصة.</span><span class="sxs-lookup"><span data-stu-id="70c29-101">Watch this video to see how to build a custom workspace.</span></span>
 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4MvtU]

## <a name="scenario"></a><span data-ttu-id="70c29-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="70c29-102">Scenario</span></span>

<span data-ttu-id="70c29-103">بصفتك مدير علاقات عملاء، ترغب في إنشاء مساحة عمل لعرض معلومات معينة بسرعة.</span><span class="sxs-lookup"><span data-stu-id="70c29-103">As a customer relations manager, you want to create a workspace to quickly view certain information.</span></span> <span data-ttu-id="70c29-104">وترغب في رؤية عدد العملاء الإجمالي وتتمكن من التصفح للاطلاع على مزيد من التفاصيل حول العملاء.</span><span class="sxs-lookup"><span data-stu-id="70c29-104">You want to see the total number of customers and be able to drill through to see more details on customers.</span></span> <span data-ttu-id="70c29-105">كما أنك تريد مشاهدة قائمة بجميع العملاء المتوقعين الذين يمكنك تصفيتهم.</span><span class="sxs-lookup"><span data-stu-id="70c29-105">You also want to see a list of all the leads that you can filter.</span></span> <span data-ttu-id="70c29-106">ستحتاج فقط إلى رؤية التاريخ الذي تم فيه فتح العميل المتوقع ومعرف العميل المتوقع وحالة العميل المتوقع وموضوع العميل المتوقع والتعليقات التي تمت على العميل المتوقع.</span><span class="sxs-lookup"><span data-stu-id="70c29-106">You only need to see the date that the lead was opened, the lead ID, status of the lead, the subject of the lead, and comments made on the lead.</span></span> <span data-ttu-id="70c29-107">يمكن لمخطط لمبيعات مجموعات عملاء أن يكون مفيداً، وكذلك احتواؤه على طريقة للانتقال السريع من مساحة العمل إلى صفحة عروض الأسعار.</span><span class="sxs-lookup"><span data-stu-id="70c29-107">A chart of the sales of customer groups would be useful, as would having a way to quickly go from the workspace to the quotations page.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="70c29-108">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="70c29-108">Before you begin</span></span> 


<span data-ttu-id="70c29-109">لإكمال هذا التدريب، ستحتاج إلى الوصول إلى بيئة تحتوي على عينة قياسية من البيانات في تطبيقات Finance and Operations، ومتصلة بـ Power BI.</span><span class="sxs-lookup"><span data-stu-id="70c29-109">To complete this exercise, you will need access to an environment that has a standard sample of data in Finance and Operations apps, and is connected to Power BI.</span></span>

## <a name="create-a-new-workspace"></a><span data-ttu-id="70c29-110">إنشاء مساحة عمل جديدة</span><span class="sxs-lookup"><span data-stu-id="70c29-110">Create a new workspace</span></span> 


1.  <span data-ttu-id="70c29-111">افتح واجهة المستخدم.</span><span class="sxs-lookup"><span data-stu-id="70c29-111">Open the user interface.</span></span>
2.  <span data-ttu-id="70c29-112">في **الشاشة الرئيسية**، انقر بزر الماوس الأيمن في منطقة مساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="70c29-112">On the **Home** screen, right-click in the workspace area.</span></span>
3.  <span data-ttu-id="70c29-113">حدد الخيار **تخصيص: TilePageContainer**.</span><span class="sxs-lookup"><span data-stu-id="70c29-113">Select the **Personalize: TilePageContainer** option.</span></span>
4.  <span data-ttu-id="70c29-114">حدد الخيار **إضافة مساحة عمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-114">Select the **Add a Workspace** option.</span></span>
5.  <span data-ttu-id="70c29-115">انقر بزر الماوس الأيمن فوق لوحة **مساحة عملي 1**.</span><span class="sxs-lookup"><span data-stu-id="70c29-115">Right-click the **My Workspace 1** tile.</span></span>
6.  <span data-ttu-id="70c29-116">حدد الخيار **تخصيص: مساحة عملي 1**.</span><span class="sxs-lookup"><span data-stu-id="70c29-116">Select the **Personalize: My Workspace 1** option.</span></span>
7.  <span data-ttu-id="70c29-117">في حقل **النص**، أدخل **CRM**.</span><span class="sxs-lookup"><span data-stu-id="70c29-117">In the **Text** field, enter **CRM**.</span></span>

## <a name="add-a-tile-to-your-workspace"></a><span data-ttu-id="70c29-118">إضافة لوحة إلى مساحة العمل الخاصة بك</span><span class="sxs-lookup"><span data-stu-id="70c29-118">Add a tile to your workspace</span></span> 


1.  <span data-ttu-id="70c29-119">افتح **المبيعات والتسويق > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="70c29-119">Open **Sales and marketing > Customers > All customers**.</span></span>
2.  <span data-ttu-id="70c29-120">حدد علامة التبويب **خيارات** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="70c29-120">Select the **Options** tab on the Action Pane.</span></span>
3.  <span data-ttu-id="70c29-121">في قسم **مخصص**، حدد **إضافة إلى مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-121">In the **Personalize** section, select **Add to workspace**.</span></span>
4.  <span data-ttu-id="70c29-122">في النموذج المنسدل، حدد **CRM** في حقل **مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-122">In the drop-down form, select **CRM** in the **Workspace** field.</span></span>
5.  <span data-ttu-id="70c29-123">حدد الخيار **تجانب** في حقل **العرض التقديمي**.</span><span class="sxs-lookup"><span data-stu-id="70c29-123">Select the **Tile** option in the **Presentation** field.</span></span>
6.  <span data-ttu-id="70c29-124">حدد الزر **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="70c29-124">Select the **Configure** button.</span></span>
7.  <span data-ttu-id="70c29-125">في النموذج **إضافة كمربع**، أدخل **العملاء** في حقل **الاسم الموجود على التجانب**.</span><span class="sxs-lookup"><span data-stu-id="70c29-125">On the **Add as tile** form, enter **Customers** in the **Name on tile** field.</span></span>
8.  <span data-ttu-id="70c29-126">حدد **نعم** في الحقل **عرض العدد بالتجانب** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="70c29-126">Select **Yes** on the **Show count on the tile** field and then select **OK**.</span></span>

## <a name="add-a-list-to-your-workspace"></a><span data-ttu-id="70c29-127">إضافة قائمة إلى مساحة العمل الخاصة بك</span><span class="sxs-lookup"><span data-stu-id="70c29-127">Add a list to your workspace</span></span> 


1.  <span data-ttu-id="70c29-128">افتح **المبيعات والتسويق > العلاقات > العملاء المحتملون > كافة العملاء الهامين المحتملين**.</span><span class="sxs-lookup"><span data-stu-id="70c29-128">Open **Sales and marketing > Relationships > Leads > All leads**.</span></span>
2.  <span data-ttu-id="70c29-129">حدد علامة التبويب **خيارات** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="70c29-129">Select the **Options** tab on the Action Pane.</span></span>
3.  <span data-ttu-id="70c29-130">في قسم **مخصص**، حدد **إضافة إلى مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-130">In the **Personalize** section, select **Add to workspace**.</span></span>
4.  <span data-ttu-id="70c29-131">في النموذج المنسدل، حدد **CRM** في حقل **مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-131">In the drop-down form, select **CRM** in the **Workspace** field.</span></span>
5.  <span data-ttu-id="70c29-132">حدد **قائمة** في حقل **العرض التقديمي**.</span><span class="sxs-lookup"><span data-stu-id="70c29-132">Select **List** in the **Presentation** field.</span></span>
6.  <span data-ttu-id="70c29-133">حدد الزر **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="70c29-133">Select the **Configure** button.</span></span>
7.  <span data-ttu-id="70c29-134">في النموذج **إضافة كقائمة**، أدخل **العملاء المحتملون** في حقل **الاسم الخاص بعلامة التبويب**.</span><span class="sxs-lookup"><span data-stu-id="70c29-134">On the **Add as list** form, enter **Leads** in the **Name for tab** field.</span></span>
8.  <span data-ttu-id="70c29-135">في حقل **نمط القائمة**، حدد الخيار **جدولي‬ (يصل إلى 8 أعمدة)**.</span><span class="sxs-lookup"><span data-stu-id="70c29-135">In the **List style** field, select the **Tabular (up to 8 columns)** option.</span></span>
9.  <span data-ttu-id="70c29-136">حدد خانة الاختيار الخاصة بالأعمدة التالية:</span><span class="sxs-lookup"><span data-stu-id="70c29-136">Select the check box for the following columns:</span></span>
    -   <span data-ttu-id="70c29-137">تاريخ الفتح</span><span class="sxs-lookup"><span data-stu-id="70c29-137">Date opened</span></span>
    -   <span data-ttu-id="70c29-138">معرف العميل المحتمل</span><span class="sxs-lookup"><span data-stu-id="70c29-138">Lead ID</span></span>
    -   <span data-ttu-id="70c29-139">‏الحالة</span><span class="sxs-lookup"><span data-stu-id="70c29-139">Status</span></span>
    -   <span data-ttu-id="70c29-140">الموضوع</span><span class="sxs-lookup"><span data-stu-id="70c29-140">Subject</span></span>
    -   <span data-ttu-id="70c29-141">الاسم</span><span class="sxs-lookup"><span data-stu-id="70c29-141">Name</span></span>
    -   <span data-ttu-id="70c29-142">التعليقات</span><span class="sxs-lookup"><span data-stu-id="70c29-142">Comments</span></span>
10. <span data-ttu-id="70c29-143">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="70c29-143">Select **OK**.</span></span>

## <a name="add-a-link-to-your-workspace"></a><span data-ttu-id="70c29-144">إضافة ارتباط إلى مساحة العمل الخاصة بك</span><span class="sxs-lookup"><span data-stu-id="70c29-144">Add a link to your workspace</span></span> 


1.  <span data-ttu-id="70c29-145">افتح **المبيعات والتسويق > العلاقات > الفرص > كافة الفرص**.</span><span class="sxs-lookup"><span data-stu-id="70c29-145">Open **Sales and marketing > Relationships > Opportunities > All    opportunities**.</span></span>
2.  <span data-ttu-id="70c29-146">حدد علامة التبويب **خيارات** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="70c29-146">Select the **Options** tab on the Action Pane.</span></span>
3.  <span data-ttu-id="70c29-147">في قسم **مخصص**، حدد **إضافة إلى مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-147">In the **Personalize** section, select **Add to workspace**.</span></span>
4.  <span data-ttu-id="70c29-148">في النموذج المنسدل، حدد **CRM** في حقل **مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-148">In the drop-down form, select **CRM** in the **Workspace** field.</span></span>
5.  <span data-ttu-id="70c29-149">حدد **ارتباط** في حقل **العرض التقديمي**.</span><span class="sxs-lookup"><span data-stu-id="70c29-149">Select **Link** in the **Presentation** field.</span></span>
6.  <span data-ttu-id="70c29-150">حدد الزر **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="70c29-150">Select the **Configure** button.</span></span>
7.  <span data-ttu-id="70c29-151">في النموذج **إضافة كرابط**، أدخل **الفرص** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="70c29-151">On the **Add as link** form, enter **Opportunities** in the **Name** field.</span></span>
8.  <span data-ttu-id="70c29-152">في الحقل **اسم المجموعة**، أدخل **المفضلة**.</span><span class="sxs-lookup"><span data-stu-id="70c29-152">On the **Group name** field, enter **Favorites**.</span></span>
9.  <span data-ttu-id="70c29-153">حدد الزر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="70c29-153">Select the **OK** button.</span></span>
10. <span data-ttu-id="70c29-154">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="70c29-154">Close the page.</span></span>

## <a name="embed-a-power-bi-report"></a><span data-ttu-id="70c29-155">تضمين تقرير Power BI</span><span class="sxs-lookup"><span data-stu-id="70c29-155">Embed a Power BI report</span></span> 


1.  <span data-ttu-id="70c29-156">لتضمين تقرير Power BI، افتح مساحة عمل CRM الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="70c29-156">To embed a Power BI report, open your CRM workspace.</span></span>
2.  <span data-ttu-id="70c29-157">في جزء الإجراء، حدد علامة التبويب **خيارات**.</span><span class="sxs-lookup"><span data-stu-id="70c29-157">On the Action Pane, select the **Options** tab.</span></span>
3.  <span data-ttu-id="70c29-158">حدد **تخصيص هذه الصفحة**.</span><span class="sxs-lookup"><span data-stu-id="70c29-158">Select **Personalize this page**.</span></span>
4.  <span data-ttu-id="70c29-159">وستظهر قائمة تخصيص.</span><span class="sxs-lookup"><span data-stu-id="70c29-159">A personalization menu will appear.</span></span> <span data-ttu-id="70c29-160">حدد زر **إضافة حقل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-160">Select the **Add a field** button.</span></span>
5.  <span data-ttu-id="70c29-161">حدد منطقة مفتوحة في نموذج مساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="70c29-161">Select an open area on the workspace form.</span></span>
6.  <span data-ttu-id="70c29-162">سيظهر الشريط الجانبي **خيارات مساحة العمل**.</span><span class="sxs-lookup"><span data-stu-id="70c29-162">A **Workspace options** sidebar will appear.</span></span> <span data-ttu-id="70c29-163">عيِّن خيار **السماح بعنصر تحكم Power BI** إلى **نعم**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="70c29-163">Set the **Allow Power BI Control** option to **Yes** and then select **OK**.</span></span>
7.  <span data-ttu-id="70c29-164">في مساحة العمل، ستتوفر لوحة Power BI.</span><span class="sxs-lookup"><span data-stu-id="70c29-164">In the workspace, the Power BI tile will be available.</span></span> <span data-ttu-id="70c29-165">في لوحة **Power BI**، حدد **بدء الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="70c29-165">In the **Power BI** tile, select **Get started**.</span></span>
8.  <span data-ttu-id="70c29-166">عند مطالبتك في الجزء الجانبي "تخويل Power BI"، حدد **انقر هنا لمنح التخويل إلى Power BI**.</span><span class="sxs-lookup"><span data-stu-id="70c29-166">When prompted on the Authorize Power BI side pane, select **Click here to provide authorization to Power BI**.</span></span>
9.  <span data-ttu-id="70c29-167">عندما تكون متصلاً، ستتوفر لديك قائمة بتقارير Power BI المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="70c29-167">When you are connected, you will have a list of available Power BI reports.</span></span> <span data-ttu-id="70c29-168">حدد علامة تبويب **المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="70c29-168">Select the **Sales** tab.</span></span>
10. <span data-ttu-id="70c29-169">حدد مخطط **المبيعات حسب مجموعة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="70c29-169">Select the **Sales by Customer Group** chart.</span></span>
11. <span data-ttu-id="70c29-170">حدد **موافق** لتضمين تقارير Power BI في مساحة العمل الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="70c29-170">Select **OK** to embed the Power BI reports to your workspace.</span></span>
