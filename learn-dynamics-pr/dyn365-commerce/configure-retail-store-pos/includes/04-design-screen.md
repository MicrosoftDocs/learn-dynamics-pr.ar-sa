---
ms.openlocfilehash: a4ade90a422468ded95e7649226bc89d6666e293
ms.sourcegitcommit: 87bfbce5cff1a2ceba28af60632730a16c68acd9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/21/2021
ms.locfileid: "6070418"
---
<span data-ttu-id="4f645-101">تكون تخطيطات شاشة MPOS وCPOS في نقطة البيع قابلة للتكوين لكثير من المتطلبات.</span><span class="sxs-lookup"><span data-stu-id="4f645-101">The MPOS and CPOS screen layouts in the POS are configurable for many requirements.</span></span> <span data-ttu-id="4f645-102">ويتم تكوين تخطيطات الشاشة على مستوى المخزن ولكن يمكن تجاوزها على مستوى السجل والمستخدمين، إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="4f645-102">Screen layouts are configured at the store level but can be overridden at the register and user level, if needed.</span></span> <span data-ttu-id="4f645-103">تتيح لك هذه الميزة تكوين السجلات مرة واحدة، ولكنها لا تزال تسمح بتخطيط جديد لتخطيط خط محدد أو لمدير أو مستخدم متمرس يطوف بين المتاجر.</span><span class="sxs-lookup"><span data-stu-id="4f645-103">This feature lets you configure registers once, but still allows a new layout for a line buster-specific layout or for a manager or power user that floats between stores.</span></span> 

<span data-ttu-id="4f645-104">المكونات الرئيسية لتخطيطات نقطة البيع في **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع >نقطة البيع > تخطيطات الشاشة** هي:</span><span class="sxs-lookup"><span data-stu-id="4f645-104">Key components of POS screen layouts in **Retail and Commerce > Channel setup > POS Setup > POS > Screen layouts** are:</span></span>

- <span data-ttu-id="4f645-105">**أحجام التخطيط**</span><span class="sxs-lookup"><span data-stu-id="4f645-105">**Layout Sizes**</span></span>
- <span data-ttu-id="4f645-106">**أشرطة الأوامر**</span><span class="sxs-lookup"><span data-stu-id="4f645-106">**Button grids**</span></span>
- <span data-ttu-id="4f645-107">**الصور**</span><span class="sxs-lookup"><span data-stu-id="4f645-107">**Images**</span></span>

![لقطة لصفحة تخطيطات شاشة Dynamics 365 Commerce.](../media/screen-layouts-ss.jpg)

<span data-ttu-id="4f645-109">تحتوي مكون **تخطيطات الشاشة** على السجلات الرئيسية المرفقة بالمخازن والسجلات والمستخدمين.</span><span class="sxs-lookup"><span data-stu-id="4f645-109">The **Screen layouts** component contains the main records that are attached to the stores, registers, and users.</span></span> <span data-ttu-id="4f645-110">تحدد هذه التخطيطات دقة شاشات الأجهزة المختلفة، لكل منها أشرطة الأوامر الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="4f645-110">These layouts define the various device screen resolutions, each having its own button grids assigned to it.</span></span> <span data-ttu-id="4f645-111">كل دقة شاشة لها تخطيط يتم تعريفه من خلال **مصمم التخطيط** ويمكن تعيينها إما بحجم كامل أو تخطيط مدمج.</span><span class="sxs-lookup"><span data-stu-id="4f645-111">Each screen resolution has a layout that is defined through the **Layout designer** and can be designated as either a full sized or a compact layout.</span></span> <span data-ttu-id="4f645-112">تسمح لك التخطيطات الكاملة بتصميم شاشة عرض للشاشات الكبيرة أو الكمبيوتر اللوحي، في حين أن التخطيط المدمج هو للأجهزة الصغيرة مثل الهواتف وله خيارات تكوين محدودة.</span><span class="sxs-lookup"><span data-stu-id="4f645-112">Full layouts allow you to design a display for large monitors or tablets, while a compact layout is for smaller devices like phones and has limited configuration options.</span></span> <span data-ttu-id="4f645-113">يتم دعم التخطيطات الأفقية أو العمودية.</span><span class="sxs-lookup"><span data-stu-id="4f645-113">Landscape or portrait layouts are supported.</span></span> 

