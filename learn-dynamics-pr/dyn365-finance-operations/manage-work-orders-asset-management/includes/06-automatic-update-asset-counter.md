---
ms.openlocfilehash: 58f8d1236a9b8192541bb1097cbd65935f1e8018
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072374"
---
<span data-ttu-id="f8028-101">يمكن تحديث العدادات يدوياً في أحد الأصول، كما يمكن تحديثها تلقائياً استناداً إلى ساعات الإنتاج أو كمية الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f8028-101">Counters can be updated manually on an asset and they can also be updated automatically based on production hours or production quantity.</span></span> 

<span data-ttu-id="f8028-102">ويمكن تحديث القيم من تسجيلات الإنتاج إذا كانت مرتبطة بمَورد تم إعداده في وحدة التحكم في الإنتاج، ومن جانبك تقوم بتسجيل عدد الساعات المستخدمة في المَورد أو الأصناف التي تم إنتاجها.</span><span class="sxs-lookup"><span data-stu-id="f8028-102">Values can be updated from production registrations if they are related to a resource that is set up in the Production control module, and you are recording the number of hours that are used on the resource or items produced.</span></span> 

<span data-ttu-id="f8028-103">بالنسبة إلى عدد الأصناف التي تم إنتاجها، فإنها تشتمل على كل من الكمية المناسبة والكمية غير الصحيحة، والتي يتم تسجيلها عند ترحيل دفتر يومية **تم بالإبلاغ عنه كمنتهٍ** في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f8028-103">For the number of items produced, it would include both the good quantity and the error quantity, which are recorded when a **Reported as finished** journal is posted in production.</span></span> 

<span data-ttu-id="f8028-104">اتبع الخطوات الآتية لتحديث عدادات الأصول:</span><span class="sxs-lookup"><span data-stu-id="f8028-104">Follow these steps to update asset counters:</span></span>

1.  <span data-ttu-id="f8028-105">انتقل إلى **إدارة الأصول > دوري > الأصول > تحديث عدادات الأصول**.</span><span class="sxs-lookup"><span data-stu-id="f8028-105">Go to **Asset management > Periodic > Assets > Update asset counters**.</span></span>
2.  <span data-ttu-id="f8028-106">في الحقل **تاريخ البدء**، أدخل التاريخ الذي تريد أن يبدأ فيه التحديث التلقائي.</span><span class="sxs-lookup"><span data-stu-id="f8028-106">In the **From date** field, enter the date when you want the automatic update to start.</span></span> 

    <span data-ttu-id="f8028-107">وهذا التاريخ سيُلغي التاريخ الفعلي الذي تم الإخبار به في "التحكم في الإنتاج".</span><span class="sxs-lookup"><span data-stu-id="f8028-107">This date will reflect the actual physical date that is reported in Production control.</span></span> <span data-ttu-id="f8028-108">وسيقوم كل تسجيل إنتاج بعد هذا التاريخ بتحديث عداد الأصول.</span><span class="sxs-lookup"><span data-stu-id="f8028-108">Every production registration after that date will update the counter of the asset.</span></span> <span data-ttu-id="f8028-109">(يجب تعيين الأصل إلى مَورد محدد).</span><span class="sxs-lookup"><span data-stu-id="f8028-109">(The asset must be assigned to a specific resource.)</span></span>

    <span data-ttu-id="f8028-110">في لقطة الشاشة، لاحظ أنه بعد 31 ديسمبر 2019، سيتم تحديث عدادات أصول بإجمالي 109 استناداً إلى عمليات تسجيل الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="f8028-110">In the screenshot, notice that after 31 December 2019, a total of 109 assets had their counters updated based on production registrations.</span></span>
 
    ![لقطة شاشة لصفحة تحديث عدادات الأصول مع تمييز المعلمات الخاصة بها.](../media/update-asset-counters-ssm.png)

<span data-ttu-id="f8028-112">عند التعامل مع عدادات الأصول، يجب تذكر النقاط الآتية:</span><span class="sxs-lookup"><span data-stu-id="f8028-112">When working with asset counters, you should keep the following points in mind:</span></span>

- <span data-ttu-id="f8028-113">لا يزال بإمكانك إنشاء عمليات تسجيل قيم العدادات اليدوية، حتى وإن كان يتم تحديث نوع العدادات تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="f8028-113">You can still create manual counter value registrations, even if the counter type is automatically updated.</span></span> 
- <span data-ttu-id="f8028-114">يمكنك إعداد العدادات المرتبطة بعداد آخر.</span><span class="sxs-lookup"><span data-stu-id="f8028-114">You can set up counters that are related to another counter.</span></span> <span data-ttu-id="f8028-115">وفي هذه الحالة، عند تحديث عداد، فإنه يقوم تلقائياً بتحديث أي عدادات ذات صلة.</span><span class="sxs-lookup"><span data-stu-id="f8028-115">In this case, when a counter is updated, it automatically updates any related counters.</span></span> 