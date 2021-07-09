---
ms.openlocfilehash: 210369f1fd2a0b38e30a91453d5ffaad1f78a498
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073725"
---

<span data-ttu-id="1ccac-101">يستخدم التعاقد من الباطن المستند إلى النشاط في Supply Chain Management أنشطة العملية كجزء من حساب التكلفة للمنتج النهائي، بناءً على تدفق الإنتاج باستخدام نوع مجموعة التكاليف **للإسناد المباشر إلى جهة أخرى**.</span><span class="sxs-lookup"><span data-stu-id="1ccac-101">Activity-based subcontracting in Supply Chain Management uses process activities as part of the cost calculation for the finished product, based on the production flow by using a cost group type of **Direct outsourcing**.</span></span>

<span data-ttu-id="1ccac-102">تساهم إيصالات خدمات المقاول من الباطن وفواتيره بشكل مباشر في تكلفة تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="1ccac-102">Receipts for subcontractor services and invoices are directly contributing to the cost of the production flow.</span></span> <span data-ttu-id="1ccac-103">تتم تسوية إيصالات استلام المنتجات المُخرجة وفواتير المورّد مقابل حسابات العمل الجاري (WIP).</span><span class="sxs-lookup"><span data-stu-id="1ccac-103">Output product receipts and vendor invoices are reconciled against the work in progress (WIP) accounts.</span></span> <span data-ttu-id="1ccac-104">يتم احتساب الفروق في عملية تحديد تكاليف الإصدار التلقائي.</span><span class="sxs-lookup"><span data-stu-id="1ccac-104">Variances are accounted for in the backflush costing process.</span></span>

## <a name="direct-outsourcing-cost-group-type"></a><span data-ttu-id="1ccac-105">نوع مجموعة تكاليف الإسناد المباشر إلى جهة أخرى</span><span class="sxs-lookup"><span data-stu-id="1ccac-105">Direct outsourcing cost group type</span></span>

<span data-ttu-id="1ccac-106">يتم تعيين نوع مجموعة التكاليف الخاصة **بالإسناد المباشر إلى جهة أخرى** لجميع الأعمال التي يتم توفيرها بواسطة خلايا عمل التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="1ccac-106">The cost group type of **Direct outsourcing** is assigned to all work that is provided by subcontracting work cells.</span></span>

<span data-ttu-id="1ccac-107">**إدارة التكلفة > إعدادات سياسات محاسبة المخزون > مجموعات التكلفة**</span><span class="sxs-lookup"><span data-stu-id="1ccac-107">**Cost management > Inventory accounting policies setup > Cost groups**</span></span>

![لقطة شاشة لصفحة مجموعات التكاليف مع نوع مجموعة تكاليف الإسناد المباشر إلى جهة أخرى.](../media/direct-outsourcing.png) 


<span data-ttu-id="1ccac-109">لحساب تكلفة الصنف للتعاقد من الباطن بصورة صحيحة، يجب إعداد بعض المتطلبات الأساسية:</span><span class="sxs-lookup"><span data-stu-id="1ccac-109">To properly calculate the item cost for subcontracting, you must set up a few prerequisites:</span></span>

-   <span data-ttu-id="1ccac-110">يتم تعيين نوع مجموعة تكاليف خاصة **بالإسناد المباشر إلى جهة أخرى** لجميع خلايا عمل التعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="1ccac-110">A cost group type of **Direct outsourcing** is assigned to all subcontracting work cells.</span></span>

-   <span data-ttu-id="1ccac-111">يجب تنشيط التعاقد من الباطن في كشف التكاليف، مع مجموعات التكاليف الخاصة بالإسناد المباشر إلى جهة أخرى المرتبطة بها.</span><span class="sxs-lookup"><span data-stu-id="1ccac-111">Subcontracting must be activated in the costing sheet, with the cost groups for direct outsourcing associated with them.</span></span>

-   <span data-ttu-id="1ccac-112">يتم إنشاء قواعد كانبان من خلال أنشطة التعاقد من الباطن في تدفق الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="1ccac-112">Kanban rules are created with the subcontracting activities in the production flow.</span></span>

<span data-ttu-id="1ccac-113">عند حساب تكلفة الصنف بناءً على تدفق الإنتاج، تستخدم Finance and Operations إعدادات نشاط خدمة التعاقد من الباطن لتحديد تكلفة الصنف.</span><span class="sxs-lookup"><span data-stu-id="1ccac-113">When calculating the item cost based on the production flow, Finance and Operations uses the subcontracting service activity settings to define the item cost.</span></span> <span data-ttu-id="1ccac-114">يعرض تصنيف التكاليف صنف الخدمة بدلاً من خلية العمل كمورد.</span><span class="sxs-lookup"><span data-stu-id="1ccac-114">The cost breakdown shows the service item instead of the work cell as a resource.</span></span>
