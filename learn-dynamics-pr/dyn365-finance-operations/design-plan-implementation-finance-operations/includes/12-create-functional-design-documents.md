---
ms.openlocfilehash: 30d090e4e1185e48a6a5b41832a294366f929864
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071392"
---

<span data-ttu-id="1baa2-101">تصف مستندات التصميم الوظيفية (FDD) الميزات المخططة في التخصيصات.</span><span class="sxs-lookup"><span data-stu-id="1baa2-101">Functional design documents (FDD) describe the planned features in customizations.</span></span> <span data-ttu-id="1baa2-102">يمكن ان يتضمن المستند أشياء مثل المخططات الانسيابية ولقطات الشاشة وإطارات الأسلاك.</span><span class="sxs-lookup"><span data-stu-id="1baa2-102">The document can include things such as flowcharts, screenshots, and wire frames.</span></span> <span data-ttu-id="1baa2-103">ويمكن أن يحتوي أيضا على قائمة منظمة بالمتطلبات التي يمكن استخدامها للتطوير والاختبار وتسجيل العميل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-103">It can also contain an organized list of requirements that can be used for development, testing, and client sign-off.</span></span>
 
## <a name="benefits-of-functional-design-documents"></a><span data-ttu-id="1baa2-104">فوائد مستندات التصميم الوظيفية</span><span class="sxs-lookup"><span data-stu-id="1baa2-104">Benefits of functional design documents</span></span>

<span data-ttu-id="1baa2-105">فيما يلي بعض فوائد مستندات التصميم الوظيفية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-105">The following are some of the benefits of functional design documents:</span></span>

- <span data-ttu-id="1baa2-106">مساعدة فريق التطوير لفهم الميزة وتوفير نطاق واضح وتعريف ما يتم تطويره.</span><span class="sxs-lookup"><span data-stu-id="1baa2-106">Help the development team to understand the feature and provide a clear scope and definition of what to develop.</span></span> <span data-ttu-id="1baa2-107">تعمل هذه المستندات على تسهيل عملية التطوير، ويكون لفريق التطوير الذي يعمل على الميزة فهم وإجابات واضحة لكافة الاسئلة المتعلقة بالوظائف قبل بدء التطوير.</span><span class="sxs-lookup"><span data-stu-id="1baa2-107">These documents streamline the development process, and the development team working on the feature has a clear understanding and answers to all their functionality-related questions before starting development.</span></span> <span data-ttu-id="1baa2-108">ونظرا لأن هذا المستند معتمد من قبل العميل، سيقوم المطورون فقط بتطوير التخصيصات والملحقات التي تم اعتمادها.</span><span class="sxs-lookup"><span data-stu-id="1baa2-108">Because this document is approved by the customer, the developers only develop customizations and extensions that are approved.</span></span>

    - <span data-ttu-id="1baa2-109">فد هو العمل الجاري، لذا يجب تعيين فرق التطوير وفرق QA إلى كل منطقه وظيفية.</span><span class="sxs-lookup"><span data-stu-id="1baa2-109">The FDD is a work in progress, so you need to assign the development and QA teams to each functional area.</span></span> <span data-ttu-id="1baa2-110">وهذا يعني أنك تحتاج إلى القيام بذلك لمراجعة التصميم الوظيفي ودعم محللي الأعمال المعنية في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="1baa2-110">This means that you need to engage them in reviewing the functional design and support the respective business analysts early on.</span></span>
    - <span data-ttu-id="1baa2-111">الملحق هو نموذج التطوير الوحيد الذي يمكن للمطور فيه استخدام الأحداث وربطها داخل التعليمات البرمجية للتطبيق لتضمين وظائف إضافية دون التأثير على التعليمات البرمجية لـ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1baa2-111">Extension is the only development model where the developer can use events and hooks within the application code to include additional functionalities without impacting the Microsoft code.</span></span>
    - <span data-ttu-id="1baa2-112">حاول أن تقوم بالإقرار بالوظيفة القياسية قدر الإمكان أثناء تصميم الحلول.</span><span class="sxs-lookup"><span data-stu-id="1baa2-112">Try to adopt the standard functionality as much as possible while designing solutions.</span></span>
