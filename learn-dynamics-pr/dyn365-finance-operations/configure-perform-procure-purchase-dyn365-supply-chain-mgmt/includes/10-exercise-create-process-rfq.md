---
ms.openlocfilehash: 8df6d2c6722f1d0183c565f8cb570419ba59b998
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6073858"
---
## <a name="scenario"></a><span data-ttu-id="d90a8-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="d90a8-101">Scenario</span></span>

<span data-ttu-id="d90a8-102">أرسل طلب عرض الأسعار إلى الموردين الإضافيين US-111 (مكتب معدات Contoso) وUS-103 (أجهزة عرض المطر) لعدد 500 من A0001 (كابلات HDMI 6)، ثم قم بالرد على طلب عرض الأسعار (RFQ) وقبوله.</span><span class="sxs-lookup"><span data-stu-id="d90a8-102">Send out a request for quotation to additional suppliers US-111 (Contoso Office Supply) and US-103 (Rain Projectors) for 500 of A0001 (HDMI 6' Cables), then reply and accept a request for quotation (RFQ).</span></span>

<span data-ttu-id="d90a8-103">ستقوم بالعمل في الشركة التجريبية **USMF**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-103">You will be working in the demo company **USMF**.</span></span>

## <a name="prerequisite---enable-the-rfq-to-be-edited"></a><span data-ttu-id="d90a8-104">المتطلب الأساسي: تمكين طلب عرض الأسعار (RFQ) المطلوب تحريره</span><span class="sxs-lookup"><span data-stu-id="d90a8-104">Prerequisite - Enable the RFQ to be edited</span></span>

1.    <span data-ttu-id="d90a8-105">انتقل إلى **التدبير والتوريد > إعداد > معلمات التدبير والتوريد**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-105">Go to **Procurement and sourcing > Setup > Procurement and sourcing parameters**.</span></span>
2.    <span data-ttu-id="d90a8-106">حدد علامة تبويب **طلب عرض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-106">Select the **Request for quotation** tab.</span></span>
3.    <span data-ttu-id="d90a8-107">قم بتمكين خيار **يمكن للمشتري تحرير عرض أسعار الموردين**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-107">Enable the **Purchaser can edit vendors bid** option.</span></span> 
4.    <span data-ttu-id="d90a8-108">اضغط على **حفظ**، ثم أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="d90a8-108">Click **Save**, and close the page.</span></span> 


## <a name="create-a-request-for-quotation"></a><span data-ttu-id="d90a8-109">إنشاء طلب لعرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="d90a8-109">Create a request for quotation</span></span> 

1.  <span data-ttu-id="d90a8-110">انتقل إلى **‏‫التدبير والتوريد‬ > طلبات عروض الأسعار > كافة طلبات عروض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-110">Go to **Procurement and sourcing > Requests for quotations > All requests for quotations**.</span></span>
2.  <span data-ttu-id="d90a8-111">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-111">Select **New**.</span></span>
3.  <span data-ttu-id="d90a8-112">في حقل **نوع الشراء**، حدد **أمر شراء**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-112">In the **Purchase type** field, select **Purchase order**.</span></span>
4.  <span data-ttu-id="d90a8-113">في حقل **عنوان المستند**، أدخِل **كابلات HDMI**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-113">In the **Document title** field, enter **HDMI Cables**.</span></span>
5.  <span data-ttu-id="d90a8-114">في حقل **الموقع**، حدد **1** (إنتاج مكبرات الصوت المنزلية).</span><span class="sxs-lookup"><span data-stu-id="d90a8-114">In the **Site** field, select **1** (Home speakers production).</span></span>
6.  <span data-ttu-id="d90a8-115">في حقل **المستودع**، حدد **13** (الموقع 1 - السلع المنتهية).</span><span class="sxs-lookup"><span data-stu-id="d90a8-115">In the **Warehouse** field, select **13** (Site 1 - Finished Goods).</span></span>
7.  <span data-ttu-id="d90a8-116">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-116">Select **OK**.</span></span>
 
## <a name="add-a-line-to-the-request-for-quotation"></a><span data-ttu-id="d90a8-117">إضافة سطر إلى طلب عرض الأسعار</span><span class="sxs-lookup"><span data-stu-id="d90a8-117">Add a line to the request for quotation</span></span>

1.  <span data-ttu-id="d90a8-118">إذا لزم الأمر، حدد **إضافة سطر** لإضافة سطر إلى القائمة.</span><span class="sxs-lookup"><span data-stu-id="d90a8-118">If necessary, select **Add line** to add a line to the list.</span></span>
2.  <span data-ttu-id="d90a8-119">في حقل **نوع السطر**، حدد **عنصر**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-119">In the **Line type** field, select **Item**.</span></span>
3.  <span data-ttu-id="d90a8-120">في حقل **رقم الصنف**، حدد **A0001** (كابلات HDMI 6).</span><span class="sxs-lookup"><span data-stu-id="d90a8-120">In the **Item number** field, select **A0001** (HDMI 6' Cables).</span></span>
4.  <span data-ttu-id="d90a8-121">في حقل **الكمية**، أدخِل **500**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-121">In the **Quantity** field, enter **500**.</span></span>
5.  <span data-ttu-id="d90a8-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-122">Select **Save**.</span></span>

## <a name="send-the-request-for-quotation-to-the-vendors"></a><span data-ttu-id="d90a8-123">إرسال طلب عرض الأسعار إلى الموردين</span><span class="sxs-lookup"><span data-stu-id="d90a8-123">Send the request for quotation to the vendors</span></span>

1.  <span data-ttu-id="d90a8-124">حدد **خيارات** في الأعلى، ثم حدد عرض **رأس الصفحة**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-124">Select **Options** at the top, and then select **Header** view.</span></span>
2.  <span data-ttu-id="d90a8-125">افتح علامة التبويب السريعة **المورد**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-125">Open the **Vendor** FastTab.</span></span>
3.  <span data-ttu-id="d90a8-126">إذا لزم الأمر، حدد **إضافة** لإضافة سطر إلى القائمة.</span><span class="sxs-lookup"><span data-stu-id="d90a8-126">If necessary, select **Add** to add a line to the list.</span></span>
4.  <span data-ttu-id="d90a8-127">في حقل **حساب المورد**، حدد **US-111** (مكتب معدات Contoso).</span><span class="sxs-lookup"><span data-stu-id="d90a8-127">In the **Vendor account** field, select **US-111** (Contoso office supply).</span></span>
5.  <span data-ttu-id="d90a8-128">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-128">Select **Add**.</span></span>
6.  <span data-ttu-id="d90a8-129">في حقل **حساب المورد**، حدد **US-103** (أجهزة عرض المطر).</span><span class="sxs-lookup"><span data-stu-id="d90a8-129">In the **Vendor account** field, select **US-103** (Rain Projectors).</span></span>
7.  <span data-ttu-id="d90a8-130">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-130">Select **Save**.</span></span>
8.  <span data-ttu-id="d90a8-131">حدد **عرض أسعار** في الجزء العلوي، ثم حدد **إرسال** ضمن قسم **العملية**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-131">Select **Quotation** at the top, and then select **Send** under the **Process** section.</span></span>
9.  <span data-ttu-id="d90a8-132">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-132">Select **OK**.</span></span>

## <a name="reply-to-an-rfq"></a><span data-ttu-id="d90a8-133">الرد على عروض الأسعار</span><span class="sxs-lookup"><span data-stu-id="d90a8-133">Reply to an RFQ</span></span>

1.  <span data-ttu-id="d90a8-134">انتقل إلى **‏‫التدبير والتوريد‬ > طلبات عروض الأسعار > كافة طلبات عروض الأسعار**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-134">Go to **Procurement and sourcing > Requests for quotations > All requests for quotations**.</span></span>
2.  <span data-ttu-id="d90a8-135">افتح طلبات عروض الأسعار التي تم إنشاؤها في الخطوات السابقة.</span><span class="sxs-lookup"><span data-stu-id="d90a8-135">Open the requests for quotations that were created in the previous steps.</span></span>
3. <span data-ttu-id="d90a8-136">حدد **خيارات** في جزء الإجراء، ثم حدد **عرض رأس الصفحة**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-136">Select **Options** in the Action Pane, and then select **Header view**.</span></span>
4.  <span data-ttu-id="d90a8-137">من **عرض رأس الصفحة**، انتقل إلى قائمة الموردين بواسطة توسيع علامة التبويب السريعة **المورد**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-137">From **Header view**, go to the list of vendors by expanding the **Vendor** FastTab.</span></span>
5.  <span data-ttu-id="d90a8-138">حدد المورد **US-111** في علامة التبويب السريعة **المورد**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-138">Select the vendor **US-111** in the **Vendor** FastTab.</span></span>
6.  <span data-ttu-id="d90a8-139">حدد **إدارة الردود** في علامة تبويب **عرض أسعار** ضمن جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="d90a8-139">Select **Manage replies** in the **Quotation** tab on the Action Pane.</span></span>
7.  <span data-ttu-id="d90a8-140">في جزء الإجراء، حدد علامة التبويب **رد**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-140">On the Action Pane, select the **Reply** tab.</span></span>
8.  <span data-ttu-id="d90a8-141">حدد **طلب عرض أسعار** الخاص بالمورد في **US-111** (مكتب معدات Contoso).</span><span class="sxs-lookup"><span data-stu-id="d90a8-141">Select the **Request for quotation** for vendor **US-111** (Contoso Office Supply).</span></span>
9.  <span data-ttu-id="d90a8-142">حدد **تحرير رد RFQ** في علامة التبويب **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-142">Select **Edit RFQ reply** in the **Edit** tab.</span></span>
10. <span data-ttu-id="d90a8-143">حدد علامة التبويب السريعة **سطور**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-143">Select the **Lines** FastTab.</span></span>
11. <span data-ttu-id="d90a8-144">في حقل **الوحدة**، أدخل **ea**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-144">In the **Unit** field, enter **ea**.</span></span>
12. <span data-ttu-id="d90a8-145">في حقل **سعر الوحدة**، أدخِل **10.00**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-145">In the **Unit price** field, enter **10.00**.</span></span>
13. <span data-ttu-id="d90a8-146">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-146">Select **Save**.</span></span>
14. <span data-ttu-id="d90a8-147">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-147">Select **Submit**.</span></span>
15. <span data-ttu-id="d90a8-148">حدد **إغلاق** في مربع الحوار الذي يعرض **لقد قمت بإرسال عرض السعر بنجاح**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-148">Select **Close** in the dialog box displaying **You have successfully submitted your bid** which appears.</span></span>

## <a name="accept-a-vendors-reply"></a><span data-ttu-id="d90a8-149">قبول رد المورد</span><span class="sxs-lookup"><span data-stu-id="d90a8-149">Accept a vendor's reply</span></span>

1.  <span data-ttu-id="d90a8-150">حدد **طلب عرض أسعار** رقم **US-111** (مكتب معدات Contoso).</span><span class="sxs-lookup"><span data-stu-id="d90a8-150">Select the **Request for quotation** number for **US-111** (Contoso Office Supply).</span></span>
2.  <span data-ttu-id="d90a8-151">حدد **رد** في الجزء العلوي، ثم حدد **قبول** ضمن قسم **العملية**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-151">Select **Reply** at the top, and then select **Accept** under the **Process** section.</span></span>
3.  <span data-ttu-id="d90a8-152">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d90a8-152">Select **OK**.</span></span>


