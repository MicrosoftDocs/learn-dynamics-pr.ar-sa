---
ms.openlocfilehash: 691f9bfe7778784a820722ce8f10957113302801
ms.sourcegitcommit: 0af0a6f1739b0e2a5ec60989ffbf8aa131de41c3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/08/2021
ms.locfileid: "6072235"
---
<span data-ttu-id="ab5aa-101">يمكن إنشاء مؤشرات الأداء الأساسية (KPI) في بيئة المطور ثم تضمينها في مساحات العمل لتزويد المستخدمين بقيم أساسية قابلة للقياس تسمح لهم بمعرفة كيفية أداء الأعمال.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-101">KPIs can be created in the developer environment and then embedded into workspaces to provide users with key measurable values that allow them to see how business is performing.</span></span> <span data-ttu-id="ab5aa-102">تُظهر الصورة أدناه مثالاً على لوحة مؤشرات الأداء الأساسية (KPI) في مساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-102">The below image shows an example of a KPI tile in a workspace.</span></span> 
 
![لقطة شاشة لإطار متجانب مؤشرات الأداء الأساسية (KPI) في مساحة عمل.](../media/kpi.png)

<span data-ttu-id="ab5aa-104">يجب أن يكون لمؤشرات الأداء الأساسية (KPI) أهداف واضحة يتم مراجعتها بشكل دوري لضمان تحقيق الأهداف.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-104">KPIs should have clear objectives that are periodically reviewed to ensure that the objectives are being met.</span></span> <span data-ttu-id="ab5aa-105">يمكن إنشاء مؤشرات الأداء الأساسية (KPI) باستخدام البيانات المجمعة المضمنة في القياسات المجمعة، وهو نموذج يحتوي على مجموعة من القياسات والأبعاد المقابلة لها.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-105">KPIs can be created by using aggregate data contained in aggregate measurements, which is a model that contains a collection of measures and their corresponding dimensions.</span></span> <span data-ttu-id="ab5aa-106">القياسات المستخدمة هي أرقام مجمعة، مثل إجمالي المبيعات.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-106">The measures that are used are aggregate numbers, such as total sales.</span></span> <span data-ttu-id="ab5aa-107">يمكن تعيين القياسات الإجمالية لقياس المجموع أو الحد الأدنى أو الحد الأقصى أو العد أو العد المميز أو المتوسط باستخدام خاصية التجميع الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-107">Aggregate measurements can be set to measure the sum, minimum, maximum, count, distinct count, or average by using the Default aggregate property.</span></span> 

<span data-ttu-id="ab5aa-108">بشكل افتراضي، تستخدم خاصية التجميع الافتراضية قياس العد.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-108">By default, the Default aggregate property uses the count measure.</span></span> <span data-ttu-id="ab5aa-109">يمكنك نشر القياس المجمع بطريقتين مختلفتين باستخدام خاصية الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-109">You can deploy the aggregate measurement two different ways by using the Usage property.</span></span> <span data-ttu-id="ab5aa-110">**InMemoryRealTime** يستخدم فهارس مخزن الأعمدة لقاعدة بيانات SQL Server للحصول على بيانات في الوقت الحقيقي.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-110">**InMemoryRealTime** uses Column store indexes of the SQL Server database to get real-time data.</span></span>
<span data-ttu-id="ab5aa-111">**StagedEntityStore** يستخدم مخزن الكيانات الذي يستخدم تقارير Power BI في الوقت الحقيقي تقريباً. </span><span class="sxs-lookup"><span data-stu-id="ab5aa-111">**StagedEntityStore** uses the Entity store that uses near real-time Power BI reporting.</span></span> <span data-ttu-id="ab5aa-112">يتيح لك هذا الخيار نشر توزيع القياس في مخزن الكيانات وتحديث البيانات بشكل دوري.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-112">This option allows you to deploy the measure to the Entity store and have the data refreshed periodically.</span></span>

