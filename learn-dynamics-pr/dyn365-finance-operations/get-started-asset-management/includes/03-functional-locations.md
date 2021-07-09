---
ms.openlocfilehash: 15413464d050f61b815d120740e26da6389ad2aa
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072278"
---
<span data-ttu-id="2c2a9-101">تصف الأقسام التالية المكونات الرئيسية لإدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-101">The following sections describe the key components of Asset Management.</span></span> 

## <a name="functional-locations"></a><span data-ttu-id="2c2a9-102">مواقع العمل</span><span class="sxs-lookup"><span data-stu-id="2c2a9-102">Functional locations</span></span>
<span data-ttu-id="2c2a9-103">تُستخدم مواقع العمل لتعقب الأصول الفعلية ومواقعها.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-103">Functional locations are used to track physical assets and their locations.</span></span> <span data-ttu-id="2c2a9-104">يمكن أن تتضمن أمثلة المواقع المصانع والمستودعات والساحات ومباني المكاتب.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-104">Examples of locations can include plants, warehouses, yards, and office buildings.</span></span> 

- <span data-ttu-id="2c2a9-105">ويتم ترتيبها بشكل هرمي، ويمكن أن تحتوي المواقع على مواقع فرعية.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-105">They are structured hierarchically, and locations can have sub locations.</span></span> 
- <span data-ttu-id="2c2a9-106">لا يمكن تغيير بنية مواقع العمل بعد إنشائها.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-106">The structure of functional locations cannot be changed after they have been created.</span></span> <span data-ttu-id="2c2a9-107">بمعنى آخر، لا يمكن نقل المواقع.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-107">In other words, locations can’t move.</span></span> 
- <span data-ttu-id="2c2a9-108">تعتمد كيفية إنشاء التدرج الهرمي لمواقع العمل علي البنية التنظيمية للشركة وإعداداتها التفضيلية.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-108">How you build your hierarchy of functional locations depends on your company's organizational structure and preferences.</span></span>

<span data-ttu-id="2c2a9-109">يُعد الشكل التالي مثالاً على موقع عمل يستند إلى موقع.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-109">The following figure is an example of a functional location based on a site.</span></span>

![مخطط لمثال على موقع عمل يستند إلى موقع.](../media/functional-location-review-c.png)
 
<span data-ttu-id="2c2a9-111">ويتضمن هذا المثال شركة "مزرعة مونسون للمخللات والمعلبات".</span><span class="sxs-lookup"><span data-stu-id="2c2a9-111">This example features the Munson's Pickles and Preserves Farm company.</span></span> <span data-ttu-id="2c2a9-112">هذه العينة هي مصنع صلصة (بعنوان الموقع أ) وهو موقع عمل يتم فيه استخدام الأصول المثبتة في موقع العمل هذا لإعداد الصلصة.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-112">This sample is a salsa plant (titled Site A) and is a functional location where assets that are installed at this functional location are used to make salsa.</span></span> 

<span data-ttu-id="2c2a9-113">ينشئ خط الإنتاج 01، وهو موقع عمل آخر، تسميات للحاويات ويرفقها بالحاويات باستخدام الماكينات (الأصول).</span><span class="sxs-lookup"><span data-stu-id="2c2a9-113">Production Line 01, another functional location, creates the labels for the jars and attaches them to the jars by using machinery (assets).</span></span> 

<span data-ttu-id="2c2a9-114">خط الإنتاج 02، موقع العمل، هو مكان إعداد الصلصة في مراكز العمل المتنوعة.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-114">Production line 02, functional location, is where they are making the salsa at the various work centers.</span></span> <span data-ttu-id="2c2a9-115">وهذه المراكز أيضاً هي مواقع عمل تستخدم الأصول التالية:</span><span class="sxs-lookup"><span data-stu-id="2c2a9-115">These centers, too, are functional locations that use the following assets:</span></span>

- <span data-ttu-id="2c2a9-116">مركز العمل 02-أ يحضر مكونات الصلصة.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-116">Work center 02-A prepares the ingredients for the salsa.</span></span>
- <span data-ttu-id="2c2a9-117">مركز العمل 02-ب يخلط المكونات ويضيف التوابل معاً.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-117">Work center 02-B mixes the ingredients and adds spices together.</span></span>
- <span data-ttu-id="2c2a9-118">يتم طهي الصلصة في مركز عمل موقع العمل 02-ط.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-118">Cooking the salsa occurs at the functional location Work center 02-C.</span></span> 
- <span data-ttu-id="2c2a9-119">مكان التعبئة 02-ت هو المكان الذي يتم فيه تعبئة الحاويات التي تمت تسميتها ليتم تسليمها.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-119">Packing 02-P is where the labeled jars are packed for delivery.</span></span>

<span data-ttu-id="2c2a9-120">تلخص القائمة التالية مواقع العمل:</span><span class="sxs-lookup"><span data-stu-id="2c2a9-120">The following list summarizes functional locations:</span></span>
 
