---
ms.openlocfilehash: c4c3657f70fb00d5993a9bc46f5651f6716d077b
ms.sourcegitcommit: e0a1238596690b3b6eedd86c2ac14099948a5e25
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "6073849"
---
## <a name="scenario"></a><span data-ttu-id="dabf0-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="dabf0-101">Scenario</span></span>
<span data-ttu-id="dabf0-102">يريد مدير العمليات في USMF المزيد من الرؤية في أوامر الإنتاج التي تم تأخيرها.</span><span class="sxs-lookup"><span data-stu-id="dabf0-102">The Operations Manager at USMF, wants more visibility into production orders that are delayed.</span></span> <span data-ttu-id="dabf0-103">لقد أعطوك تعليمات لتتبع ما يلي:</span><span class="sxs-lookup"><span data-stu-id="dabf0-103">They have given you instructions to track the following:</span></span>

- <span data-ttu-id="dabf0-104">أوامر الإنتاج المتعاقد عليها من الباطن التي لم يتم تسليمها</span><span class="sxs-lookup"><span data-stu-id="dabf0-104">Subcontracted production orders that are missing deliveries</span></span>
- <span data-ttu-id="dabf0-105">أوامر الإنتاج ذات المواد المفقودة</span><span class="sxs-lookup"><span data-stu-id="dabf0-105">Production orders with missing materials</span></span>
- <span data-ttu-id="dabf0-106">الأوامر المتأخرة بسبب فشل في الجهاز</span><span class="sxs-lookup"><span data-stu-id="dabf0-106">Orders delayed due to machine failures</span></span>

<span data-ttu-id="dabf0-107">باستخدام المعلومات المقدمة، قم بإنشاء ثلاث مجموعات إنتاج جديدة لاستخدامها في أوامر الإنتاج الجديدة.</span><span class="sxs-lookup"><span data-stu-id="dabf0-107">By using the information provided, create three new production pools for use on new production orders.</span></span>

## <a name="create-a-production-pool-for-delayed-subcontracted-work"></a><span data-ttu-id="dabf0-108">إنشاء مجموعة إنتاج للعمل المؤجل المتعاقد عليه من الباطن</span><span class="sxs-lookup"><span data-stu-id="dabf0-108">Create a production pool for delayed subcontracted work</span></span> 

1.  <span data-ttu-id="dabf0-109">افتح **التحكم في الإنتاج > إعداد > الإنتاج > مجموعات الإنتاج**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-109">Open **Production control > Setup > Production > Production pools**.</span></span>
2.  <span data-ttu-id="dabf0-110">حدد **جديد** لإنشاء مجموعة جديدة.</span><span class="sxs-lookup"><span data-stu-id="dabf0-110">Select **New** to create a new pool.</span></span>
3.  <span data-ttu-id="dabf0-111">أدخل **المهلة الفرعية** في الحقل **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-111">Enter **Delay-Sub** in the **Pool** field.</span></span>
4.  <span data-ttu-id="dabf0-112">أدخل **تأجيل العمل المتعاقد عليه من الباطن** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-112">Enter **Subcontracted Work Delayed** in the **Name** field.</span></span>


## <a name="create-a-production-pool-for-missing-materials"></a><span data-ttu-id="dabf0-113">إنشاء مجموعة إنتاج للمواد المفقودة</span><span class="sxs-lookup"><span data-stu-id="dabf0-113">Create a production pool for missing materials</span></span> 

1.  <span data-ttu-id="dabf0-114">حدد **جديد** لإنشاء مجموعة جديدة.</span><span class="sxs-lookup"><span data-stu-id="dabf0-114">Select **New** to create a new pool.</span></span>
2.  <span data-ttu-id="dabf0-115">أدخل **MATMISSING** في الحقل **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-115">Enter **MATMISSING** in the **Pool** field.</span></span>
3.  <span data-ttu-id="dabf0-116">في الحقل **الاسم**، أدخل **المواد المفقودة**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-116">Enter **Materials Missing** in the **Name** field.</span></span>

## <a name="create-a-production-pool-for-machine-failures"></a><span data-ttu-id="dabf0-117">إنشاء مجموعة إنتاج لحالات فشل الجهاز</span><span class="sxs-lookup"><span data-stu-id="dabf0-117">Create a production pool for machine failures</span></span> 

1.  <span data-ttu-id="dabf0-118">حدد **جديد** لإنشاء مجموعة جديدة.</span><span class="sxs-lookup"><span data-stu-id="dabf0-118">Select **New** to create a new pool.</span></span>
2.  <span data-ttu-id="dabf0-119">أدخل **MACHFAIL** في الحقل **المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-119">Enter **MACHFAIL** in the **Pool** field.</span></span>
3.  <span data-ttu-id="dabf0-120">أدخل **فشل الجهاز** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="dabf0-120">Enter **Machine Failure** in the **Name** field.</span></span>
4.  <span data-ttu-id="dabf0-121">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="dabf0-121">Select **Save**</span></span>
4.  <span data-ttu-id="dabf0-122">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="dabf0-122">Close all pages.</span></span>


