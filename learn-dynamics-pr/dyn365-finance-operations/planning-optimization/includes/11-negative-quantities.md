---
ms.openlocfilehash: d6cc350c87b2962ae5c588d89764a4a5d408f979
ms.sourcegitcommit: 01f8d224bf1e548ba0cbe53b3e2150c43302c125
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "6072089"
---
<span data-ttu-id="be18c-101">باستخدام تحسين التخطيط، عندما يعرض النظام الكمية الفعلية بقيمة سالبة، فإنه يفترض أن هناك عنصراً غير متزامن مع القيم الفعلية.</span><span class="sxs-lookup"><span data-stu-id="be18c-101">With Planning Optimization, when the system shows a negative on-hand quantity, it is assumed that something is out of sync with actuals.</span></span> <span data-ttu-id="be18c-102">بالتالي، ستتم معاملة الكمية على أنها صفر (0) لمنع التوريد الزائد.</span><span class="sxs-lookup"><span data-stu-id="be18c-102">Therefore, it will treat the quantity as zero (0) to prevent oversupply.</span></span> 

<span data-ttu-id="be18c-103">سيقوم النظام بالنظر إلى بُعد التغطية (الموقع والمستودع والموقع وهكذا) ثم تجميع الكميات الفعلية في أدنى مستوى.</span><span class="sxs-lookup"><span data-stu-id="be18c-103">The system will look at the coverage dimension (site, warehouse, location, and so on) and then aggregate the on-hand quantities at the lowest level.</span></span> <span data-ttu-id="be18c-104">إذا كانت النتيجة قيمة سالبة، فسوف يفترض أن الكمية هي صفر.</span><span class="sxs-lookup"><span data-stu-id="be18c-104">If the result is negative, it will assume that the quantity is zero.</span></span> 


## <a name="scenario-1"></a><span data-ttu-id="be18c-105">السيناريو 1</span><span class="sxs-lookup"><span data-stu-id="be18c-105">Scenario 1</span></span>

<span data-ttu-id="be18c-106">المستودع 13:</span><span class="sxs-lookup"><span data-stu-id="be18c-106">Warehouse 13:</span></span>

- <span data-ttu-id="be18c-107">**كود التغطية**: **الحد الأدنى/الحد الأقصى**</span><span class="sxs-lookup"><span data-stu-id="be18c-107">**Coverage code**: **Min/Max**</span></span>
- <span data-ttu-id="be18c-108">**الحد الأدنى**: 15</span><span class="sxs-lookup"><span data-stu-id="be18c-108">**Minimum**: 15</span></span>
- <span data-ttu-id="be18c-109">**الحد الأقصى**: 25</span><span class="sxs-lookup"><span data-stu-id="be18c-109">**Maximum**: 25</span></span>
- <span data-ttu-id="be18c-110">أقل مستوى لبُعد التغطية هو المستودع</span><span class="sxs-lookup"><span data-stu-id="be18c-110">Lowest level of coverage dimension is warehouse</span></span>
- <span data-ttu-id="be18c-111">الكميات المتاحة:</span><span class="sxs-lookup"><span data-stu-id="be18c-111">On-hand quantities:</span></span>
    - <span data-ttu-id="be18c-112">الموقع 1: 20</span><span class="sxs-lookup"><span data-stu-id="be18c-112">Location 1: 20</span></span>
    - <span data-ttu-id="be18c-113">الموقع 2: -12</span><span class="sxs-lookup"><span data-stu-id="be18c-113">Location 2: -12</span></span>

<span data-ttu-id="be18c-114">الإجمالي في المستودع 13 هو 8 (20-12) الذي يتم استخدامه ككمية فعلية.</span><span class="sxs-lookup"><span data-stu-id="be18c-114">Total in Warehouse 13 is 8 (20 – 12), which is used as the on-hand quantity.</span></span> <span data-ttu-id="be18c-115">يتم إنشاء أمر مخطط لإجمالي 17 صنفاً.</span><span class="sxs-lookup"><span data-stu-id="be18c-115">A planned order is generated for a total of 17 items.</span></span>

## <a name="scenario-2"></a><span data-ttu-id="be18c-116">السيناريو 2</span><span class="sxs-lookup"><span data-stu-id="be18c-116">Scenario 2</span></span>

<span data-ttu-id="be18c-117">المستودع 13:</span><span class="sxs-lookup"><span data-stu-id="be18c-117">Warehouse 13:</span></span>

- <span data-ttu-id="be18c-118">**كود التغطية**: **الحد الأدنى/الحد الأقصى**</span><span class="sxs-lookup"><span data-stu-id="be18c-118">**Coverage code**: **Min/Max**</span></span>
- <span data-ttu-id="be18c-119">**الحد الأدنى**: 15</span><span class="sxs-lookup"><span data-stu-id="be18c-119">**Minimum**: 15</span></span>
- <span data-ttu-id="be18c-120">**الحد الأقصى**: 25</span><span class="sxs-lookup"><span data-stu-id="be18c-120">**Maximum**: 25</span></span>
- <span data-ttu-id="be18c-121">أقل مستوى لبُعد التغطية هو المستودع</span><span class="sxs-lookup"><span data-stu-id="be18c-121">Lowest level of coverage dimension is warehouse</span></span>
- <span data-ttu-id="be18c-122">الكميات المتاحة:</span><span class="sxs-lookup"><span data-stu-id="be18c-122">On-hand quantities:</span></span>
    - <span data-ttu-id="be18c-123">الموقع 1: 5</span><span class="sxs-lookup"><span data-stu-id="be18c-123">Location 1: 5</span></span>
    - <span data-ttu-id="be18c-124">الموقع 2: -10</span><span class="sxs-lookup"><span data-stu-id="be18c-124">Location 2: -10</span></span>

<span data-ttu-id="be18c-125">الإجمالي في المستودع 13 هو-5 (5-10)، وهو أقل من الصفر.</span><span class="sxs-lookup"><span data-stu-id="be18c-125">Total in Warehouse 13 is -5 (5 – 10), which is less than zero.</span></span> <span data-ttu-id="be18c-126">بالتالي، تتم معاملته على أنه صفر ويتم إنشاء أمر مخطط لعدد 25 عنصراً، وهو الحد الأقصى، وليس 30، الذي سيتم إنشاؤه في محرك التخطيط الرئيسي المضمن.</span><span class="sxs-lookup"><span data-stu-id="be18c-126">Therefore, it is treated as zero and a planned order is generated for 25 items, which is the maximum, rather than 30, which would be generated in the built-in master planning engine.</span></span> 
