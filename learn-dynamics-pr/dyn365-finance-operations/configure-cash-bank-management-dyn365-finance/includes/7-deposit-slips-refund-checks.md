---
ms.openlocfilehash: 86cc60ab654887fa6567a48a32902401b7747d0b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070951"
---
## <a name="deposit-slips"></a><span data-ttu-id="e6962-101">إيصالات الإيداع</span><span class="sxs-lookup"><span data-stu-id="e6962-101">Deposit slips</span></span> 

<span data-ttu-id="e6962-102">إيصال الإيداع هو مستند يُستخدم لإيداع الشيكات وإشعارات بطاقات الائتمان والنقد في حساب بنكي.</span><span class="sxs-lookup"><span data-stu-id="e6962-102">A deposit slip is a document used to deposit checks, credit card notes, and cash into a bank account.</span></span> <span data-ttu-id="e6962-103">يمكنك استخدام صفحة **إيصال الإيداع** لعرض وإدارة إيصالات الإيداع للمدفوعات في الحسابات البنكية.</span><span class="sxs-lookup"><span data-stu-id="e6962-103">You can use the **Deposit slip** page to view and manage deposit slips for payments into bank accounts.</span></span>

<span data-ttu-id="e6962-104">قد ترغب في إلغاء دفع إيصال الإيداع إذا كانت عملية دفع العميل غير صالحة.</span><span class="sxs-lookup"><span data-stu-id="e6962-104">You might want to cancel a deposit slip payment if a customer payment is invalid.</span></span> <span data-ttu-id="e6962-105">إذا كنت قد قمت بالفعل بتسوية إيصال الإيداع في كشف الحساب البنكي، فلا يمكنك إلغاء عملية الدفع.</span><span class="sxs-lookup"><span data-stu-id="e6962-105">If you have already reconciled the deposit slip in the bank statement, you cannot cancel the payment.</span></span> 

<span data-ttu-id="e6962-106">إذا كنت تريد إلغاء إيصال إيداع، فقد يطلب منك قسم الشؤون المالية **كود سبب**، إذا تم تحديد خانة الاختيار **طلب أسباب عمليات إلغاء الدفع بإيصال الإيداع** بعلامة التبويب السريعة **عام** لصفحة **معلمات إدارة النقد والبنوك**.</span><span class="sxs-lookup"><span data-stu-id="e6962-106">If you were to cancel a deposit slip, Finance might require a **Reason code**, if the **Require reasons for deposit slip payment cancellations** check box is selected on the **General** FastTab of the **Cash and bank management parameters** page.</span></span> 

<span data-ttu-id="e6962-107">إذا كنت تريد إرسال إلغاء دفع إيصال إيداع للمراجعة، فحدد خانة الاختيار **استخدام عملية المراجعة لإلغاء دفع إيصال الإيداع** بعلامة التبويب السريعة **عام** لصفحة **معلمات إدارة النقد والبنوك**.</span><span class="sxs-lookup"><span data-stu-id="e6962-107">If you want to submit a deposit slip payment cancellation for review, select the **Use review process for deposit slip payment cancellations** check box on the **General** FastTab of the **Cash and bank management parameters** page.</span></span>

<span data-ttu-id="e6962-108">وأثناء المراجعة، يمكنك إما الموافقة على دفتر اليومية وترحيله أو رفض الإلغاء.</span><span class="sxs-lookup"><span data-stu-id="e6962-108">During review, you can either approve and post the journal, or reject the cancellation.</span></span> 

## <a name="refund-checks"></a><span data-ttu-id="e6962-109">شيكات المبالغ المستردة</span><span class="sxs-lookup"><span data-stu-id="e6962-109">Refund checks</span></span> 

<span data-ttu-id="e6962-110">في ظل ظروف معينة، تحتاج الشركات إلى إنشاء مبالغ مستردة لعملائها أو معالجة المبالغ المستردة التي استلمتها من مورديها.</span><span class="sxs-lookup"><span data-stu-id="e6962-110">Under certain circumstances, companies need to generate payment refunds to their customers or process refunds that they received from their vendors.</span></span> <span data-ttu-id="e6962-111">يحدث هذا عادةً عندما يتم تضمين الإشعارات الائتمانية والمدفوعات الزائدة والمكافآت في حركات الجهة الأخرى.</span><span class="sxs-lookup"><span data-stu-id="e6962-111">This usually occurs when credit notes, overpayments, and bonuses are involved in third-party transactions.</span></span>