## <a name="button-grids"></a><span data-ttu-id="4f645-114">أشرطة الأوامر</span><span class="sxs-lookup"><span data-stu-id="4f645-114">Button grids</span></span>
<span data-ttu-id="4f645-115">المكون **أشرطة الأوامر** هو مجموعة من عمليات نقطة البيع التي يتم تعيينها لزر يمكن أن يكون لها صور متراكبة.</span><span class="sxs-lookup"><span data-stu-id="4f645-115">The **Button grids** component is a collection of POS operations that are assigned to a button that can have an overlaid image.</span></span> <span data-ttu-id="4f645-116">اعتماداً على المهمة، مثل تحديد فئة منتج أو صورة، يمكن للزر تنفيذ إجراء ما مباشرة.</span><span class="sxs-lookup"><span data-stu-id="4f645-116">Depending on the task, such as specifying a product category or image, the button can directly perform an action.</span></span> 

<span data-ttu-id="4f645-117">على سبيل المثال، يمكن لزر في شريط أوامر توجيه المستخدم إلى فئة من الأصناف، أو السماح للمستخدم بإضافة صنف إلى الحركة دون الحاجة إلى التنقل من خلال الطرق التقليدية لإضافة الصنف.</span><span class="sxs-lookup"><span data-stu-id="4f645-117">For example, a button in the button grid can direct the user to a category of items, or allow the user to add an item to the transaction without having to navigate through the traditional methods to add the item.</span></span> 

<span data-ttu-id="4f645-118">تعرض لقطة الشاشة التالية صفحة **عمليات نقطة البيع**، الموجودة في **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع > نقطة البيع**، والتي تسرد العمليات التي يمكن تخصيصها للأزرار.</span><span class="sxs-lookup"><span data-stu-id="4f645-118">The following screenshot shows the **POS operations** page, located in **Retail and Commerce > Channel setup > POS Setup > POS**, which lists the operations that can be assigned to buttons.</span></span>  
 
