---
ms.openlocfilehash: da751d9f89219b62c29ce6b25f7f01c90a78482b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073021"
---

<span data-ttu-id="f4bb3-101">يغطي تحديد تكاليف الإصدار التلقائي في Supply Chain Management المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="f4bb3-101">Backflush costing in Supply Chain Management cover the following tasks:</span></span>

-   <span data-ttu-id="f4bb3-102">يسمح بإعداد تقارير مبسطة عن الموارد المادية والتشغيلية، مثل الإبلاغ عن الاستهلاك في الصناديق الفارغة أو عدم الإبلاغ عن الاستهلاكات والقضاء على الحاجة إلى الإبلاغ عن استخدام موارد التشغيل.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-102">It allows simplified reporting on material and operation resources, such as reporting consumption on empty bins or else not reporting consumptions and eliminating the need for reporting usage of operation resources</span></span>

-   <span data-ttu-id="f4bb3-103">يقدِّر ناتج تدفق الإنتاج (الكميات المنتجة) بالتكلفة القياسية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-103">Values the production flow output (quantities produced) at the product's standard cost.</span></span>

-   <span data-ttu-id="f4bb3-104">يستوعب وينطبق على حساب WIP لتدفق الإنتاج وتكاليف عمليات التحويل القياسية (تكلفة التصنيع المباشرة وغير المباشرة) لمخرجات الإنتاج من تدفق إنتاج.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-104">Absorbs and applies to the production flow's WIP account, the standard conversions costs (direct and indirect manufacturing cost) for the production outputs from a production flow.</span></span>

-   <span data-ttu-id="f4bb3-105">يسمح بعملية تحديد تكاليف الإصدار التلقائي لنهاية الفترة، لحساب الفروق على التكلفة القياسية لكميات المنتجات التي تم إنتاجها للفترة، وتصحيح الوضع المالي (بالنسبة إلى إدخالات دفتر اليومية المحذوفة لدورة المنتج).</span><span class="sxs-lookup"><span data-stu-id="f4bb3-105">Allows an end-of-period backflush costing process, for computing the variances to standard cost for quantities of products that are produced for the period, and the correction of the financial situation (relative to the omitted journal entries for the product cycle).</span></span>
    
-   <span data-ttu-id="f4bb3-106">تنفيذ حساب BOM للأصناف التي تم إنتاجها من خلال تدفقات الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-106">Performs BOM calculation for items that are produced through production flows.</span></span>

-   <span data-ttu-id="f4bb3-107">يحسب تكلفة نقل المواد المباشرة إلى العمل الجاري، للمنتجات التي تساهم في تدفق الإنتاج، ولكن لا يتم الإبلاغ عن التدفق المادي له في تدفق الإنتاج أو الاحتفاظ به في إدخالات دفتر اليومية المبسطة لتحديد تكاليف الإصدار التلقائي.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-107">Accounts for moving direct material cost to work in progress, for products that are contributed to production flow, but whose physical flow in the production flow is not reported or maintained in simplified backflush costing journal entries.</span></span>

-   <span data-ttu-id="f4bb3-108">يقوم بإجراء محاسبة التكاليف من خلال استبدال تعريف تدفق الإنتاج للمسارات.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-108">Performs cost accounting through substituting the production flow definition for routes.</span></span>

-   <span data-ttu-id="f4bb3-109">يقوم بإجراء محاسبة التكاليف لتكلفة المواد المباشرة الناتجة عن المنتجات التي تتم المحافظة على تدفقها المادي في تدفق الإنتاج من خلال المخزون الفعلي (بدون الإصدار التلقائي).</span><span class="sxs-lookup"><span data-stu-id="f4bb3-109">Performs cost accounting of the direct material cost resulting from products whose physical flow in the production flow is maintained through on-hand inventory (no backflush).</span></span>

