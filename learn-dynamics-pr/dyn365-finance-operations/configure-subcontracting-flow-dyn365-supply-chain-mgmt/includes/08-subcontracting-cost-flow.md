---
ms.openlocfilehash: 9a2f8bf2feaa24849765b480c1f2e2f121f2fede
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073019"
---

<span data-ttu-id="96fbd-101">يشكل التعاقد من الباطن على أساس الأنشطة في Supply Chain Management جزءاً من مساهمات التكلفة لتدفقات الإنتاج بناءً على أنشطة تدفق الإنتاج المتعاقد عليها من الباطن.</span><span class="sxs-lookup"><span data-stu-id="96fbd-101">Activity-based subcontracting in Supply Chain Management accounts for cost contributions to production flows based on subcontracted production flow activities.</span></span> <span data-ttu-id="96fbd-102">يتم تقدير مساهمة التكلفة للأنشطة المتعاقد عليها من الباطن بالتكلفة القياسية للخدمة باستخدام حساب كمية الخدمة للكمية المستخدمة لحساب قائمة مكونات الصنف (BOM).</span><span class="sxs-lookup"><span data-stu-id="96fbd-102">The cost contribution of subcontracted activities is estimated at standard cost of the service by using the service quantity calculation for the quantity that is used for the BOM calculation.</span></span> <span data-ttu-id="96fbd-103">بشكل افتراضي، هذا التقدير هو كمية أمر المخزون الافتراضية للصنف.</span><span class="sxs-lookup"><span data-stu-id="96fbd-103">By default, this estimation is the inventory default order quantity of the item.</span></span>

<span data-ttu-id="96fbd-104">عندما تستلم المواد مرة أخرى من المقاول من الباطن، وبعد أن تقوم بترحيل إشعار الاستلام أو إيصال تعبئة المورد في أمر الشراء الذي تم إنشاؤه لنشاط متعاقد عليه من الباطن، يقوم النظام بحساب قيمة الإيصال في حسابات الأعمال تحت التنفيذ (WIP) في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="96fbd-104">When you receive material back from the subcontractor, and after you have posted the receipt advisory advice or a vendor packing slip on a purchase order that was created for a subcontracted activity, the system accounts for the value of the receipt in the WIP accounts of the production flow.</span></span> <span data-ttu-id="96fbd-105">يخصم هذا الأسلوب الأعمال تحت التنفيذ لتدفق الإنتاج الفعلي للخدمة التي يوفرها المقاول من الباطن للشركة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-105">This approach debits the actual production flow work in process for the service that is provided by the subcontractor to the company.</span></span>

<span data-ttu-id="96fbd-106">وتُعد انحرافات الفواتير عن الإيصالات أيضاً فروقاً في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="96fbd-106">Deviations of invoices to the receipts are also considered variances to the production flow.</span></span> <span data-ttu-id="96fbd-107">تسمح فئة التكلفة بالتتبع الشفاف لقيمة العمل المتعاقد عليه من الباطن الذي تم تخصيصه للأعمال تحت التنفيذ (WIP) واستهلاكه كل فترة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-107">The cost category allows for transparent tracking of the value of subcontracted work that is allocated to WIP and consumed each period.</span></span>

<span data-ttu-id="96fbd-108">يحسب تحديد تكاليف الإصدار التلقائي لـ lean manufacturing في نهاية فترة التكلفة الفروق الفعلية للمنتجات بالنسبة إلى التكلفة القياسية للمنتجات التي تم إنتاجها من تدفق الإنتاج أثناء فترة التكلفة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-108">Backflush costing for lean manufacturing at the end of a costing period calculates the actual variances of the products to standard cost for products that are produced out of the production flow during the costing period.</span></span>

## <a name="scenario"></a><span data-ttu-id="96fbd-109">السيناريو</span><span class="sxs-lookup"><span data-stu-id="96fbd-109">Scenario</span></span>

<span data-ttu-id="96fbd-110">يصف هذا السيناريو تدفق تكلفة التعاقد من الباطن، حيث يتم ترك المواد في حسابات الأعمال تحت التنفيذ (WIP) خلال عملية التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="96fbd-110">This scenario describes the subcontracting cost flow, where material is left over in the WIP accounts throughout the subcontracting process.</span></span>

<span data-ttu-id="96fbd-111">في هذا السيناريو، المنتج الذي يتم تصنيعه من عملية التعاقد من الباطن هو L0101، وهو مشغل مكبر صوت.</span><span class="sxs-lookup"><span data-stu-id="96fbd-111">In this scenario, the product that is being manufactured out of the subcontracting process is L0101, a Speaker driver.</span></span> <span data-ttu-id="96fbd-112">ينفذ المقاول من الباطن العملية.</span><span class="sxs-lookup"><span data-stu-id="96fbd-112">The subcontractor performs the process.</span></span> <span data-ttu-id="96fbd-113">تبلغ التكلفة القياسية لمشغل مكبر الصوت النهائي 0.90 دولار أمريكي (USD).</span><span class="sxs-lookup"><span data-stu-id="96fbd-113">The finished Speaker driver has a standard cost of 0.90 US dollars (USD).</span></span>

<span data-ttu-id="96fbd-114">ويتم حساب هذه التكلفة القياسية على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="96fbd-114">This standard cost is calculated as such:</span></span>

