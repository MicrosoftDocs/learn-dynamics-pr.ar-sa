---
ms.openlocfilehash: fdcf10ab237698280afd5a720e4be489f56e817e
ms.sourcegitcommit: e0a1238596690b3b6eedd86c2ac14099948a5e25
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "6073850"
---

<span data-ttu-id="064b6-101">تُعد قياسات قائمة مكونات الصنف (BOM) نوعاً من التكوين.</span><span class="sxs-lookup"><span data-stu-id="064b6-101">BOM measurements are a type of configuration.</span></span> <span data-ttu-id="064b6-102">يمكن تحديد الأبعاد التالية كقياسات BOM:</span><span class="sxs-lookup"><span data-stu-id="064b6-102">The following dimensions can be specified as BOM measurements:</span></span>

-   <span data-ttu-id="064b6-103">الارتفاع</span><span class="sxs-lookup"><span data-stu-id="064b6-103">Height</span></span>
-   <span data-ttu-id="064b6-104">العرض</span><span class="sxs-lookup"><span data-stu-id="064b6-104">Width</span></span>
-   <span data-ttu-id="064b6-105">العمق</span><span class="sxs-lookup"><span data-stu-id="064b6-105">Depth</span></span>
-   <span data-ttu-id="064b6-106">الكثافة</span><span class="sxs-lookup"><span data-stu-id="064b6-106">Density</span></span>

<span data-ttu-id="064b6-107">يمكنك استخدام تكوينات القياس لتقليل عدد إصدارات BOM.</span><span class="sxs-lookup"><span data-stu-id="064b6-107">You can use measurement configurations to reduce the number of BOM versions.</span></span> <span data-ttu-id="064b6-108">بعبارة أخرى، سيتعين عليك فقط إنشاء إصدار BOM واحد لمجموعة من الأصناف يكون الاختلاف الوحيد بينها في القياسات الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="064b6-108">In other words, you will only have to create one BOM version for a group of items in which the only variation between them is in their measurements.</span></span>

<span data-ttu-id="064b6-109">على سبيل المثال، تصنع إحدى الشركات الطاولات المتداخلة في مجموعات من ثلاث طاولات.</span><span class="sxs-lookup"><span data-stu-id="064b6-109">For example, a company manufactures nested tables in sets of three.</span></span>
<span data-ttu-id="064b6-110">وتكون جميع الطاولات متطابقة فيما يتعلق بعمليات الإنتاج والمواد.</span><span class="sxs-lookup"><span data-stu-id="064b6-110">Each table is identical in terms of its production processes and materials.</span></span> <span data-ttu-id="064b6-111">ولا تختلف الطاولات فيما بينها إلا فيما يتعلق بالارتفاع والعرض والعمق.</span><span class="sxs-lookup"><span data-stu-id="064b6-111">The tables only differ from one another with respect to their height, width, and depth.</span></span> <span data-ttu-id="064b6-112">وباستخدام تكوينات القياس، يمكن إنتاج هذه الطاولات المتداخلة باستخدام قائمة BOM واحدة.</span><span class="sxs-lookup"><span data-stu-id="064b6-112">By using measurement configurations, these nested tables can be produced by using one BOM.</span></span>

<span data-ttu-id="064b6-113">يمكنك أيضاً استخدام أسلوب التقريب لأعلى لتوجيه كيفية تطبيق القياسات والاستهلاك.</span><span class="sxs-lookup"><span data-stu-id="064b6-113">You can also use the rounding-up method for guiding how measurements and consumption will be applied.</span></span>

## <a name="bom-measurements-defined-on-bom-lines"></a><span data-ttu-id="064b6-114">قياسات BOM المحددة في سطور BOM</span><span class="sxs-lookup"><span data-stu-id="064b6-114">BOM measurements defined on BOM lines</span></span>

<span data-ttu-id="064b6-115">نظراً لأن جميع مكونات BOM المطلوبة لعمل منتج نهائي واحد تكون معروضة في سطور BOM، ولأن كل سطر BOM يجب أن يحتوي على معلومات حول تخطيط المواد وحسابها واستهلاكها، يمكنك أيضاً تحديد المعلمات التالية:</span><span class="sxs-lookup"><span data-stu-id="064b6-115">Because all the BOM components that are required to make one finished product are shown on the BOM lines, and each BOM line must contain information on the planning, calculation, and consumption of the materials, you can also specify the following parameters:</span></span>

