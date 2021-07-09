---
ms.openlocfilehash: 35ec40bfe400e164db2e87a58281ba692eda0038
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073719"
---
<span data-ttu-id="65fbc-101">تسمح قوائم الموردين المعتمدين (AVL) بوضع قيود على صنف ما لتحديد الموردين الذين يمكن شراء الصنف منهم.</span><span class="sxs-lookup"><span data-stu-id="65fbc-101">Approved vendor lists (AVL) allow for the placement of limitations on an item to specify which vendors that the item can be purchased from.</span></span> <span data-ttu-id="65fbc-102">تضمن هذه الطريقة أن حركات الشراء يتم إجراؤها دائماً على القائمة المعتمدة فقط.</span><span class="sxs-lookup"><span data-stu-id="65fbc-102">This method ensures that the purchasing transactions are always performed only on the approved list.</span></span>

<span data-ttu-id="65fbc-103">أثناء إعداد مجموعة نماذج الصنف، يتم تحديد التحقق من المورد الافتراضي ضمن مجموعة نماذج الصنف، والذي يمكن تغييره على مستوى الصنف إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="65fbc-103">During the setup of the item model group, a default vendor check is specified within the item model group, which can be changed on the item level if needed.</span></span>

<span data-ttu-id="65fbc-104">على مستوى المنتج، يمكن تعديل أسلوب التحقق من المورِد لإملاء مدى تقييد التحكم في قائمة الموردين المعتمدين لهذا الصنف المحدد.</span><span class="sxs-lookup"><span data-stu-id="65fbc-104">At the product level, the vendor check method can be modified to dictate how restrictive the control for the approved vendor list is for that specific item.</span></span> <span data-ttu-id="65fbc-105">الخيارات الموجودة في أسلوب التحقق من المورد هي:</span><span class="sxs-lookup"><span data-stu-id="65fbc-105">The options in the vendor check method are:</span></span>

-   <span data-ttu-id="65fbc-106">**لا يوجد شيك** - يمكن استخدام أي مورد سواء كان المورد موجوداً في قوائم الموردين المعتمدين أم لا.</span><span class="sxs-lookup"><span data-stu-id="65fbc-106">**No check** - Any vendor can be used whether the vendor is on the AVL or not.</span></span>

-   <span data-ttu-id="65fbc-107">**تحذير فقط** - عندما يتم استخدام مورد غير موجود في قوائم الموردين المعتمدين، سيحصل المستخدم على تحذير، ولكن سيتم حفظ الحركة.</span><span class="sxs-lookup"><span data-stu-id="65fbc-107">**Warning only** - When a vendor is used that is not on the AVL, the user will get a warning, but the transaction will save.</span></span>

-   <span data-ttu-id="65fbc-108">**غير مسموح به** - عندما يتم استخدام مورد غير موجود في قوائم الموردين المعتمدين، سيتلقى المستخدم رسالة خطأ ولن يتم حفظ الحركة.</span><span class="sxs-lookup"><span data-stu-id="65fbc-108">**Not allowed** - When a vendor is used that is not on the AVL, the user will get an error message, and the transaction will not save.</span></span>

<span data-ttu-id="65fbc-109">**إدارة المخزون> إعداد> مخزون> مجموعات نماذج الصنف**</span><span class="sxs-lookup"><span data-stu-id="65fbc-109">**Inventory management > Setup > Inventory > Item model groups**</span></span>

