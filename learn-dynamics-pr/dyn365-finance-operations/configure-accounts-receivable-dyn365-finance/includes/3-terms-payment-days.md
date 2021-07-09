---
ms.openlocfilehash: ab804084bbb3b0b0de58c5894667152e21d5eec3
ms.sourcegitcommit: e3f27696e7d66a3d06c8371b64691e113b3e91f4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "6071048"
---
<span data-ttu-id="435cd-101">يتم تقاسم شروط الدفع لحسابات المقبوضات والحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="435cd-101">The terms of payment are shared for accounts receivable and accounts payable.</span></span> <span data-ttu-id="435cd-102">ويعني هذا أنه يمكن أيضاً استخدام شروط الدفع التي تم إنشاؤها في حسابات المقبوضات في الحسابات الدائنة والعكس صحيح.</span><span class="sxs-lookup"><span data-stu-id="435cd-102">That means that terms of payment that were created in accounts receivable can also be used in accounts payable and vice-versa.</span></span> <span data-ttu-id="435cd-103">استخدم صفحة **شروط الدفع** لتحديد جميع شروط الدفع المستخدمة من قِبل الشركة والعملاء.</span><span class="sxs-lookup"><span data-stu-id="435cd-103">Use the **Terms of payment** page to define all the terms of payment used by a company and the customers.</span></span> <span data-ttu-id="435cd-104">استخدم شرط الدفع لحساب تاريخ الاستحقاق استناداً إلى تاريخ الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="435cd-104">Use a term of payment for calculating a due date based on the date of the invoice.</span></span>

<span data-ttu-id="435cd-105">حدد شروط الدفع لكل مما يلي:</span><span class="sxs-lookup"><span data-stu-id="435cd-105">Specify terms of payment for each of the following:</span></span>

-   <span data-ttu-id="435cd-106">العميل في صفحة **العملاء**</span><span class="sxs-lookup"><span data-stu-id="435cd-106">Customer on the **Customers** page</span></span>
-   <span data-ttu-id="435cd-107">أمر المبيعات في صفحة **أمر المبيعات**</span><span class="sxs-lookup"><span data-stu-id="435cd-107">Sales order on the **Sales order** page</span></span>

### <a name="scenario"></a><span data-ttu-id="435cd-108">السيناريو</span><span class="sxs-lookup"><span data-stu-id="435cd-108">Scenario</span></span>
<span data-ttu-id="435cd-109">تتمتع Adventure Works Cycles بمدة دفع قياسية للعميل تبلغ 30 يوماً.</span><span class="sxs-lookup"><span data-stu-id="435cd-109">Adventure Works Cycles has a standard customer payment term of Net 30 days.</span></span> <span data-ttu-id="435cd-110">إذا قامت فاتورة بمدة دفع صافية تبلغ 30 يوماً بشحن البضائع في 15 سبتمبر، وكانت الفاتورة مؤرخة في 15 نوفمبر، يكون الدفع مستحقاً في 15 ديسمبر.</span><span class="sxs-lookup"><span data-stu-id="435cd-110">If an invoice with a Net 30 payment term ships goods on September 15, and the invoice is dated November 15, then payment is due December 15.</span></span> <span data-ttu-id="435cd-111">مع تسوية لمدة 30 يوماً، يجب أن تتلقى Adventure Works Cycles المدفوعات في غضون 30 يوماً من تاريخ الفاتورة، وفقاً للتسوية.</span><span class="sxs-lookup"><span data-stu-id="435cd-111">With a Net 30 Days settlement, Adventure Works Cycles must receive payments within 30 days of the invoice date, according to the settlement.</span></span> <span data-ttu-id="435cd-112">بعد هذا التاريخ، إذا لم تكتمل الدفعة، فقد تتم إضافة رسوم فائدة بنسبة مئوية محددة شهرياً إلى الفاتورة، ويجب على العميل دفع رسوم إضافية.</span><span class="sxs-lookup"><span data-stu-id="435cd-112">After that date, if the payment is not completed, an interest charge of a specified percent per month might be added to the invoice, and the customer must pay additional fees.</span></span>
<span data-ttu-id="435cd-113">قد يتم تطبيق رسوم خدمات أخرى.</span><span class="sxs-lookup"><span data-stu-id="435cd-113">Other services charges might also apply.</span></span>

