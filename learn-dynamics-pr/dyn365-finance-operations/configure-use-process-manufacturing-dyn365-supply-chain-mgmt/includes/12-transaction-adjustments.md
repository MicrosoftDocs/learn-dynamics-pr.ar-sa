---
ms.openlocfilehash: d718f9e83a16eefb727d39ce4b84494e5907b071
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073306"
---
<span data-ttu-id="bbcfa-101">نظراً لأن وزن المخزون عند وجوده في مستودع يختلف عن وزن المخزون عند إصداره خارج المستودع، فيجب أن تقوم معالجة منتج وزن التعبئة بتعديل المخزون.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-101">Because the weight of inventory when it comes into a warehouse can differ from the weight of inventory when it is issued out of the warehouse, catch weight product processing must adjust the inventory.</span></span>

## <a name="example-1"></a><span data-ttu-id="bbcfa-102">المثال 1</span><span class="sxs-lookup"><span data-stu-id="bbcfa-102">Example 1</span></span>

<span data-ttu-id="bbcfa-103">أثناء الإنتاج، يتم تعبئة كمية **الإبلاغ كمنتهٍ** على بالته.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-103">During production, the **Report as finished** quantity is packed on a pallet.</span></span> <span data-ttu-id="bbcfa-104">يتم قياس الوزن الإجمالي الذي تم الإبلاغ عنه للبضائع المنتهية على البالتة على أنه 80.1 كجم.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-104">The reported total weight of the finished goods on the pallet is measured as 80.1 kg.</span></span> <span data-ttu-id="bbcfa-105">ويتم وضع البالتة بعيداً عن موقع التخزين وأثناء فتره التخزين، تفقد البضائع المنتهية في البالتة الوزن بسبب التبخر.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-105">The pallet is put away to a storing location and, during the storage period, the finished goods on the pallet lose weight due to evaporation.</span></span>

<span data-ttu-id="bbcfa-106">في وقت لاحق، كجزء من عملية انتقاء أمر المبيعات، يتم التقاط وزن لوحة الترخيص نفسها على أنها 79.8 كجم.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-106">Later, as part of a sales order picking process, the weight of the same license plate is captured as 79.8 kg.</span></span> <span data-ttu-id="bbcfa-107">يتم انتقاء البالتة لاحقاً لأمر المبيعات، وكجزء من هذه العملية، يتم وزنها على مقياس.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-107">The pallet is later picked for a sales order and, as part of this process, weighed on a scale.</span></span> <span data-ttu-id="bbcfa-108">يتم تعديل الفرق الموجود في الوزن بين **الإبلاغ كمنتهٍ** وانتقاء المبيعات تلقائياً بواسطة النظام كفرق في المخزون.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-108">The difference in weight between the **Report as finished** status and sales picking is automatically adjusted by the system as an inventory difference.</span></span>

<span data-ttu-id="bbcfa-109">في هذه الحالة، يقوم النظام تلقائياً بضبط الفرق عن طريق ترحيل الحركة المفقودة 0.3 كجم.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-109">In this case, the system automatically adjusts the difference by posting a transaction for the missing 0.3 kg.</span></span>

## <a name="example-2"></a><span data-ttu-id="bbcfa-110">المثال 2</span><span class="sxs-lookup"><span data-stu-id="bbcfa-110">Example 2</span></span>

<span data-ttu-id="bbcfa-111">يشتمل صنف وزن التعبئة المتضمن لوحدة وزن التعبئة ووحدة المخزون بالكيلو على الحد الأدنى من الكمية 8 والحد الأقصى للكمية 10.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-111">A catch weight item with a catch weight unit of boxes and an inventory unit of kilos has a minimum quantity of 8 and a maximum quantity of 10.</span></span>
<span data-ttu-id="bbcfa-112">الكمية المستهدفة هي 10.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-112">The target quantity is 10.</span></span> <span data-ttu-id="bbcfa-113">يتم إعداد الصنف ليتم تتبعه على أنه صنف وزن التعبئة بالرؤية الجزئية.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-113">The item is set up to be tracked as a Partial visibility catch weight item.</span></span>


<span data-ttu-id="bbcfa-114">لديك صندوقين من المنتج ولديهم وزن مسجل قيمته 16 كجم.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-114">You have two boxes of the product and they have a registered weight of 16 kg.</span></span> <span data-ttu-id="bbcfa-115">إذا اختار عامل المستودع أحد الصناديق ووزنه، وتم التقاط الوزن على أنه 9 كجم، فإن الصندوق المتبقي يزن 7 كجم.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-115">If a warehouse worker picks and weighs one of the boxes, and the weight is captured as 9 kg, the remaining box will weigh 7 kg.</span></span> <span data-ttu-id="bbcfa-116">ومع ذلك، لأن 7 كجم أقل من الحد الأدنى للوزن، يقوم النظام بإجراء تعديل تلقائي لزيادة وزن المخزون الفعلي بمقدار 1 كجم.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-116">However, because 7 kg is below the minimum weight, the system performs an automatic adjustment to increase the weight of the on-hand inventory by 1 kg.</span></span>

<span data-ttu-id="bbcfa-117">لإعداد الحسابات التي يتم ترحيل هذه التعديلات إليها، انتقل إلى **إدارة التكاليف > إعداد سياسات تكامل دفتر الأستاذ > ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="bbcfa-117">To set up the accounts that these adjustments are posted to, go to **Cost management > Ledger integration policies setup > Posting**.</span></span>
<span data-ttu-id="bbcfa-118">بعد ذلك، في علامة التبويب **المخزون** حدد الحسابات التالية:</span><span class="sxs-lookup"><span data-stu-id="bbcfa-118">Then, on the **Inventory** tab, define the following accounts:</span></span>

-   <span data-ttu-id="bbcfa-119">فقد وزن التعبئة</span><span class="sxs-lookup"><span data-stu-id="bbcfa-119">Catch weight loss</span></span> 

-   <span data-ttu-id="bbcfa-120">ربح وزن التعبئة</span><span class="sxs-lookup"><span data-stu-id="bbcfa-120">Catch weight profit</span></span> 