- <span data-ttu-id="1baa2-113">تساعد فريق الاختبار على فهم الميزات ضمن التطوير ولتطوير خطة اختبار حولها.</span><span class="sxs-lookup"><span data-stu-id="1baa2-113">Help the testing team to understand the feature under development and to develop a test plan around it.</span></span> 
- <span data-ttu-id="1baa2-114">تحديد كافة المتطلبات الوظيفية التبادلية.</span><span class="sxs-lookup"><span data-stu-id="1baa2-114">Identify all the cross-functional requirements.</span></span> <span data-ttu-id="1baa2-115">يجب أن يقودك مهندس الحلول لتصميمات مناسبة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-115">The solution architect should lead them to suitable designs.</span></span>
- <span data-ttu-id="1baa2-116">قم بتزويد العميل برؤية واضحة وتعريف للميزة التي يتم تطويرها.</span><span class="sxs-lookup"><span data-stu-id="1baa2-116">Provide the customer with a clear vision and definition of the feature being developed.</span></span> <span data-ttu-id="1baa2-117">وكذلك، قم بمساعدة فريق المشروع بالكامل ليتمكن من عرض الحل ومشاهدته قبل إنشائه.</span><span class="sxs-lookup"><span data-stu-id="1baa2-117">Also, help the entire project team to be able to visualize and see the solution before it is built.</span></span> 
- <span data-ttu-id="1baa2-118">قم بتوفير الأساس لوثائق التدريب الخاصة بفريق دعم التطبيقات ومستخدمي الأعمال.</span><span class="sxs-lookup"><span data-stu-id="1baa2-118">Provide the baseline of the training documentation for the application support team and business users.</span></span>

## <a name="business-requirement-definition-phase"></a><span data-ttu-id="1baa2-119">مرحلة تعريف متطلبات العمل</span><span class="sxs-lookup"><span data-stu-id="1baa2-119">Business requirement definition phase</span></span>

<span data-ttu-id="1baa2-120">في مرحلة تعريف المشروع، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-120">In the definition phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-121">سيناريوهات الأعمال والعمليات في تنسيق هرمي.</span><span class="sxs-lookup"><span data-stu-id="1baa2-121">The business scenarios and processes in a hierarchical format.</span></span>
- <span data-ttu-id="1baa2-122">تدفقات معالجة نهاية إلى نهاية.</span><span class="sxs-lookup"><span data-stu-id="1baa2-122">End-to-end process flows.</span></span>
- <span data-ttu-id="1baa2-123">حالات الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="1baa2-123">Use cases.</span></span>
- <span data-ttu-id="1baa2-124">عمليات سير العمل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-124">Business flows.</span></span>
- <span data-ttu-id="1baa2-125">مخطط الحل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-125">Solution blueprint.</span></span>

<span data-ttu-id="1baa2-126">بعد تعريف النطاق، يجب أن يقوم فريق التنفيذ بتحليل كل متطلب في مرحلة التحليل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-126">After defining the scope, the implementation team should analyze each requirement in the analysis phase.</span></span>

## <a name="solution-analysis-phase"></a><span data-ttu-id="1baa2-127">مرحلة تحليل الحل</span><span class="sxs-lookup"><span data-stu-id="1baa2-127">Solution analysis phase</span></span>
<span data-ttu-id="1baa2-128">في مرحلة تحليل المشروع، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-128">In the analysis phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-129">‏‫تحليل الملاءمة/الفجوات.</span><span class="sxs-lookup"><span data-stu-id="1baa2-129">Fit/gap analysis.</span></span>
- <span data-ttu-id="1baa2-130">خيارات التخصيص والحلول البديلة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-130">Workarounds and customization options.</span></span>
- <span data-ttu-id="1baa2-131">البناء مقابل تقييم الشراء.</span><span class="sxs-lookup"><span data-stu-id="1baa2-131">Build versus buy evaluation.</span></span>
- <span data-ttu-id="1baa2-132">تحليل SWOT (القوه والضعف والفرص والتهديدات) الخاص بالحلول والتخصيصات/التحسينات.</span><span class="sxs-lookup"><span data-stu-id="1baa2-132">The SWOT (Strength, Weakness, Opportunities, and Threats) analysis for workarounds and customizations/enhancements.</span></span>

## <a name="solution-design-phase"></a><span data-ttu-id="1baa2-133">مرحله تصميم الحل</span><span class="sxs-lookup"><span data-stu-id="1baa2-133">Solution design phase</span></span>

