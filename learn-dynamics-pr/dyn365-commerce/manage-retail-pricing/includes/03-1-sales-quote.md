---
ms.openlocfilehash: ef3bff5178ce4f51f8c2dde5e07bda75583ed4fd
ms.sourcegitcommit: b2c1f5af6813dd8bf520fa8af24dbee5d38de050
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/06/2021
ms.locfileid: "6070480"
---
<span data-ttu-id="c8c5c-101">يدعم محرك تسعير Commerce معظم سيناريوهات تسعير ‏‫متاجرة عمل-مستهلك‬ (B2C)، بما في ذلك التسعير على مستوى المتجر والتسعير المستند إلى الولاء والانتماء وخصومات الخلط والمطابقة وخصومات الكمية وخصومات الحد الفاصل.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-101">Most business-to-consumer (B2C) pricing scenarios are supported by the Commerce pricing engine, including store-level pricing, affiliation and loyalty-based pricing, mix-and-match discounts, quantity discounts, and threshold discounts.</span></span> <span data-ttu-id="c8c5c-102">يستخدم محرك التسعير قواعد معقدة لتحديد أفضل سعر لعرض أسعار أو أمر معين.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-102">The pricing engine uses complex rules to determine the best price for a given quotation or order.</span></span>
<span data-ttu-id="c8c5c-103">عند استخدام الكتابة المزدوجة، يتوفر لديك ثلاثة خيارات تسعير للاختيار من بينها:</span><span class="sxs-lookup"><span data-stu-id="c8c5c-103">When you use dual-write, you have three pricing options to choose from:</span></span>

- <span data-ttu-id="c8c5c-104">التسعير الثابت من قائمة أسعار Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="c8c5c-104">The static pricing from the Dynamics 365 Sales price list</span></span>
- <span data-ttu-id="c8c5c-105">محرك تسعير Dynamics 365 Supply Chain Management</span><span class="sxs-lookup"><span data-stu-id="c8c5c-105">The Dynamics 365 Supply Chain Management pricing engine</span></span>
- <span data-ttu-id="c8c5c-106">محرك تسعير Dynamics 365 Commerce.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-106">The Dynamics 365 Commerce pricing engine.</span></span>

<span data-ttu-id="c8c5c-107">يعد محرك تسعير Commerce هو الأكثر ملائمة لسيناريوهات متاجرة عمل-مستهلك‬ (B2C) من بين هذه الخيارات.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-107">The Commerce pricing engine is the best fit for B2C scenarios among these options.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8c5c-108">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="c8c5c-108">Prerequisites</span></span>

<span data-ttu-id="c8c5c-109">قبل أن تتمكن من استخدام محرك التسعير التجاري في المبيعات، يجب عليك اتباع الخطوات الواردة في [‏‫العميل المتوقع إلى النقدية في الكتابة المزدوجة‬](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-prospect-to-cash/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="c8c5c-109">Before you can use the Commerce pricing engine in Sales, you must follow the steps in [Prospect-to-cash in dual-write](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-prospect-to-cash/?azure-portal=true).</span></span>

<span data-ttu-id="c8c5c-110">يجب عليك أيضاً إيقاف تشغيل تقييم الاتفاقية التجارية للإدخال اليدوي باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c8c5c-110">You must also turn off trade agreement evaluation for manual entry by following these steps:</span></span>

1.  <span data-ttu-id="c8c5c-111">في بيئة Commerce الخاصة بحك، انتقل إلى **الحسابات المدينة > الإعداد > معلمات الحسابات المدينة**.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-111">In your Commerce environment, go to **Accounts receivable > Setup > Accounts receivable parameters**.</span></span>

2.  <span data-ttu-id="c8c5c-112">في علامة التبويب **الأسعار** في علامة التبويب السريعة **‬‏‫تقييم اتفاقية التجارة**، قم بإلغاء تحديد مربع الاختيار **الإدخال اليدوي**.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-112">On the **Prices** tab, on the **Trade agreement evaluation** FastTab, clear the **Manual entry** check box.</span></span>

## <a name="use-the-commerce-pricing-engine-in-sales"></a><span data-ttu-id="c8c5c-113">استخدام محرك تسعير Commerce في المبيعات</span><span class="sxs-lookup"><span data-stu-id="c8c5c-113">Use the Commerce pricing engine in Sales</span></span>

> [!NOTE]
> <span data-ttu-id="c8c5c-114">في الوقت الحالي، يمكن استخدام محرك تسعير Commerce فقط لإنشاء عروض الأسعار في المبيعات.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-114">Currently, the Commerce pricing engine can be used only for quotation creation in the Sales.</span></span> <span data-ttu-id="c8c5c-115">لا يتوفر تكامل أمر المبيعات مع محرك تسعير Commerce بعد.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-115">Sales order integration with the Commerce pricing engine isn't yet available.</span></span>

<span data-ttu-id="c8c5c-116">ينسخ إطار عمل الكتابة المزدوجة تفاصيل عرض الأسعار من المبيعات إلى Commerce عندما يبدأ المستخدمون بوضع عرض أسعار في المبيعات.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-116">The dual-write framework copies the quotation details from Sales to Commerce when users initiate a quotation in Sales.</span></span> <span data-ttu-id="c8c5c-117">يتم نسخ أي تغييرات يتم إجراؤها على بنود عرض الأسعار الموجودة في المبيعات، بالإضافة إلى أي سطور عروض أسعار مضافة حديثاً، إلى Commerce.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-117">Any changes made to existing quotation lines in Sales, as well as any newly added quotation lines, are copied to Commerce.</span></span> <span data-ttu-id="c8c5c-118">عندما يرغب المستخدمون في تسعير عرض الأسعار باستخدام محرك تسعير Commerce، يمكنهم تحديد **عرض أسعار** لتحديث أسعار عرض الأسعار باستخدام محرك تسعير Commerce.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-118">When users want to price the quotation using the Commerce pricing engine, they can select **Price quote** to update the quotation's prices using the Commerce pricing engine.</span></span> <span data-ttu-id="c8c5c-119">يتم بعد ذلك تحديث كل من أسعار المبيعات وCommerce تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="c8c5c-119">Both Sales and Commerce prices are then automatically updated.</span></span>
