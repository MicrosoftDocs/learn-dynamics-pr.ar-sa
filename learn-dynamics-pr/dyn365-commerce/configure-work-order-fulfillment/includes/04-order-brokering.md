---
ms.openlocfilehash: c55be93ac4f46a3413476af38b9c096bb493302a
ms.sourcegitcommit: afc018f2c4899625e3acf83d0e82eeda93c14bcf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/22/2021
ms.locfileid: "6070420"
---
<span data-ttu-id="db919-101">في وقت المعالجة، لا يأخذ DOM في الاعتبار جميع الأوامر وبنود الأوامر في النظام ولكن فقط القليل منها:</span><span class="sxs-lookup"><span data-stu-id="db919-101">At the time of processing, DOM does not consider all orders and order lines in the system but only a few:</span></span> 

- <span data-ttu-id="db919-102">بنود الأمر التي تلبي معايير أصول المبيعات وأوضاع التسليم والكيان القانوني (كما هو محدد في ملف تعريف استيفاء DOM)، والتي تلبي أيضاً أي واحد من المعايير التالية:</span><span class="sxs-lookup"><span data-stu-id="db919-102">Order lines that meet the criteria for sales order origins, modes of delivery, and legal entity (as defined in the DOM fulfillment profile), and that also meet any of these criteria:</span></span>
    - <span data-ttu-id="db919-103">يتم إنشاؤها في قنوات Commerce.</span><span class="sxs-lookup"><span data-stu-id="db919-103">Are created in Commerce channels.</span></span> <span data-ttu-id="db919-104">يتم تحديد الأوامر كأوامر مبيعات عندما يتم تعيين الخيار **بيع Commerce** إلى **نعم** في رأس أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="db919-104">Orders are identified as sales orders when the **Commerce sale** option is set to **Yes** on the sales order header.</span></span>
    - <span data-ttu-id="db919-105">لم يتم بوساطة DOM.</span><span class="sxs-lookup"><span data-stu-id="db919-105">Have not been brokered by DOM.</span></span>
    - <span data-ttu-id="db919-106">أجرت DOM الوساطة من قبل، ولكن تم وضع علامة عليها كاستثناءات وهي لم تصل إلى الحد الأقصى للمحاولات.</span><span class="sxs-lookup"><span data-stu-id="db919-106">Have been brokered by DOM before, but are marked as exceptions and are below the maximum threshold for attempts.</span></span>
    - <span data-ttu-id="db919-107">لم يتم تمييزها على أنها تستخدم طريقة الاستلام أو التسليم الإلكتروني؛ اختار العميل استلام الأمر الخاص به، لذلك لا احتاج DOM إلى النظر في هذا الأمر للوفاء به.</span><span class="sxs-lookup"><span data-stu-id="db919-107">Have not been marked as using a pick-up or electronic delivery mode; the customer has chosen to pick up their order, so DOM does not need to consider this order for fulfillment.</span></span>
    - <span data-ttu-id="db919-108">لم يتم تمييزها للتسليم المباشر؛ سيتم تنفيذ هذه الأوامر مباشرة من البائع للعميل.</span><span class="sxs-lookup"><span data-stu-id="db919-108">Are not marked for direct delivery; these orders will be fulfilled directly by the vendor to the customer.</span></span>
    - <span data-ttu-id="db919-109">غير مستثناة يدوياً.</span><span class="sxs-lookup"><span data-stu-id="db919-109">Are not manually excluded.</span></span>
- <span data-ttu-id="db919-110">الأوامر التي ليست قيد الانتظار</span><span class="sxs-lookup"><span data-stu-id="db919-110">Orders that are not on hold</span></span>

<span data-ttu-id="db919-111">يقوم نظام DOM، بعد تطبيق القواعد وقيود المخزون والتحسين، بانتقاء الموقع الأقرب إلى عنوان التسليم الخاص بالعميل.</span><span class="sxs-lookup"><span data-stu-id="db919-111">After it applies the rules, inventory constraints, and optimization, DOM picks the location that is closest to the customer's delivery address.</span></span>
 
![رسم تخطيطي يوضح معايير وساطة الأمر‬ في Dynamics 365 Commerce.](../media/dom-order-criteria.png)

<span data-ttu-id="db919-113">إن DOM غير متوافقة تماماً مع وظائف المستودعات المتقدمة، على الرغم من أنها قد تعمل بشكل كافٍ لسيناريوهات أعمال معينة في مثل هذه البيئات.</span><span class="sxs-lookup"><span data-stu-id="db919-113">DOM is not fully compatible with the advanced warehouse functionality, even though it might work sufficiently for certain business scenarios in such environments.</span></span> <span data-ttu-id="db919-114">تتوفر وظيفة DOM في إصدار Commerce على السحابة.</span><span class="sxs-lookup"><span data-stu-id="db919-114">DOM is only available on the cloud version of Commerce.</span></span>