-   <span data-ttu-id="064b6-116">ما إذا كان للصنف إيه تكوينات</span><span class="sxs-lookup"><span data-stu-id="064b6-116">Whether the item has any configurations</span></span>

-   <span data-ttu-id="064b6-117">ما تلك التكوينات</span><span class="sxs-lookup"><span data-stu-id="064b6-117">What the configurations are</span></span>

<span data-ttu-id="064b6-118">ويمكن بعد ذلك استخدام تكوينات القياس عند حساب استهلاك المادة الخام لكل سطر من سطور BOM.</span><span class="sxs-lookup"><span data-stu-id="064b6-118">Measurement configurations can then be used when you are calculating the consumption of the raw material of each BOM line.</span></span>

### <a name="example---consumption-calculation-based-on-size"></a><span data-ttu-id="064b6-119">مثال - حساب الاستهلاك بناءً على الحجم</span><span class="sxs-lookup"><span data-stu-id="064b6-119">Example - Consumption calculation based on size</span></span>


<span data-ttu-id="064b6-120">تقدم الشركة خزانة مكبر صوت بأحجام متنوعة، مثل 16x38 بوصة، و14x36 بوصة، و18x50 بوصة.</span><span class="sxs-lookup"><span data-stu-id="064b6-120">A company offers a speaker cabinet in various sizes, such as 16x38 inches, 14x36 inches, and 18x50 inches.</span></span> <span data-ttu-id="064b6-121">تتطلب هذه الخزانة المكونات نفسها في أثناء الإنتاج، ولكن اعتماداً على الحجم المحدد للجزء النهائي، ستختلف كمية بعض المكونات.</span><span class="sxs-lookup"><span data-stu-id="064b6-121">This cabinet requires the same components during production, but depending on the selected size of the finished part, the quantity of some components will be different.</span></span>

<span data-ttu-id="064b6-122">في حالة استخدام وظيفة قياسات BOM، يتم إنشاء قائمة BOM واحدة فقط ويتم استخدامها لكل الأحجام المختلفة.</span><span class="sxs-lookup"><span data-stu-id="064b6-122">If the BOM measurements functionality is used, only one BOM is created and used for all different sizes.</span></span> <span data-ttu-id="064b6-123">وتوفر الخزانة النهائية الأبعاد المطلوبة، ويستخدم كل سطر من سطور BOM هذه الأبعاد لحساب الكمية المناسبة من أصناف المكونات التي يمكن استخدامها في أثناء الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="064b6-123">The finished cabinet provides the required dimensions, and each BOM line uses these dimensions to calculate the appropriate quantity of component items that can be used during production.</span></span>

## <a name="set-up-measurement-configurations"></a><span data-ttu-id="064b6-124">إعداد تكوينات القياس</span><span class="sxs-lookup"><span data-stu-id="064b6-124">Set up measurement configurations</span></span>

<span data-ttu-id="064b6-125">يتم تحديد تكوينات القياس في علامة التبويب **إعداد** في الصفحة **سطر BOM**.</span><span class="sxs-lookup"><span data-stu-id="064b6-125">Measurement configurations are defined on the **Setup** tab of the **BOM line** page.</span></span> <span data-ttu-id="064b6-126">حدد **معلومات المنتج وإدارته > قوائم مكونات الصنف والمعادلات > قوائم مكونات الصنف**.</span><span class="sxs-lookup"><span data-stu-id="064b6-126">Select **Product information and management > Bills of materials and formulas > Bills of materials**.</span></span> <span data-ttu-id="064b6-127">حدد BOM، ثم في السطور، حدد علامة التبويب **إعداد**، ثم أدخل المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="064b6-127">Select a BOM and then, on the lines, select the **Setup** tab and enter the following information:</span></span>

-   <span data-ttu-id="064b6-128">معادلة بُعد القياس التي تُستخدم لحساب استهلاك المواد.</span><span class="sxs-lookup"><span data-stu-id="064b6-128">The measurement dimension formula that is used to calculate the consumption of material.</span></span>

-   <span data-ttu-id="064b6-129">ما إذا كان سيتم تقريب الحساب.</span><span class="sxs-lookup"><span data-stu-id="064b6-129">Whether the calculation is to be rounded.</span></span> <span data-ttu-id="064b6-130">وإذا كان الأمر كذلك، فحدد الطريقة والعامل الذي يتم ذلك بواسطته.</span><span class="sxs-lookup"><span data-stu-id="064b6-130">If it is, specify how and by which factor.</span></span>

