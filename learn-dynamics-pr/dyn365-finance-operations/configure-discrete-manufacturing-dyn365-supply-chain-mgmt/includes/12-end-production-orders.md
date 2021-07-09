---
ms.openlocfilehash: bbc492274df6d582e598d4c4a72a825d7163e7b4
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073681"
---
<span data-ttu-id="8d4af-101">قبل إنهاء الإنتاج، تقوم Supply Chain Management بحساب التكاليف الفعلية للكمية التي تم إنتاجها.</span><span class="sxs-lookup"><span data-stu-id="8d4af-101">Before ending production, Supply Chain Management calculates the actual costs for the quantity that was produced.</span></span> <span data-ttu-id="8d4af-102">يتم عكس جميع التكاليف المقدرة للمواد والعمالة والنفقات العامة واستبدالها بالتكاليف الفعلية.</span><span class="sxs-lookup"><span data-stu-id="8d4af-102">All estimated costs of material, labor, and overhead are reversed and replaced with actual costs.</span></span> <span data-ttu-id="8d4af-103">وتستند هذه التكاليف إلى استهلاك المواد والوقت المحقق.</span><span class="sxs-lookup"><span data-stu-id="8d4af-103">These costs are based on realized material and time consumption.</span></span> 

<span data-ttu-id="8d4af-104">يمكن مقارنه التكاليف الفعلية بتكاليف استهلاك الوقت والمواد المقدرة التي تم حسابها عند تقدير أمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-104">You can compare actual costs to estimated material and time consumption costs that were calculated when the production order was estimated.</span></span> <span data-ttu-id="8d4af-105">يغطي حساب السعر النهائي استهلاك الأصناف والخدمات وأرباح الأصناف والعمليات.</span><span class="sxs-lookup"><span data-stu-id="8d4af-105">Final price calculation covers the consumption of items, services, item gains, and operations.</span></span>

<span data-ttu-id="8d4af-106">عند إنهاء أوامر الإنتاج، يتم حسابها بالتكلفة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-106">When production orders are ended, they are cost-accounted.</span></span> <span data-ttu-id="8d4af-107">يتم إنشاء حركة استلام بالحالة **تم الشراء** لصنف الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-107">A receipt transaction with the **Purchased** status is generated for the production item.</span></span> <span data-ttu-id="8d4af-108">تغطي هذه الحركة عمليات الاستلام للأصناف التي تم إنشاؤها والتي ضمن الحالة **تم الطلب**، والأصناف التي تم الإعلام عن انتهائها والتي ضمن الحالة **تم الاستلام** ويتم حذف حركات الاستلام التي تم إنشاؤها في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="8d4af-108">This transaction covers receipts for items that were created and have the status **Ordered**, items that were reported-as-finished and have the status **Received**, and receipt transactions that were generated earlier are deleted.</span></span> <span data-ttu-id="8d4af-109">يتم حجز الأصناف والأعمال تحت التنفيذ التي تم ترحيلها مسبقاً تلقائياً في دفتر الأستاذ ويتم ترحيل كافة دفاتر اليومية وإغلاقها.</span><span class="sxs-lookup"><span data-stu-id="8d4af-109">Previously posted items and WIP are automatically reversed in the ledger and all journals are posted and closed.</span></span>

<span data-ttu-id="8d4af-110">إذا قمت بتحديد خانة الاختيار **إنهاء المهمة**، فعند تشغيل حساب التكلفة، تتغير حالة أمر الإنتاج إلى **تم الإنهاء**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-110">If you select the **End job** check box when you run the cost calculation, the production order status changes to **Ended**.</span></span> <span data-ttu-id="8d4af-111">تمنع هذه الحالة ترحيل أية تكاليف إضافية دون قصد إلى أمر إنتاج مكتمل.</span><span class="sxs-lookup"><span data-stu-id="8d4af-111">This status prevents any additional costs from being inadvertently posted to a completed production order.</span></span>