<span data-ttu-id="65fbc-110">[![لقطة شاشة لصفحة مجموعات نماذج الصنف.](../media/item-model-group.png)](../media/item-model-group.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="65fbc-110">[![Screenshot of the Item model groups page.](../media/item-model-group.png)](../media/item-model-group.png#lightbox)</span></span>


<span data-ttu-id="65fbc-111">عند إضافة صنف إلى سطر مستند الشراء، تكمل Supply Chain Management التحقق من الصنف لتحديد ما إذا كان أسلوب التحقق من المورد المعتمد **تحذير فقط** أو **غير مسموح به** مطلوباً للصنف.</span><span class="sxs-lookup"><span data-stu-id="65fbc-111">When an item is added to a purchase document line, Supply Chain Management completes a check on the item to determine if a **Warning only** or **Not allowed** approved vendor check method is required on the item.</span></span> <span data-ttu-id="65fbc-112">إذا تم تعيين إما **تحذير فقط** أو **غير مسموح به** على الصنف، يتم استكمال مراجعة قائمة المورِّدين المعتمدين للصنف للعثور على المورد في مستند الشراء.</span><span class="sxs-lookup"><span data-stu-id="65fbc-112">If either **Warning only** or **Not allowed** is set on the item, a review of the approved vendor list for the item to find the vendor on the purchase document is completed.</span></span> 

<span data-ttu-id="65fbc-113">يتم بعد ذلك التحقق من صحة التواريخ الموجودة في قوائم الموردين المعتمدين للتحقق من اعتماد المورد لتاريخ مستند الشراء.</span><span class="sxs-lookup"><span data-stu-id="65fbc-113">The dates on the AVL are then validated to verify that the vendor is approved for the date of the purchase document.</span></span> <span data-ttu-id="65fbc-114">إذا لم تتم الموافقة على المورد وتم تعيين **رسالة التحقق من المورد** على تحذير، فستظهر رسالة تفيد بأن المورد المحدد غير مخول للصنف، ولكن يتم إنشاء أمر شراء.</span><span class="sxs-lookup"><span data-stu-id="65fbc-114">If the vendor is not approved and the **Vendor check message** is set to warning, a message will display stating that the specified vendor is not authorized for the item, but a purchase order is created.</span></span> <span data-ttu-id="65fbc-115">إذا تم تعيين **أسلوب التحقق من المورد المعتمد** على **غير مسموح به**، فلن يتم إنشاء سطر أمر الشراء، ويجب على المستخدم تغيير إعداد المورد المعتمد أو تغيير الموردين في أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="65fbc-115">If the **Approved vendor check method** is set to **Not allowed**, the purchase order line will not be created, and the user must change the approved vendor setting or change vendors on the PO.</span></span>

<span data-ttu-id="65fbc-116">يتم التحقق من صحة إعداد علاقة الصنف والمورد في قائمة الموردين المعتمدين عند إدخال الصنف في:</span><span class="sxs-lookup"><span data-stu-id="65fbc-116">The validation of the item and vendor relationship setup on the approved vendor list is validated on entry of the item into:</span></span>

-   <span data-ttu-id="65fbc-117">أمر الشراء</span><span class="sxs-lookup"><span data-stu-id="65fbc-117">Purchase order</span></span>

-   <span data-ttu-id="65fbc-118">اتفاقيات الشراء</span><span class="sxs-lookup"><span data-stu-id="65fbc-118">Purchase agreements</span></span>

-   <span data-ttu-id="65fbc-119">طلبات الشراء</span><span class="sxs-lookup"><span data-stu-id="65fbc-119">Purchase requisitions</span></span>

-   <span data-ttu-id="65fbc-120">ردود طلب عرض أسعار (RFQ) - عندما تتلقى رداً من الموردين للحصول على عرض أسعار، يتم إدخال سعر الشراء الذي يحدده المورد في صفحة **الرد على طلب عرض الأسعار** وقبوله.</span><span class="sxs-lookup"><span data-stu-id="65fbc-120">Request for quote (RFQ) responses - When you receive a reply from vendors for a quotation, the purchase price that is quoted by the vendor is entered on the **Request for quotation reply** page and accepted.</span></span> <span data-ttu-id="65fbc-121">أثناء قبولك عرض أسعار الشراء، يتم التحقق من صحة قائمة الموردين المعتمدين للصنف مع المورد الذي يتم وضع رد طلب عرض الأسعار معه.</span><span class="sxs-lookup"><span data-stu-id="65fbc-121">While you are accepting the purchase quotation, the approved vendor list for the item is validated with the vendor with whom the RFQ response is placed.</span></span>