- <span data-ttu-id="96fbd-115">المواد المباشرة = 0.10 دولار أمريكي، محسوبة بوحدة واحدة لكل منتج من الصنف L0101، مشغل مكبر الصوت بتكلفة 0.10 دولار أمريكي.</span><span class="sxs-lookup"><span data-stu-id="96fbd-115">Direct material = USD 0.10, calculated with one unit for each product of item L0101, Speaker driver with a cost of USD 0.10.</span></span>

- <span data-ttu-id="96fbd-116">التكلفة غير المباشرة = 0.20 دولار أمريكي، محسوبة بنسبة 200 في المائة من تكلفة المواد المباشرة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-116">Indirect cost = USD 0.20, calculated with 200 percent of direct material cost.</span></span>

- <span data-ttu-id="96fbd-117">الإسناد المباشر إلى جهة أخرى = 0.60 دولار أمريكي، محسوباً كوحدة خدمة واحدة للنشاط المتعاقد عليه من الباطن لكل منتج بتكلفة 0.60 دولار أمريكي.</span><span class="sxs-lookup"><span data-stu-id="96fbd-117">Direct outsourcing = USD 0.60, calculated as one unit of service for the subcontracted activity for each product at a cost of USD 0.60.</span></span>

<span data-ttu-id="96fbd-118">في الوقت الحالي، تم البدء في أربعة كانبان لكل 50 وحدة، وتم إنتاج كانبان واحد من 50 وحدة، وتمت إضافة ثلاثة كانبان من 50 وحدة من المواد الخام في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="96fbd-118">Currently, four kanbans for 50 units each have been initiated, one kanban of 50 units has been produced, and three kanbans of 50 units of raw materials have been replenished into the production flow.</span></span> <span data-ttu-id="96fbd-119">تم استلام مائة (100) وحدة خدمة لعملية التعاقد من الباطن مقابل 0.65 دولار أمريكي لكل وحدة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-119">One hundred (100) units of service for the subcontracting process have been received at USD 0.65 for each unit.</span></span>

<span data-ttu-id="96fbd-120">تم إصدار فاتورة لخمسين من هذه الوحدات بمبلغ 0.70 دولار أمريكي لكل وحدة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-120">Fifty of these units were invoiced at USD 0.70 for each unit.</span></span>

<span data-ttu-id="96fbd-121">توضح الخطوات التالية ما يحدث في عملية التعاقد من الباطن والنتائج اللاحقة لتلك الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="96fbd-121">The following steps show what occurs within the subcontracting process and the subsequent results of those actions.</span></span>

1.  <span data-ttu-id="96fbd-122">يسلم المقاول من الباطن 50 وحدة بتكلفة قياسية قدرها 0.90 دولار أمريكي لكل وحدة، مما ينتج عنه ائتمان WIP بقيمة 45.00 دولاراً أمريكياً وخصم بضائع نهائية بقيمة 45.00 دولاراً أمريكياً.</span><span class="sxs-lookup"><span data-stu-id="96fbd-122">The subcontractor delivers 50 units at a standard cost of USD 0.90 for each unit, resulting in a WIP credit of USD 45.00 and a finished goods debit of USD 45.00.</span></span>

2.  <span data-ttu-id="96fbd-123">يتم استلام إيصال استلام المنتجات لـ 100 وحدة خدمة بمبلغ 0.65 دولار أمريكي لكل وحدة، مما ينتج عنه ائتمان التزام بقيمة 65.00 دولاراً أمريكياً وخصم إلى WIP بقيمة 65.00 دولاراً أمريكياً.</span><span class="sxs-lookup"><span data-stu-id="96fbd-123">The product receipt for 100 service units is received at USD 0.65 for each unit, resulting in a liability credit of USD 65.00 and a debit to WIP of USD 65.00.</span></span>

3.  <span data-ttu-id="96fbd-124">يتم استلام فاتورة المورّد مقابل 50 وحدة بسعر 0.70 دولار أمريكي لكل وحدة، مما ينتج عنه فرق قدره 0.05 دولار أمريكي لكل وحدة.</span><span class="sxs-lookup"><span data-stu-id="96fbd-124">The vendor invoice is received for 50 units at USD 0.70 for each unit, resulting in a variance of USD 0.05 for each unit.</span></span> <span data-ttu-id="96fbd-125">تمت إضافة 2.50 دولار أمريكي إلى حساب الالتزام وحساب WIP بمبلغ 2.50 دولار أمريكي.</span><span class="sxs-lookup"><span data-stu-id="96fbd-125">The liability account is credited for USD 2.50 and the WIP account is debited for USD 2.50.</span></span>

<span data-ttu-id="96fbd-126">في نهاية الفترة، يتم تشغيل تحديد تكاليف الإصدار التلقائي، وفي هذا السيناريو، تؤخذ حالة المنتجات في الاعتبار.</span><span class="sxs-lookup"><span data-stu-id="96fbd-126">At period-end, backflush costing is run, and in this scenario, the status of products is then considered.</span></span>

-   <span data-ttu-id="96fbd-127">45 وحدة من الغطاء غير المصبوغ تظل غير مستخدمة في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="96fbd-127">45 units of unpainted cover remain unused in the production flow.</span></span>

-   <span data-ttu-id="96fbd-128">50 وحدة من غطاء الكروم لا تزال قيد المعالجة في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="96fbd-128">50 units of chrome cover are still in process in the production flow.</span></span>

-   <span data-ttu-id="96fbd-129">تم استلام 50 وحدة من غطاء الكروم كناتج لتدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="96fbd-129">50 units of chrome cover have been received as output of the production flow.</span></span>
