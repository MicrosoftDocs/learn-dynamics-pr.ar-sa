---
ms.openlocfilehash: b7d1e50547fe7887d24dc0fbacc342244c3cda33
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070270"
---
<span data-ttu-id="61c98-101">نظراً لأن محرك الأسعار عادةً ما يختار السعر الأقل من بين سعرين، فإنه لا يدعم مطلب إجبار محرك الأسعار على تحديد السعر الأعلى من بين سعرين دون تكوين هيكل التسعير مرتين لجعل السعر الأعلى من بين السعرين صالحاً لقنوات Commerce.</span><span class="sxs-lookup"><span data-stu-id="61c98-101">Because the pricing engine will usually select the lower of two prices, it does not support the requirement to force the pricing engine to select the higher of the two prices without configuring the pricing structure twice to make the higher of the two prices valid for the Commerce channels.</span></span> <span data-ttu-id="61c98-102">تهدف أولويات التسعير إلى تبسيط هذه الأنواع من المتطلبات.</span><span class="sxs-lookup"><span data-stu-id="61c98-102">Pricing priorities are meant to streamline those types of requirements.</span></span> <span data-ttu-id="61c98-103">يمكن أن تساعد أولويات التسعير في تحديد ضرورة استخدام مجموعة أسعار أو خصم ما قبل خصم آخر، مثل خصم أقل.</span><span class="sxs-lookup"><span data-stu-id="61c98-103">Pricing priorities can help specify that a price group or discount needs to be used before another discount is, such as a lower discount.</span></span> 

<span data-ttu-id="61c98-104">تُستخدم أولويات التسعير في تقييم أسعار البيع والخصومات بشكل مستقل.</span><span class="sxs-lookup"><span data-stu-id="61c98-104">Pricing priorities are used in evaluating selling prices and discounts independently.</span></span> 

<span data-ttu-id="61c98-105">هناك مكانان يمكنك فيهما تحديد أولوية التسعير، وهما:</span><span class="sxs-lookup"><span data-stu-id="61c98-105">Two places where you can specify a pricing priority are:</span></span> 

- <span data-ttu-id="61c98-106">مجموعات الأسعار</span><span class="sxs-lookup"><span data-stu-id="61c98-106">Price groups</span></span>
- <span data-ttu-id="61c98-107">الخصومات</span><span class="sxs-lookup"><span data-stu-id="61c98-107">Discounts</span></span> 
 
<span data-ttu-id="61c98-108">يتم توريث أولوية التسعير للخصومات من الأولوية المحددة في مجموعة الأسعار المرتبطة بالخصومات، ما لم يتم تجاوزها في الخصم.</span><span class="sxs-lookup"><span data-stu-id="61c98-108">The pricing priority for discounts is inherited from the specific priority on the price group that is associated with the discounts, unless they are overridden on the discount.</span></span> <span data-ttu-id="61c98-109">بصورة افتراضية، تكون جميع أولويات التسعير **صفر**.</span><span class="sxs-lookup"><span data-stu-id="61c98-109">By default, all pricing priorities are **zero**.</span></span> <span data-ttu-id="61c98-110">عند تعيين أولوية تسعير على أولوية أعلى، تكون لها الأسبقية على الأرقام الأقل.</span><span class="sxs-lookup"><span data-stu-id="61c98-110">When a pricing priority is set to a higher priority, it takes precedence over lower numbers.</span></span> <span data-ttu-id="61c98-111">على سبيل المثال، عشرة ستأخذ الأولوية على خمسة في تقييم سعر البيع أو الخصم المطلوب استخدامه.</span><span class="sxs-lookup"><span data-stu-id="61c98-111">For example, ten would take priority over five in evaluating a sales price or discount to use.</span></span> 

> [!NOTE]
> <span data-ttu-id="61c98-112">لكل أولوية تسعير، يلزم المرور الكامل عبر منطق محرك أسعار البيع بالتجزئة.</span><span class="sxs-lookup"><span data-stu-id="61c98-112">For each pricing priority, a full pass through the logic for the retail pricing engine is required.</span></span> <span data-ttu-id="61c98-113">لذلك، للمساعدة في الحفاظ على أداء حساب السعر والخصم، يجب عليك استخدام أولويات التسعير باعتدال.</span><span class="sxs-lookup"><span data-stu-id="61c98-113">Therefore, to help maintain the performance of the price and discount calculation, you should use pricing priorities sparingly.</span></span>