<span data-ttu-id="ab5aa-113">الأبعاد عبارة عن مقسمات يمكن استخدامها لتحليل البيانات.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-113">Dimensions are slicers that can be used to analyze data.</span></span> <span data-ttu-id="ab5aa-114">من هذه القياسات والأبعاد المجمعة، يمكنك إنشاء كيان بيانات مجمعة.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-114">From these aggregate measurements and dimensions, you can create an aggregate data entity.</span></span> <span data-ttu-id="ab5aa-115">يمكنك استخدام البيانات المجمعة لتحديد مؤشر الأداء الأساسي (KPI) باستخدام X++.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-115">You can use the aggregate data to define a KPI by using X++.</span></span> <span data-ttu-id="ab5aa-116">بعد تحديد مؤشر الأداء الأساسي (KPI)، يمكن للمستخدمين تخصيصه في وقت التشغيل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-116">After the KPI has been defined, users can customize it at run time.</span></span>

![رسم تخطيطي للعلاقة بين القياسات والأبعاد الكلية ومؤشر الأداء الأساسي (KPI) الذي يحددونه.](../media/measure-dimension.png)

## <a name="create-aggregate-measurements"></a><span data-ttu-id="ab5aa-118">إنشاء قياسات مجمعة</span><span class="sxs-lookup"><span data-stu-id="ab5aa-118">Create aggregate measurements</span></span> 


<span data-ttu-id="ab5aa-119">لإنشاء قياسات مجمعة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-119">To create aggregate measurements, follow these steps:</span></span>



1.  <span data-ttu-id="ab5aa-120">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروعك وحدد **إضافة جديد > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-120">In the **Solution explorer**, right-click your project and select **Add New > New item**.</span></span>
2.  <span data-ttu-id="ab5aa-121">حدد **التحليلات > القياس المجمع**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-121">Select **Analytics > Aggregate Measurement**.</span></span>
3.  <span data-ttu-id="ab5aa-122">افتح **مستكشف التطبيق**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-122">Open **Application Explorer**.</span></span>
4.  <span data-ttu-id="ab5aa-123">انتقل إلى **النتائج > نموذج البيانات > طرق العرض** وحدد طريقة العرض لإنشاء القياسات.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-123">Go to **Artifacts > Data Model > Views** and select the view to create measurements.</span></span>
5.  <span data-ttu-id="ab5aa-124">اسحب **طريقة العرض** إلى **القياس المجمع**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-124">Drag the **View** into the **Aggregate measure**.</span></span>
6.  <span data-ttu-id="ab5aa-125">اسحب حقول **طريقة العرض** وأفلتها في مجموعة **القياس** للحصول على القياس المجمع.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-125">Drag and drop the **View** fields in the **Measure** group for the Aggregate measure.</span></span>
7.  <span data-ttu-id="ab5aa-126">يحتوي كل قياس على خاصية تجميع افتراضية يمكنك تعيينها:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-126">Each measure has a default Aggregate property that you can set:</span></span>
    -   <span data-ttu-id="ab5aa-127">العد</span><span class="sxs-lookup"><span data-stu-id="ab5aa-127">Count</span></span>
    -   <span data-ttu-id="ab5aa-128">المجموع</span><span class="sxs-lookup"><span data-stu-id="ab5aa-128">Sum</span></span>
    -   <span data-ttu-id="ab5aa-129">AverageOfChildren</span><span class="sxs-lookup"><span data-stu-id="ab5aa-129">AverageOfChildren</span></span>
    -   <span data-ttu-id="ab5aa-130">DistinctCount</span><span class="sxs-lookup"><span data-stu-id="ab5aa-130">DistinctCount</span></span>
    -   <span data-ttu-id="ab5aa-131">‏‫الحد الأقصى</span><span class="sxs-lookup"><span data-stu-id="ab5aa-131">Max</span></span>
    -   <span data-ttu-id="ab5aa-132">الحد الأدنى</span><span class="sxs-lookup"><span data-stu-id="ab5aa-132">Min</span></span>