<span data-ttu-id="e6962-112">في Finance، يمكنك إنشاء مبلغ شيك مسترد يقوم بطباعة شيك.</span><span class="sxs-lookup"><span data-stu-id="e6962-112">In Finance, you can create a check refund that prints out a check.</span></span> <span data-ttu-id="e6962-113">يتم تنفيذ ميزة الاسترداد في دفاتر يومية مدفوعات العملاء.</span><span class="sxs-lookup"><span data-stu-id="e6962-113">The refunding feature is implemented in payment journals for customers.</span></span>

<span data-ttu-id="e6962-114">استخدم الحقل **مدين** لتحديد المبلغ الذي سيتم استرداده.</span><span class="sxs-lookup"><span data-stu-id="e6962-114">Use the **Debit** field to specify the amount to be refunded.</span></span> <span data-ttu-id="e6962-115">لا تستخدم أبداً مبلغاً سالباً بالحقل **دائن**.</span><span class="sxs-lookup"><span data-stu-id="e6962-115">Never use a negative amount of the **Credit** field.</span></span>

<span data-ttu-id="e6962-116">قبل إنشاء شيك بمبلغ مسترد، قم بإعداد **طريقة الدفع** لرد الشيك إلى العميل.</span><span class="sxs-lookup"><span data-stu-id="e6962-116">Before you create a check refund, set up a **Method of payment** to refund a check to a customer.</span></span> 

## <a name="payment-reversal"></a><span data-ttu-id="e6962-117">إلغاء الدفع</span><span class="sxs-lookup"><span data-stu-id="e6962-117">Payment reversal</span></span> 

<span data-ttu-id="e6962-118">في بعض الأحيان، تحتاج إلى إلغاء الشيك بعد قيامك بالدفع وترحيل الشيك.</span><span class="sxs-lookup"><span data-stu-id="e6962-118">Occasionally, you need to reverse a check after you have made a payment and posted the check.</span></span> <span data-ttu-id="e6962-119">على سبيل المثال، قد يكون لشركة التسليم الشيك، أو قد يلاحظ أحد أعضاء فريق المحاسبة أن أحد الموظفين يدفع الشيك بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="e6962-119">For example, the delivery company might have the check, or a member of the accounting staff might notice that an employee paid the check incorrectly.</span></span> 

<span data-ttu-id="e6962-120">تتوفر طريقتان لإلغاء الشيكات التي تم ترحيلها:</span><span class="sxs-lookup"><span data-stu-id="e6962-120">Two methods are available for reversing posted checks:</span></span>

- <span data-ttu-id="e6962-121">يتم تسجيل عمليات الإلغاء فوراً عند النقر فوق الزر **إلغاء الدفع** في صفحة **الشيك**.</span><span class="sxs-lookup"><span data-stu-id="e6962-121">Reversals are posted immediately when you click the **Payment reversal** button in the **Check** page.</span></span>
- <span data-ttu-id="e6962-122">عند النقر فوق الزر **إلغاء الدفع** في صفحة **الشيك** يتم إرسال الإلغاء أولاً إلى دفتر يومية **عمليات إلغاء الشيكات** في إدارة البنك والنقد، حيث يمكن للمراجع بعد ذلك ترحيل الإلغاء أو رفضه.</span><span class="sxs-lookup"><span data-stu-id="e6962-122">When you click the **Payment reversal** button in the **Check** page, the reversal is sent first to the **Check reversals** journal in cash and bank management, where a reviewer can then post or reject the reversal.</span></span>

<span data-ttu-id="e6962-123">قد تقوم بإلغاء شيك لإعادة إصدار دفعة تم دفعها إلى المورد.</span><span class="sxs-lookup"><span data-stu-id="e6962-123">You might reverse a check to reissue a payment made to a vendor.</span></span> <span data-ttu-id="e6962-124">يمكنك إلغاء الشيكات التي تم ترحيلها والتي تكون حالتها **مدفوعة**.</span><span class="sxs-lookup"><span data-stu-id="e6962-124">You can reverse only posted checks that have a status of **Paid**.</span></span> <span data-ttu-id="e6962-125">يختلف إلغاء الشيكات عن حذفها أو إلغاؤها لأنه يمكنك فقط حذف الشيكات التي تكون حالتها **تم إنشاؤها** فقط، بينما يمكنك إلغاء الشيكات التي لم يتم ترحيلها فقط.</span><span class="sxs-lookup"><span data-stu-id="e6962-125">Reversing differs from deleting or voiding checks because you can delete only checks that have a status of **Created**, and you can void only unposted checks.</span></span>

<span data-ttu-id="e6962-126">يؤدي حذف دفتر اليومية إلى إزالة الإلغاء من Finance، ولكن يظل الشيك الأصلي في صفحة **الشيك**.</span><span class="sxs-lookup"><span data-stu-id="e6962-126">Deleting the journal removes the reversal from Finance, but the original check remains in the **Check** page.</span></span> 