<span data-ttu-id="f4bb3-110">يؤدي الدمج الدوري لتكلفة تدفق الإنتاج أو تحديد تكاليف الإصدار التلقائي إلى إعادة حساب التكلفة الفعلية للمواد والمنتجات في WIP استناداً إلى حالة وظائف كانبان ووحدات معالجة المواد في تدفق الإنتاج وتحديد الفروق للمنتجات التي يوفرها تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-110">The periodic consolidation of the cost for a production flow or backflush costing recalculates the actual cost of material and products in WIP based on the status of kanban jobs and handling units in the production flow and determines variances for the products that are supplied by the production flow.</span></span>

## <a name="end-of-period---backflush-costing"></a><span data-ttu-id="f4bb3-111">نهاية الفترة - تحديد تكاليف الإصدار التلقائي</span><span class="sxs-lookup"><span data-stu-id="f4bb3-111">End of period - backflush costing</span></span>

<span data-ttu-id="f4bb3-112">في نهاية فترة تحديد التكلفة، يتم تشغيل تحديد تكاليف الإصدار التلقائي للفترة لجميع تدفقات الإنتاج للكيان القانوني في الدُفعة نفسها التي تم تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-112">At the end of a costing period, backflush costing is run for the period for all production flows of the legal entity in the same batch run.</span></span> <span data-ttu-id="f4bb3-113">عند بدء حساب تحديد تكاليف الإصدار التلقائي، يجب تحديد التاريخ الأخير لفترة تحديد تكاليف الإصدار التلقائي.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-113">When backflush costing calculation is started, the last date of the backflush costing period must be selected.</span></span> <span data-ttu-id="f4bb3-114">يتم تشغيل تحديد تكاليف الإصدار التلقائي من صفحة **حساب تحديد تكاليف الإصدار التلقائي** أو كوظيفة دفعية.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-114">Backflush costing is run either from the **Backflush costing calculation** page or as a batch job.</span></span>

<span data-ttu-id="f4bb3-115">ما لم تبدأ الوظيفة في نهاية يوم التصنيع، يجب عليك دائماً تحديد يوم في الماضي للوظيفة.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-115">Unless the job is started at the end of the manufacturing day, you should always select a day in the past for the job.</span></span> <span data-ttu-id="f4bb3-116">لا يمكن ترحيل الحركات إلى فترة (يوم) تم فيها تشغيل حساب تحديد تكاليف الإصدار التلقائي.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-116">It is not possible to post transactions to a period (day) where the backflush costing calculation was run.</span></span>

<span data-ttu-id="f4bb3-117">تنفذ عملية تحديد تكاليف الإصدار التلقائي الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f4bb3-117">The backflush costing process implements the following steps:</span></span>

1.  <span data-ttu-id="f4bb3-118">تحديد الكميات غير المستخدمة لتدفق الإنتاج اعتباراً من تاريخ انتهاء الفترة.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-118">Determine the production flow's unused quantities as of the period end date.</span></span>

2.  <span data-ttu-id="f4bb3-119">حساب صافي الاستخدام المحقق لتدفق الإنتاج خلال الفترة.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-119">Calculate the production flow's net realized usage over the period.</span></span>

3.  <span data-ttu-id="f4bb3-120">مسح WIP من استهلاك الموارد والمنتجات المحققة.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-120">Clear the WIP from the realized resource consumptions and products.</span></span>

4.  <span data-ttu-id="f4bb3-121">حساب فروق الإنتاج حسب التكلفة القياسية لكل مجموعة تكلفة.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-121">Calculate the production variances to standard cost for each cost group.</span></span>

<span data-ttu-id="f4bb3-122">بعد تشغيل عملية تحديد تكاليف الإصدار التلقائي، يمكن عرض الكميات غير المستخدمة في تاريخ تشغيل التكلفة من عرض WIP لتدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f4bb3-122">After the backflush costing process is run, the unused quantities at the date of the costing run can be viewed from the production flow's WIP display.</span></span>