8.  <span data-ttu-id="ab5aa-133">احفظ الكل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-133">Save all.</span></span>

## <a name="create-aggregate-dimensions"></a><span data-ttu-id="ab5aa-134">إنشاء الأبعاد المجمعة</span><span class="sxs-lookup"><span data-stu-id="ab5aa-134">Create aggregate dimensions</span></span> 


<span data-ttu-id="ab5aa-135">لإنشاء أبعاد مجمعة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-135">To create aggregate dimensions, follow these steps:</span></span>

1.  <span data-ttu-id="ab5aa-136">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروعك وحدد **إضافة جديد > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-136">In the **Solution explorer**, right-click your project and select **Add New > New Item**.</span></span>
2.  <span data-ttu-id="ab5aa-137">حدد **التحليلات > البُعد المجمع**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-137">Select **Analytics > Aggregate Dimension**.</span></span>
3.  <span data-ttu-id="ab5aa-138">افتح **مستكشف التطبيق**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-138">Open **Application Explorer**.</span></span>
4.  <span data-ttu-id="ab5aa-139">انتقل إلى **النتائج > نموذج البيانات > طرق العرض** وحدد طريقة العرض لسحب القياسات.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-139">Go to **Artifacts > Data model > Views** and select the view to pull measurements.</span></span>
5.  <span data-ttu-id="ab5aa-140">اسحب الصنف المحدد إلى جذر الأبعاد المجمعة.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-140">Drag the selected item onto the root of the aggregate dimensions.</span></span>
6.  <span data-ttu-id="ab5aa-141">اسحب الحقول من طريقة العرض إلى **البُعد المجمع > السمات**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-141">Drag the fields from the view into **Aggregate dimension >     Attributes**.</span></span>
7.  <span data-ttu-id="ab5aa-142">احفظ الكل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-142">Save all.</span></span>

## <a name="create-model-dimension-references"></a><span data-ttu-id="ab5aa-143">إنشاء مراجع أبعاد النماذج</span><span class="sxs-lookup"><span data-stu-id="ab5aa-143">Create model dimension references</span></span>  


<span data-ttu-id="ab5aa-144">لإنشاء مراجع أبعاد النماذج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-144">To create model dimension references, follow these steps:</span></span>

1.  <span data-ttu-id="ab5aa-145">اسحب البُعد المجمع وأفلته في عقدة **البُعد** الخاصة بالقياس المجمع.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-145">Drag and drop the aggregate dimension into the aggregate  measurement's **Dimension** node.</span></span>
2.  <span data-ttu-id="ab5aa-146">أنشئ علاقة جديدة في عقدة بُعد القياس المجمع.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-146">Create a new relation on the aggregate measurement dimension node.</span></span>
3.  <span data-ttu-id="ab5aa-147">قم بتعيين خاصية **سمة البُعد** في العلاقة إلى **نموذج**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-147">Set the **Dimension Attribute** property of the relation to **Model**.</span></span>
4.  <span data-ttu-id="ab5aa-148">احفظ الكل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-148">Save all.</span></span>

## <a name="deploy-aggregate-measurements"></a><span data-ttu-id="ab5aa-149">توزيع القياسات المجمعة</span><span class="sxs-lookup"><span data-stu-id="ab5aa-149">Deploy aggregate measurements</span></span> 


<span data-ttu-id="ab5aa-150">لتوزيع قياسات مجمعة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-150">To deploy aggregate measurements, follow these steps:</span></span>

1.  <span data-ttu-id="ab5aa-151">حدد القياس المجمع.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-151">Select the aggregate measurement.</span></span>
2.  <span data-ttu-id="ab5aa-152">قم بتعيين خاصية **الاستخدام**:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-152">Set the **Usage** property:</span></span>
    -   <span data-ttu-id="ab5aa-153">InMemoryRealTime</span><span class="sxs-lookup"><span data-stu-id="ab5aa-153">InMemoryRealTime</span></span>
    -   <span data-ttu-id="ab5aa-154">StagedEntityStore</span><span class="sxs-lookup"><span data-stu-id="ab5aa-154">StagedEntityStore</span></span>