<span data-ttu-id="1baa2-134">في مرحلة التصميم، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-134">In the design phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-135">القدرات الجاهزة لتناسب العمليات التجارية للحل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-135">Out-of-the-box capabilities to fit the business processes of the solution.</span></span>
- <span data-ttu-id="1baa2-136">تصميمات وظيفية وتقنيات لأية فجوات في الحل الحالي.</span><span class="sxs-lookup"><span data-stu-id="1baa2-136">Functional and technical designs for any gaps in the present solution.</span></span>
- <span data-ttu-id="1baa2-137">سيناريوهات اختبار نهاية الطرف الخاصة بالقبول الكلي للحل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-137">End-to-end test scenarios for overall solution acceptance.</span></span>
- <span data-ttu-id="1baa2-138">نهاية لمنطقة العملية التجارية.</span><span class="sxs-lookup"><span data-stu-id="1baa2-138">End-to-end for a business process area.</span></span>
- <span data-ttu-id="1baa2-139">واحد أو أكثر من برامج الاختبار النصية لكل متطلب.</span><span class="sxs-lookup"><span data-stu-id="1baa2-139">One or more test script(s) per requirement.</span></span>
- <span data-ttu-id="1baa2-140">مخطط حل الحالة المستقبلية.</span><span class="sxs-lookup"><span data-stu-id="1baa2-140">Future-state solution blueprint.</span></span>

## <a name="prototyping"></a><span data-ttu-id="1baa2-141">صنع نماذج نمطية</span><span class="sxs-lookup"><span data-stu-id="1baa2-141">Prototyping</span></span>
<span data-ttu-id="1baa2-142">في مرحلة صنع النماذج النمطية، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-142">In the prototyping phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-143">تكوين نموذج أولي لتدفق الأعمال في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="1baa2-143">A prototype configuration of the business flow in Finance and Operations apps.</span></span>
- <span data-ttu-id="1baa2-144">ترحيل البيانات العينة</span><span class="sxs-lookup"><span data-stu-id="1baa2-144">Sample data migration.</span></span>
- <span data-ttu-id="1baa2-145">بيانات العرض التوضيحي وإرشادات المهام ومقاطع فيديو التدريب.</span><span class="sxs-lookup"><span data-stu-id="1baa2-145">Demo data, task guides, and training videos.</span></span>
- <span data-ttu-id="1baa2-146">مشاركة عملية.</span><span class="sxs-lookup"><span data-stu-id="1baa2-146">Hands-on labs.</span></span>
 
<span data-ttu-id="1baa2-147">بعد قبول النموذج الأولي، يمكن تعيين أية فجوات أو واجهات أو تقارير إلى فريق التطوير.</span><span class="sxs-lookup"><span data-stu-id="1baa2-147">After the acceptance of the prototype, any gaps, interfaces, or reports can be assigned to the development team.</span></span>

## <a name="development-phase"></a><span data-ttu-id="1baa2-148">مرحله التطوير</span><span class="sxs-lookup"><span data-stu-id="1baa2-148">Development phase</span></span>
<span data-ttu-id="1baa2-149">في مرحلة التطوير، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-149">In the development phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-150">منتجات التطوير.</span><span class="sxs-lookup"><span data-stu-id="1baa2-150">Development artifacts.</span></span>
- <span data-ttu-id="1baa2-151">علاقة الكيان (ER).</span><span class="sxs-lookup"><span data-stu-id="1baa2-151">Entity relationship (ER).</span></span>
- <span data-ttu-id="1baa2-152">الرمز.</span><span class="sxs-lookup"><span data-stu-id="1baa2-152">Code.</span></span>
- <span data-ttu-id="1baa2-153">التصميمات.</span><span class="sxs-lookup"><span data-stu-id="1baa2-153">Designs.</span></span>

## <a name="testing-and-acceptance-phase"></a><span data-ttu-id="1baa2-154">مرحله الاختبار والقبول</span><span class="sxs-lookup"><span data-stu-id="1baa2-154">Testing and acceptance phase</span></span> 
<span data-ttu-id="1baa2-155">في مرحلة الاختبار، يجب أن يقوم فريق التنفيذ بمعالجة التالي:</span><span class="sxs-lookup"><span data-stu-id="1baa2-155">In the testing phase of the project, the implementation team should address the following:</span></span>

