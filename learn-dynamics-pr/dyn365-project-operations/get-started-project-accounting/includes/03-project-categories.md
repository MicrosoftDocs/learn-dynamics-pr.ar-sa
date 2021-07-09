---
ms.openlocfilehash: 84e48034480036a705274e25c610113f7cec1c77
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6072929"
---
<span data-ttu-id="4c56a-101">يوفر Project Operations إمكانات فعّالة لتصنيف الإيرادات والمصروفات في المشاريع.</span><span class="sxs-lookup"><span data-stu-id="4c56a-101">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="4c56a-102">تُتيح لك الفئات إمكانية إعداد تقارير حول معاملات المشروع وتحليلها وتعزيز الترحيل إلى دفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="4c56a-102">Categories provide you with the ability to report on and analyze project transactions and drive posting to the general ledger.</span></span>

<span data-ttu-id="4c56a-103">يوضّح الرسم التخطيطي التالي الارتباط بين فئات المعاملات والفئات المشتركة وفئات المشاريع.</span><span class="sxs-lookup"><span data-stu-id="4c56a-103">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span>

![رسم تخطيطي يُبيّن الارتباط بين فئات المعاملات والفئات المشتركة وفئات المشاريع.](../media/project-categories-cc.png)

<span data-ttu-id="4c56a-105">وتمثّل فئات المعاملات التجميعات الأساسية لمعاملات المشروع.</span><span class="sxs-lookup"><span data-stu-id="4c56a-105">Transaction categories are the basic groupings for project transactions.</span></span> <span data-ttu-id="4c56a-106">وتندرج ضمن هذا التجميع مجموعة من الفئات المشتركة التي يمكن مشاركتها عبر التطبيقات والوحدات النمطية.</span><span class="sxs-lookup"><span data-stu-id="4c56a-106">Within that grouping is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="4c56a-107">وتُشكِّل فئات المشاريع مستوى الفئات الأكثر دقة وتتعلق تحديداً بالكيان القانوني والوحدة النمطية والتطبيق.</span><span class="sxs-lookup"><span data-stu-id="4c56a-107">Project categories are the most granular level of categories and are specific to legal entity, module, and application.</span></span>

## <a name="transaction-categories"></a><span data-ttu-id="4c56a-108">فئات المعاملات</span><span class="sxs-lookup"><span data-stu-id="4c56a-108">Transaction categories</span></span>
<span data-ttu-id="4c56a-109">تُمثّل فئات المعاملات التجميع الأساسي لمعاملات المشروع ولا تتعلق بنوع الشركة أو المعاملة.</span><span class="sxs-lookup"><span data-stu-id="4c56a-109">Transaction categories represent the basic grouping for project transactions and are not company or transaction type specific.</span></span> <span data-ttu-id="4c56a-110">على سبيل المثال، تستخدم شركة Contoso Robotics فئات التصميم والسفر والتثبيت ومعاملة الخدمة لتجميع معاملات المشروع.</span><span class="sxs-lookup"><span data-stu-id="4c56a-110">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group project transactions.</span></span>

<span data-ttu-id="4c56a-111">يمكنك تحديد فئات المعاملات في Project Operations:</span><span class="sxs-lookup"><span data-stu-id="4c56a-111">You can define transaction categories in Project Operations:</span></span>

1.  <span data-ttu-id="4c56a-112">انتقل إلى **الإعدادات > فئات المعاملات** لفتح الصفحة.</span><span class="sxs-lookup"><span data-stu-id="4c56a-112">Go to **Settings > Transaction Categories** to open the page.</span></span>
2.  <span data-ttu-id="4c56a-113">يمكنك إنشاء فئة معاملة جديدة من خلال تحديد **جديد** أو **استيراد من Excel**.</span><span class="sxs-lookup"><span data-stu-id="4c56a-113">Create a new transaction category by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="4c56a-114">الفئات المشتركة</span><span class="sxs-lookup"><span data-stu-id="4c56a-114">Shared categories</span></span>
<span data-ttu-id="4c56a-115">يستخدم Microsoft Dynamics 365 مفهوم الفئات المشتركة لتصنيف المصروفات في تطبيقات مختلفة، مثل Finance وSupply Chain Management وProject Operations.</span><span class="sxs-lookup"><span data-stu-id="4c56a-115">Microsoft Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as  Finance, Supply Chain Management, and Project Operations.</span></span> 