3.  <span data-ttu-id="ab5aa-155">انقر بزر الماوس الأيمن فوق القياس المجمع وحدد **إضافة فهارس مخزن الأعمدة**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-155">Right-click the aggregate measurement and select **Add Column Store Indices**.</span></span>

## <a name="create-the-aggregate-data-entity"></a><span data-ttu-id="ab5aa-156">إنشاء كيان البيانات المجمعة</span><span class="sxs-lookup"><span data-stu-id="ab5aa-156">Create the aggregate data entity</span></span> 


<span data-ttu-id="ab5aa-157">لإنشاء كيان البيانات المجمعة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-157">To create the aggregate data entity, follow these steps:</span></span>



1.  <span data-ttu-id="ab5aa-158">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروعك وحدد **إضافة جديد > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-158">In the **Solution explorer**, right-click your project and select **Add new > New item**.</span></span>
2.  <span data-ttu-id="ab5aa-159">حدد **التحليلات > كيان البيانات المجمعة**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-159">Select **Analytics > Aggregate Data Entity**.</span></span>
3.  <span data-ttu-id="ab5aa-160">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-160">Select **Add**.</span></span>
4.  <span data-ttu-id="ab5aa-161">اسحب وأفلت القياس المجمع في مصدر البيانات لكيان البيانات المجمعة.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-161">Drag and drop the aggregate measure to the data source of the   aggregate data entity.</span></span>
5.  <span data-ttu-id="ab5aa-162">في مصدر البيانات، اسحب القياسات وأفلتها في عقدة **حقول إدخالات البيانات المجمعة**</span><span class="sxs-lookup"><span data-stu-id="ab5aa-162">In the data source, drag and drop the measures into the **Aggregate data entity fields** node.</span></span>
6.  <span data-ttu-id="ab5aa-163">في مصدر البيانات، اسحب الأبعاد وأفلتها في عقدة **حقول إدخالات البيانات المجمعة**</span><span class="sxs-lookup"><span data-stu-id="ab5aa-163">In the data source, drag and drop the dimensions into the **Aggregate data entity fields** node.</span></span>
7.  <span data-ttu-id="ab5aa-164">أنشئ الحل واحفظه.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-164">Save and build the solution.</span></span>

## <a name="create-a-kpi"></a><span data-ttu-id="ab5aa-165">إنشاء مؤشر الأداء الأساسي (KPI)</span><span class="sxs-lookup"><span data-stu-id="ab5aa-165">Create a KPI</span></span> 


<span data-ttu-id="ab5aa-166">لإنشاء مؤشر الأداء الأساسي (KPI)، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-166">To create a KPI, follow these steps:</span></span>

 
1.  <span data-ttu-id="ab5aa-167">انقر بزر الماوس الأيمن فوق مشروع وحدد **إضافة > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-167">Right-click the project and select **Add > New Item**.</span></span>
2.  <span data-ttu-id="ab5aa-168">حدد **التحليلات > مؤشر الأداء الأساسي (KPI)**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-168">Select **Analytics > Key Performance Indicator**.</span></span>
3.  <span data-ttu-id="ab5aa-169">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-169">Select **Add**.</span></span>
4.  <span data-ttu-id="ab5aa-170">قم بتعيين خاصية **القياس** لتحديد قياس مؤشر الأداء الأساسي (KPI).</span><span class="sxs-lookup"><span data-stu-id="ab5aa-170">Set the **Measurement** property to select the measurement for the KPI.</span></span>
5.  <span data-ttu-id="ab5aa-171">حدد عقدة **القيمة** الخاصة بمؤشر الأداء الأساسي (KPI).</span><span class="sxs-lookup"><span data-stu-id="ab5aa-171">Select the **Value** node of the KPI.</span></span>
6.  <span data-ttu-id="ab5aa-172">قم بتعيين مجموعة القياسات في خاصية **مجموعة القياسات**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-172">Set the measurement group on the **Measure group** property.</span></span>
7.  <span data-ttu-id="ab5aa-173">قم بتعيين القياس في خاصية **القياس**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-173">Set the measure on the **Measure** property.</span></span>
8.  <span data-ttu-id="ab5aa-174">حدد عقدة **الهدف** الخاصة بمؤشر الأداء الأساسي (KPI).</span><span class="sxs-lookup"><span data-stu-id="ab5aa-174">Select the **Goal** node of the KPI.</span></span>
9.  <span data-ttu-id="ab5aa-175">قم بتعيين خاصية **نوع الهدف**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-175">Set the **Goal Type** property.</span></span>
10. <span data-ttu-id="ab5aa-176">قم بتعيين مجموعة القياسات في خاصية **مجموعة القياسات**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-176">Set the measurement group on the **Measure group** property.</span></span>
11. <span data-ttu-id="ab5aa-177">قم بتعيين القياس في خاصية **القياس**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-177">Set the measure on the **Measure** property.</span></span>
12. <span data-ttu-id="ab5aa-178">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-178">Select **Save**.</span></span>