- <span data-ttu-id="1baa2-156">خطه الاختبار.</span><span class="sxs-lookup"><span data-stu-id="1baa2-156">Test plan.</span></span>
- <span data-ttu-id="1baa2-157">سيناريوهات الاختبار.</span><span class="sxs-lookup"><span data-stu-id="1baa2-157">Test scenarios.</span></span>
- <span data-ttu-id="1baa2-158">حالات الاختبار.</span><span class="sxs-lookup"><span data-stu-id="1baa2-158">Test cases.</span></span>
- <span data-ttu-id="1baa2-159">سجلات المشاكل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-159">Issue logs.</span></span>

## <a name="training-phase"></a><span data-ttu-id="1baa2-160">مرحلة التدريب</span><span class="sxs-lookup"><span data-stu-id="1baa2-160">Training phase</span></span> 
<span data-ttu-id="1baa2-161">في مرحلة التدريب، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-161">In the training phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-162">كتيبات التدريب.</span><span class="sxs-lookup"><span data-stu-id="1baa2-162">Training manuals.</span></span>
- <span data-ttu-id="1baa2-163">دلائل المهام/المستخدم.</span><span class="sxs-lookup"><span data-stu-id="1baa2-163">User/task guides.</span></span> 

## <a name="go-live-phase"></a><span data-ttu-id="1baa2-164">مرحلة الانتقال المباشر</span><span class="sxs-lookup"><span data-stu-id="1baa2-164">Go-live phase</span></span>
<span data-ttu-id="1baa2-165">في مرحلة البث المباشر، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-165">In the Go-live phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-166">مرحلي قائمة اختيار.</span><span class="sxs-lookup"><span data-stu-id="1baa2-166">Cutover checklist.</span></span>
- <span data-ttu-id="1baa2-167">استعداد الانتقال المباشر</span><span class="sxs-lookup"><span data-stu-id="1baa2-167">Go-live readiness</span></span>
- <span data-ttu-id="1baa2-168">البيئة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-168">Environment.</span></span>
- <span data-ttu-id="1baa2-169">الوصول.</span><span class="sxs-lookup"><span data-stu-id="1baa2-169">Access.</span></span>
- <span data-ttu-id="1baa2-170">مراسلات الاتصال.</span><span class="sxs-lookup"><span data-stu-id="1baa2-170">Communication mailers.</span></span>

<span data-ttu-id="1baa2-171">بعد الانتهاء من الزيارة الناجحة، من المهم الاستمرار في الرحلة والاحتفاظ بمزايا الحصد من النظام الأساسي للأعمال مع الحفاظ عليها سليمة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-171">After a successful Go-live, it is important to continue the journey and keep reaping benefits from the business platform while keeping it healthy.</span></span>

## <a name="support-phase"></a><span data-ttu-id="1baa2-172">مرحله الدعم</span><span class="sxs-lookup"><span data-stu-id="1baa2-172">Support phase</span></span> 
<span data-ttu-id="1baa2-173">في مرحلة الدعم، يجب أن يقوم فريق التنفيذ بمعالجة الأحداث الرئيسية التالية:</span><span class="sxs-lookup"><span data-stu-id="1baa2-173">In the support phase of the project, the implementation team should address the following milestones:</span></span>

- <span data-ttu-id="1baa2-174">خطة الدعم/الصيانة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-174">Support/maintenance plan.</span></span>
- <span data-ttu-id="1baa2-175">الفريق الذي يمتد على مستويات متنوعة من الدعم.</span><span class="sxs-lookup"><span data-stu-id="1baa2-175">Team that spans various levels of support needs.</span></span>
- <span data-ttu-id="1baa2-176">المبادرات المحسنة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-176">Enhancement initiatives.</span></span>
- <span data-ttu-id="1baa2-177">الاحتياجات الجيدة للأعمال.</span><span class="sxs-lookup"><span data-stu-id="1baa2-177">Good-to-have business needs.</span></span> 
- <span data-ttu-id="1baa2-178">مشاكل المدخل.</span><span class="sxs-lookup"><span data-stu-id="1baa2-178">Issues portal.</span></span>
- <span data-ttu-id="1baa2-179">التدريب الجاري وجمع المبادرات وأنواع أخرى من المساعدة.</span><span class="sxs-lookup"><span data-stu-id="1baa2-179">Ongoing training, roll out initiatives, and other kinds of assistance.</span></span>

 