-   <span data-ttu-id="064b6-131">أبعاد القياس ذات الصلة في مجموعة القياس.</span><span class="sxs-lookup"><span data-stu-id="064b6-131">The relevant measurement dimensions in the Measurement group.</span></span>

<span data-ttu-id="064b6-132">عند اكتمال الإعداد، يمكنك حساب الاستهلاك من خلال تشغيل حساب BOM أو تقدير التكلفة.</span><span class="sxs-lookup"><span data-stu-id="064b6-132">When the setup is complete, you can calculate the consumption by running a BOM calculation or a cost estimation.</span></span>

<span data-ttu-id="064b6-133">وتتمثل خيارات حساب الاستهلاك فيما يلي:</span><span class="sxs-lookup"><span data-stu-id="064b6-133">Options for consumption calculation are:</span></span>

-   <span data-ttu-id="064b6-134">**القياسي** - لا يتناسب الاستهلاك مع أي بُعد للمنتج النهائي، والقيمة التي تم إدخالها في حقل **الكمية** هي الرقم المستخدم للمنتج النهائي.</span><span class="sxs-lookup"><span data-stu-id="064b6-134">**Standard** - The consumption is not proportional to any dimension of the finished product, and the value that is entered in the **Quantity** field is the number that is used for the finished product.</span></span>

-   <span data-ttu-id="064b6-135">**الارتفاع\*ثابت** - يتناسب الاستهلاك مع الارتفاع فقط.</span><span class="sxs-lookup"><span data-stu-id="064b6-135">**Height \* Constant** - The consumption is proportional to the height only.</span></span>

-   <span data-ttu-id="064b6-136">**الارتفاع \* العرض \* ثابت** - يتناسب الاستهلاك مع الارتفاع والعرض.</span><span class="sxs-lookup"><span data-stu-id="064b6-136">**Height \* Width \* Constant** - The consumption is proportional to the height and width.</span></span>

-   <span data-ttu-id="064b6-137">**الارتفاع \* العرض \* العمق \* ثابت** - يتناسب الاستهلاك مع الارتفاع والعرض والعمق.</span><span class="sxs-lookup"><span data-stu-id="064b6-137">**Height \* Width \* Depth \* Constant** - The consumption is proportional to the height, width, and depth.</span></span>

-   <span data-ttu-id="064b6-138">**(الارتفاع \* العرض \* العمق/الكثافة) \* ثابت** - يتناسب الاستهلاك مع الارتفاع والعرض والعمق/الكثافة.</span><span class="sxs-lookup"><span data-stu-id="064b6-138">**(Height \* Width \* Depth/Density) \* Constant** - The consumption is proportional to the height, width, and depth/density.</span></span>

<span data-ttu-id="064b6-139">تتمثل خيارات الاستهلاك المستخدمة للقياس فيما يلي:</span><span class="sxs-lookup"><span data-stu-id="064b6-139">Consumption options that are used for measurement are:</span></span>

-   <span data-ttu-id="064b6-140">**المتغير** - يتناسب عدد الوحدات في المنتج النهائي مع عدد الأصناف التي تم إنتاجها.</span><span class="sxs-lookup"><span data-stu-id="064b6-140">**Variable** - The number of units in the finished product is proportional to the number of items produced.</span></span> <span data-ttu-id="064b6-141">يتم حساب الاستهلاك المتغير بالطريقة التالية: كمية الإنتاج x الكمية (في قائمة BOM) = الاستهلاك (المتغير).</span><span class="sxs-lookup"><span data-stu-id="064b6-141">Variable consumption is calculated in the following way: Production Quantity x Quantity (in the BOM) = Consumption (variable).</span></span> <span data-ttu-id="064b6-142">يتساوى استهلاك الوحدات مع الكمية الموجودة في قائمة BOM.</span><span class="sxs-lookup"><span data-stu-id="064b6-142">The unit consumption is equal to the quantity in the BOM.</span></span>
-   <span data-ttu-id="064b6-143">**ثابت** - هذا الخيار هو كمية ثابتة مطلوبة للإنتاج، بغض النظر عن الكمية التي يتم إنتاجها.</span><span class="sxs-lookup"><span data-stu-id="064b6-143">**Constant** - This option is a fixed volume/quantity that is required for the production, regardless of quantity produced.</span></span>