## <a name="final-price-calculation"></a><span data-ttu-id="8d4af-112">حساب السعر النهائي</span><span class="sxs-lookup"><span data-stu-id="8d4af-112">Final price calculation</span></span>

<span data-ttu-id="8d4af-113">يغطي الحساب النهائي للسعر ما يلي:</span><span class="sxs-lookup"><span data-stu-id="8d4af-113">Final price calculation covers the following:</span></span>

-   <span data-ttu-id="8d4af-114">**استهلاك الأصناف**: يتم حساب مبلغ التكلفة لاستهلاك الأصناف على النحو التالي: *استهلاك صنف المكون \* سعر تكلفه الصنف = مبلغ التكلفة المحقق*</span><span class="sxs-lookup"><span data-stu-id="8d4af-114">**Consumption of items** - The cost amount for item consumption is calculated as: *Component item consumption \* Item's cost price = Realized cost amount*</span></span>

    - <span data-ttu-id="8d4af-115">إذا لم تكن الأصناف المستهلكة ذات حركة مفتوحة، يتم استخدام متوسط التكلفة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-115">If the consumed items are not open-transaction marked, the average cost is used.</span></span> <span data-ttu-id="8d4af-116">يتم أخذ سعر تكلفة الصنف من المخزون.</span><span class="sxs-lookup"><span data-stu-id="8d4af-116">The item's cost price is taken from inventory.</span></span> <span data-ttu-id="8d4af-117">ومع ذلك، إذا كان الصنف من الحركات المفتوحة التي تم تحديدها لحركه استلام ضمن الحالة **تم الشراء**، يتم أخذ سعر تكلفة الصنف من حركة الاستلام هذه.</span><span class="sxs-lookup"><span data-stu-id="8d4af-117">However, if the item is open-transaction selected for a receipt transaction with the **Purchased** status, the item's cost price is taken from that receipt transaction.</span></span> <span data-ttu-id="8d4af-118">بالنسبة لتكلفة استهلاك الصنف، يقوم النظام بإصدار حركة ضمن الحالة **مُباع**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-118">For costing of the item consumption, the system issues a transaction with the **Sold** status.</span></span> <span data-ttu-id="8d4af-119">يتم حذف حركة الإصدار الأصلية التي ضمن الحالة **قيد الطلب** أو **منتقاة‬‏‫**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-119">The original issue transaction with the **On order** or **Picked** status is deleted.</span></span>



    - <span data-ttu-id="8d4af-120">عندما يتعلق أمر الإنتاج بالتكاليف، تتم معالجة جميع المنتجات من نوع الصنف أو الخدمة في قائمة مكونات المواد بنفس الطريقة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-120">When the production order comes to the costing, all products with type Item or Service in the BOM are handled the same way.</span></span>

-   <span data-ttu-id="8d4af-121">**الأصناف المنتهية**: يتم حساب مبلغ التكلفة للأصناف المنتهية كالتالي: *عدد الأصناف المنتهية \* سعر تكلفه الصنف= مبلغ التكلفة المحقق*</span><span class="sxs-lookup"><span data-stu-id="8d4af-121">**Finished items** - The cost amount for finished items is calculated as: *Number of finished items \* Item's cost price = Realized cost amount*</span></span>



    - <span data-ttu-id="8d4af-122">يتم الحصول على سعر تكلفة الصنف من الصنف عند حساب التكاليف.</span><span class="sxs-lookup"><span data-stu-id="8d4af-122">The item's cost price is taken from the item when you calculate costing.</span></span> <span data-ttu-id="8d4af-123">وخلال التكلفة الخاصة بأرباح الأصناف، يتم تحديث حركة المخزون الأصلية إلى الحالة **تم الشراء** من **تم الطلب** أو **تم الاستلام**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-123">During the costing of item gains, the original inventory transaction is updated to the **Purchased** status from **Ordered** or **Received**.</span></span>

