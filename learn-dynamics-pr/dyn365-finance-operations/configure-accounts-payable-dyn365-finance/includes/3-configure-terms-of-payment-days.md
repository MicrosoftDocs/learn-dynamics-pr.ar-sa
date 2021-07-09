---
ms.openlocfilehash: db6e3dfd87377910e49f8b065e81a75c04a9fb88
ms.sourcegitcommit: e3f27696e7d66a3d06c8371b64691e113b3e91f4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "6071051"
---
<span data-ttu-id="2b6de-101">استخدم صفحة **شروط الدفع** لتحديد جميع شروط الدفع المستخدمة من قِبل الشركة ومورديها.</span><span class="sxs-lookup"><span data-stu-id="2b6de-101">Use the **Terms of payment** page to define all the terms of payment used by a company and their vendors.</span></span> <span data-ttu-id="2b6de-102">استخدم شرط الدفع لحساب تاريخ الاستحقاق استناداً إلى تاريخ الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="2b6de-102">Use a term of payment for calculation of a due date based on the date of the invoice.</span></span>

<span data-ttu-id="2b6de-103">حدد شروط الدفع لكل مما يلي:</span><span class="sxs-lookup"><span data-stu-id="2b6de-103">Specify terms of payment for each of the following:</span></span>

- <span data-ttu-id="2b6de-104">المورد في صفحة **الموردين**.</span><span class="sxs-lookup"><span data-stu-id="2b6de-104">Vendor on the **Vendors** page.</span></span>
- <span data-ttu-id="2b6de-105">العميل في صفحة **العملاء**.</span><span class="sxs-lookup"><span data-stu-id="2b6de-105">Customer on the **Customers** page.</span></span>
- <span data-ttu-id="2b6de-106">أمر الشراء في صفحة **أمر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="2b6de-106">Purchase order on the **Purchase order** page.</span></span>
- <span data-ttu-id="2b6de-107">أمر المبيعات في صفحة **أمر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="2b6de-107">Sales order on the **Sales order** page.</span></span>

<span data-ttu-id="2b6de-108">تأمل السيناريو التالي؛ تتمتع Adventure Works Cycles بمدة دفع قياسية للمورد وهي 30 يوماً.</span><span class="sxs-lookup"><span data-stu-id="2b6de-108">Consider the following scenario; Adventure Works Cycles has a standard vendor payment term of Net 30 days.</span></span> <span data-ttu-id="2b6de-109">إذا قامت فاتورة بمدة دفع صافية تبلغ 30 يوماً بشحن البضائع في 15 سبتمبر، وكانت الفاتورة مؤرخة في 15 نوفمبر، يكون الدفع مستحقاً في 15 ديسمبر.</span><span class="sxs-lookup"><span data-stu-id="2b6de-109">If an invoice with a Net 30 payment term ships goods on September 15, and the invoice is dated November 15, then payment is due December 15.</span></span> <span data-ttu-id="2b6de-110">مع تسوية صافي لمدة 30 يوماً، يجب على Adventure Works Cycles دفع صافي المستحق في غضون 30 يوماً من تاريخ الفاتورة، وفقاً للتسوية.</span><span class="sxs-lookup"><span data-stu-id="2b6de-110">With a Net 30 Days settlement, Adventure Works Cycles must pay the net due within 30 days of the invoice date, according to the settlement.</span></span> <span data-ttu-id="2b6de-111">بعد هذا التاريخ، إذا لم تكتمل الدفعة، يمكن إضافة رسوم فائدة بنسبة مئوية محددة لكل شهر إلى الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="2b6de-111">After that date, if the payment is not completed, an interest charge of a specified percent per month can be added to the invoice.</span></span> <span data-ttu-id="2b6de-112">قد يتم تطبيق رسوم خدمات أخرى.</span><span class="sxs-lookup"><span data-stu-id="2b6de-112">Other service charges may also apply.</span></span>

<span data-ttu-id="2b6de-113">إذا كانت شروط الدفع مرتبطة بجدول الدفع، يتم استخدام القواعد الموضوعة في شروط الدفع لحساب تاريخ استحقاق القسط الأول.</span><span class="sxs-lookup"><span data-stu-id="2b6de-113">If terms of payment are linked to a payment schedule, the rules set up in the terms of payment are used to calculate the due date of the first installment.</span></span> <span data-ttu-id="2b6de-114">يتم استخدام القواعد المحددة في جدول الدفع لحساب تاريخ استحقاق الأقساط التالية.</span><span class="sxs-lookup"><span data-stu-id="2b6de-114">The rules set up in the payment schedule are used to calculate the due date of the following installments.</span></span>

<span data-ttu-id="2b6de-115">إذا تم تحديد طريقة الدفع نقداً عند الاستلام (COD) وتم تمكين **الدفع النقدي**، فهذا يشير إلى أن الدفعات يجب أن تتم نقداً وليس بشيك.</span><span class="sxs-lookup"><span data-stu-id="2b6de-115">If the cash on delivery (COD) payment method is selected, and the **Cash payment** is enabled, it indicates that payments should be made in cash and not by check.</span></span> <span data-ttu-id="2b6de-116">ولذلك، في منطقة **ترحيل دفتر الأستاذ** في حقل **النقد**، تحتاج إلى تحديد حساب رئيسي لتسوية الفواتير التي سيتم استخدامها للدفع النقدي.</span><span class="sxs-lookup"><span data-stu-id="2b6de-116">Therefore, in the **Ledger posting** area in the **Cash** field, you need to select a main account for settlement of invoices that will be used for cash payment.</span></span>

<span data-ttu-id="2b6de-117">انتقل إلى **الحسابات الدائنة > إعداد الدفع > شروط الدفع**.</span><span class="sxs-lookup"><span data-stu-id="2b6de-117">**Accounts payable > Payment setup > Terms of payment**</span></span>
 
![لقطة شاشة لصفحة شروط الدفع مع تحديد النقد.](../media/terms-payment.png)
 
## <a name="payment-days"></a><span data-ttu-id="2b6de-119">أيام الدفع</span><span class="sxs-lookup"><span data-stu-id="2b6de-119">Payment days</span></span> 

<span data-ttu-id="2b6de-120">استخدم أيام الدفع لتحديد يوم الدفع المستخدم لحساب تاريخ الاستحقاق.</span><span class="sxs-lookup"><span data-stu-id="2b6de-120">Use payment days to define the payment day used for calculating a due date.</span></span> <span data-ttu-id="2b6de-121">يتم دائماً تقريب تاريخ الاستحقاق إلى أقرب تاريخ محدد.</span><span class="sxs-lookup"><span data-stu-id="2b6de-121">The due date is always rounded up to the nearest specified date.</span></span> <span data-ttu-id="2b6de-122">يمكن تحديد يوم الدفع إما ليوم في الأسبوع أو في الشهر.</span><span class="sxs-lookup"><span data-stu-id="2b6de-122">Payment day can be specified for either a day in the week, or in the month.</span></span>

<span data-ttu-id="2b6de-123">**الحسابات الدائنة > إعداد الدفع > أيام الدفع**</span><span class="sxs-lookup"><span data-stu-id="2b6de-123">**Accounts payable > Payment setup > Payment days**</span></span>
 

![لقطة شاشة لصفحة أيام الدفع مع تحديد اليوم السابع عشر من الشهر.](../media/payment-days.png)
