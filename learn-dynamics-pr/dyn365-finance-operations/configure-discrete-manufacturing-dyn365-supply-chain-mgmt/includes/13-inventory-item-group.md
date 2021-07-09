---
ms.openlocfilehash: 170dc8fe446f0fbe1d80ac97480c6ba3cb869a52
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073680"
---
<span data-ttu-id="05de7-101">يتحكم ملف تعريف ترحيل المخزون في الحسابات الرئيسية التي سيتم استخدامها مع كل تحديث ترحيل في دفتر الأستاذ الفرعي للمخزون ودفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="05de7-101">The inventory posting profile controls which main accounts will be used with each posting update in the inventory subledger and the general ledger.</span></span>

<span data-ttu-id="05de7-102">**إدارة المخزون > إعداد > ترحيل > ترحيل**</span><span class="sxs-lookup"><span data-stu-id="05de7-102">**Inventory management > Setup > Posting > Posting**</span></span>

![لقطة شاشة لصفحة ملف تعريف ترحيل المخزون.](../media/inventory-posting-profile.png) 



## <a name="item-groups"></a><span data-ttu-id="05de7-104">مجموعات الأصناف</span><span class="sxs-lookup"><span data-stu-id="05de7-104">Item groups</span></span>

<span data-ttu-id="05de7-105">يتم استخدام مجموعة الأصناف المعينة لكل صنف معاً مع ترحيلات دفتر الأستاذ.</span><span class="sxs-lookup"><span data-stu-id="05de7-105">The item group that is assigned to each item is used together with the ledger postings.</span></span> <span data-ttu-id="05de7-106">استخدم مجموعات الأصناف لمتابعة الإحصائيات الخاصة بمبيعات الأصناف والمشتريات والمخزون وعمليات الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="05de7-106">Use item groups to follow statistics on item sales, purchases, inventory, and productions.</span></span>

<span data-ttu-id="05de7-107">ضع في اعتبارك بنية مجموعات الأصناف بعناية قبل المتابعة.</span><span class="sxs-lookup"><span data-stu-id="05de7-107">Consider the structure of item groups carefully before proceeding.</span></span> <span data-ttu-id="05de7-108">بعد إنشاء المجموعات واستخدامها في الجدول الرئيسي للصنف، لا يمكن حذفها.</span><span class="sxs-lookup"><span data-stu-id="05de7-108">After the groups have been created and used in the item main table, they cannot be deleted.</span></span> <span data-ttu-id="05de7-109">يمكنك اختيار إنشاء عدد كبير من مجموعات الأصناف وتعيين حسابات دفتر أستاذ محددة لكل مجموعة.</span><span class="sxs-lookup"><span data-stu-id="05de7-109">You can choose to create a large number of item groups and assign specific ledger accounts to each group.</span></span> <span data-ttu-id="05de7-110">ويسمح ذلك بالتحكم المفصل لتعقب قيمة الأصناف الموجودة في العملية.</span><span class="sxs-lookup"><span data-stu-id="05de7-110">This allows for detailed control for tracking the value of items in process.</span></span>
<span data-ttu-id="05de7-111">وبدلاً من ذلك، يمكنك اختيار إنشاء مجموعة أصناف واحدة فقط لاستخدامها مع كافة الأصناف الفعلية.</span><span class="sxs-lookup"><span data-stu-id="05de7-111">Alternatively, you can choose to create only one item group to be used for all physical items.</span></span>

<span data-ttu-id="05de7-112">في النهاية، تحدد متطلبات التحكم المالي للعميل عدد مجموعات الأصناف التي يجب تأسيسها وتكوينها.</span><span class="sxs-lookup"><span data-stu-id="05de7-112">Ultimately, the customer's financial control requirements determine the number of item groups that have to be established and configured.</span></span>

## <a name="item-model-group"></a><span data-ttu-id="05de7-113">مجموعة نماذج الصنف</span><span class="sxs-lookup"><span data-stu-id="05de7-113">Item model group</span></span>

<span data-ttu-id="05de7-114">تحتوي مجموعات نماذج الأصناف على إعدادات تحدد كيفية التحكم في الأصناف ومعالجتها في المخزون وكيفية حساب الاستهلاك.</span><span class="sxs-lookup"><span data-stu-id="05de7-114">Item model groups contain settings that determine how items are controlled and handled in inventory and how consumption is calculated.</span></span>
<span data-ttu-id="05de7-115">يحدد العمل مع العميل وتقييم الإعدادات في إعداد نموذج المخزون عدد مجموعات نماذج المخزون المختلفة التي تحتاج إلى إنشائها.</span><span class="sxs-lookup"><span data-stu-id="05de7-115">Working with the customer and evaluating the settings in the inventory model setup determines the number of different inventory model groups you need to create.</span></span>

<span data-ttu-id="05de7-116">لتحديد عدد مجموعات نماذج المخزون التي يجب إنشاؤها للتنفيذ، حدد ما إذا كان يجب:</span><span class="sxs-lookup"><span data-stu-id="05de7-116">To determine the number of inventory model groups to create for the implementation, decide whether to:</span></span>

-   <span data-ttu-id="05de7-117">استخدام نفس نموذج المخزون لكافة الأصناف.</span><span class="sxs-lookup"><span data-stu-id="05de7-117">Use the same inventory model for all items.</span></span>

-   <span data-ttu-id="05de7-118">فحص الأصناف الخاصة بالعميل.</span><span class="sxs-lookup"><span data-stu-id="05de7-118">Quarantine a customer's specific items.</span></span>

-   <span data-ttu-id="05de7-119">الالتزام بمتطلبات الانتقاء أو الحجز الخاصة في أصناف محددة.</span><span class="sxs-lookup"><span data-stu-id="05de7-119">Adhere to special picking or reservation requirements on specific items.</span></span>
