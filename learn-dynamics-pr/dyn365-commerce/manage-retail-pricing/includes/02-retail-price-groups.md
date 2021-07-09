---
ms.openlocfilehash: a1800a2cf976d6e6c65931f0f342e866897e732a
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070383"
---
<span data-ttu-id="a3eaf-101">تُستخدم مجموعات أسعار البيع بالتجزئة لربط مكونات أسعار المبيعات بالخصومات إلى كيانات مختلفة مثل القنوات والكتالوجات وانتماءات العملاء وبرامج الولاء ومجموعات العملاء.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-101">Retail price groups are used to link the sales price components with the discounts to different entities such as channels, catalogs, customer affiliations, loyalty programs, and groups of customers.</span></span>

<span data-ttu-id="a3eaf-102">يوضح الرسم التوضيحي التالي كيفية استخدام مجموعات الأسعار.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-102">The following illustration shows how price groups are used.</span></span> 

![مجموعات الأسعار وكيفية ارتباطها بالكيانات](../media/price-groups.jpg)

<span data-ttu-id="a3eaf-104">في هذا الرسم التوضيحي، لاحظ أن **مجموعة الأسعار** تكون في مركز التسعير وإدارة الخصومات.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-104">In this illustration, notice that **Price group** is at the center of pricing and discount management.</span></span> <span data-ttu-id="a3eaf-105">توجد كيانات Commerce التي يمكنك استخدامها لإدارة الأسعار والخصومات التفاضلية على اليسار، ويوجد السعر الفعلي وسجلات الخصم على اليمين.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-105">The Commerce entities that you can use to manage differential prices and discounts are on the left, and the actual price and discount records are on the right.</span></span> 
 
<span data-ttu-id="a3eaf-106">عند إنشاء مجموعات أسعار، يجب ألا تستخدم مجموعة أسعار واحدة لأنواع متعددة من كيانات Commerce.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-106">When you create price groups, you should not use one price group for multiple types of Commerce entities.</span></span> <span data-ttu-id="a3eaf-107">وبخلاف ذلك، قد يكون من الصعب تحديد سبب تطبيق سعر أو خصم معين على حركة.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-107">Otherwise, determining why a specific price or discount is being applied to a transaction can be difficult.</span></span>

<span data-ttu-id="a3eaf-108">كما يُظهر الخط الأحمر المتقطع في الصورة، تدعم التجارة وظيفة Dynamics 365 الأساسية لمجموعة أسعار تم تعيينها مباشرة على العميل.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-108">As the red dashed line in the image shows, Commerce supports the core Dynamics 365 functionality of a price group that is set directly on a customer.</span></span> <span data-ttu-id="a3eaf-109">ومع ذلك، في هذه الحالة، ستحصل فقط على اتفاقيات تجارة سعر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-109">However, in this case, you will only get sales price trade agreements.</span></span> <span data-ttu-id="a3eaf-110">إذا كنت ترغب في تطبيق أسعار خاصة بالعميل، نوصيك بعدم تعيين مجموعات أسعار مباشرة على العميل.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-110">If you want to apply customer-specific prices, we recommend that you not set price groups directly on the customer.</span></span> <span data-ttu-id="a3eaf-111">بدلاً من ذلك، استخدم الانتماءات.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-111">Instead, use affiliations.</span></span>

<span data-ttu-id="a3eaf-112">إذا تم تعيين مجموعة الأسعار على العميل، فسيتم إقران مجموعة الأسعار هذه برأس أمر المبيعات للأوامر التي يتم إنشاؤها لهذا العميل.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-112">If the price group is set on the customer, then this price group will be associated with the sales order header of the orders that are created for this customer.</span></span> <span data-ttu-id="a3eaf-113">إذا قام المستخدم بتغيير مجموعة الأسعار في رأس الأمر، فسيتم استبدال مجموعة الأسعار القديمة بمجموعة الأسعار الجديدة ولكن للأمر الحالي فقط.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-113">If the user changes the price group on the order header, then the old price group is replaced with the new price group but only for the current order.</span></span> 

<span data-ttu-id="a3eaf-114">على سبيل المثال، لن تؤثر مجموعة الأسعار القديمة على الأمر الحالي، لكنها ستظل مرتبطة بالعميل للطلبات المستقبلية.</span><span class="sxs-lookup"><span data-stu-id="a3eaf-114">For example, the old price group will not affect the current order, but it will still be associated with the customer for future orders.</span></span>
