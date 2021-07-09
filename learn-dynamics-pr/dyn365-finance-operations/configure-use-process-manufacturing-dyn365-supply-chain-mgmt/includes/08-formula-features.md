---
ms.openlocfilehash: e0f3aa79db791bd0eae6e9bd1981c1d7d0da16a3
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6072996"
---
<span data-ttu-id="5230c-101">تصف الأقسام التالية الميزات الفريدة المتوفرة في معادلة ما.</span><span class="sxs-lookup"><span data-stu-id="5230c-101">The following sections describe the unique features that are available on a formula.</span></span> 

<span data-ttu-id="5230c-102">**التحكم في الإصدار**</span><span class="sxs-lookup"><span data-stu-id="5230c-102">**Version control**</span></span>

<span data-ttu-id="5230c-103">كما هو الحال مع قوائم مكونات الصنف (BOM)، يدعم التحكم في إصدار المعادلة التخلص التدريجي من المكونات القديمة بحيث يمكن البدء في إنتاج المكونات الجديدة أو شرائها ولتمكين اختيار الإصدارات البديلة، اعتماداً على احتياجات الإنتاج أو التخطيط المحددة.</span><span class="sxs-lookup"><span data-stu-id="5230c-103">As with BOMs, formula version control supports the phasing out of old ingredients so that new ingredients can start to be produced or bought and to enable the selection of alternative versions, depending on the specific production or planning needs.</span></span>

<span data-ttu-id="5230c-104">**المعادلة الرسومية**</span><span class="sxs-lookup"><span data-stu-id="5230c-104">**Graphical formula**</span></span>

<span data-ttu-id="5230c-105">يتيح لك مصمم المعادلة اختيار العمل باستخدام بنية المعادلة بتنسيق رسومي يعرض إصدارات المعادلة المتوفرة للصنف المحدد إلى جانب المنتجات المساعدة والمنتجات الثانوية لتلك المعادلة.</span><span class="sxs-lookup"><span data-stu-id="5230c-105">The formula designer lets you choose to work with the formula structure in a graphical format, which shows the formula versions that are available for the selected item along with the coproducts and by-products for that formula.</span></span>

<span data-ttu-id="5230c-106">**حجم المعادلة**</span><span class="sxs-lookup"><span data-stu-id="5230c-106">**Formula size**</span></span>

<span data-ttu-id="5230c-107">يستخدم إصدار المعادلة حجم معادلة أساسي مثل الحقل **لكل كمية** في سطور المعادلة.</span><span class="sxs-lookup"><span data-stu-id="5230c-107">The formula version uses a base formula size as the **Per quantity** field on the formula lines.</span></span> <span data-ttu-id="5230c-108">يؤدي تحديث هذا الحقل إلى تحديث جميع الحقول **لكل كمية** في سطور المعادلة.</span><span class="sxs-lookup"><span data-stu-id="5230c-108">Updating this field updates all the **Per quantity** fields on the formula lines.</span></span>

<span data-ttu-id="5230c-109">**مضاعفات المعادلة**</span><span class="sxs-lookup"><span data-stu-id="5230c-109">**Formula multiples**</span></span>

<span data-ttu-id="5230c-110">يستخدم إصدار المعادلة المضاعفات لتحديد حجم أمر الدُفعة المسموح به للإنتاج من خلال التخطيط الرئيسي أو أمر الدُفعة اليدوي.</span><span class="sxs-lookup"><span data-stu-id="5230c-110">The formula version uses multiples to determine the batch order size that is allowed for production through master planning or manual batch order.</span></span> <span data-ttu-id="5230c-111">يجب أن يلبي حجم المعادلة في الإصدار متطلبات المضاعف.</span><span class="sxs-lookup"><span data-stu-id="5230c-111">The formula size on the version must meet the multiple requirement.</span></span>

<span data-ttu-id="5230c-112">**العائد**</span><span class="sxs-lookup"><span data-stu-id="5230c-112">**Yield**</span></span>

<span data-ttu-id="5230c-113">يمكنك تحديد عائد على إصدارات المعادلات يقوم بتطبيق عامل العائد على جميع سطور المعادلة عندما يتم إنشاء أمر دُفعة للصنف المركب.</span><span class="sxs-lookup"><span data-stu-id="5230c-113">You can specify a yield on the formula versions, which applies a yield factor to all formula lines when a batch order is created for the formula item.</span></span> <span data-ttu-id="5230c-114">يتم حساب العائد على أنه *(المخرجات الفعلية / المخرجات النظرية) \* 100%*.</span><span class="sxs-lookup"><span data-stu-id="5230c-114">The yield is calculated as the *(actual output / theoretical output) \* 100%*.</span></span>

<span data-ttu-id="5230c-115">**إصدارات المعادلة المعتمدة على الكمية**</span><span class="sxs-lookup"><span data-stu-id="5230c-115">**Quantity-dependent formula versions**</span></span>

