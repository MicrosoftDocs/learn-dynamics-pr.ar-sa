---
ms.openlocfilehash: fe332db3034e40d8117c83066b6e3cb7daadf63e
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073778"
---
<span data-ttu-id="0226e-101">تتكوّن قائمة مكونات الصنف (BOM) أحادية المستوى من مكونات تابعة بشكل مباشر تُعد ضرورية لصناعة المنتج.</span><span class="sxs-lookup"><span data-stu-id="0226e-101">A single-level BOM consists of the immediately subordinate components that are necessary to build the product.</span></span> <span data-ttu-id="0226e-102">إنها لا تحتوي على "مكونات المكونات".</span><span class="sxs-lookup"><span data-stu-id="0226e-102">It does not contain the "components of the components."</span></span>

<span data-ttu-id="0226e-103">عندما تحتوي قائمة مكونات الصنف (BOM) على قائمة مكونات صنف أخرى كمكون لها، فإنها تُعرف باسم قائمة مكونات صنف (BOM) متعددة المستويات، حيث يُشار إلى قائمة مكونات الصنف (BOM) الفرعية على أنها المستوى الأول ويُشار إلى مكوناتها على أنها المستوى الثاني.</span><span class="sxs-lookup"><span data-stu-id="0226e-103">When a BOM contains another BOM as its component, it is known as a multilevel BOM, where the sub-BOM is referred to as level one and its components as level two.</span></span> <span data-ttu-id="0226e-104">بإمكان قوائم مكونات الصنف (BOM) أن تتكوّن من العدد المطلوب من المستويات، بحسب نوع المنتج الجاري إنتاجه.</span><span class="sxs-lookup"><span data-stu-id="0226e-104">BOMs can consist of as many levels as necessary, depending on the type of product being produced.</span></span>

<span data-ttu-id="0226e-105">**إدارة معلومات المنتج > قوائم مكونات الصنف والمعادلات > قائمة مكونات الصنف >** (حدد المنتج) **> صيانة > المصمم**</span><span class="sxs-lookup"><span data-stu-id="0226e-105">**Product information management > Bills of materials and formulas > Bill of materials >** (Select product) **> Maintain > Designer**</span></span>

![لقطة شاشة لصفحة مصمم قائمة مكونات الصنف (BOM) تعرض قائمة مكونات صنف (BOM) متعددة المستويات.](../media/multi-level-bom.png)




## <a name="example-of-a-multilevel-bom"></a><span data-ttu-id="0226e-107">مثال عن قائمة مكونات صنف (BOM) متعددة المستويات</span><span class="sxs-lookup"><span data-stu-id="0226e-107">Example of a multilevel BOM</span></span>

<span data-ttu-id="0226e-108">تتكوّن دراجات البالغين من عجلتين ومقعد ومقاود واطار.</span><span class="sxs-lookup"><span data-stu-id="0226e-108">Adult bicycles consist of two wheels, a seat, handlebars, and a frame.</span></span>
<span data-ttu-id="0226e-109">وتظهر جميع هذه المكونات في قائمة مكونات الصنف (BOM) الخاصة بالدراجة.</span><span class="sxs-lookup"><span data-stu-id="0226e-109">All these components are reflected in the bicycle BOM.</span></span> <span data-ttu-id="0226e-110">ومع ذلك، يتكوّن الإطار أيضاً من عدة عناصر منفصلة (ثلاثة أو أربعة أنابيب ملحومة معاً).</span><span class="sxs-lookup"><span data-stu-id="0226e-110">However, the frame also consists of several discrete items (three or four tubes welded together).</span></span> <span data-ttu-id="0226e-111">وبالتالي، تتوفر لدى الإطار قائمة مكونات صنف (BOM) خاصة به.</span><span class="sxs-lookup"><span data-stu-id="0226e-111">Therefore, the frame has a BOM of its own.</span></span> <span data-ttu-id="0226e-112">تُعرف قائمة مكونات الصنف (BOM) الخاصة بالإطار على أنها قائمة مكونات صنف فرعية، أي قائمة مكونات صنف داخل قائمة مكونات صنف للمنتج النهائي، الدراجة.</span><span class="sxs-lookup"><span data-stu-id="0226e-112">The frame's BOM is known as a sub-BOM, that is, a bill of material within the bill of material for the end product, the bicycle.</span></span>

