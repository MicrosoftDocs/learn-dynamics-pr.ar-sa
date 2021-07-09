---
ms.openlocfilehash: 44c7e00fbed1035803fb9ff913cbd6255593a9af
ms.sourcegitcommit: dd4400e44ab6efbe2a1e339f9939e90a8414cab3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/14/2020
ms.locfileid: "6073631"
---
<span data-ttu-id="aa950-101">بصفتك مديراً جدولة المواد والإنتاج، تحتاج إلى تطوير مجموعة تخطيط جديدة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="aa950-101">As the materials and production scheduling manager, you need to develop a new intercompany planning group.</span></span> <span data-ttu-id="aa950-102">يتم شحن التجميعات من شركة DEMF إلى شركة USMF.</span><span class="sxs-lookup"><span data-stu-id="aa950-102">Assemblies are shipped from company DEMF to company USMF.</span></span> <span data-ttu-id="aa950-103">في USMF، يتم تلوين التجميعات وإنهائها باستخدام الشعار أمريكا الشمالية، ثم يتم تحويلها إلى USRT للبيع.</span><span class="sxs-lookup"><span data-stu-id="aa950-103">At USMF, the assemblies are painted and finished with the North American logo, and then they are transferred to USRT for sale.</span></span> 

<span data-ttu-id="aa950-104">استخدم Plans 20 وDynPlan وMasterPlan لإنجاز هذا الهدف.</span><span class="sxs-lookup"><span data-stu-id="aa950-104">Use the Plans 20, DynPlan, and MasterPlan to accomplish this goal.</span></span>

## <a name="create-an-intercompany-planning-group"></a><span data-ttu-id="aa950-105">إنشاء مجموعة تخطيط بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="aa950-105">Create an intercompany planning group</span></span>

1.  <span data-ttu-id="aa950-106">في الشركة **USMF**، حدد **‏‫عرض جزء التنقل‬**.</span><span class="sxs-lookup"><span data-stu-id="aa950-106">In company **USMF**, select **Show navigation pane**.</span></span>
2.  <span data-ttu-id="aa950-107">افتح **التخطيط الرئيسي > إعداد > مجموعات التخطيط بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-107">Open **Master planning > Setup > Intercompany planning groups**.</span></span>
3.  <span data-ttu-id="aa950-108">حدد **جديد** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="aa950-108">Select **New** on the Action Pane.</span></span>
4.  <span data-ttu-id="aa950-109">في الحقل **الاسم**، أدخل **40**.</span><span class="sxs-lookup"><span data-stu-id="aa950-109">Enter **40** in the **Name** field.</span></span>
5.  <span data-ttu-id="aa950-110">أدخل **مجموعة ممتدة بين الشركات الشقيقة** في الحقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="aa950-110">Enter **Intercompany Extended Group** in the **Description** field.</span></span> 
6.  <span data-ttu-id="aa950-111">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="aa950-111">Select **Save**.</span></span>
7.  <span data-ttu-id="aa950-112">حدد **جديد** في شريط الأدوات من علامة التبويب **أعضاء مجموعة التخطيط بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-112">Select **New** on the tool bar for the **Intercompany planning group members** tab.</span></span>
12. <span data-ttu-id="aa950-113">في حقل **الكيان القانوني**، حدد **DEMF**.</span><span class="sxs-lookup"><span data-stu-id="aa950-113">Select **DEMF** in the **Legal entity** field.</span></span>
13. <span data-ttu-id="aa950-114">حدد **0** في الحقل **تسلسل الجدولة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-114">Select **0** in the **Scheduling sequence** field.</span></span>
12. <span data-ttu-id="aa950-115">حدد **20** في حقل **الخطة الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="aa950-115">Select **20** in the **Master plan** field.</span></span>
11. <span data-ttu-id="aa950-116">قم بإلغاء تحديد خانتي الاختيار **النسخ التلقائي للخطة الثابتة** و **النسخ التلقائي للخطة المتغيرة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-116">Clear the **Automatic Copy to Static Plan** and **Automatic Copy to Dynamic Plan** check boxes.</span></span>
12. <span data-ttu-id="aa950-117">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="aa950-117">Select **Save**.</span></span>

## <a name="assign-an-item-allocation-key"></a><span data-ttu-id="aa950-118">تعيين مفتاح تخصيص صنف</span><span class="sxs-lookup"><span data-stu-id="aa950-118">Assign an item allocation key</span></span>

1.  <span data-ttu-id="aa950-119">حدد **التخطيط الرئيسي > إعداد > التنبؤ بالطلب > مفاتيح تخصيص الأصناف**.</span><span class="sxs-lookup"><span data-stu-id="aa950-119">Select **Master Planning > Setup > Demand Forecasting > Item Allocation Keys**.</span></span>
2.  <span data-ttu-id="aa950-120">حدد **معالج**.</span><span class="sxs-lookup"><span data-stu-id="aa950-120">Select **Wizard**.</span></span>
2.  <span data-ttu-id="aa950-121">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="aa950-121">Select **Next**.</span></span>
3.  <span data-ttu-id="aa950-122">حدد **الصوت** من القائمة المنسدلة **مجموعة الصنف**.</span><span class="sxs-lookup"><span data-stu-id="aa950-122">Select **Audio** from the **Item Group** drop-down menu.</span></span>
3.  <span data-ttu-id="aa950-123">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="aa950-123">Select **Next**.</span></span>
4.  <span data-ttu-id="aa950-124">في الحقل **الاسم**، اكتب **مجموعة الصوت**.</span><span class="sxs-lookup"><span data-stu-id="aa950-124">Type **Audio Group** in the **Name** field.</span></span>
5.  <span data-ttu-id="aa950-125">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="aa950-125">Select **Next**.</span></span>
6.  <span data-ttu-id="aa950-126">حدد **التالي** في الصفحة **نظرة عامة** بعد التحقق من صحة المعلومات.</span><span class="sxs-lookup"><span data-stu-id="aa950-126">Select **Next** on the **Overview** page after verifying that the information is correct.</span></span>
7.  <span data-ttu-id="aa950-127">حدد **إنهاء** في الصفحة **مكتمل** بعد التحقق من صحة المعلومات.</span><span class="sxs-lookup"><span data-stu-id="aa950-127">Select **Finish** on the **Completed** page after verifying that the information is correct.</span></span>