<span data-ttu-id="435cd-114">إذا كان شرط الدفع مرتبطاً بجدول الدفع، يتم استخدام القواعد التي تم إعدادها في شرط الدفع لحساب تاريخ استحقاق القسط الأول.</span><span class="sxs-lookup"><span data-stu-id="435cd-114">If a term of payment is linked to a payment schedule, the rules set up in the term of payment are used to calculate the due date of the first installment.</span></span>

<span data-ttu-id="435cd-115">يتم استخدام القواعد التي تم إعدادها في جدول الدفع لحساب تاريخ استحقاق الأقساط التالية.</span><span class="sxs-lookup"><span data-stu-id="435cd-115">The rules that are set up in the payment schedule are used to calculate the due date of the following installments.</span></span>

<span data-ttu-id="435cd-116">في حالة تحديد طريقة الدفع **COD** (**نقداً عند الاستلام**) وتمكين **الدفع النقدي**، فهذا يشير إلى أن الدفعات يجب أن تتم نقداً وليس بشيك.</span><span class="sxs-lookup"><span data-stu-id="435cd-116">If the **COD** (**cash on delivery**) payment method is selected, and **Cash payment** is enabled, it indicates that payments should be made in cash and not by check.</span></span> <span data-ttu-id="435cd-117">ولذلك، في منطقة **ترحيل دفتر الأستاذ** من حقل **النقد**، تحتاج إلى تحديد حساب رئيسي لتسوية الفواتير التي سيتم استخدامها للدفع النقدي.</span><span class="sxs-lookup"><span data-stu-id="435cd-117">Therefore, In the **Ledger posting** area from the **Cash** field, you need to select a main account for settlement of invoices that will be used for cash payment.</span></span>


## <a name="payment-days"></a><span data-ttu-id="435cd-118">أيام الدفع</span><span class="sxs-lookup"><span data-stu-id="435cd-118">Payment days</span></span> 

<span data-ttu-id="435cd-119">يمكنك استخدام أيام الدفع لتحديد يوم الدفع المستخدم لحساب تاريخ الاستحقاق.</span><span class="sxs-lookup"><span data-stu-id="435cd-119">You can use payment days to define the payment day used for calculating the due date.</span></span> <span data-ttu-id="435cd-120">يمكن تحديد يوم الدفع إما ليوم في الأسبوع أو في الشهر.</span><span class="sxs-lookup"><span data-stu-id="435cd-120">Payment day can be specified for either a day in the week or in the month.</span></span> <span data-ttu-id="435cd-121">يساعد هذا في اقتراح الدفع لاقتراح فواتير العملاء التي يجب إحضارها إلى دفتر يوميات دفع العميل للترحيل.</span><span class="sxs-lookup"><span data-stu-id="435cd-121">This helps payment proposal to suggest those customer invoices that should be brought into the customer payment journal for posting.</span></span> <span data-ttu-id="435cd-122">يجب إدخال التاريخ كرقم رقمي، مثل **10**، بدلاً من رقم ترتيبي مثل العاشر.</span><span class="sxs-lookup"><span data-stu-id="435cd-122">The date should be entered as a numeral, such as **10**, rather than an ordinal number like 10th.</span></span>

<span data-ttu-id="435cd-123">**حسابات المقبوضات > إعداد المدفوعات > أيام الدفع**</span><span class="sxs-lookup"><span data-stu-id="435cd-123">**Accounts receivable > Payments setup > Payment days**</span></span>

![لقطة شاشة لصفحة أيام الدفع في Finance and Operations.](../media/payment-days.png) 


