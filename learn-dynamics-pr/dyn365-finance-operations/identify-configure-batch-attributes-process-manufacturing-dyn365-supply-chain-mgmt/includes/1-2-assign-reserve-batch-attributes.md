---
ms.openlocfilehash: 41c8898203785b7bd1823a54c5a4d259409e93c9
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073461"
---
## <a name="assign-batch-attributes"></a><span data-ttu-id="e5813-101">تعيين سمات الدُفعات</span><span class="sxs-lookup"><span data-stu-id="e5813-101">Assign batch attributes</span></span>

<span data-ttu-id="e5813-102">يمكنك تعيين سمات الدُفعات للمنتجات الفردية التي يتم الاحتفاظ بها في دُفعات المخزون، أو يمكنك تعيين الحد الأدنى للقيم الدنيا وكذلك الحد الأقصى والقيم المستهدفة لسمة الدُفعة للمنتجات أو العملاء المحددين.</span><span class="sxs-lookup"><span data-stu-id="e5813-102">You can assign batch attributes to individual products that are held in inventory batches, or you can assign the threshold for minimum, maximum, and target values for a batch attribute to products or specific customers.</span></span> <span data-ttu-id="e5813-103">قبل أن تتمكن من تعيين سمة دفعية على مستوى العميل، يجب تعيينها على مستوى المنتج.</span><span class="sxs-lookup"><span data-stu-id="e5813-103">Before you can assign a batch attribute at the customer level, you must assign it at the product level.</span></span>

<span data-ttu-id="e5813-104">يجب أن يتم تعيين بُعد الدُفعة المنتج إلى **نشط** في مجموعة أبعاد التعقب.</span><span class="sxs-lookup"><span data-stu-id="e5813-104">The product must have the batch dimension set to **Active** in the tracking dimension group.</span></span> <span data-ttu-id="e5813-105">لتعيين سمة الدُفعة لمنتج فردي، استخدم الصفحة الخاصة بالمنتج.</span><span class="sxs-lookup"><span data-stu-id="e5813-105">To assign a batch attribute to an individual product, use the product-specific page.</span></span> <span data-ttu-id="e5813-106">إذا كانت السمة محددة لمنتج خاص بأحد العملاء، استخدم الصفحة الخاصة بالعميل.</span><span class="sxs-lookup"><span data-stu-id="e5813-106">If the attribute is specific to a product for a customer, use the customer-specific page.</span></span>

<span data-ttu-id="e5813-107">عند إضافة سمة إلى منتج، يجب عليك أيضاً تعريف معلمات أخرى، مثل:</span><span class="sxs-lookup"><span data-stu-id="e5813-107">When you add an attribute to a product, you must also define other parameters, such as:</span></span>

-   <span data-ttu-id="e5813-108">نطاقات الحد الأدنى والأقصى لنوع السمة **عدد صحيح** أو **كسر** .</span><span class="sxs-lookup"><span data-stu-id="e5813-108">The minimum and maximum ranges for an attribute of the **Integer** or **Fraction** type.</span></span>

-   <span data-ttu-id="e5813-109">إجراءات التفاوت لنوع السمة **عدد صحيح** أو **كسر** .</span><span class="sxs-lookup"><span data-stu-id="e5813-109">The tolerance actions for an attribute of the **Integer** or **Fraction** type.</span></span> <span data-ttu-id="e5813-110">إذا كانت قيمة السمة تقع خارج الحد الأدنى والأقصى للنطاق، يمكن أن يكون الإجراء إما رسالة تحذير أو رسالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="e5813-110">If the value of the attribute falls outside the minimum and maximum range, the action can be either a warning message or an error message.</span></span>

-   <span data-ttu-id="e5813-111">القيمة المستهدفة للسمة.</span><span class="sxs-lookup"><span data-stu-id="e5813-111">The target value for the attribute.</span></span> <span data-ttu-id="e5813-112">هذه القيمة هي القيمة المثلى للسمة، وتنطبق على كافة أنواع السمات.</span><span class="sxs-lookup"><span data-stu-id="e5813-112">This value is the optimal value of the attribute, and it applies to all attribute types.</span></span>

## <a name="reserve-batches"></a><span data-ttu-id="e5813-113">حجز الدُفعات</span><span class="sxs-lookup"><span data-stu-id="e5813-113">Reserve batches</span></span>

<span data-ttu-id="e5813-114">يمكنك البحث في سمات الدُفعة عند إجراء حجوزات الدُفعات لأمر مبيعات لتنفيذ أمر العميل أو عند اختيار دُفعات لأمر إنتاج وحجزها.</span><span class="sxs-lookup"><span data-stu-id="e5813-114">You can search on batch attributes when you perform batch reservations for a sales order to fulfill a customer's order or when you pick and reserve batches for a production order.</span></span> <span data-ttu-id="e5813-115">يساعدك البحث على العثور على دُفعات المنتجات التي تحتوي على قيم سمة الدُفعات ضمن النطاق المطلوب للإنتاج أو أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="e5813-115">The search helps you find product batches with batch attribute values that are within the range that is required for your production or sales order.</span></span> <span data-ttu-id="e5813-116">بعد تحديد موقع الدُفعة أو الدُفعات، يمكنك حجز المنتج إلى بند حركة المخزون الأصلي.</span><span class="sxs-lookup"><span data-stu-id="e5813-116">After you locate the batch or batches, you can reserve the product to the originating inventory transaction line.</span></span>