## <a name="consumption-of-operations"></a><span data-ttu-id="8d4af-124">استهلاك العمليات</span><span class="sxs-lookup"><span data-stu-id="8d4af-124">Consumption of operations</span></span>

<span data-ttu-id="8d4af-125">يتضمن استهلاك العملية أوقات التشغيل ووقت الإعداد والكمية المعالجة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-125">Operation consumption includes run times, setup time, and processed quantity.</span></span> <span data-ttu-id="8d4af-126">يتم حساب مبلغ التكلفة لاستهلاك وقت التشغيل ووقت الإعداد والكمية المعالجة على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="8d4af-126">The cost amount for the consumption of run time, setup time, and processed quantity is calculated as follows:</span></span>

<span data-ttu-id="8d4af-127">*(الوقت المستهلك المبلغ عنه \* سعر التكلفة لكل ساعة المبلغ عنه) + (الكمية التي تمت معالجتها \* سعر تكلفة الكمية المبلغ عنه)*</span><span class="sxs-lookup"><span data-stu-id="8d4af-127">*(Reported time consumption \* Reported hourly cost price) + (Reported processed quantity \* Reported quantity cost price) = Realized cost amount*</span></span>

<span data-ttu-id="8d4af-128">عند تحديد الانتقاء التلقائي للموارد، يتم استرداد سعر التكلفة تلقائياً من فئة وقت التشغيل وفئة الإعداد وفئة الكمية المعالجة المذكورة في المسار.</span><span class="sxs-lookup"><span data-stu-id="8d4af-128">When you select automatic picking of resources, the cost price is retrieved automatically from the run time category, setup category, and processed quantity category that are stated on the route.</span></span>

<span data-ttu-id="8d4af-129">إذا تم الإبلاغ عن عدد الأصناف المنتهية للعمليات باستخدام دفتر يومية التقرير كمنتهٍ، فإن هذه الأصناف هي تلك المستخدمة في التكاليف.</span><span class="sxs-lookup"><span data-stu-id="8d4af-129">If the number of finished items has been reported for the operations by using the Report as finished journal, these items are the ones used in costing.</span></span>

## <a name="end-page"></a><span data-ttu-id="8d4af-130">إنهاء الصفحة</span><span class="sxs-lookup"><span data-stu-id="8d4af-130">End page</span></span>

<span data-ttu-id="8d4af-131">استخدم **إنهاء الصفحة** لإنهاء أوامر الإنتاج وتعيين الحالة "تم الإنهاء" لها.</span><span class="sxs-lookup"><span data-stu-id="8d4af-131">Use the **End** page to finish production orders and assign them the status of Ended.</span></span> <span data-ttu-id="8d4af-132">بمجرد أن يتم الإنهاء، لا يمكن تحديثها أو إعادتها إلى حالة سابقة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-132">As soon as they are ended, they cannot be updated or reverted to an earlier status.</span></span>

<span data-ttu-id="8d4af-133">الحقول الرئيسة في صفحة **الإنهاء** هي:</span><span class="sxs-lookup"><span data-stu-id="8d4af-133">The main fields in the **End** page are:</span></span>

-   <span data-ttu-id="8d4af-134">**الإنتاج**: أدخل رقم أمر الإنتاج الذي ترغب في إنهائه.</span><span class="sxs-lookup"><span data-stu-id="8d4af-134">**Production** - Enter the production order number that you want to end.</span></span> <span data-ttu-id="8d4af-135">يمكنك إدخال أي رقم أمر إنتاج موجود واستخدام الزر **تحديد** لتصفية رقم أمر إنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-135">You can enter any existing production order number and use the **Select** button to filter for a production order number.</span></span> <span data-ttu-id="8d4af-136">إذا قمت بالوصول إلى الصفحة من صفحة **أوامر الإنتاج**، يتم ملء الحقل تلقائياً بأمر الإنتاج المحدد.</span><span class="sxs-lookup"><span data-stu-id="8d4af-136">If you access the page from the **Production orders** page, the field is automatically filled in with the selected production order.</span></span>