<span data-ttu-id="4c56a-116">يُنشئ Project Operations تلقائياً لكل فئة معاملة يتم إنشاؤها أربع فئات مشتركة ذات صلة:</span><span class="sxs-lookup"><span data-stu-id="4c56a-116">For each Transaction category that is created, Project Operations automatically creates four related Shared categories:</span></span>

- <span data-ttu-id="4c56a-117">**الساعات‬**</span><span class="sxs-lookup"><span data-stu-id="4c56a-117">**Hours**</span></span>
- <span data-ttu-id="4c56a-118">**المصروفات**</span><span class="sxs-lookup"><span data-stu-id="4c56a-118">**Expense**</span></span>
- <span data-ttu-id="4c56a-119">**الرسوم**</span><span class="sxs-lookup"><span data-stu-id="4c56a-119">**Fee**</span></span>
- <span data-ttu-id="4c56a-120">**الصنف**</span><span class="sxs-lookup"><span data-stu-id="4c56a-120">**Item**</span></span>

<span data-ttu-id="4c56a-121">يمكنك مراجعة الفئات المشتركة وتعديلها من خلال الانتقال إلى **إدارة المشاريع والمحاسبة > الإعداد > الفئات > الفئات المشتركة**.</span><span class="sxs-lookup"><span data-stu-id="4c56a-121">You can review and adjust the shared categories by going to **Project management and accounting > Setup > Categories > Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="4c56a-122">فئات المشاريع</span><span class="sxs-lookup"><span data-stu-id="4c56a-122">Project categories</span></span>
<span data-ttu-id="4c56a-123">تعتبر فئات المشاريع المستوى الأكثر دقة لتكوين الفئات ويجب تكوينها بشكل منفصل لكل شركة من خلال محاسب المشروع.</span><span class="sxs-lookup"><span data-stu-id="4c56a-123">Project categories represent the most granular level of category configuration and must be configured separately, and for each company, by a project accountant.</span></span>

1.  <span data-ttu-id="4c56a-124">انتقل إلى **إدارة المشاريع والمحاسبة‬‬‏‫ > الإعداد > الفئات > فئات المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="4c56a-124">Go to **Project management and accounting > Setup > Categories > Project categories**.</span></span>
2.  <span data-ttu-id="4c56a-125">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="4c56a-125">Select **New**.</span></span>
3.  <span data-ttu-id="4c56a-126">حدد **معرّف الفئة** للفئة المشتركة التي أنشأتها في القسم السابق.</span><span class="sxs-lookup"><span data-stu-id="4c56a-126">Select the **Category ID** of the Shared category that you created in the previous section.</span></span> <span data-ttu-id="4c56a-127">يُتيح لك Project Operations استخدام تلك الفئات المشتركة المقترنة بفئات المعاملات فقط.</span><span class="sxs-lookup"><span data-stu-id="4c56a-127">Project Operations allows you to use only those shared categories that are associated with transaction categories.</span></span>
4.  <span data-ttu-id="4c56a-128">حدد ‏‫مجموعة الفئات.</span><span class="sxs-lookup"><span data-stu-id="4c56a-128">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="4c56a-129">مجموعات الفئات</span><span class="sxs-lookup"><span data-stu-id="4c56a-129">Category groups</span></span>
<span data-ttu-id="4c56a-130">تُستخدم مجموعات الفئات لمشاركة الخصائص، وملفات تعريف الترحيل بشكل أساسي، بين فئات المشاريع ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="4c56a-130">Category groups are used to share properties, primarily posting profiles, between related project categories.</span></span> <span data-ttu-id="4c56a-131">يجب أن يكون هناك مجموعة فئات واحدة على الأقل لكل نوع معاملة ويتم تعيين مجموعة لكل فئة مشاريع.</span><span class="sxs-lookup"><span data-stu-id="4c56a-131">At least one category group must exist for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="4c56a-132">يتم تحديد مواصفات الترحيل في Project Operations وفقاً لقواعد ملفات تعريف تكلفة المشروع وإيراداته وفئات المشاريع ومجموعات الفئات.</span><span class="sxs-lookup"><span data-stu-id="4c56a-132">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="4c56a-133">يمكنك إعداد مجموعات الفئات من خلال **إدارة المشاريع والمحاسبة > الإعداد > الفئات > مجموعات الفئات**.</span><span class="sxs-lookup"><span data-stu-id="4c56a-133">You can set up category groups in **Project management and accounting > Setup > Categories > Category groups**.</span></span>
