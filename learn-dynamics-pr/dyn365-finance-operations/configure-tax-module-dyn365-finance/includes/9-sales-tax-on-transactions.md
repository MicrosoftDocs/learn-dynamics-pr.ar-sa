---
ms.openlocfilehash: 249c9197d36e3d6ec4a20d57bccc279b15ba0dc4
ms.sourcegitcommit: d190aa41f6104061e6ebe52ee5c86b6cb9febaf2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/12/2021
ms.locfileid: "6071153"
---
<span data-ttu-id="7c77d-101">تحتاج في كل حركة (بنود مستند المبيعات/الشراء، ودفاتر اليومية، وما إلى ذلك)، إلى إدخال مجموعة ضريبة المبيعات ومجموعة ضريبة مبيعات للصنف لحساب ضريبة المبيعات.</span><span class="sxs-lookup"><span data-stu-id="7c77d-101">On every transaction (sales/purchase document lines, journals, and so on), you need to enter a sales tax group and an item sales tax group to calculate sales tax.</span></span> 

<span data-ttu-id="7c77d-102">يتم تحديد المجموعات الافتراضية في البيانات الرئيسية (على سبيل المثال، العميل والمورد والبند وفئة التدبير)، ولكن يمكنك تغيير المجموعات يدوياً في إحدى الحركات، إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="7c77d-102">Default groups are specified in master data (for example, customer, vendor, item, and procurement category), but you can manually change the groups on a transaction, if necessary.</span></span> <span data-ttu-id="7c77d-103">تحتوي كلتا المجموعتين على قائمة بأكواد ضريبة المبيعات، ويحدد تقاطع قائمتين من أكواد ضريبة المبيعات قائمة أكواد ضريبة المبيعات القابلة للتطبيق على الحركة.</span><span class="sxs-lookup"><span data-stu-id="7c77d-103">Both groups contain a list of sales tax codes, and the intersection of the two lists of sales tax codes determines the list of applicable sales tax codes for the transaction.</span></span>

<span data-ttu-id="7c77d-104">في كل حركة، يمكنك البحث عن ضريبة المبيعات المحسوبة بفتح صفحة **حركة ضريبة المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="7c77d-104">On every transaction, you can look up the calculated sales tax by opening the **Sales tax transaction** page.</span></span> <span data-ttu-id="7c77d-105">يمكنك البحث عن ضريبة المبيعات لبند في مستند أو للمستند بأكمله.</span><span class="sxs-lookup"><span data-stu-id="7c77d-105">You can look up the sales tax for a document line or for the whole document.</span></span>

<span data-ttu-id="7c77d-106">بالنسبة لمستندات معينة (على سبيل المثال، فاتورة المورد ودفاتر اليومية العامة)، يمكنك ضبط ضريبة المبيعات المحسوبة إذا كان المستند الأصلي يعرض مبالغ غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="7c77d-106">For certain documents (for example, vendor invoice and general journals), you can adjust the calculated sales tax if the original document shows deviant amounts.</span></span>


<span data-ttu-id="7c77d-107">[ ![لقطة شاشة لصفحة أمر مبيعات تعرض بنود أوامر المبيعات.](../media/transaction.png) ](../media/transaction.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7c77d-107">[ ![Screenshot of a sales order page showing Sales order lines.](../media/transaction.png) ](../media/transaction.png#lightbox)</span></span>

## <a name="tax-calculation-dates"></a><span data-ttu-id="7c77d-108">مواعيد حساب الضريبة</span><span class="sxs-lookup"><span data-stu-id="7c77d-108">Tax calculation dates</span></span>
<span data-ttu-id="7c77d-109">تواجه العديد من البلدان والمناطق تعديلات منتظمة في معدلات الضرائب، ويمكن لمعدل الضريبة في النظام أن يمثل هذه التعديلات بدقة اعتماداً على تاريخ الشحن.</span><span class="sxs-lookup"><span data-stu-id="7c77d-109">Numerous countries and regions experience regular adjustments in tax rates, and the system's tax rate can accurately represent these adjustments depending on the date of shipment.</span></span> <span data-ttu-id="7c77d-110">توجد أربعة خيارات للتاريخ لتحديد معدل الضريبة المناسب:</span><span class="sxs-lookup"><span data-stu-id="7c77d-110">There are four date options to determine the appropriate tax rate:</span></span> 

- <span data-ttu-id="7c77d-111">تاريخ التسليم</span><span class="sxs-lookup"><span data-stu-id="7c77d-111">Delivery date</span></span>
- <span data-ttu-id="7c77d-112">تاريخ الفاتورة</span><span class="sxs-lookup"><span data-stu-id="7c77d-112">Invoice date</span></span>
- <span data-ttu-id="7c77d-113">تاريخ المستند</span><span class="sxs-lookup"><span data-stu-id="7c77d-113">Document date</span></span>
- <span data-ttu-id="7c77d-114">تاريخ إيصال التعبئة</span><span class="sxs-lookup"><span data-stu-id="7c77d-114">Packing slip date</span></span>

<span data-ttu-id="7c77d-115">عند قيام المستخدمين بإنشاء إيصال تعبئة لبند أمر مبيعات، فإنهم سيحددون تاريخ إيصال التعبئة في الفاتورة، ويمكن للنظام استخدام هذا التاريخ لاستخراج معدل الضريبة من جدول قيمة كود الضريبة.</span><span class="sxs-lookup"><span data-stu-id="7c77d-115">When users create a packaging slip for a sales order line, they will specify the packing slip date on the invoice, and the system can use this date to extract the tax rate from the tax code value table.</span></span>
