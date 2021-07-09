---
ms.openlocfilehash: 3dbe4a11dc4a120760a8f4c6ee4b5db121cf1297
ms.sourcegitcommit: 53e9b556e7b6f3d5c3572dca51b838fa1678f792
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/07/2021
ms.locfileid: "6070494"
---
<span data-ttu-id="d6b2e-101">يمكن تعليق الحركات الجارية للوصول لاحقاً من ذلك السجل أو من سجل نقطة بيع مختلف.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-101">Transactions that are in process can be suspended for later access from that register or from a different POS register.</span></span> 

<span data-ttu-id="d6b2e-102">هذه الميزة مفيدة للسيناريوهات التي يحتاج فيها العميل، بعد إنشاء الحركة وإضافة المنتجات، إلى استرداد صنف آخر أو الحصول على بطاقة ائتمان من سيارته.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-102">This feature is helpful for scenarios where, after the transaction has been created and products have been added, the customer needs to retrieve another item or get a credit card from their vehicle.</span></span> <span data-ttu-id="d6b2e-103">يمكن تعليق الحركة والاحتفاظ بها حتى لا يحتاج مساعد المبيعات إلى إعادة فحص المنتجات عند عودة العميل.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-103">The transaction can be suspended and held so that the sales associate doesn't need to rescan the products when the customer returns.</span></span> <span data-ttu-id="d6b2e-104">عندما يكون العميل جاهزاً لإنهاء معاملته، يمكن لأي شريك متجر في أي سجل نقاط البيع استدعاء حركته لاستئنافها أو إكمالها.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-104">When the customer is ready to finish their transaction, any store associate on any POS register can recall their transaction to resume or complete it.</span></span>

<span data-ttu-id="d6b2e-105">من خلال عملية استدعاء الطلب، يمكن للمستخدمين البحث عن طلبات العملاء عن طريق فحص الأمر أو الرقم المعرّف لمرجع القناة أو الرقم المعرّف للرموز الشريطية (الباركود).</span><span class="sxs-lookup"><span data-stu-id="d6b2e-105">With the order recall operation, users can search for customer orders by scanning order, channel reference ID, or receipt ID barcodes.</span></span> <span data-ttu-id="d6b2e-106">يمكن للمستخدمين أيضاً البحث باستخدام آليات التصفية الأخرى، بما في ذلك ثلاثة عوامل تصفية محددة مسبقاً تعرض:</span><span class="sxs-lookup"><span data-stu-id="d6b2e-106">Users can also search using other filtering mechanisms, including three predefined filters that display:</span></span>

- <span data-ttu-id="d6b2e-107">قائمة الطلبات التي يجب على المتجر الوفاء بها (استلام أو شحن).</span><span class="sxs-lookup"><span data-stu-id="d6b2e-107">A list of orders that need to be fulfilled by the store (pick up or ship).</span></span>
- <span data-ttu-id="d6b2e-108">من المقرر أن يتم استلام الطلبات المجدولة من المتجر.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-108">Orders scheduled to be picked up at the store.</span></span>
- <span data-ttu-id="d6b2e-109">الطلبات التي يجب شحنها من المتجر.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-109">Orders that need to be shipped from the store.</span></span>

<span data-ttu-id="d6b2e-110">يمكن أيضاً ربط هذه المرشحات المحددة مسبقاً بتكوين زر التشغيل في مصمم شبكة الأزرار للسماح للأزرار المخصصة بعرض الطلبات الموجودة في تلك الحالات.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-110">These predefined filters can also be linked to the operation button configuration in the button grid designer to allow for custom buttons to display orders that are in those states.</span></span> 

<span data-ttu-id="d6b2e-111">تتيح صفحة **طلب الاسترداد** للمستخدمين تحديد موقع طلبات العملاء بسرعة وبدء العمليات بسرعة لهذه الطلبات مثل التحرير أو الوفاء أو الإرجاع أو بدء الاستلام.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-111">The **Recall order** page allows users to quickly locate customer orders and quickly start operations for these orders such as editing, fulfilling, returning, or initiating a pickup.</span></span>


> [!NOTE]
> <span data-ttu-id="d6b2e-112">عندما تكون في وضع غير متصل بالشبكة، لا يمكن استدعاء الحركة المعلقة في سجل مختلف عن الذي تم تعليقها فيه.</span><span class="sxs-lookup"><span data-stu-id="d6b2e-112">When in offline mode, a suspended transaction cannot be recalled on a different register than the one that it was suspended on.</span></span>


