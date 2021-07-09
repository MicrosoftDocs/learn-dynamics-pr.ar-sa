---
ms.openlocfilehash: 73ea5dafe0114674d329d0df6c4773a9d4f331f9
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073807"
---

<span data-ttu-id="efe62-101">في Supply Chain Management، يمكنك إنشاء اتفاقيات شراء وإقرانها بتدفقات الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="efe62-101">In Supply Chain Management, you can create purchase agreements and associate them with production flows.</span></span> <span data-ttu-id="efe62-102">تحتوي اتفاقية الشراء على جميع معلومات التسعير الخاصة بالخدمة المرتبطة، والتي يوفرها المقاول الفرعي.</span><span class="sxs-lookup"><span data-stu-id="efe62-102">The purchase agreement contains all the pricing information for the associated service, which is provided by the subcontractor.</span></span>


<span data-ttu-id="efe62-103">سيتم إنشاء أوامر التحرير من اتفاقية الشراء للإشارة إلى الطلبات وإدارة التأكيدات والإبلاغ عن الإيصالات والدفع مقابل خدمة التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="efe62-103">Release orders will be created from the purchase agreement to signal demands, manage confirmations, report receipts, and pay for the subcontracting service.</span></span>

<span data-ttu-id="efe62-104">لحساب تكلفة المنتجات، يجب تحديد التكلفة القياسية للخدمة.</span><span class="sxs-lookup"><span data-stu-id="efe62-104">For cost calculation of the products, a standard cost of the service must be defined.</span></span> <span data-ttu-id="efe62-105">يمكنك تحديد التكلفة عن طريق الاختيار **التكاليف القياسية** في **نموذج المخزون** مجال مجموعات نماذج الصنف التي سيتم تخصيص المنتجات المصنعة لها.</span><span class="sxs-lookup"><span data-stu-id="efe62-105">You can define the cost by selecting **Standard cost** in the **Inventory model** field of the item model groups that the manufactured products are going to be assigned to.</span></span>


<span data-ttu-id="efe62-106">ويجب أن يكون لديك اتفاقية شراء مع المورد قبل أن يتاح له التعاقد من الباطن على أساس النشاط.</span><span class="sxs-lookup"><span data-stu-id="efe62-106">You must have a purchase agreement with the vendor before they can be made available for activity-based subcontracting.</span></span>

<span data-ttu-id="efe62-107">لمزيد من المعلومات حول اتفاقيات الشراء وعملية الشراء حتى الشراء، راجع الروابط الموجودة في وحدة الملخص في نهاية هذه الوحدة.</span><span class="sxs-lookup"><span data-stu-id="efe62-107">For more information regarding purchase agreements and the procure-to-purchase process, see the links in the Summary unit at the end of this module.</span></span>

## <a name="resource-group-acts-as-a-work-cell"></a><span data-ttu-id="efe62-108">تعمل مجموعة الموارد كخلية عمل</span><span class="sxs-lookup"><span data-stu-id="efe62-108">Resource group acts as a work cell</span></span>

<span data-ttu-id="efe62-109">لتكوين خلية عمل على أنها متعاقد عليها من الباطن، يجب إنشاء مَورد نوع **المُورّد** وربطه بخلية العمل (مجموعة الموارد).</span><span class="sxs-lookup"><span data-stu-id="efe62-109">To configure a work cell as subcontracted, a resource of the **vendor** type needs to be created and associated with the work cell (resource group).</span></span> <span data-ttu-id="efe62-110">يجب أن يكون المورد المحدد في اتفاقية الشراء هو أيضاً البائع المتصل بخلية العمل.</span><span class="sxs-lookup"><span data-stu-id="efe62-110">The vendor that is defined in the purchase agreement must also be the vendor that is connected to the work cell.</span></span>

<span data-ttu-id="efe62-111">**مراقبة الإنتاج> إعدادات> الموردين> الموردين**</span><span class="sxs-lookup"><span data-stu-id="efe62-111">**Production control > Setup > Resources > Resources**</span></span>

<span data-ttu-id="efe62-112">[![لقطة شاشة على Finance and Operations صفحة موردي.](../media/resource-1.png)](../media/resource-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="efe62-112">[![Screenshot of the Finance and Operations Resources page.](../media/resource-1.png)](../media/resource-1.png#lightbox)</span></span> 

<span data-ttu-id="efe62-113">يجب تعيين فئة تكلفة وقت التشغيل مع نوع مجموعة تكلفة "الاستعانة بمصادر خارجية مباشرة" إلى خلية العمل.</span><span class="sxs-lookup"><span data-stu-id="efe62-113">A runtime cost category with a "direct outsourcing" cost group type should be assigned to the work cell.</span></span> <span data-ttu-id="efe62-114">لا نحتاج إلى فئات التكلفة للإعداد والكمية.</span><span class="sxs-lookup"><span data-stu-id="efe62-114">The cost categories for setup and quantity are not needed.</span></span>

<span data-ttu-id="efe62-115">Supply Chain Management، يمكن تصميم المواقع وخلايا العمل على أنها مورد من خلال تعيين حساب المورّد إلى مستودع أو إلى مورد لمجموعة موارد.</span><span class="sxs-lookup"><span data-stu-id="efe62-115">In Supply Chain Management, locations and work cells can be modeled as vendor-managed by assigning the vendor account to a warehouse or to a resource of a resource group.</span></span>
