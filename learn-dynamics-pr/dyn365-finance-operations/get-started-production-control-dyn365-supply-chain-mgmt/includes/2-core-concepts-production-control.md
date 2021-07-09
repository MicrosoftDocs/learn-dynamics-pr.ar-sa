---
ms.openlocfilehash: 9cbeec125ba8208db280805f16e7aa99b105956a
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073734"
---
<span data-ttu-id="81f5d-101">على الرغم من تفرد عمليات التصنيع لكل شركة، تبعاً لطبيعة بيئة التشغيل، فإن العناصر التصورية الأساسية المستخدمة في وحدة التحكم في الإنتاج متشابهة في كثير من الأحيان.</span><span class="sxs-lookup"><span data-stu-id="81f5d-101">Although each company’s manufacturing processes are unique, depending on the nature of the production environment, the core conceptual elements that are used in the Production control module are frequently similar.</span></span>

<span data-ttu-id="81f5d-102">المفاهيم الأساسية في وحدة التحكم في الإنتاج هي كما يلي:</span><span class="sxs-lookup"><span data-stu-id="81f5d-102">The core concepts in the Production control module are as follows:</span></span>

- <span data-ttu-id="81f5d-103">التقويمات</span><span class="sxs-lookup"><span data-stu-id="81f5d-103">Calendars</span></span>
- <span data-ttu-id="81f5d-104">الموارد</span><span class="sxs-lookup"><span data-stu-id="81f5d-104">Resources</span></span>
- <span data-ttu-id="81f5d-105">أنواع الموارد</span><span class="sxs-lookup"><span data-stu-id="81f5d-105">Resource types</span></span>
- <span data-ttu-id="81f5d-106">قدرات الموارد</span><span class="sxs-lookup"><span data-stu-id="81f5d-106">Resource capabilities</span></span>
- <span data-ttu-id="81f5d-107">قائمة مكونات الصنف (BOM)</span><span class="sxs-lookup"><span data-stu-id="81f5d-107">Bill of materials (BOM)</span></span>
- <span data-ttu-id="81f5d-108">المسارات والعمليات</span><span class="sxs-lookup"><span data-stu-id="81f5d-108">Routes and operations</span></span>
- <span data-ttu-id="81f5d-109">المعادلة</span><span class="sxs-lookup"><span data-stu-id="81f5d-109">Formula</span></span>
- <span data-ttu-id="81f5d-110">تدفقات القيم</span><span class="sxs-lookup"><span data-stu-id="81f5d-110">Value streams</span></span>
- <span data-ttu-id="81f5d-111">نماذج تدفق الإنتاج</span><span class="sxs-lookup"><span data-stu-id="81f5d-111">Production flow models</span></span>
- <span data-ttu-id="81f5d-112">وحدات الإنتاج</span><span class="sxs-lookup"><span data-stu-id="81f5d-112">Production units</span></span>
- <span data-ttu-id="81f5d-113">مجموعات الإنتاج</span><span class="sxs-lookup"><span data-stu-id="81f5d-113">Production groups</span></span>
- <span data-ttu-id="81f5d-114">مجموعات الإنتاج</span><span class="sxs-lookup"><span data-stu-id="81f5d-114">Production pools</span></span>
- <span data-ttu-id="81f5d-115">مفاتيح التوزيع</span><span class="sxs-lookup"><span data-stu-id="81f5d-115">Allocation keys</span></span>
- <span data-ttu-id="81f5d-116">وظيفة كانبان</span><span class="sxs-lookup"><span data-stu-id="81f5d-116">Kanban functionality</span></span>

## <a name="resources"></a><span data-ttu-id="81f5d-117">الموارد</span><span class="sxs-lookup"><span data-stu-id="81f5d-117">Resources</span></span> 

<span data-ttu-id="81f5d-118">الموارد هي إجمالي موارد العمل الخاصة بالشركة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-118">Resources are the company’s total working resources.</span></span> <span data-ttu-id="81f5d-119">يمكن أن تكون هذه الأصناف أي شيء يتم استخدامه لإنشاء أو إنتاج أو تسليم بضاعة و/أو خدمة، بالإضافة إلى المواد التي يتم استهلاكها في العملية.</span><span class="sxs-lookup"><span data-stu-id="81f5d-119">They can be anything that is used for the creation, production, or delivery of a good and/or service over and beyond the materials consumed in the process.</span></span> <span data-ttu-id="81f5d-120">يمكن أن تكون الموارد أنواعاً مختلفة، بما في ذلك الأجهزة أو الأدوات أو الأشخاص أو الموردين أو المواقع.</span><span class="sxs-lookup"><span data-stu-id="81f5d-120">Resources can be of different types, including machines, tools, people, vendors, or locations.</span></span>

