---
ms.openlocfilehash: f0cd3a3571359fc22e7750bb5c94b1e5cea79b3d
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073707"
---
<span data-ttu-id="5a939-101">هناك العديد من المكونات التي يجب إعدادها لاستخدام lean manufacturing في Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="5a939-101">There are several components that need to be set up to use lean manufacturing in Supply Chain Management.</span></span> <span data-ttu-id="5a939-102">ستناقش هذه الوحدة المكونات ووظائفها في lean manufacturing.</span><span class="sxs-lookup"><span data-stu-id="5a939-102">This unit will discuss the components and their functionality in lean manufacturing.</span></span> 

![<span data-ttu-id="5a939-103">رسم تخطيطي للعملية والمكونات التي سيتم إعدادها في lean manufacturing.</span><span class="sxs-lookup"><span data-stu-id="5a939-103">Diagram of the process and components to be set up in lean manufacturing.</span></span> ](../media/process.png)



# <a name="lean-manufacturing-parameters"></a><span data-ttu-id="5a939-104">محددات Lean manufacturing</span><span class="sxs-lookup"><span data-stu-id="5a939-104">Lean manufacturing parameters</span></span>

<span data-ttu-id="5a939-105">انتقل إلى **التحكم بالإنتاج > إعداد > محددات التحكم في الإنتاج** وحدد علامة التبويب **Lean manufacturing**.</span><span class="sxs-lookup"><span data-stu-id="5a939-105">Go to **Production control > Setup > Production control parameters** and select the **Lean manufacturing** tab.</span></span>

<span data-ttu-id="5a939-106">في الحقل **إرشادات الإنتاج**، يمكنك تحديد نوع المستند المستخدم لإرشادات الإنتاج التي يتم عرضها على لوحة كانبان.</span><span class="sxs-lookup"><span data-stu-id="5a939-106">In the **Production instruction** field, you can select the type of document that is used for production instructions that are displayed on the kanban board.</span></span>
 
## <a name="production-flow-costing"></a><span data-ttu-id="5a939-107">تكلفة تدفق الإنتاج</span><span class="sxs-lookup"><span data-stu-id="5a939-107">Production flow costing</span></span>

<span data-ttu-id="5a939-108">يعطل Lean manufacturing مفاهيم التكلفة التقليدية لتكلفة الوظيفة لأن سياق أمر الإنتاج غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="5a939-108">Lean manufacturing disrupts the traditional cost concepts of job costing because the context of a production order is not available.</span></span>
<span data-ttu-id="5a939-109">يستخدم Lean manufacturing لـ Supply Chain Management تدفق الإنتاج كمُراكم للتكلفة.</span><span class="sxs-lookup"><span data-stu-id="5a939-109">Lean manufacturing for Supply Chain Management uses the production flow as the cost accumulator.</span></span>

<span data-ttu-id="5a939-110">يتم تعقب تكلفة المواد والمنتجات شبه المنتهية والمنتجات المنتهية لكل صنف ومجموعة تكلفة.</span><span class="sxs-lookup"><span data-stu-id="5a939-110">Cost of material and semi-finished and finished products are tracked for each item and cost group.</span></span> <span data-ttu-id="5a939-111">يتم تعقب العمل قيد التنفيذ (WIP) لكل تدفق إنتاج.</span><span class="sxs-lookup"><span data-stu-id="5a939-111">Work in process (WIP) is tracked for every production flow.</span></span>

<span data-ttu-id="5a939-112">لإعداد حسابات WIP للتعاقد من الباطن، انتقل إلى **التحكم بالإنتاج > إعداد > الإنتاج > مجموعات الإنتاج**، وقم بتوسيع الخيار **دفتر الأستاذ - تعاقد من الباطن محدود الفاقد**، ثم قم بتعيين حسابات دفتر الأستاذ.</span><span class="sxs-lookup"><span data-stu-id="5a939-112">To set up WIP accounts for subcontracting, go to **Production control > Setup > Production > Production groups**, expand the **Ledger-Lean subcontracting** option, and then assign ledger accounts.</span></span>

![لقطة شاشة لخيار دفتر الأستاذ - تعاقد من الباطن محدود الفاقد في صفحة مجموعات الإنتاج.](../media/wip-1.png)


<span data-ttu-id="5a939-114">تحدد مجموعة الإنتاج مجموعة الحسابات المستخدمة للترحيلات المالية المرتبطة بتدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="5a939-114">The production group defines the set of accounts that are used for the financial postings that are related to the production flow.</span></span> <span data-ttu-id="5a939-115">أهم الحسابات هي حسابات WIP والحسابات المقابلة، والتي تعد أساس حساب الفروق لتدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="5a939-115">The most important accounts are the WIP and Offset accounts, which are the basis of variance calculation for the production flow.</span></span>

## <a name="lean-schedule-group"></a><span data-ttu-id="5a939-116">مجموعة الجداول محدودة الفاقد</span><span class="sxs-lookup"><span data-stu-id="5a939-116">Lean schedule group</span></span>

<span data-ttu-id="5a939-117">يتم تحديد مجموعات الجداول محدودة الفاقد لتجميع المنتجات وتمييزها في جدولة كانبان.</span><span class="sxs-lookup"><span data-stu-id="5a939-117">Lean schedule groups are defined to group and distinguish products in kanban scheduling.</span></span> <span data-ttu-id="5a939-118">يمكن إجراء التجميع كاقتران عام لكل شركة أو يمكن أن يكون محدداً لخلية عمل.</span><span class="sxs-lookup"><span data-stu-id="5a939-118">The grouping can be done as generic association for each company or can be specific to a work cell.</span></span> <span data-ttu-id="5a939-119">تحتوي كل مجموعة على رمز لون معين للإشارة المرئية في صفحة قائمة جدولة كانبان.</span><span class="sxs-lookup"><span data-stu-id="5a939-119">Each group has an assigned color code for visual indication in the kanban scheduling list page.</span></span>

<span data-ttu-id="5a939-120">انتقل إلى **إدارة معلومات المنتج > Lean manufacturing > مجموعات الجداول محدودة الفاقد** لإنشاء مجموعة الجداول ثم تعيين لون وإضافة أصناف الجداول محدودة الفاقد لعرض بطاقات كانبان للأصناف المعينة بألوان مختلفة من أجل رؤية أفضل.</span><span class="sxs-lookup"><span data-stu-id="5a939-120">Go to **Product information management > Lean manufacturing > Lean schedule groups** to create a schedule group and then set a color and add lean schedule items to show kanbans for assigned items with different colors for better visibility.</span></span>

<span data-ttu-id="5a939-121">[![لقطة شاشة لصفحة مجموعات الجداول محدودة الفاقد.](../media/lean-sched-group.png)](../media/lean-sched-group.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="5a939-121">[![Screenshot of the Lean schedule groups page.](../media/lean-sched-group.png)](../media/lean-sched-group.png#lightbox)</span></span>
