---
ms.openlocfilehash: 4830d93f76f1490f810658719b3f73c14270284b
ms.sourcegitcommit: 0484f01637a384540476f9c6e45ba64bd86526a8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/19/2021
ms.locfileid: "6070416"
---
<span data-ttu-id="28721-101">تتطلب كل قناة تجارية مخزوناً، ولكي يكون لها مخزون، يجب أن يكون لديها مستودع مرتبط بها.</span><span class="sxs-lookup"><span data-stu-id="28721-101">Each commerce channel requires inventory, and to have inventory, it must have a warehouse associated with it.</span></span> <span data-ttu-id="28721-102">لإنشاء تكوين المستودع لقناة Commerce، يتعين عليك أيضاً إنشاء العديد من التبعيات.</span><span class="sxs-lookup"><span data-stu-id="28721-102">To create the warehouse configuration for a Commerce channel, you must also create several dependencies.</span></span> 

<span data-ttu-id="28721-103">يجب إنشاء السجلات بالتسلسل التالي:</span><span class="sxs-lookup"><span data-stu-id="28721-103">The records must be created in the following sequence:</span></span>

1.  <span data-ttu-id="28721-104">إنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="28721-104">Create a site.</span></span>
2.  <span data-ttu-id="28721-105">إنشاء مستودع.</span><span class="sxs-lookup"><span data-stu-id="28721-105">Create a warehouse.</span></span>
3.  <span data-ttu-id="28721-106">إنشاء ممر للمخزون.</span><span class="sxs-lookup"><span data-stu-id="28721-106">Create an inventory aisle.</span></span>
4.  <span data-ttu-id="28721-107">إنشاء موقع مخزون المستودع.</span><span class="sxs-lookup"><span data-stu-id="28721-107">Create a warehouse inventory location.</span></span>
5.  <span data-ttu-id="28721-108">تعيين مواقع الاستلام والإصدار الافتراضية إلى المستودع.</span><span class="sxs-lookup"><span data-stu-id="28721-108">Assign the default receipt and issue locations to the warehouse.</span></span> 

<span data-ttu-id="28721-109">إن الموقع هو تجميع منطقي للمستودعات.</span><span class="sxs-lookup"><span data-stu-id="28721-109">A site is a logical grouping of warehouses.</span></span> <span data-ttu-id="28721-110">حتى إذا كان هناك مستودع واحد فقط في الموقع، فلا يزال من المفترض تعيين الموقع.</span><span class="sxs-lookup"><span data-stu-id="28721-110">Even if only one warehouse is in a site, a site must still be assigned.</span></span> <span data-ttu-id="28721-111">يمكن العثور على صفحة **المواقع** من خلال الذهاب إلى **‬‏‫‬‏‫البيع بالتجزئة والتجارة > ‏‫إعداد القناة‬ > المواقع**.</span><span class="sxs-lookup"><span data-stu-id="28721-111">The **Sites** page can be found under **Retail and Commerce > Channel setup > Sites**.</span></span>


![لقطة شاشة لصفحة المواقع في Dynamics 365 Commerce.](../media/sites-08-ss.jpg) 

<span data-ttu-id="28721-113">المستودع هو الموقع الفعلي الذي يتم فيه تخزين المخزون.</span><span class="sxs-lookup"><span data-stu-id="28721-113">A warehouse is a physical location in which inventory is stored.</span></span> <span data-ttu-id="28721-114">توجد بين المستودعات والقنوات التجارية علاقة واحد إلى واحد (1:1).</span><span class="sxs-lookup"><span data-stu-id="28721-114">Warehouses and commerce channels have a 1:1 relationship.</span></span> <span data-ttu-id="28721-115">يمكن العثور على صفحة **المتاجر** من خلال الذهاب إلى **‬‏‫‬‏‫البيع بالتجزئة والتجارة > القنوات‬ > المتاجر > جميع المتاجر**.</span><span class="sxs-lookup"><span data-stu-id="28721-115">The **Stores** page can be found under **Retail and Commerce > Channels > Stores > All stores**.</span></span>

 
<span data-ttu-id="28721-116">[ ![لقطة شاشة لصفحة المتاجر في Dynamics 365 Commerce.](../media/stores-09-ssm.jpg) ](../media/stores-09-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="28721-116">[ ![Screenshot of the Dynamics 365 Commerce Stores page.](../media/stores-09-ssm.jpg) ](../media/stores-09-ssm.jpg#lightbox)</span></span>

<span data-ttu-id="28721-117">يجب تعيين موقع لكل مستودع.</span><span class="sxs-lookup"><span data-stu-id="28721-117">Each warehouse must be assigned a site.</span></span> <span data-ttu-id="28721-118">يجب تعيين مستودع لكل ممر مخزون وموقع مخزون.</span><span class="sxs-lookup"><span data-stu-id="28721-118">Each inventory aisle and inventory location must be assigned a warehouse.</span></span> <span data-ttu-id="28721-119">يمكن العثور على الصفحة التالية من خلال الذهاب إلى **‬‏‫‬‏‫البيع بالتجزئة والتجارة > ‏‫إعداد القناة‬ > المستودعات**.</span><span class="sxs-lookup"><span data-stu-id="28721-119">The following page can be found under **Retail and Commerce > Channel setup > Warehouses**.</span></span>

 
<span data-ttu-id="28721-120">[ ![لقطة شاشة لصفحة المستودعات في Dynamics 365 Commerce.](../media/warehouses-10-ss.jpg) ](../media/warehouses-10-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="28721-120">[ ![Screenshot of the Dynamics 365 Commerce warehouse page.](../media/warehouses-10-ss.jpg) ](../media/warehouses-10-ss.jpg#lightbox)</span></span>

<span data-ttu-id="28721-121">بعد قيامك بإنشاء المكونات الأربعة، سوف تحتاج إلى إعداد عدة تكوينات للمستودع في **البيع بالتجزئة والتجارة > ‏‫إعداد القناة > المستودعات**.</span><span class="sxs-lookup"><span data-stu-id="28721-121">After you have created the four components, you will need to set up several configurations for the warehouse in **Retail and Commerce > Channel setup > Warehouses**.</span></span> <span data-ttu-id="28721-122">يجب تعيين **موقع الاستلام الافتراضي** **وموقع الإصدار الافتراضي** للسجلات التي تم إنشاؤها كسجلات افتراضية.</span><span class="sxs-lookup"><span data-stu-id="28721-122">The **Default receipt location** and **Default issue location** need to be set for the records that were created as a default.</span></span> <span data-ttu-id="28721-123">ويمكن تغييرها إلى تطبيق أكثر تعقيداً، إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="28721-123">They can be changed in a more complex implementation, if needed.</span></span> <span data-ttu-id="28721-124">يجب أيضاً تكوين أبعاد **الإرجاع** **والتخزين** بشكل مناسب.</span><span class="sxs-lookup"><span data-stu-id="28721-124">The **Return** and **Storage** dimensions should also be configured appropriately.</span></span> 

<span data-ttu-id="28721-125">بالنسبة لإعداد **المخزون السالب** يتعين عليك تحديد ما إذا كان المخزون السالب مسموحاً به.</span><span class="sxs-lookup"><span data-stu-id="28721-125">For the **Negative inventory** setting on the warehouse, you need to decide if negative inventory is allowed.</span></span> 