<span data-ttu-id="5230c-116">يمكن استخدام الحقل **من حجم المعادلة** (في إصدار المعادلة) للتحكم في إصدار المعادلة الذي سيتم استخدامه في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="5230c-116">The **From formula size** field (on the formula version) can be used for controlling which formula version is to be used in a production.</span></span> <span data-ttu-id="5230c-117">على سبيل المثال، إذا تم طب أقل من 500 كجم من الصنف المركب، فسيتم استخدام الإصدار 1، وعندما يتم طلب أكثر من 500 كجم، يتم استخدام الإصدار 2 بحجم معادلة 1000.</span><span class="sxs-lookup"><span data-stu-id="5230c-117">For example, if less than 500 kg of a formula item is ordered, Version 1 is used; when more than 500 kg is ordered, Version 2 with a formula size of 1000 is used.</span></span>

<span data-ttu-id="5230c-118">**إجمالي توزيع التكلفة**</span><span class="sxs-lookup"><span data-stu-id="5230c-118">**Total cost allocation**</span></span>

<span data-ttu-id="5230c-119">يوزع الخيار **إجمالي توزيع التكلفة** التكلفة الإجمالية للإنتاج عبر المنتجات المساعدة والصنف المركب.</span><span class="sxs-lookup"><span data-stu-id="5230c-119">The **Total cost allocation** option allocates the total cost of production across the coproducts and the formula item.</span></span> <span data-ttu-id="5230c-120">بالنسبة إلى صنف التخطيط، يتم توزيع التكلفة بالكامل عبر المنتجات المساعدة.</span><span class="sxs-lookup"><span data-stu-id="5230c-120">For the planning item, the entire cost is allocated across the coproducts.</span></span> <span data-ttu-id="5230c-121">عند تحديد هذه المعلمة، يجب إدخال المنتجات المساعدة مع توزيع التكلفة قبل الموافقة على المعادلة وتنشيطها.</span><span class="sxs-lookup"><span data-stu-id="5230c-121">When selecting this parameter, you must enter the coproducts with the cost allocation before the formula can be approved and activated.</span></span>

<span data-ttu-id="5230c-122">**استخدام للحساب**</span><span class="sxs-lookup"><span data-stu-id="5230c-122">**Use for calculation**</span></span>

<span data-ttu-id="5230c-123">يحدد الخيار **استخدام للحساب** حجم المعادلة الذي يجب استخدامه إذا كانت هناك أصناف خاضعة للرقابة بالنسبة المئوية لحساب الكمية في سطر المعادلة.</span><span class="sxs-lookup"><span data-stu-id="5230c-123">The **Use for calculation** option determines which formula size to use if there are percent-controlled items to calculate quantity on the formula line.</span></span>

<span data-ttu-id="5230c-124">**مجموعة الخطط**</span><span class="sxs-lookup"><span data-stu-id="5230c-124">**Plan group**</span></span>

<span data-ttu-id="5230c-125">تساعد مجموعات الخطط في استبدال الأصناف بناءً على الأولوية.</span><span class="sxs-lookup"><span data-stu-id="5230c-125">Plan groups help substitute items based on a priority.</span></span> <span data-ttu-id="5230c-126">تكون الأصناف المرتبطة بالمجموعة قابلة للتبديل بناءً على تعريف الأولوية.</span><span class="sxs-lookup"><span data-stu-id="5230c-126">Items that are associated with the group are interchangeable based on the priority definition.</span></span>

<span data-ttu-id="5230c-127">**الاستهلاك المرحلي**</span><span class="sxs-lookup"><span data-stu-id="5230c-127">**Step consumption**</span></span>

<span data-ttu-id="5230c-128">تساعد وظيفة **الاستهلاك المرحلي** في إعداد قواعد استهلاك معقدة (غير خطية) دون الحاجة إلى إعداد عدة BOM/معادلات.</span><span class="sxs-lookup"><span data-stu-id="5230c-128">The **Step consumption** functionality helps set up complex (non-linear) consumption rules without the need for setting up multiple BOM/formulas.</span></span>


<span data-ttu-id="5230c-129">**سطور قابلة للتوسيع**</span><span class="sxs-lookup"><span data-stu-id="5230c-129">**Scalable lines**</span></span>

<span data-ttu-id="5230c-130">يشير الخيار **سطور قابلة للتوسيع** إلى ما إذا كان سطر المعادلة قابلاً للتوسيع بناءً على الحقل **حجم المعادلة** أو سطور معادلة أخرى قابلة للتوسيع.</span><span class="sxs-lookup"><span data-stu-id="5230c-130">The **Scalable lines** option indicates if a formula line is scalable based on the **Formula size** field or other scalable formula lines.</span></span> <span data-ttu-id="5230c-131">إذا تم تحديث الحقل **حجم المعادلة** أو كمية سطر معادلة آخر قابل للتوسيع، فسيتم تعديل جميع السطور القابلة للتوسيع وفقاً لذلك للحفاظ على النسب الحالية.</span><span class="sxs-lookup"><span data-stu-id="5230c-131">If the **Formula size** field or another scalable formula line quantity is updated, all scalable lines will adjust accordingly to maintain the current ratios.</span></span>

<span data-ttu-id="5230c-132">شاهد مقطع الفيديو التالي لمشاهدة عرض توضيحي لكيفية التعامل مع سطور المعادلة القابلة للتوسيع.</span><span class="sxs-lookup"><span data-stu-id="5230c-132">Watch the following video to see a demonstration of how to work with scalable formula lines.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4a8if]