## <a name="set-up-a-working-time-calendar-for-demf"></a><span data-ttu-id="aa950-128">إعداد تقويم زمني للعمل لدى DEMF‬‏‫</span><span class="sxs-lookup"><span data-stu-id="aa950-128">Set up a working time calendar for DEMF</span></span>

1.  <span data-ttu-id="aa950-129">في شركة **DEMF**، انتقل إلى **إدارة المؤسسة > إعداد > تقويمات > تقويمات**.</span><span class="sxs-lookup"><span data-stu-id="aa950-129">In the **DEMF** company, go to **Organization administration > Setup > Calendars > Calendars**.</span></span>
2.  <span data-ttu-id="aa950-130">في التقويم **قياسي**، حدد **أوقات العمل** من جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="aa950-130">On the **Standard** calendar, select **Working times** from the Action Pane.</span></span>
3.  <span data-ttu-id="aa950-131">حدد **إنشاء أوقات العمل** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="aa950-131">Select **Compose working times** on the Action Pane.</span></span> 
4.  <span data-ttu-id="aa950-132">في شاشه الحوار، حدد التقويم **قياسي**.</span><span class="sxs-lookup"><span data-stu-id="aa950-132">On the dialog screen, select the **Standard** calendar.</span></span>
5.  <span data-ttu-id="aa950-133">قم بتحديد **تاريخ البدء** اعتباراً من اليوم.</span><span class="sxs-lookup"><span data-stu-id="aa950-133">Fill in the **From date** as of today.</span></span> 
6.  <span data-ttu-id="aa950-134">قم بتحديد **تاريخ الانتهاء** في غضون سنة واحدة اعتباراً من اليوم.</span><span class="sxs-lookup"><span data-stu-id="aa950-134">Fill in the **To date** as one year from today.</span></span>
7.  <span data-ttu-id="aa950-135">حدد **قالب مواعيد العمل، قياسي**.</span><span class="sxs-lookup"><span data-stu-id="aa950-135">Select for the **Working time template, Standard**.</span></span>
8.  <span data-ttu-id="aa950-136">حدد **موافق**</span><span class="sxs-lookup"><span data-stu-id="aa950-136">Select **OK**</span></span>
9.  <span data-ttu-id="aa950-137">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="aa950-137">Close the page.</span></span>

## <a name="run-an-intercompany-master-plan"></a><span data-ttu-id="aa950-138">تشغيل خطة رئيسية بين الشركات الشقيقة</span><span class="sxs-lookup"><span data-stu-id="aa950-138">Run an intercompany master plan</span></span>

1.  <span data-ttu-id="aa950-139">في **DEMF**، افتح **التخطيط الرئيسي > التخطيط الرئيسي > تشغيل > تخطيط رئيسي بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-139">Open, in **DEMF**, **Master planning > Master planning > Run > Intercompany master planning**.</span></span>
2.  <span data-ttu-id="aa950-140">حدد **40** لـ **مجموعة التخطيط بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-140">Select **40** for **Intercompany planning group**.</span></span>
3.  <span data-ttu-id="aa950-141">أدخل **2** لـ **عدد تكرارات التخطيط بين الشركات الشقيقة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-141">Enter **2** for **Number of intercompany planning iterations**.</span></span>
4.  <span data-ttu-id="aa950-142">حدد **إعادة إنشاء** **للتكرار الأول**.</span><span class="sxs-lookup"><span data-stu-id="aa950-142">Select **Regeneration** for **First iteration**.</span></span>
5.  <span data-ttu-id="aa950-143">حدد **صافي التغيير** **للتكرارات اللاحقة**.</span><span class="sxs-lookup"><span data-stu-id="aa950-143">Select **Net change** for **Subsequent iterations**.</span></span>
6.  <span data-ttu-id="aa950-144">قم بتعيين شريط تمرير **وقت معالجة التعقب** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="aa950-144">Set the **Track processing time** slider to **No**.</span></span>
7.  <span data-ttu-id="aa950-145">قم بتعيين **عدد مؤشرات الترابط** إلى **0**.</span><span class="sxs-lookup"><span data-stu-id="aa950-145">Set **Number of threads** to **0**.</span></span>
8. <span data-ttu-id="aa950-146">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="aa950-146">Select **OK**.</span></span>
9. <span data-ttu-id="aa950-147">افتح **التخطيط الرئيسي > الاستعلامات والتقارير > التخطيط الرئيسي بين الشركات الشقيقة > التوريد والطلب بين الشركات الشقيقة** لعرض النتائج.</span><span class="sxs-lookup"><span data-stu-id="aa950-147">Open **Master planning > Inquiries and reports > Intercompany  master planning > Intercompany supply and demand** to view the results.</span></span> <span data-ttu-id="aa950-148">قد ترغب في فرز **تاريخ الطلب** حسب التاريخ الأحدث أولاً لعرض نتائج تشغيل التخطيط الرئيسي التي قمت بإكمالها.</span><span class="sxs-lookup"><span data-stu-id="aa950-148">You may want to sort **Requirement date** by newest date first to see the results of the master planning run you have just completed.</span></span> 
