---
ms.openlocfilehash: 39650c652348b178d33fc878394b2df0399c182b
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071081"
---
## <a name="financial-dimension-templates"></a><span data-ttu-id="4d2b4-101">قوالب الأبعاد المالية</span><span class="sxs-lookup"><span data-stu-id="4d2b4-101">Financial dimension templates</span></span> 

<span data-ttu-id="4d2b4-102">يمكن استخدام قوالب الأبعاد المالية للنماذج الشائعة التي تستخدمها لتوزيع قيم المستند المصدر.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-102">Financial dimension templates can be used for common patterns that you use to distribute source document amounts.</span></span> 

<span data-ttu-id="4d2b4-103">استخدم الصفحة **قوالب الأبعاد المالية الافتراضية** لإنشاء قالب النسبة المئوية ومجموعات قيم الأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-103">Use the **Financial dimension default templates** page to create a template of percentage and financial dimension value combinations.</span></span> <span data-ttu-id="4d2b4-104">سيتم استخدام المعلومات الموجودة في القالب لعرض قيم الأبعاد المالية الافتراضية عند توزيع مبالغ مستند المصدر.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-104">The information in the template will be used to display default financial dimension values when you distribute source document amounts.</span></span>
 
<span data-ttu-id="4d2b4-105">**دفتر الأستاذ العام > دليل الحسابات > الأبعاد > القوالب الافتراضية للأبعاد المالية**</span><span class="sxs-lookup"><span data-stu-id="4d2b4-105">**General ledger > Chart of accounts > Dimensions > Financial dimension default templates**</span></span>

![لقطة شاشة لصفحة قوالب الأبعاد المالية الافتراضية.](../media/fin-dim-template.png)


## <a name="financial-dimension-sets"></a><span data-ttu-id="4d2b4-107">مجموعات الأبعاد المالية</span><span class="sxs-lookup"><span data-stu-id="4d2b4-107">Financial dimension sets</span></span> 

<span data-ttu-id="4d2b4-108">تتضمن مجموعة الأبعاد المالية إما أبعاداً مالية أو مجموعات أبعاد مالية.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-108">A financial dimension set contains either financial dimensions or financial dimension combinations.</span></span>  <span data-ttu-id="4d2b4-109">السبب الرئيسي لمجموعة الأبعاد المالية هو لأغراض إعداد التقارير.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-109">The main reason for a financial dimension set is for reporting purposes.</span></span>  <span data-ttu-id="4d2b4-110">يمكنك الإبلاغ عن الحسابات المتعددة ومجموعات الأبعاد.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-110">You can report on multiple accounts and dimension combinations.</span></span>  

<span data-ttu-id="4d2b4-111">تشتمل مجموعات الأبعاد المالية على أغراض متعددة.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-111">The financial dimension sets have several purposes.</span></span> <span data-ttu-id="4d2b4-112">ويتم استخدامها لتحديد كيفية تقديم التقارير والاستعلامات المرتبطة بدفتر الأستاذ العام.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-112">They are used to determine how reports and inquiries related to the general ledger are rendered.</span></span> <span data-ttu-id="4d2b4-113">كما تستخدم مجموعات الأبعاد المالية لحساب الأرصدة أثناء عملية الترحيل.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-113">Financial dimension sets are also used to calculate balances during the posting process.</span></span> <span data-ttu-id="4d2b4-114">ويمكن جدولة الأرصدة أيضاً للحساب أو التحديث اليدوي.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-114">Balances can also be scheduled for calculation or manually updated.</span></span>

<span data-ttu-id="4d2b4-115">يتم تخزين الأرصدة استنادا إلى مجموعة الأبعاد المالية ويتم حسابها استنادا إلى الخيار الذي يتم حسابه مع الترحيل أو جدول المجموعة.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-115">Balances are stored based on the financial dimension set and are calculated based on the option to calculate with posting or batch schedule.</span></span> <span data-ttu-id="4d2b4-116">تقوم مجموعات الأبعاد المالية أيضاً بتحريك البيانات المعروضة في الصفحة **قائمة ميزان المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-116">Financial dimension sets also drive the data displayed in the **Trial balance list** page.</span></span>

<span data-ttu-id="4d2b4-117">التسلسل الذي يتم اعتبار مجموعات الأبعاد المالية فيه يؤثر على كيفية فرز الحركات، ويتم تقديم الحقول.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-117">The sequence in which financial dimension sets are considered in reporting affect how transactions are sorted, and fields are presented.</span></span> 

<span data-ttu-id="4d2b4-118">على سبيل المثال، تشير المجموعة "القسم" و"مركز التكلفة" إلى أن نوع بُعد "القسم" هو الأول و"مركز التكلفة" هو الثاني.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-118">For example, the set Department and Cost center indicates that the Department dimension type is first and Cost center second.</span></span> <span data-ttu-id="4d2b4-119">لذلك، فإن المجموعة المالية تعتبر مركبة من "القسم" و"مركز التكلفة".</span><span class="sxs-lookup"><span data-stu-id="4d2b4-119">Therefore, the considered financial set is the composite of Department and Cost center.</span></span> <span data-ttu-id="4d2b4-120">يتم تقديم مبالغ القسم أولا، ويتم عرض مبالغ مركز التكلفة ثانياً.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-120">Department amounts are presented first, and Cost center amounts are presented second.</span></span>

<span data-ttu-id="4d2b4-121">**دفتر الأستاذ العام > دليل الحسابات > الأبعاد > مجموعات الأبعاد المالية**</span><span class="sxs-lookup"><span data-stu-id="4d2b4-121">**General ledger > Chart of accounts > Dimensions > Financial dimension sets**</span></span>
 
![لقطة شاشة لصفحة مجموعات الأبعاد المالية.](../media/fin-dim-set.png)

<span data-ttu-id="4d2b4-123">يمكن استخدام مجموعة الأبعاد المالية المحددة كوحدة أو في شكل أزواج عند الاستعلام عن الحركات المالية أو الإبلاغ عنها.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-123">The defined financial dimension set can be used alone or in pairs when inquiring or reporting on financial transactions.</span></span> <span data-ttu-id="4d2b4-124">ويعتبر تحديد مجموعة الأبعاد المالية الأساسية والثانوية عند تقديم النتائج.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-124">The selection of a primary and secondary financial dimension set is considered when presenting the results.</span></span> 

<span data-ttu-id="4d2b4-125">تفصِّل مجموعة الأبعاد المالية الثانوية الأرقام الخاصة بمجموعة الأبعاد الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-125">The secondary financial dimension set details the figures of the primary dimension set.</span></span> <span data-ttu-id="4d2b4-126">يقتصر تحديد مجموعة الأبعاد المالية الثانوية على التركيز على تلك التي لا تشترك في نوع بُعد بمجموعة أبعاد رئيسية.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-126">The selection of a secondary financial dimension set is limited to focus on those  that do not share a dimension type with a primary dimension set.</span></span> 

<span data-ttu-id="4d2b4-127">لذلك، إذا كانت مجموعة الأبعاد الرئيسية مركبة للحساب الرئيسي والقسم، فلا يمكن تحديدها في المجموعة المالية الثانوية.</span><span class="sxs-lookup"><span data-stu-id="4d2b4-127">Therefore, if the primary dimension set is the composite of Main account and Department, these cannot be select in the secondary financial set.</span></span>