## <a name="add-the-kpi-to-a-workspace"></a><span data-ttu-id="ab5aa-179">إضافة مؤشر الأداء الأساسي (KPI) إلى مساحة عمل</span><span class="sxs-lookup"><span data-stu-id="ab5aa-179">Add the KPI to a workspace</span></span> 


<span data-ttu-id="ab5aa-180">لإضافه مؤشر الأداء الأساسي (KPI) إلى مساحة عمل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab5aa-180">To add the KPI to a workspace, follow these steps:</span></span>

1.  <span data-ttu-id="ab5aa-181">انقر بزر الماوس الأيمن فوق مشروع وحدد **إضافة > صنف جديد**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-181">Right-click the project and select **Add > New item**.</span></span>
2.  <span data-ttu-id="ab5aa-182">حدد **واجهة المستخدم > الإطار المتجانب**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-182">Select **User Interface > Tile**.</span></span>
3.  <span data-ttu-id="ab5aa-183">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-183">Select **Add**.</span></span>
4.  <span data-ttu-id="ab5aa-184">اسحب وأفلت مؤشر الأداء الأساسي (KPI) من **مستكشف الحلول** في الإطار المتجانب الموجود في **مصم الإطارات المتجانبة**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-184">Drag and drop the KPI from **Solution explorer** onto the tile in the **Tile designer**.</span></span>
5.  <span data-ttu-id="ab5aa-185">احفظ.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-185">Save.</span></span>
6.  <span data-ttu-id="ab5aa-186">أنشئ ملحقاً لنموذج مساحة عمل موجود أو أنشئ نموذج مساحة عمل جديداً.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-186">Create an extension of an existing workspace form or create a new  workspace form.</span></span>
7.  <span data-ttu-id="ab5aa-187">في المصمم، أضف زر **الإطار المتجانب**.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-187">In the Designer, add a **Tile** button.</span></span>
8.  <span data-ttu-id="ab5aa-188">قم بتعيين الخيار المنسدل **خاصية الإطار المتجانب** إلى إطار متجانب مؤشر الأداء الأساسي (KPI) الذي أنشأته.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-188">Set the **Tile property** drop-down option to the KPI tile that you created.</span></span>
9.  <span data-ttu-id="ab5aa-189">احفظ الكل وأنشئ الحل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-189">Save all and build the solution.</span></span>
10. <span data-ttu-id="ab5aa-190">ستُظهر مساحة العمل مؤشر الأداء الأساسي (KPI) الجديد الذي تم إنشاؤه.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-190">Workspace will show the new KPI that was created.</span></span> <span data-ttu-id="ab5aa-191">حدد إطار متجانب مؤشر الأداء الأساسي (KPI) لعرض التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="ab5aa-191">Select the KPI tile to view details.</span></span>