<span data-ttu-id="064b6-144">تحدد **قاعدة التفريغ** كيفية استهلاك المكون.</span><span class="sxs-lookup"><span data-stu-id="064b6-144">The **Flushing principle** determines how the component is consumed.</span></span> <span data-ttu-id="064b6-145">في حالة ترك هذا الحقل فارغاً، يتم استخدام إعداد "قاعدة التفريغ" الخاص بالصنف.</span><span class="sxs-lookup"><span data-stu-id="064b6-145">If you leave this field blank, the Flushing principle setting on the item is used.</span></span> <span data-ttu-id="064b6-146">الخيارات الموجودة في هذا الحقل هي:</span><span class="sxs-lookup"><span data-stu-id="064b6-146">The options in this field are:</span></span>

-   <span data-ttu-id="064b6-147">**البدء** - يتم تمكين الاستهلاك التلقائي عندما يقوم المستخدم بتحديث أمر إنتاج لمرحلة البدء.</span><span class="sxs-lookup"><span data-stu-id="064b6-147">**Start** - Automatic consumption is enabled when the user updates a production order to the start phase.</span></span>
-   <span data-ttu-id="064b6-148">**إنهاء** - يتم تمكين الاستهلاك التلقائي عندما يقوم المستخدم بتحديث أمر إنتاج للتقرير كمرحلة منتهية.</span><span class="sxs-lookup"><span data-stu-id="064b6-148">**Finish** - Automatic consumption is enabled when the user updates a production order to the report as finished phase.</span></span>
-   <span data-ttu-id="064b6-149">**يدوي** - لا يتم تسجيل الاستهلاك تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="064b6-149">**Manual** - Consumption is not registered automatically.</span></span> <span data-ttu-id="064b6-150">ويجب إدخاله يدوياً في قائمة الانتقاء.</span><span class="sxs-lookup"><span data-stu-id="064b6-150">It must be entered manually on the picking list.</span></span>


## <a name="rounding-up-options"></a><span data-ttu-id="064b6-151">خيارات التقريب لأعلى</span><span class="sxs-lookup"><span data-stu-id="064b6-151">Rounding-up options</span></span>

<span data-ttu-id="064b6-152">تتمثل خيارات التقريب لأعلى فيما يلي:</span><span class="sxs-lookup"><span data-stu-id="064b6-152">The following are the rounding-up options:</span></span>

-   <span data-ttu-id="064b6-153">**لا** - لا يتم استخدام التقريب لأعلى.</span><span class="sxs-lookup"><span data-stu-id="064b6-153">**No** - Rounding-up is not used.</span></span>

-   <span data-ttu-id="064b6-154">**الكمية** - عند التقريب لأعلى وفقاً للكمية، يجب أن تكون الكمية مضاعفاً للكمية المعطاة.</span><span class="sxs-lookup"><span data-stu-id="064b6-154">**Quantity** - When you are rounding-up according to quantity, the quantity must be a multiple of the given quantity.</span></span>

-   <span data-ttu-id="064b6-155">**القياس** - يتم استخدام التقريب لأعلى وفقاً للقياسات عندما تأتي مادة خام في أبعاد محددة.</span><span class="sxs-lookup"><span data-stu-id="064b6-155">**Measurement** - Rounding-up according to measurements is used when a raw material comes in specific dimensions.</span></span>

-   <span data-ttu-id="064b6-156">**الاستهلاك** - عند التقريب لأعلى وفقاً للاستهلاك، يتم تقريب الاستهلاك المقدر لأعلى بحيث يكون قابلاً للقسمة على عدد الوحدات التي تأتي بها المادة الخام.</span><span class="sxs-lookup"><span data-stu-id="064b6-156">**Consumption** - When you are rounding-up according to consumption, the estimated consumption is rounded up so that it is divisible by the number of units that the raw material comes in.</span></span>