-   <span data-ttu-id="8d4af-137">**التاريخ**: تحديد التاريخ المطلوب فيه ترحيل الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-137">**Date** - Specify the date to post the production.</span></span> <span data-ttu-id="8d4af-138">ويكون تاريخ النظام هو التاريخ الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="8d4af-138">The system date is the default.</span></span>

-   <span data-ttu-id="8d4af-139">**الإبلاغ كمنتهٍ**: حدد هذا الحقل للإبلاغ عن انتهاء أمر الإنتاج قبل إنهائه.</span><span class="sxs-lookup"><span data-stu-id="8d4af-139">**Report as finished** - Select this to report the production order as finished before you end it.</span></span>

-   <span data-ttu-id="8d4af-140">**نهج الخردة**: يستخدم لتحديد كيفية ترحيل استهلاك الصنف والمورد لكمية الخردة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-140">**Scrap method** - Specify how to post item and resource consumption for scrap quantity.</span></span> <span data-ttu-id="8d4af-141">إذا كانت الكمية التي تم تشغيلها أكبر من الكمية التي تم الإبلاغ عنها كمنتهية، فهناك خردة.</span><span class="sxs-lookup"><span data-stu-id="8d4af-141">If the quantity that is started is larger than the quantity that is reported as finished, there is scrap.</span></span>

<span data-ttu-id="8d4af-142">**التحكم في الإنتاج > أوامر الإنتاج > كافة أوامر الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-142">**Production control > Production orders > All production orders**.</span></span> <span data-ttu-id="8d4af-143">البحث عن أمر ضمن الحالة "الإبلاغ كمنتهٍ"، ثم تحديد علامة التبويب **أمر إنتاج** > **مجموعه المعالجة > إنهاء**</span><span class="sxs-lookup"><span data-stu-id="8d4af-143">Find an order with the status of Reported as finished, then select **Production order** tab > **Process group > End**</span></span>

![لقطة شاشة للقائمة المنسدلة لنهج الخردة على صفحة الإنهاء.](../media/scrap-method.png) 


<span data-ttu-id="8d4af-145">يتم حساب معدل الخردة على النحو التالي: *(الكمية التي تم استخدامها للبدء - الكمية التي تم الإبلاغ عنها كمنتهية)/(الكمية > الكمية المبدوءة) \* 100*</span><span class="sxs-lookup"><span data-stu-id="8d4af-145">Scrap is calculated as: *(Quantity started - Quantity reported as finished) / (Quantity > started) \* 100*</span></span> 

<span data-ttu-id="8d4af-146">تكون الخيارات كما يلي:</span><span class="sxs-lookup"><span data-stu-id="8d4af-146">The options are as follows:</span></span>

-   <span data-ttu-id="8d4af-147">**حساب الخردة**: يتم ترحيل الخردة المحسوبة في حساب دفتر الأستاذ إلى حساب الخردة المحدد في الحقل **حساب الخردة**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-147">**Scrap account** - The calculated scrap in the ledger account is posted to the scrap account that is specified in the **Scrap account** field.</span></span>

-   <span data-ttu-id="8d4af-148">**التخصيص**: يتم تخصيص الخردة التي تم حسابها كتكلفة مضافة إلى كمية الأصناف المنتهية التي تم الإبلاغ عنها كمنتهية.</span><span class="sxs-lookup"><span data-stu-id="8d4af-148">**Allocation** - The calculated scrap is allocated as an added cost to the quantity of finished items that are reported as finished.</span></span>