<span data-ttu-id="4f645-119">[ ![لقطة شاشة لصفحة عمليات نقطة البيع في Dynamics 365 Commerce.](../media/pos-operations-ss.jpg) ](../media/pos-operations-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4f645-119">[ ![Screenshot of the Dynamics 365 Commerce  POS operations page.](../media/pos-operations-ss.jpg) ](../media/pos-operations-ss.jpg#lightbox)</span></span>

<span data-ttu-id="4f645-120">يتم تصميم أشرطه الأوامر كمكونات منفصلة، بحيث يمكن إنشاؤها مرة واحدة ثم استخدامها عبر تخطيطات متعددة.</span><span class="sxs-lookup"><span data-stu-id="4f645-120">Button grids are designed as separate components, so they can be created once and then used across multiple layouts.</span></span> <span data-ttu-id="4f645-121">يمكن تكوين الأزرار الموجودة في شريط الأوامر للحصول على أحجام وألوان متنوعة لتوفير التركيز وتمييز الوظائف بين الأزرار (على سبيل المثال، الأزرق = بطاقات الوقت، والأخضر = المدفوعات، وهكذا).</span><span class="sxs-lookup"><span data-stu-id="4f645-121">The buttons in the button grid can be configured to have varying sizes and colors to provide emphasis and the differentiation of functions between buttons (for example, blue = timecards, green = payments, and more).</span></span> <span data-ttu-id="4f645-122">تكون أشرطة الأوامر قابلة للتكوين من قبل المستخدمين دون الحاجة إلى مطور.</span><span class="sxs-lookup"><span data-stu-id="4f645-122">Button grids are configurable by users without the need for a developer.</span></span> 

<span data-ttu-id="4f645-123">توضح صفحة **أشرطة الأوامر** في **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع >نقطة البيع** خيار **المصمم** وإجراءات **جدول شريط الأوامر**.</span><span class="sxs-lookup"><span data-stu-id="4f645-123">The **Button grids** page in **Retail and Commerce > Channel setup > POS Setup > POS** shows the **Designer** option and **Button grid table** actions.</span></span> 
  
<span data-ttu-id="4f645-124">[ ![لقطة شاشة لصفحة أشرطة أوامر Dynamics 365 Commerce.](../media/button-grids-ss.jpg) ](../media/button-grids-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4f645-124">[ ![Screenshot of the Dynamics 365 Commerce Button grids page.](../media/button-grids-ss.jpg) ](../media/button-grids-ss.jpg#lightbox)</span></span>

<span data-ttu-id="4f645-125">تعرض لقطة الشاشة التالية من **مصمم أشرطة الأوامر**، الموجود في **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع > نقطة البيع > أشرطة الأوامر** مثالاً على كيفية وضع الأزرار لشريط الأوامر السابق، بما في ذلك النص والصور بدلاً من النص.</span><span class="sxs-lookup"><span data-stu-id="4f645-125">The following screenshot of the **Button grid designer**, which is located in **Retail and Commerce > Channel setup > POS Setup > POS > Button grids**, shows an example of how the buttons can be placed for the previous button grid, including text and images in lieu of text.</span></span>

 
![لقطة شاشة لمصمم أشرطة أوامر Dynamics 365 Commerce.](../media/button-grid-designer-ss.jpg)


## <a name="layout-zones"></a><span data-ttu-id="4f645-127">مناطق التخطيط</span><span class="sxs-lookup"><span data-stu-id="4f645-127">Layout zones</span></span>
<span data-ttu-id="4f645-128">لكل تخطيط شاشة منطقتان للتخطيط يجب تصميمهما:</span><span class="sxs-lookup"><span data-stu-id="4f645-128">For each screen layout are two layout zones that must be designed:</span></span> 

- <span data-ttu-id="4f645-129">شاشة **الترحيب**</span><span class="sxs-lookup"><span data-stu-id="4f645-129">**Welcome** screen</span></span>
- <span data-ttu-id="4f645-130">شاشة **الحركة**</span><span class="sxs-lookup"><span data-stu-id="4f645-130">**Transaction** screen</span></span> 

<span data-ttu-id="4f645-131">في مصمم التخطيط، يجب تعريف أشرطه الأوامر التي سيتم استخدامها في كل شاشة كما هو مبين في صفحة **تخطيطات الشاشة** التالية في **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع >نقطة البيع**.</span><span class="sxs-lookup"><span data-stu-id="4f645-131">In the layout designer, button grids that will be used in each screen must be defined as shown in the following **Screen layouts** page in **Retail and Commerce > Channel setup > POS Setup > POS**.</span></span>

![لقطة شاشة لمناطق تخطيط Dynamics 365 Commerce.](../media/layout-zones-ss.jpg) 

### <a name="welcome-screen"></a><span data-ttu-id="4f645-133">شاشة الترحيب</span><span class="sxs-lookup"><span data-stu-id="4f645-133">Welcome screen</span></span>
<span data-ttu-id="4f645-134">تعرض لقطة الشاشة التالية مثالاً على شاشة **الترحيب**، والتي تم تكوينها في مصمم التخطيط، وأشرطه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="4f645-134">The following screenshot shows an example of the **Welcome** screen, which is configured in the layout designer, and the button grids.</span></span> <span data-ttu-id="4f645-135">يمكنك الحصول على أكبر عدد من مجموعات شريط الأوامر حسب الحاجة وعادة ما تكون مصممة حسب المنطقة الوظيفي، مثل **بداية اليوم**، و **نهاية اليوم**، و **المخزون**، و **الوردية والدرج**، والمزيد.</span><span class="sxs-lookup"><span data-stu-id="4f645-135">You can have as many button grid groups as needed, and they are typically designed by functional area, such as **Start of day**, **End of day**, **Inventory**, **Shift and Drawer**, and more.</span></span> 

<span data-ttu-id="4f645-136">تُظهر لقطة الشاشة التالية شاشة **الترحيب** من متجر **HOUSTON** لنقطة البيع السحابية‬، السجل **HOUSTON-14**.</span><span class="sxs-lookup"><span data-stu-id="4f645-136">The following screenshot shows the **Welcome** screen from the Cloud POS **HOUSTON** store **HOUSTON-14** register.</span></span> <span data-ttu-id="4f645-137">تتوافق الأرقام التالية مع الأرقام الموجودة في لقطة الشاشة التي تعرض هذه المكونات:</span><span class="sxs-lookup"><span data-stu-id="4f645-137">The following numbers correspond with the numbers in the screenshot that shows these components:</span></span> 
 
1.  <span data-ttu-id="4f645-138">أشرطة الأوامر</span><span class="sxs-lookup"><span data-stu-id="4f645-138">Button grids</span></span>
2.  <span data-ttu-id="4f645-139">صور شاشة الترحيب</span><span class="sxs-lookup"><span data-stu-id="4f645-139">Welcome screen images</span></span> 

<span data-ttu-id="4f645-140">[ ![لقطه شاشه لشاشه الترحيب في متجر Houston.](../media/houston-ssm.jpg) ](../media/houston-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4f645-140">[ ![Screenshot of the welcome screen of the Houston store.](../media/houston-ssm.jpg) ](../media/houston-ssm.jpg#lightbox)</span></span>

### <a name="transaction-screen"></a><span data-ttu-id="4f645-141">شاشة الحركة</span><span class="sxs-lookup"><span data-stu-id="4f645-141">Transaction screen</span></span>
<span data-ttu-id="4f645-142">المثال التالي هو شاشة **حركة** نقطة البيع مع العناصر المرقمة التالية الموضحة في الارتباط مع مصمم تخطيط نقطة البيع:</span><span class="sxs-lookup"><span data-stu-id="4f645-142">The subsequent example is of the POS **Transaction** screen with the following numbered elements shown in correlation to the POS layout designer:</span></span> 

1.  <span data-ttu-id="4f645-143">الإيصال</span><span class="sxs-lookup"><span data-stu-id="4f645-143">Receipt</span></span>
2.  <span data-ttu-id="4f645-144">لوحة الإجماليات</span><span class="sxs-lookup"><span data-stu-id="4f645-144">Totals panel</span></span>
3.  <span data-ttu-id="4f645-145">بطاقة العميل</span><span class="sxs-lookup"><span data-stu-id="4f645-145">Customer card</span></span>
4.  <span data-ttu-id="4f645-146">لوحة الأرقام</span><span class="sxs-lookup"><span data-stu-id="4f645-146">Number pad</span></span>
5.  <span data-ttu-id="4f645-147">أشرطة الأوامر</span><span class="sxs-lookup"><span data-stu-id="4f645-147">Button grids</span></span>
6.  <span data-ttu-id="4f645-148">عنصر التحكم في علامة التبويب</span><span class="sxs-lookup"><span data-stu-id="4f645-148">Tab control</span></span>

 
<span data-ttu-id="4f645-149">[ ![لقطة شاشة لشاشة حركة نقطة البيع في Dynamics 365 Commerce.](../media/houston-transaction-ssm.jpg) ](../media/houston-transaction-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4f645-149">[ ![Screenshot of the Dynamics 365 Commerce POS Transaction screen.](../media/houston-transaction-ssm.jpg) ](../media/houston-transaction-ssm.jpg#lightbox)</span></span>

## <a name="layout-designer"></a><span data-ttu-id="4f645-150">مصمم التخطيط</span><span class="sxs-lookup"><span data-stu-id="4f645-150">Layout designer</span></span>
<span data-ttu-id="4f645-151">يتطلب مصمم تخطيط Microsoft Dynamics Commerce Designer لتثبيته على الجهاز.</span><span class="sxs-lookup"><span data-stu-id="4f645-151">The layout designer requires the Microsoft Dynamics Commerce Designer to be installed on a machine.</span></span> <span data-ttu-id="4f645-152">لقطة الشاشة التالية هي مثال على تخطيط شاشة حركة نقطة البيع كما هو موضح في مصمم التخطيط في **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع > نقطة البيع > تخطيطات الشاشة >مصمم التخطيط**.</span><span class="sxs-lookup"><span data-stu-id="4f645-152">The following screenshot is an example of a POS transaction screen layout as seen in the layout designer in **Retail and Commerce > Channel setup > POS Setup > POS > Screen layouts > Layout designer**.</span></span> 

<span data-ttu-id="4f645-153">[ ![لقطة شاشة لتخطيط شاشة حركة نقطة البيع كما هو موضح في مصمم التخطيط. ](../media/layout-designer-ssm.jpg) ](../media/layout-designer-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4f645-153">[ ![Screenshot of a POS transaction screen layout as seen in the layout designer. ](../media/layout-designer-ssm.jpg) ](../media/layout-designer-ssm.jpg#lightbox)</span></span>

<span data-ttu-id="4f645-154">الأرقام الواردة في لقطة الشاشة ترتبط بالأقسام التالية:</span><span class="sxs-lookup"><span data-stu-id="4f645-154">The numbers in the screenshot correlate to the following sections:</span></span>

1.  <span data-ttu-id="4f645-155">الإيصال</span><span class="sxs-lookup"><span data-stu-id="4f645-155">Receipt</span></span>
2.  <span data-ttu-id="4f645-156">بطاقة العميل</span><span class="sxs-lookup"><span data-stu-id="4f645-156">Customer card</span></span>
3.  <span data-ttu-id="4f645-157">لوحة الإجماليات</span><span class="sxs-lookup"><span data-stu-id="4f645-157">Totals panel</span></span>
4.  <span data-ttu-id="4f645-158">أشرطة الأوامر</span><span class="sxs-lookup"><span data-stu-id="4f645-158">Button grids</span></span>
5.  <span data-ttu-id="4f645-159">عنصر التحكم في علامة التبويب</span><span class="sxs-lookup"><span data-stu-id="4f645-159">Tab control</span></span>


<span data-ttu-id="4f645-160">عندما تقوم بتطوير تخطيطات الشاشة وأشرطة الأوامر، يمكن استخدام أمثلة Contoso الموجودة في مجموعة بيانات العروض التوضيحية لـ Commerce ومساعدتك في الحصول على الإلهام.</span><span class="sxs-lookup"><span data-stu-id="4f645-160">When you are developing screen layouts and button grids, the existing Contoso examples in the Commerce demo data set can be used as a template and to help you gain inspiration.</span></span> 

## <a name="language-support"></a><span data-ttu-id="4f645-161">الدعم اللغوي</span><span class="sxs-lookup"><span data-stu-id="4f645-161">Language support</span></span>
<span data-ttu-id="4f645-162">تدعم Commerce التوزيعات الدولية، وبالتالي تدعم لغات متعددة.</span><span class="sxs-lookup"><span data-stu-id="4f645-162">Commerce supports international deployments and therefore supports multiple languages.</span></span> <span data-ttu-id="4f645-163">يتم تكوين اللغات على المتجر والعامل.</span><span class="sxs-lookup"><span data-stu-id="4f645-163">Languages are configured on the store and the worker.</span></span> 

<span data-ttu-id="4f645-164">ويتم استخدام لغة المتجر التي تم تكوينها لجميع عناصر البيانات، مثل أسماء العملاء والمنتجات والسمات وطرق الدفع والإيصالات، والمزيد.</span><span class="sxs-lookup"><span data-stu-id="4f645-164">The store’s configured language is used for all data items such as customer names, products and attributes, payment methods, receipts, and more.</span></span> 

<span data-ttu-id="4f645-165">سيتم استخدام لغة العامل بشكل افتراضي من المتجر، ولكن إذا تم تجاوزها في تكوين العامل، فسيتم استخدامها لترجمة العناصر غير التابعة للبيانات، مثل التسميات والقوائم واللوائح.</span><span class="sxs-lookup"><span data-stu-id="4f645-165">The worker’s language will default from the store, but if overridden on the worker’s configuration, it will be used to translate non-data elements such as labels, menus, and lists.</span></span> <span data-ttu-id="4f645-166">يعتبر النص الموجود على أشرطة الأوامر بمثابة بيانات، لذلك إذا كان النص موجوداً على الأزرار، فقد يحتاج شريط الأوامر إلى أن يتم نسخه لكل لغة مدعومة.</span><span class="sxs-lookup"><span data-stu-id="4f645-166">The text on the button grids is considered as data, so if text exists on buttons, the button grid might need to be copied for each language that is supported.</span></span> 

## <a name="notifications"></a><span data-ttu-id="4f645-167">الإعلامات</span><span class="sxs-lookup"><span data-stu-id="4f645-167">Notifications</span></span>

<span data-ttu-id="4f645-168">قد تكون المواقف التي قد تحدث عند إرسال إخطار إلى عامل في متجر مفيدة.</span><span class="sxs-lookup"><span data-stu-id="4f645-168">Situations might occur when sending a notification to a worker in a store would be helpful.</span></span> 

<span data-ttu-id="4f645-169">على سبيل المثال، المتجر "أ" لديه بضع عمليات استلام اليوم.</span><span class="sxs-lookup"><span data-stu-id="4f645-169">For example, Store A has a few pickups for the day.</span></span> <span data-ttu-id="4f645-170">فإذا كانت نقطة البيع تشير إلى عدد مرات عمليات الاستلام المجدولة لليوم في المتجر، يمكن للعامل جمعها قبل افتتاح المتجر.</span><span class="sxs-lookup"><span data-stu-id="4f645-170">If the POS indicates how many store pickups are scheduled for the day, the worker could collect them before the store opens.</span></span> <span data-ttu-id="4f645-171">وبدلاً من الاضطرار إلى الانتقال إلى صفحة لتحديد ما إذا كانت عمليات الاستلام قد تمت جدولتها، فإن العامل يتلقى بدلاً من ذلك إخطاراً على زر **نقطة البيع** يشير إلى الحاجة إلى اتخاذ إجراءات، الأمر الذي من شأنه أن يؤدي إلى تسهيل هذه الإجراءات بسرعة.</span><span class="sxs-lookup"><span data-stu-id="4f645-171">Rather than having to navigate to a page to determine if pickups were scheduled, the worker would instead receive a notification on the **POS** button indicating that actions were needed, which would result in quick facilitation of those actions.</span></span> 

<span data-ttu-id="4f645-172">يساعد إطار عمل الإخطار في نقطة البيع من خلال السماح لتجار التجزئة بتكوين الإخطارات القائمة على الأدوار.</span><span class="sxs-lookup"><span data-stu-id="4f645-172">The notification framework in POS helps by letting retailers configure role-based notifications.</span></span> 

<span data-ttu-id="4f645-173">على سبيل المثال، قد لا تحتاج تحويلات الانتقاء سوى أن يتم إكمالها من قبل مديري المتاجر.</span><span class="sxs-lookup"><span data-stu-id="4f645-173">For example, picking transfers might only need to be completed by store managers.</span></span> <span data-ttu-id="4f645-174">لتجنب تكوين كل مدير متجر بهذه الوظيفة، من الأسهل تكوينه مرة واحدة ومن ثم تطبيقه على جميع المديرين.</span><span class="sxs-lookup"><span data-stu-id="4f645-174">To avoid configuring each store manager with this functionality, it's easier to configure it once and then have it applied to all managers.</span></span> 

<span data-ttu-id="4f645-175">يتم تكوين **الإخطارات** على صفحة **مجموعات أذونات نقطة البيع** ضمن **البيع بالتجزئة والتجارة > الموظفون**، كما هو موضح في لقطة الشاشة التالية.</span><span class="sxs-lookup"><span data-stu-id="4f645-175">**Notifications** are configured on the **POS Permission groups** page under **Retail and Commerce > Employees**, as shown in the following screenshot.</span></span> 
 
![لقطة شاشة لصفحة مجموعات أذونان نقطة البيع في Dynamics 365 Commerce.](../media/pos-permission-groups-ssm.jpg) 

<span data-ttu-id="4f645-177">لتكوين إجراءات الإخطارات، يكون لدى صفحة **عمليات نقطة البيع** حقل **تمكين الإخطارات**.</span><span class="sxs-lookup"><span data-stu-id="4f645-177">To configure actions for notifications, the **POS Operations** page has an **Enable notifications** field.</span></span> <span data-ttu-id="4f645-178">في ملف التعريف الوظيفي، يمكن تعيين **فترة الإخطار** لإملاء عدد مرات إرسال الإخطار إلى المخازن.</span><span class="sxs-lookup"><span data-stu-id="4f645-178">On the functionality profile, the **Notification interval** can be set to dictate how often the notifications are pushed to the stores.</span></span> <span data-ttu-id="4f645-179">يمكن أن تسمح الأزرار التي تم تكوينها في أحد أشرطة الأوامر بمؤشرات مباشرة عند تلقي إعلاماً، مثل الحاجة إلى سحب الأصناف من الدور الأرضي للمتجر ليتم شحنها.</span><span class="sxs-lookup"><span data-stu-id="4f645-179">The buttons that are configured in a button grid can allow for live indicators when a notification is received, such as the need to pull items from the store floor for shipping.</span></span> 

<span data-ttu-id="4f645-180">تعرض لقطة الشاشة التالية مثالاً لإعلام خاص بعملية **تنفيذ الأمر** كما هو موضح من نقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="4f645-180">The following screenshot shows an example of a notification for the **Order fulfillment** operation as seen from the POS.</span></span> 

 
![لقطة شاشة لعملية تنفيذ الأمر كما هو موضح من نقطة البيع.](../media/order-fulfillment-ssm.jpg)  


