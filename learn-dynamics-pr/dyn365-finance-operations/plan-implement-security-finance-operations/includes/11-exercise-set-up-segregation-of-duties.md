---
ms.openlocfilehash: 397febf4aef74da4685c3ddbee8c8aa20e18f626
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071274"
---
## <a name="scenario"></a><span data-ttu-id="ef391-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="ef391-101">Scenario</span></span>
<span data-ttu-id="ef391-102">طلبت إدارة الموارد البشرية في USMF قاعدة الفصل بين المهام لمساحة عمل **مزايا الوصول**، و **الموافقة دفتر يومية الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="ef391-102">The HR department of USMF has requested a rule for segregation of duties for the **Access benefits** workspace, and the **Approve production** journal.</span></span> <span data-ttu-id="ef391-103">يجب أن تقوم بإنشاء القاعدة في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="ef391-103">You must create the rule in Finance and Operations apps.</span></span>

<span data-ttu-id="ef391-104">أكمل الإجراء التالي لإنشاء قاعدة.</span><span class="sxs-lookup"><span data-stu-id="ef391-104">Complete the following procedure to create a rule.</span></span> <span data-ttu-id="ef391-105">يجب أن تكون مسؤول نظام لإكمال الإجراء.</span><span class="sxs-lookup"><span data-stu-id="ef391-105">You must be a system administrator to complete the procedure.</span></span> <span data-ttu-id="ef391-106">إن شركة بيانات العرض التوضيحي المستخدمة لإنشاء هذا الاجراء هي DAT.</span><span class="sxs-lookup"><span data-stu-id="ef391-106">The demo data company used to create this procedure is DAT.</span></span>

1. <span data-ttu-id="ef391-107">انتقل إلى **إدارة النظام** > **الأمان** > **الفصل بين المهام** > **قواعد الفصل بين المهام**.</span><span class="sxs-lookup"><span data-stu-id="ef391-107">Go to **System administration** > **Security** > **Segregation of duties** > **Segregation of duties rules**.</span></span>
1. <span data-ttu-id="ef391-108">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="ef391-108">Select **New**.</span></span>
1. <span data-ttu-id="ef391-109">في الحقل **الاسم**، أدخِل اسماً للقاعدة.</span><span class="sxs-lookup"><span data-stu-id="ef391-109">In the **Name** field, enter a name for the rule.</span></span>
1. <span data-ttu-id="ef391-110">في الحقل **المهمة الأولى**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="ef391-110">In the **First duty** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="ef391-111">في القائمة، ابحث عن المهمة الأولى التي يتم التحكم فيها بواسطة القاعدة وقم بتحديدها.</span><span class="sxs-lookup"><span data-stu-id="ef391-111">In the list, find and select the first duty that is controlled by the rule.</span></span>
1. <span data-ttu-id="ef391-112">في الحقل **المهمة الثانية**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="ef391-112">In the **Second duty** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="ef391-113">في القائمة، ابحث عن المهمة الثانية التي يتم التحكم فيها بواسطة القاعدة وقم بتحديدها.</span><span class="sxs-lookup"><span data-stu-id="ef391-113">In the list, find and select the second duty that is controlled by the rule.</span></span>
1. <span data-ttu-id="ef391-114">في الحقل **الخطورة**، حدد خطورة المخاطرة التي تحدث عندما يقوم نفس المستخدم أو الدور بكل من المهام الواجبة.</span><span class="sxs-lookup"><span data-stu-id="ef391-114">In the **Severity** field, select the severity of the risk that occurs when the same user or role performs both duties.</span></span>
1. <span data-ttu-id="ef391-115">في الحقل **مخاطرة الأمان**، أدخل وصفاً لمخاطرة الأمان.</span><span class="sxs-lookup"><span data-stu-id="ef391-115">In the **Security risk** field, enter a description of the security risk.</span></span>
1. <span data-ttu-id="ef391-116">في الحقل **تقليل الأمان**، اكتب قيمة.</span><span class="sxs-lookup"><span data-stu-id="ef391-116">In the **Security mitigation** field, type a value.</span></span>
1. <span data-ttu-id="ef391-117">أدخل وصفاً للإجراءات التي تتخذها لتقليل مخاطر الأمان.</span><span class="sxs-lookup"><span data-stu-id="ef391-117">Enter a description of the actions that you take to mitigate the security risk.</span></span> 
1. <span data-ttu-id="ef391-118">على سبيل المثال، يمكنك تقليل المخاطرة عن طريق القيام بمراجعات أكثر تفصيلاً للعملية، وذلك بإجراء مراجعة إدارية شهرية، أو عن طريق مشاركة الموارد مع أقسام أخرى.</span><span class="sxs-lookup"><span data-stu-id="ef391-118">For example, you can mitigate the risk by conducting more detailed reviews of the process, by conducting a monthly managerial review, or by sharing resources with other departments.</span></span>
1. <span data-ttu-id="ef391-119">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ef391-119">Select **Save**.</span></span>
2. <span data-ttu-id="ef391-120">أغلق الصفحة</span><span class="sxs-lookup"><span data-stu-id="ef391-120">Close the page</span></span>