<span data-ttu-id="0226e-113">لنفترض أنه تم إنشاء قائمة مكونات صنف (BOM) لتجميع الدراجات.</span><span class="sxs-lookup"><span data-stu-id="0226e-113">Assume that a BOM is created to assemble bicycles.</span></span> <span data-ttu-id="0226e-114">تم إعداد الأصناف التالية كنوع المنتج.</span><span class="sxs-lookup"><span data-stu-id="0226e-114">The following items are set up as the product type.</span></span> <span data-ttu-id="0226e-115">يتم استخدام أنواع المنتجات في قائمة مكونات الصنف (BOM) ولا تحتاج إلى تجميع.</span><span class="sxs-lookup"><span data-stu-id="0226e-115">The products types are used in the BOM and do not require assembly.</span></span>

-   <span data-ttu-id="0226e-116">العجلات</span><span class="sxs-lookup"><span data-stu-id="0226e-116">Wheels</span></span>
-   <span data-ttu-id="0226e-117">المقعد</span><span class="sxs-lookup"><span data-stu-id="0226e-117">Seat</span></span>
-   <span data-ttu-id="0226e-118">المقاود</span><span class="sxs-lookup"><span data-stu-id="0226e-118">Handlebars</span></span>

<span data-ttu-id="0226e-119">يتم تجميع اطار الدراجة في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="0226e-119">The bicycle frame is assembled in production.</span></span> <span data-ttu-id="0226e-120">يتم إعداد هذا الجزء من العملية كقائمة مكونات صنف (BOM) فرعية تتضمن الأصناف التالية:</span><span class="sxs-lookup"><span data-stu-id="0226e-120">This part of the process is set up as a sub-BOM that includes the following items:</span></span>

-   <span data-ttu-id="0226e-121">الأنابيب</span><span class="sxs-lookup"><span data-stu-id="0226e-121">Tubes</span></span>
-   <span data-ttu-id="0226e-122">سلك التلحيم</span><span class="sxs-lookup"><span data-stu-id="0226e-122">Welding wire</span></span>
-   <span data-ttu-id="0226e-123">الدعامات أو الحامل</span><span class="sxs-lookup"><span data-stu-id="0226e-123">Brackets or brace</span></span>

![رسم تخطيطي لمثال قائمة مكونات الصنف (BOM) لتجميع دراجة.](../media/multi-level-bom-diagram.png)
 

<span data-ttu-id="0226e-125">في أغلب الأحيان، تحتوي أصناف قائمة مكونات الصنف (BOM) المعقدة على قوائم مكونات صنف (BOM) فرعية متعددة.</span><span class="sxs-lookup"><span data-stu-id="0226e-125">Complex BOM items frequently have several sub-BOMs.</span></span> <span data-ttu-id="0226e-126">يتوقف عدد المستويات، أو قوائم مكونات الصنف (BOM) الفرعية، على كيفية إدارة الصنف.</span><span class="sxs-lookup"><span data-stu-id="0226e-126">The number of levels, or sub-BOMs, depends on how the item is managed.</span></span>

<span data-ttu-id="0226e-127">بشكل عام، يحتاج الصنف إلى مستواه الخاص في قائمة مكونات الصنف (BOM)، إذا كان من الضروري أن يكون الصنف، في مرحلة ما:</span><span class="sxs-lookup"><span data-stu-id="0226e-127">Generally, an item needs its own level in the BOM if, at a stage, the item must be:</span></span>

-   <span data-ttu-id="0226e-128">متعقّباً</span><span class="sxs-lookup"><span data-stu-id="0226e-128">Tracked</span></span>
-   <span data-ttu-id="0226e-129">مخزّناً</span><span class="sxs-lookup"><span data-stu-id="0226e-129">Stored</span></span>
-   <span data-ttu-id="0226e-130">مُباعاً</span><span class="sxs-lookup"><span data-stu-id="0226e-130">Sold</span></span>