- <span data-ttu-id="2c2a9-121">مواقع العمل هي الأماكن التي يتم فيها "تثبيت" الأصول أو وضعها.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-121">Functional locations are the places where assets are “installed” or located.</span></span>
- <span data-ttu-id="2c2a9-122">يمكن إنشاء مواقع العمل بشكل هرمي لتشمل المواقع الفرعية.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-122">Functional locations can be established hierarchically to include sub locations.</span></span>
- <span data-ttu-id="2c2a9-123">ويمكن أن يكون للمواقع الفرعية مواقع فرعية.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-123">Sub locations can have sub locations.</span></span>
- <span data-ttu-id="2c2a9-124">الأصول هي المعدات المستخدمة مثل الحزام الناقل، وماكينات طهي الصلصة، وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-124">Assets are the equipment that is used such as the conveyer belt, machinery to cook the salsa, and so on.</span></span>

<span data-ttu-id="2c2a9-125">يوضح المثال التالي موقع عمل يستند إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-125">The following example shows a functional location based on a customer.</span></span>

![مخطط لمثال على موقع عمل يستند إلى عميل.](../media/functional-location-by-customer-c.png)
 
<span data-ttu-id="2c2a9-127">يوضح هذا المثال موقع عمل حيث يكون مكتب الشركة هو العميل أ. وضمن العميل أ، تمثل المكاتب المواقع.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-127">This example shows a functional location where a corporate office is Customer A. Within Customer A, offices represent locations.</span></span> <span data-ttu-id="2c2a9-128">في هذا المثال، يمكن أن يكون المكتب 01 والمكتب 02 مكتباً أو منطقة عمل.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-128">In this example, Office 01 and Office 02 could be a desk or work area.</span></span> <span data-ttu-id="2c2a9-129">يعد المكتب 02 منطقة عمل تتضمن الطابعات والأصول المثبتة.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-129">Office 02 is a work area with printers and assets installed.</span></span> 

## <a name="assets"></a><span data-ttu-id="2c2a9-130">الأصول</span><span class="sxs-lookup"><span data-stu-id="2c2a9-130">Assets</span></span>
<span data-ttu-id="2c2a9-131">الأصول هي المعدات والماكينات الفعلية، مثل الأحزمة الناقلة والرافعات الشوكية والأجزاء والأدوات المستخدمة لدعم الأصول المادية وصيانتها.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-131">Assets are the physical equipment and machinery, such as conveyer belts, forklifts, and the parts and tools that are used to support and maintain the physical asset.</span></span> <span data-ttu-id="2c2a9-132">تصف القائمة التالية المعلومات الأساسية حول الأصول:</span><span class="sxs-lookup"><span data-stu-id="2c2a9-132">The following list describes key information about assets:</span></span>

- <span data-ttu-id="2c2a9-133">يمكن تنظيم الأصول في هيكل هرمي أو يمكن تنظيمها بواسطة مواقع العمل.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-133">Assets can be organized in a hierarchical structure or they can be organized by functional locations.</span></span>
- <span data-ttu-id="2c2a9-134">يمكن تثبيت الأصول في مواقع العمل، وإذا لزم الأمر، يمكن نقلها أو تثبيتها على مواقع عمل أخرى.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-134">Assets can be installed on functional locations and, if needed, can be moved to or installed on other functional locations.</span></span> <span data-ttu-id="2c2a9-135">باستخدام المثال من الصورة السابقة، توجد الطابعة M601-02A، وهي أحد الأصول، في موقع عمل الشركة أ وفي المكتب 02 ويمكن نقلها إلى موقع مختلف، مثل الشركة أ ثم نقلها إلى المكتب 01.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-135">By using the example from the preceding image, the printer M601-02A, which is an asset, is located at the functional location of Company A and in Office 02 and can be moved to a different location, such as Company A and then moved to Office 01.</span></span>
- <span data-ttu-id="2c2a9-136">يمكن أن تحتوي الأصول على أصول فرعية، مثل قطع غيار الأصل.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-136">Assets can have sub assets, such as spare parts for the asset.</span></span> 
- <span data-ttu-id="2c2a9-137">تكاليف الأصول تتبع دائماً موقع الأصل.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-137">Asset costs always follow the location of the asset.</span></span>
    - <span data-ttu-id="2c2a9-138">إذا قمت بتثبيت أصل على موقع عمل جديد، فسيستخدم الأصل تلقائياً الأبعاد المالية المرتبطة بموقع العمل الجديد.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-138">If you install an asset on a new functional location, the asset automatically uses the financial dimensions that are related to the new functional location.</span></span> 
    - <span data-ttu-id="2c2a9-139">تضمن هذه العملية ارتباط تكاليف الأصول دائماً بموقع العمل الذي تم تثبيت الأصل عليه حالياً.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-139">This process ensures that asset costs are always related to the functional location that the asset is currently installed on.</span></span> 
    - <span data-ttu-id="2c2a9-140">تساعد هذه المعالجة التلقائية للأبعاد المالية على ضمان التعقب الكامل للتكاليف عندما تقوم شركتك بالتحكم في المشروع وإعداد التقارير حول مواقع العمل.</span><span class="sxs-lookup"><span data-stu-id="2c2a9-140">This automatic handling of financial dimensions helps guarantee complete tracking of costs when your company does project controlling and reporting on functional locations.</span></span>