<span data-ttu-id="81f5d-121">**إدارة المؤسسة > الموارد > الموارد**.</span><span class="sxs-lookup"><span data-stu-id="81f5d-121">**Organization administration > Resources > Resources**</span></span>
 
<span data-ttu-id="81f5d-122">[![لقطه شاشة لعلامة تبويب "العمليات" الموجودة في صفحة "الموارد".](../media/resources-1.png)](../media/resources-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="81f5d-122">[![Screenshot of the Operations tab on the Resources page.](../media/resources-1.png)](../media/resources-1.png#lightbox)</span></span>


## <a name="resource-types"></a><span data-ttu-id="81f5d-123">أنواع الموارد</span><span class="sxs-lookup"><span data-stu-id="81f5d-123">Resource types</span></span> 

<span data-ttu-id="81f5d-124">يتم إنشاء الموارد في الوحدة النمطية لإدارة المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-124">Resources are created in the Organization administration module.</span></span> <span data-ttu-id="81f5d-125">ويتم استخدامها في الإنتاج إلى جانب التقويم لإدارة القدرة الإجمالية لمعدات الشركة ومواردها.</span><span class="sxs-lookup"><span data-stu-id="81f5d-125">They are used in production along with the calendar to manage the overall capacity of a company's equipment and resources.</span></span> <span data-ttu-id="81f5d-126">يمكن أن يرتبط كل مورد بمجموعة موارد، ويمكن أن يوجد مورد واحد أو عدة موارد في أي مجموعة موارد معينة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-126">Each resource can be associated with a resource group, and one or multiple resources can exist in any given resource group.</span></span>

<span data-ttu-id="81f5d-127">تتوفر أنواع الموارد التالية في إدارة سلسلة التوريد:</span><span class="sxs-lookup"><span data-stu-id="81f5d-127">The following resource types are available in Supply Chain Management:</span></span>

- <span data-ttu-id="81f5d-128">**المورد** - يمكن استخدام هذا النوع عند إجراء عملية (أو مهمة) بواسطة مورد خارجي أو مقاول من الباطن.</span><span class="sxs-lookup"><span data-stu-id="81f5d-128">**Vendor** - Use this type when an operation (or task) is performed by an outside resource or subcontractor.</span></span> <span data-ttu-id="81f5d-129">يمكن ربط رقم المورد بهذا النوع من الموارد للمساعدة في الجدولة والتعقب.</span><span class="sxs-lookup"><span data-stu-id="81f5d-129">A vendor number can be associated with this kind of resource to help with scheduling and tracking.</span></span>
- <span data-ttu-id="81f5d-130">**الموارد البشرية** - يمكن استخدام هذا النوع لتحديد الوقت الذي يقوم فيه الأفراد أو مجموعة من الموظفين بإجراء عملية ما.</span><span class="sxs-lookup"><span data-stu-id="81f5d-130">**Human resources** - Use this type to define when personnel or a group of employees conduct an operation.</span></span>
- <span data-ttu-id="81f5d-131">**الجهاز** - يمكن استخدام هذا النوع لربط جهاز فردي أو مجموعة من الأجهزة بمورد.</span><span class="sxs-lookup"><span data-stu-id="81f5d-131">**Machine** - Use this type to tie an individual machine or group of machines with a resource.</span></span> <span data-ttu-id="81f5d-132">وهو نوع المورد الأكثر استخداماً.</span><span class="sxs-lookup"><span data-stu-id="81f5d-132">It is the most frequently used type of resource.</span></span>
- <span data-ttu-id="81f5d-133">**الأداة** - يمكن استخدام هذا النوع للتحكم في حجوزات الأداة وجدولتها.</span><span class="sxs-lookup"><span data-stu-id="81f5d-133">**Tool** - Use this type to control and schedule the reservations of a tool.</span></span> <span data-ttu-id="81f5d-134">استخدم هذا النوع فقط عندما تكون القدرة محدودة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-134">Use this type only when capacity is limited.</span></span>
- <span data-ttu-id="81f5d-135">**الموقع** - يمكن استخدام هذا النوع للتحكم في حجوزات موقع محدد وجدولته.</span><span class="sxs-lookup"><span data-stu-id="81f5d-135">**Location** - Use this type to control and schedule the reservations of a specific location.</span></span>
- <span data-ttu-id="81f5d-136">**أداة الإنشاء** - بناء أو بنية ثابتة مطلوبة لتنفيذ نشاط.</span><span class="sxs-lookup"><span data-stu-id="81f5d-136">**Facility** - A building or fixed structure that is required to perform an activity.</span></span>

<span data-ttu-id="81f5d-137">**إدارة المؤسسة > الموارد > جديد**</span><span class="sxs-lookup"><span data-stu-id="81f5d-137">**Organization administration > Resources > New**</span></span>

![لقطة شاشة للقائمة المنسدلة "النوع" في صفحة "موارد" جديدة.](../media/resources-types.png)



## <a name="resource-capabilities"></a><span data-ttu-id="81f5d-139">قدرات الموارد</span><span class="sxs-lookup"><span data-stu-id="81f5d-139">Resource capabilities</span></span> 

<span data-ttu-id="81f5d-140">تم تعيين القدرات إلى مورد عملية.</span><span class="sxs-lookup"><span data-stu-id="81f5d-140">Capabilities are assigned to an operation’s resource.</span></span> <span data-ttu-id="81f5d-141">يمكن تعيين أكثر من قدرة واحدة لأحد الموارد، ويمكن تعيين قدرة لأكثر من مورد واحد.</span><span class="sxs-lookup"><span data-stu-id="81f5d-141">A resource can have more than one capability assigned to it, and a capability can be assigned to more than one resource.</span></span> <span data-ttu-id="81f5d-142">يمكن أيضاً تعيين القدرات للموارد على أساس مؤقت عن طريق تحديد تاريخ بدء وتاريخ انتهاء لتعيين القدرة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-142">Capabilities can also be assigned to resources on a temporary basis by defining a start date and expiration date on the capability assignment.</span></span>
 
<span data-ttu-id="81f5d-143">**إدارة المؤسسة > الموارد > قدرات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="81f5d-143">**Organizational administration > Resources > Resource capabilities**</span></span>

<span data-ttu-id="81f5d-144">[![لقطة شاشة لصفحة "قدرات الموارد".](../media/resource-capability.png)](../media/resource-capability.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="81f5d-144">[![Screenshot of the Resource capabilities page.](../media/resource-capability.png)](../media/resource-capability.png#lightbox)</span></span>


<span data-ttu-id="81f5d-145">القدرات التي انتهت صلاحيتها في أحد الموارد ستمنع جدولة المورد للإنتاج إذا تطلب الإنتاج تلك القدرة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-145">Capabilities that have expired on a resource will prevent the resource from being scheduled for production if the production requires that capability.</span></span> <span data-ttu-id="81f5d-146">يمكن تجديد القدرة التي انتهت صلاحيتها فيما بعد.</span><span class="sxs-lookup"><span data-stu-id="81f5d-146">A capability that has expired can be subsequently renewed.</span></span>

<span data-ttu-id="81f5d-147">عند تحديد متطلبات الموارد لمسار الإنتاج، يمكنك تحديد قدرة واحدة أو أكثر من القدرات كمتطلبات.</span><span class="sxs-lookup"><span data-stu-id="81f5d-147">When defining resource requirements for a production route, you can specify one or more capabilities as requirements.</span></span> <span data-ttu-id="81f5d-148">عند تنفيذ جدولة الإنتاج، فإن القدرات المحددة في متطلبات الموارد في مسار العمليات تتوافق مع القدرات التي تم تحديدها للموارد.</span><span class="sxs-lookup"><span data-stu-id="81f5d-148">When production scheduling is performed, the capabilities that are defined in the resource requirements on the route operation are matched with the capabilities that are defined for the resources.</span></span> 

<span data-ttu-id="81f5d-149">يتم بعد ذلك تحديد الموارد ذات القدرات التي تستوفي المتطلبات.</span><span class="sxs-lookup"><span data-stu-id="81f5d-149">The resources with capabilities that satisfy the requirements are then selected.</span></span> <span data-ttu-id="81f5d-150">عند تحديد قدرات لموارد مختلفة، يجب عليك إعداد القدرات بحيث يتم إعداد سرعات معالجة مختلفة بشكل كبير كقدرات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-150">When defining capabilities for different resources, you should set up capabilities so that significantly different processing speeds are set up as different capabilities.</span></span>

## <a name="bill-of-materials-bom"></a><span data-ttu-id="81f5d-151">قائمة مكونات الصنف (BOM)</span><span class="sxs-lookup"><span data-stu-id="81f5d-151">Bill of materials (BOM)</span></span> 

<span data-ttu-id="81f5d-152">تعد قائمة مكونات الصنف أحد أهم المستندات في شركة التصنيع.</span><span class="sxs-lookup"><span data-stu-id="81f5d-152">The BOM is one of the most important documents in a manufacturing company.</span></span> <span data-ttu-id="81f5d-153">قبل أن تتمكن الشركة من إنتاج منتج، يجب أن تعرف المكونات التي سيتم تضمينها وعدد هذه المكونات المطلوبة لصنع المنتج النهائي.</span><span class="sxs-lookup"><span data-stu-id="81f5d-153">Before a company can produce a product, it must know what components are to be included and how many of these components are needed to make the end product.</span></span> <span data-ttu-id="81f5d-154">تحتوي قائمة مكونات الصنف على كافة المكونات أو الأجزاء أو المواد الخام المطلوبة لصنع منتج نهائي واحد.</span><span class="sxs-lookup"><span data-stu-id="81f5d-154">The BOM contains all the ingredients, components, parts, or raw materials that are required to make one finished product.</span></span>

<span data-ttu-id="81f5d-155">**إدارة معلومات المنتج > قوائم مكونات الأصناف والمعادلات > قوائم مكونات الأصناف**</span><span class="sxs-lookup"><span data-stu-id="81f5d-155">**Product information management > Bill of materials and formulas > Bill of materials**</span></span>
 
<span data-ttu-id="81f5d-156">[![لقطة شاشة لصفحة قوائم مكونات الأصناف.](../media/bom-1.png)](../media/bom-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="81f5d-156">[![Screenshot of the Bills of materials page.](../media/bom-1.png)](../media/bom-1.png#lightbox)</span></span>



## <a name="routes-and-operations"></a><span data-ttu-id="81f5d-157">المسارات والعمليات</span><span class="sxs-lookup"><span data-stu-id="81f5d-157">Routes and operations</span></span> 

<span data-ttu-id="81f5d-158">تحدد المسارات خطوات العملية اللازمة لإنتاج منتج نهائي.</span><span class="sxs-lookup"><span data-stu-id="81f5d-158">The route determines the process steps that are needed to produce a finished product.</span></span>
 
<span data-ttu-id="81f5d-159">تحدد قائمة مكونات الصنف المواد المطلوبة، ويحدد المورد مكان إنتاج الصنف، ويحدد المسار تسلسل الأحداث لإنشاء المنتج النهائي.</span><span class="sxs-lookup"><span data-stu-id="81f5d-159">The BOM defines the materials required, the resource defines where the item is produced, and the route determines the sequence of events to build the finished product.</span></span> <span data-ttu-id="81f5d-160">تعد العمليات المهام الخاصة أو عمليات العمل التي يتم وضعها معاً بالمسار لإنتاج منتج معين.</span><span class="sxs-lookup"><span data-stu-id="81f5d-160">Operations are the tasks or work processes that are put together with a route to produce a specific product.</span></span> <span data-ttu-id="81f5d-161">يتم إقران كل مهمة بحصة زمنية لإكمال المهمة الفردية.</span><span class="sxs-lookup"><span data-stu-id="81f5d-161">Each task is associated with a time allotment to complete the individual task.</span></span>

<span data-ttu-id="81f5d-162">**التحكم بالإنتاج > العمليات > كافة المسارات**</span><span class="sxs-lookup"><span data-stu-id="81f5d-162">**Production control > Operations > All routes**</span></span>
 
<span data-ttu-id="81f5d-163">[![لقطة شاشة لمثال على مسار لخزانة سماعات.](../media/routes-1.png)](../media/routes-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="81f5d-163">[![Screenshot of an example of a route for a speaker cabinet.](../media/routes-1.png)](../media/routes-1.png#lightbox)</span></span>


## <a name="define-optional-settings"></a><span data-ttu-id="81f5d-164">تحديد الإعدادات الاختيارية</span><span class="sxs-lookup"><span data-stu-id="81f5d-164">Define optional settings</span></span> 

<span data-ttu-id="81f5d-165">يمكن للشركات أيضاً إعداد إعدادات اختيارية تتحكم في عملية الإنتاج إذا كانت ذات صلة ببيئات الإنتاج الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="81f5d-165">Companies can also set up optional settings that control the production process if these are relevant to their production environments.</span></span> 

<span data-ttu-id="81f5d-166">الإعدادات الاختيارية هي كالتالي:</span><span class="sxs-lookup"><span data-stu-id="81f5d-166">The optional settings are as follows:</span></span>

- <span data-ttu-id="81f5d-167">**مجموعات الإنتاج** - يمكن إعداد مجموعات الإنتاج لإنشاء علاقات بين أمر الإنتاج وحسابات دفتر الأستاذ.</span><span class="sxs-lookup"><span data-stu-id="81f5d-167">**Production groups** - Set up production groups to establish relationships between the production order and ledger accounts.</span></span> <span data-ttu-id="81f5d-168">سيتم استخدام حسابات دفتر الأستاذ لترحيل الأوامر أو تجميعها لإعداد التقارير.</span><span class="sxs-lookup"><span data-stu-id="81f5d-168">The ledger accounts will be used to post or to group orders for reporting.</span></span>
- <span data-ttu-id="81f5d-169">**أوعيه الإنتاج** - يمكن إنشاء أوعية الإنتاج لتجميع أوامر الإنتاج لمعالجة أوامر الإنتاج العاجلة أو لحذف مجموعات الأوامر وترحيلها.</span><span class="sxs-lookup"><span data-stu-id="81f5d-169">**Production pools** - Create production pools to group production orders for processing urgent production orders or for deleting and posting groups of orders.</span></span>
- <span data-ttu-id="81f5d-170">**الخصائص** - يمكن تحديد الخصائص لإنشاء سمات خاصة يمكنك يمكنك تعيينها لمواردك لاستخدامها ضمن عملية الجدولة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-170">**Properties** - Define properties to create special attributes that you can assign to your resources for use in the scheduling process.</span></span> <span data-ttu-id="81f5d-171">يتم ربط هذه السمات بقالب وقت العمل.</span><span class="sxs-lookup"><span data-stu-id="81f5d-171">These attributes are connected to the working time template.</span></span>
- <span data-ttu-id="81f5d-172">**قدرات الموارد** - يمكن إنشاء قدرات الموارد عند الحاجة إلى الموارد لتنفيذ عمليات مختلفة في المسار، والتي يمكن التعبير عنها كمجموعة قدرات للموارد.</span><span class="sxs-lookup"><span data-stu-id="81f5d-172">**Resource capabilities** - Create resource capabilities in case resources need to perform the various operations in the route that can be expressed as the set of resource capabilities.</span></span> <span data-ttu-id="81f5d-173">ويسمح هذا بتأجيل توزيع الموارد حتى تتم جدولة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="81f5d-173">This allows the allocation of resources to be deferred until production is scheduled.</span></span>

## <a name="production-control-integration-with-other-modules-in-supply-chain-management"></a><span data-ttu-id="81f5d-174">تكامل التحكم بالإنتاج مع وحدات نمطية أخرى في Supply Chain Management</span><span class="sxs-lookup"><span data-stu-id="81f5d-174">Production control integration with other modules in Supply Chain Management</span></span> 

<span data-ttu-id="81f5d-175">تتكامل الوحدة النمطية للتحكم بالإنتاج مع الوحدات النمطية التالية في Supply Chain Management:</span><span class="sxs-lookup"><span data-stu-id="81f5d-175">The Production control module is integrated with the following modules in Supply Chain Management:</span></span>

- <span data-ttu-id="81f5d-176">إدارة المخزون</span><span class="sxs-lookup"><span data-stu-id="81f5d-176">Inventory management</span></span>
- <span data-ttu-id="81f5d-177">إدارة المستودعات</span><span class="sxs-lookup"><span data-stu-id="81f5d-177">Warehouse management</span></span>
- <span data-ttu-id="81f5d-178">دفتر الأستاذ العام</span><span class="sxs-lookup"><span data-stu-id="81f5d-178">General ledger</span></span>
- <span data-ttu-id="81f5d-179">التخطيط الرئيسي</span><span class="sxs-lookup"><span data-stu-id="81f5d-179">Master planning</span></span>
- <span data-ttu-id="81f5d-180">إدارة المؤسسة</span><span class="sxs-lookup"><span data-stu-id="81f5d-180">Organization administration</span></span>
- <span data-ttu-id="81f5d-181">محاسبة المشروع</span><span class="sxs-lookup"><span data-stu-id="81f5d-181">Project accounting</span></span>
- <span data-ttu-id="81f5d-182">إدارة معلومات المنتج</span><span class="sxs-lookup"><span data-stu-id="81f5d-182">Product information management</span></span>

<span data-ttu-id="81f5d-183">ويدعم هذا التكامل تدفق المعلومات المطلوبة لإكمال تصنيع الصنف المنتهي.</span><span class="sxs-lookup"><span data-stu-id="81f5d-183">This integration supports the information flow that is needed to complete the manufacturing of a finished item.</span></span> <span data-ttu-id="81f5d-184">يتبع إنتاج الأصناف دورة حياة إنتاجية متسلسلة.</span><span class="sxs-lookup"><span data-stu-id="81f5d-184">The production of items follows a sequential production life cycle.</span></span> <span data-ttu-id="81f5d-185">تعكس دورة الحياة الخطوات الفعلية التي يتم اتخاذها لتصنيع أحد الأصناف.</span><span class="sxs-lookup"><span data-stu-id="81f5d-185">The life cycle reflects the actual steps that are taken to manufacture an item.</span></span> <span data-ttu-id="81f5d-186">وتبدأ بإنشاء أمر إنتاج، وتنتهي بصنف منتهٍ ومصنع جاهز للعميل.</span><span class="sxs-lookup"><span data-stu-id="81f5d-186">It begins with the creation of a production order and ends with a finished, manufactured item that is ready for the customer.</span></span> 

<span data-ttu-id="81f5d-187">تتطلب كل خطوة في دورة الحياة أنواعاً مختلفة من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="81f5d-187">Each step in the life cycle requires different kinds of information.</span></span> <span data-ttu-id="81f5d-188">عندما تكتمل خطوة في دوره الحياة، يقوم أمر الإنتاج بالإشارة إلى ذلك من خلال تغيير في حالة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="81f5d-188">When a step in the life cycle is completed, the production order signals this by a change in the production status.</span></span> <span data-ttu-id="81f5d-189">إذا تم تخطي خطوة أو أكثر من الخطوات الإلزامية (أو التحديثات)، فسيتم تنفيذ الخطوات تلقائياً قبل نقل أمر الإنتاج إلى الخطوة التالية.</span><span class="sxs-lookup"><span data-stu-id="81f5d-189">If one or more of the mandatory steps (or updates) are skipped, the steps are performed automatically before the production order is moved to the next step.</span></span> 

## <a name="production-life-cycle-and-statuses"></a><span data-ttu-id="81f5d-190">دوره حياة الإنتاج والحالات</span><span class="sxs-lookup"><span data-stu-id="81f5d-190">Production life cycle and statuses</span></span> 

<span data-ttu-id="81f5d-191">يتم تعيين حالة لأمر الإنتاج تعكس مكانها في دورة حياة الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="81f5d-191">The production order is assigned a status that reflects where it is in the production life cycle.</span></span> <span data-ttu-id="81f5d-192">وتكون حالة الأوامر كما يلي:</span><span class="sxs-lookup"><span data-stu-id="81f5d-192">The status of the orders is as follows:</span></span>

- <span data-ttu-id="81f5d-193">‏إنشاء</span><span class="sxs-lookup"><span data-stu-id="81f5d-193">Create</span></span>
- <span data-ttu-id="81f5d-194">تقدير</span><span class="sxs-lookup"><span data-stu-id="81f5d-194">Estimate</span></span>
- <span data-ttu-id="81f5d-195">جدولة</span><span class="sxs-lookup"><span data-stu-id="81f5d-195">Schedule</span></span>
- <span data-ttu-id="81f5d-196">تم الإصدار</span><span class="sxs-lookup"><span data-stu-id="81f5d-196">Released</span></span>
- <span data-ttu-id="81f5d-197">البدء</span><span class="sxs-lookup"><span data-stu-id="81f5d-197">Start</span></span>
- <span data-ttu-id="81f5d-198">الإبلاغ كمنتهٍ</span><span class="sxs-lookup"><span data-stu-id="81f5d-198">Report as finished</span></span>
- <span data-ttu-id="81f5d-199">الإنهاء</span><span class="sxs-lookup"><span data-stu-id="81f5d-199">End</span></span>