<span data-ttu-id="8d4af-149">يتم تعيين الحالة **مناهٍ** لأمر الإنتاج ولا يمكن تحديثه بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="8d4af-149">The production order is assigned the **Ended** status and can no longer be updated.</span></span> <span data-ttu-id="8d4af-150">يتم حساب تكلفة أمر الإنتاج، ويتم إنشاء حركة استلام ضمن الحالة **تم الشراء** للصنف الذي تم إنتاجه.</span><span class="sxs-lookup"><span data-stu-id="8d4af-150">The production order is cost accounted, and a receipt transaction with the **Purchased** status is generated for the produced item.</span></span> <span data-ttu-id="8d4af-151">يتم إغلاق كافة دفاتر اليومية المقترنة بأمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-151">All journals that are associated with the production order are closed.</span></span>

## <a name="analyzing-variances-for-a-completed-production-order"></a><span data-ttu-id="8d4af-152">تحليل نسب الفرق لأمر إنتاج مكتمل</span><span class="sxs-lookup"><span data-stu-id="8d4af-152">Analyzing variances for a completed production order</span></span>

<span data-ttu-id="8d4af-153">يتم حساب نسب الفرق في الإنتاج بعد إنهاء أمر إنتاج لصنف تكلفة قياسي.</span><span class="sxs-lookup"><span data-stu-id="8d4af-153">Production variances are calculated after you end a production order for a standard cost item.</span></span> <span data-ttu-id="8d4af-154">وتعكس الفروق مقارنة بين أنشطة الإنتاج المبلغ عنها وحساب التكلفة المعيارية لصنف الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-154">The variances reflect a comparison between the reported production activities and the standard cost calculation for the production item.</span></span>

<span data-ttu-id="8d4af-155">ولا تقدم نسب الفرق مقارنة بالتكاليف المقدرة لأمر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8d4af-155">The variances do not provide a comparison to the production order's estimated costs.</span></span> <span data-ttu-id="8d4af-156">تتضمن أنشطة الإنتاج التي تم الإبلاغ عنها استهلاك المواد وعمليات التوجيه والتكاليف غير المباشرة المقترنة والكمية التي تم الإبلاغ عنها كمنتهية.</span><span class="sxs-lookup"><span data-stu-id="8d4af-156">The reported production activities include consumption of material and routing operations, associated indirect costs, and the reported as finished quantity.</span></span>

<span data-ttu-id="8d4af-157">ويتم حساب أنواع نسب الفرق التالية:</span><span class="sxs-lookup"><span data-stu-id="8d4af-157">The following types of variances are calculated:</span></span>

-   <span data-ttu-id="8d4af-158">حجم الدفعة</span><span class="sxs-lookup"><span data-stu-id="8d4af-158">Lot size</span></span>

-   <span data-ttu-id="8d4af-159">كمية الإنتاج</span><span class="sxs-lookup"><span data-stu-id="8d4af-159">Production quantity</span></span>

-   <span data-ttu-id="8d4af-160">سعر الإنتاج</span><span class="sxs-lookup"><span data-stu-id="8d4af-160">Production price</span></span>

-   <span data-ttu-id="8d4af-161">استبدال الإنتاج</span><span class="sxs-lookup"><span data-stu-id="8d4af-161">Production substitution</span></span>

<span data-ttu-id="8d4af-162">توفر معلومات التباين التفصيلية أداة واحدة لمساعدة المستخدمين على فهم مصدر كافة نسب الفروقات.</span><span class="sxs-lookup"><span data-stu-id="8d4af-162">The detailed variance information provides one tool to help users understand the source of each variance.</span></span> <span data-ttu-id="8d4af-163">لتوقع نسب الفرق قبل إنهاء أمر الإنتاج، قم بتحليل المعلومات التفصيلية التي يتم توفيرها في تقرير **تقديرات التكلفة والتكاليف**.</span><span class="sxs-lookup"><span data-stu-id="8d4af-163">To anticipate variances prior to ending a production order, analyze the detailed information that is provided in the **Cost estimates and costings** report.</span></span>