<span data-ttu-id="064b6-157">[![لقطة شاشة للقائمة المنسدلة الخاصة بالتقريب في صفحة قائمة مكونات الصنف.](../media/rounding-1.png)](../media/rounding-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="064b6-157">[![Screenshot of the Rounding drop down list on the Bills of materials page.](../media/rounding-1.png)](../media/rounding-1.png#lightbox)</span></span> 

### <a name="example"></a><span data-ttu-id="064b6-158">مثال</span><span class="sxs-lookup"><span data-stu-id="064b6-158">Example</span></span>

<span data-ttu-id="064b6-159">يتم تخزين الطلاء في المخزون في عبوات سعة 25 لتراً</span><span class="sxs-lookup"><span data-stu-id="064b6-159">Paint is stored in inventory in 25-quart cans.</span></span> <span data-ttu-id="064b6-160">وعندما يتم سحبه من المخزون، يتم السحب بزيادة عبوة سعة 25 لتراً</span><span class="sxs-lookup"><span data-stu-id="064b6-160">When it is taken from inventory, it is taken in 25-quart can increments.</span></span> <span data-ttu-id="064b6-161">وفي هذه الحالة، يحدد المستخدم التقريب للأعلى وفقاً للاستهلاك ويعين المضاعفات على 25.</span><span class="sxs-lookup"><span data-stu-id="064b6-161">In this case, the user selects rounding-up according to Consumption and sets multiples to 25.</span></span> <span data-ttu-id="064b6-162">تكون كمية الإنتاج للمنتج النهائي 20 وحدة، ويتم استخدام 2 كوارت من الطلاء لكل وحدة.</span><span class="sxs-lookup"><span data-stu-id="064b6-162">The production quantity for the finished product is 20 units, and two quarts of paint are used for each unit.</span></span> <span data-ttu-id="064b6-163">يتم حساب الاستهلاك بمعدل 20 وحدة x 2 كوارت = 40 لتراً</span><span class="sxs-lookup"><span data-stu-id="064b6-163">Consumption is calculated as 20 units x 2 quarts = 40 quarts.</span></span>

<span data-ttu-id="064b6-164">عند تقريبه إلى رقم يمثل أحد مضاعفات الرقم 25، يقرر المستخدم أن المطلوب هو 50 كوارت من الطلاء.</span><span class="sxs-lookup"><span data-stu-id="064b6-164">When rounding-up to a multiple of 25, the user determines that 50 quarts of paint are required.</span></span>
<span data-ttu-id="064b6-165">وعند التقريب لأعلى وفقاً للاستهلاك، يتم تلقائياً حساب 10 كوارت كاستهلاك زائد أو خردة.</span><span class="sxs-lookup"><span data-stu-id="064b6-165">When the user rounds up according to Consumption, excess consumption, or scrap, 10 quarts are automatically calculated.</span></span>


## <a name="measurement-conversion-factor"></a><span data-ttu-id="064b6-166">عامل تحويل القياس</span><span class="sxs-lookup"><span data-stu-id="064b6-166">Measurement conversion factor</span></span>

<span data-ttu-id="064b6-167">عوامل التحويل هي عمليات حسابية تمثل الفرق بين قياسات المنتج القياسي وقياسات مكونات BOM.</span><span class="sxs-lookup"><span data-stu-id="064b6-167">Conversion factors are mathematical calculations that represent the difference between standard product measurements and BOM component measurements.</span></span>

<span data-ttu-id="064b6-168">لحساب استهلاك المواد الخام، حدد عوامل التحويل للارتفاع والعرض والعمق والكثافة، إذا كانت هذه القيم متناسبة مع تلك التي تم تحديدها.</span><span class="sxs-lookup"><span data-stu-id="064b6-168">To calculate the consumption of raw materials, specify conversion factors for the height, width, depth, and density, if these values are proportional to those that are specified.</span></span> <span data-ttu-id="064b6-169">يمكن القيام بهذا التحديد في المواقع التالية:</span><span class="sxs-lookup"><span data-stu-id="064b6-169">This specification can be done in the following locations:</span></span>

-   <span data-ttu-id="064b6-170">في سطر BOM عند إجراء عملية حسابية</span><span class="sxs-lookup"><span data-stu-id="064b6-170">On the BOM line when a calculation is run</span></span>
-   <span data-ttu-id="064b6-171">في أمر الإنتاج عند تشغيل تقدير التكلفة</span><span class="sxs-lookup"><span data-stu-id="064b6-171">In the production order when a cost estimation is run</span></span>

<span data-ttu-id="064b6-172">تعرض الحقول الموجودة في علامة التبويب **البُعد** في الصفحة **سطر BOM** عوامل التحويل المضمنة في حساب القياس بالإضافة إلى بُعد المنتج النهائي.</span><span class="sxs-lookup"><span data-stu-id="064b6-172">Fields on the **Dimension** tab of the **BOM line** page show the conversion factors that are included in the measurement calculation together with the dimension of the finished product.</span></span>

### <a name="example-1"></a><span data-ttu-id="064b6-173">المثال 1</span><span class="sxs-lookup"><span data-stu-id="064b6-173">Example 1</span></span>

<span data-ttu-id="064b6-174">تخزن شركة ما المعادن في 3 صفائح بطول متر واحد.</span><span class="sxs-lookup"><span data-stu-id="064b6-174">A company stocks metal in 3 x 1-meter sheets.</span></span> <span data-ttu-id="064b6-175">وعند إنشاء مصباح، تتطلب قائمة BOM صفائح معدنية مقاس 1 x 0.75 متر.</span><span class="sxs-lookup"><span data-stu-id="064b6-175">When a lamp is created, the BOM requires 1 x 0.75 meters of sheet metal.</span></span> <span data-ttu-id="064b6-176">عامل التحويل في هذا المثال هو 0.333 للارتفاع و0.75 للعرض (1/3 = 0.3333 و0.75/1 = 0.75).</span><span class="sxs-lookup"><span data-stu-id="064b6-176">The conversion factor in this example is 0.333 for height and 0.75 for width (1/3 = 0.3333 and 0.75/1 = 0.75).</span></span>

<span data-ttu-id="064b6-177">تتم إضافة هذه المبالغ إلى سطور مكونات BOM.</span><span class="sxs-lookup"><span data-stu-id="064b6-177">These amounts are added to the BOM component lines.</span></span> <span data-ttu-id="064b6-178">عند حساب الاستهلاك للصنف، يتم ضرب القياسات القياسية في عوامل التحويل.</span><span class="sxs-lookup"><span data-stu-id="064b6-178">When consumption is calculated for the item, the standard measurements are multiplied by the conversion factors.</span></span> <span data-ttu-id="064b6-179">ينتج عن هذه العملية الحسابية استهلاك مكون BOM (الكمية).</span><span class="sxs-lookup"><span data-stu-id="064b6-179">This calculation causes BOM component consumption (quantity).</span></span>

### <a name="example-2"></a><span data-ttu-id="064b6-180">المثال 2</span><span class="sxs-lookup"><span data-stu-id="064b6-180">Example 2</span></span>

<span data-ttu-id="064b6-181">في شركة USMF، يتميز **حامل مكبر الصوت الأمامي المصبوغ** **لحامل مكبر الصوت الأمامي المرفق مقاس 18 X 50 بوصة** بأبعاد ارتفاع قياسية تبلغ **2** (قدم).</span><span class="sxs-lookup"><span data-stu-id="064b6-181">At the USMF company, the **stain - front speaker mount** for the **enclosure front speaker mount 18X50 inches** has a standard height dimension of **2** (feet).</span></span>
<span data-ttu-id="064b6-182">بعد مراقبة حامل مكبر الصوت، قرر فريق الإنتاج أنه بالنسبة لـ BOM 7037-1-1، فإن حامل السماعة الأمامية له بُعد ارتفاع **3** (قدم).</span><span class="sxs-lookup"><span data-stu-id="064b6-182">After monitoring the speaker mount, the production team has determined that for BOM 7037-1-1, the front speaker mount has a height dimension of **3** (feet).</span></span> <span data-ttu-id="064b6-183">ويكون عامل التحويل لمكون BOM هو 1.5 (3/2).</span><span class="sxs-lookup"><span data-stu-id="064b6-183">The conversion factor for the BOM component is 1.5 (3/2).</span></span>

<span data-ttu-id="064b6-184">وطُلب من أوسكار، مهندس العمليات، تحديث الأبعاد التي اكتشفها فريق الإنتاج في الصنف وقائمة BOM، ثم إجراء العملية الحسابية لصنف واحد ثم لـ 50 صنفاً لتحديد الفرق في الاستهلاك.</span><span class="sxs-lookup"><span data-stu-id="064b6-184">Oscar, the Process engineer, is asked to update the dimensions that were discovered by the production team on both the item and the BOM, and then run the calculation for 1 and then for 50 items to determine the difference in consumption.</span></span>
