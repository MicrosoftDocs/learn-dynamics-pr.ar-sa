---
ms.openlocfilehash: 5a495d1d484baee79521d19e4db5559fd4f204cf
ms.sourcegitcommit: 9b600794e2cc61eeb0409f924725f765f528e8b1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6072652"
---
<span data-ttu-id="1176d-101">تُستخدم مجموعات قواعد الخطورة لحساب خطورة أمر التغيير تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="1176d-101">Severity rule sets are used to calculate the severity of the change order automatically.</span></span> <span data-ttu-id="1176d-102">عندما يقوم النظام بتقييم خطورة، فإنه يعالج القواعد التي تم تكوينها في المعلمات.</span><span class="sxs-lookup"><span data-stu-id="1176d-102">When the system evaluates a severity, it processes the rules that are configured in the parameters.</span></span> 

<span data-ttu-id="1176d-103">لاستخدام مجموعات قواعد الخطورة، افتح صفحة **المعلمات**، وقم بتعيين حقل **قاعدة الخطورة** إلى **حساب** أو **حساب تلقائياً**.</span><span class="sxs-lookup"><span data-stu-id="1176d-103">To use severity rule sets, open the **Parameters** page and set the **Severity rule** field to **Calculate** or **Calculate automatically**.</span></span>

<span data-ttu-id="1176d-104">**إدارة التغيير الهندسي** > **الإعداد** > **معلمات إدارة التغيير الهندسي**.</span><span class="sxs-lookup"><span data-stu-id="1176d-104">**Engineering change management** > **Setup** > **Engineering change management parameters**.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="1176d-105">[![لقطة شاشة لصفحة معلمات إدارة التغيير الهندسي، علامة التبويب إدارة التغيير الهندسي.](../media/engineering-change-management-parameters.png)](../media/engineering-change-management-parameters.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="1176d-105">[![Screenshot of the Engineering change management parameters page Engineering change management tab.](../media/engineering-change-management-parameters.png)](../media/engineering-change-management-parameters.png#lightbox)</span></span>

<span data-ttu-id="1176d-106">يمكن تحديد القواعد لتطبيقها على مستويات الخطورة المختلفة التي تم إعدادها.</span><span class="sxs-lookup"><span data-stu-id="1176d-106">Rules can be selected to apply to the different severities that are set up.</span></span> <span data-ttu-id="1176d-107">يعالج النظام القواعد التي تظهر فيها على الصفحة، من أعلى إلى أسفل.</span><span class="sxs-lookup"><span data-stu-id="1176d-107">The system processes the rules in which they appear on the page, from top to bottom.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="1176d-108">[![لقطة شاشة لصفحة مجموعات قواعد خطورة التغيير الهندسي. درجة الخطورة عالية جداً، والقاعدة هي EngChgEcmSeverityRuleBom والاسم هو تغيير قائمة مكونات الصنف.](../media/engineering-change-severity-rules.png)](../media/engineering-change-severity-rules.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="1176d-108">[![Screenshot of the Engineering change severity rule sets page. Severity is Very high, Rule is EngChgEcmSeverityRuleBom and Name is BOM change.](../media/engineering-change-severity-rules.png)](../media/engineering-change-severity-rules.png#lightbox)</span></span>

<span data-ttu-id="1176d-109">لإنشاء مجموعة قواعد، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1176d-109">To create a rule set, follow these steps:</span></span>

1. <span data-ttu-id="1176d-110">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="1176d-110">Select **New**.</span></span>

1. <span data-ttu-id="1176d-111">حدد **الخطورة** من القائمة المنسدلة لدرجات الخطورة التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="1176d-111">Select the **Severity** from the drop-down list of the severities that have been created.</span></span>

1. <span data-ttu-id="1176d-112">حدد **إضافة** في علامة التبويب السريعة **قواعد**.</span><span class="sxs-lookup"><span data-stu-id="1176d-112">Select **Add** in the **Rules** FastTab.</span></span>

1. <span data-ttu-id="1176d-113">حدد قاعدة من القائمة المنسدلة **قاعدة**.</span><span class="sxs-lookup"><span data-stu-id="1176d-113">Select a rule from the **Rule** drop-down list.</span></span> <span data-ttu-id="1176d-114">الاختيارات هي:</span><span class="sxs-lookup"><span data-stu-id="1176d-114">The choices are:</span></span>

    - <span data-ttu-id="1176d-115">التأثير الإجمالي للتغيير</span><span class="sxs-lookup"><span data-stu-id="1176d-115">The overall impact of the change</span></span>

    - <span data-ttu-id="1176d-116">تغيير المسار</span><span class="sxs-lookup"><span data-stu-id="1176d-116">Route change</span></span>

    - <span data-ttu-id="1176d-117">تغيير السمة</span><span class="sxs-lookup"><span data-stu-id="1176d-117">Attribute change</span></span>

    - <span data-ttu-id="1176d-118">تغيير قائمة مكونات الصنف</span><span class="sxs-lookup"><span data-stu-id="1176d-118">BOM change</span></span>

    - <span data-ttu-id="1176d-119">تغيير المستند</span><span class="sxs-lookup"><span data-stu-id="1176d-119">Document change</span></span>


