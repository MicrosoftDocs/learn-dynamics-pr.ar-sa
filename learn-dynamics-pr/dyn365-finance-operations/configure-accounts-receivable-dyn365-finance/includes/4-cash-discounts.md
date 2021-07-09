---
ms.openlocfilehash: 716b162bbadc71db45fb2ea8358f6d6ec185e102
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071082"
---
<span data-ttu-id="f368e-101">حسب الحالة، يمكنك القيام بما يلي بالخصومات النقدية:</span><span class="sxs-lookup"><span data-stu-id="f368e-101">Depending on the situation, you can do the following with cash discounts:</span></span>

-   <span data-ttu-id="f368e-102">الاستحقاق في حالة استيفاء عميل لشروط الدفع الخاصة بشركتك في الوقت المحدد، أو يتم منحه للعملاء عند دفع فواتيرهم في فترة زمنية محددة.</span><span class="sxs-lookup"><span data-stu-id="f368e-102">Accrue if a customer meets your company payment terms on time, or are given to customers when they pay their invoices in a specified period.</span></span>
-   <span data-ttu-id="f368e-103">الربط بجداول **العميل** وجداول **المورّد**.</span><span class="sxs-lookup"><span data-stu-id="f368e-103">Link to the **Customer** tables and **Vendor** tables.</span></span>
-   <span data-ttu-id="f368e-104">الترحيل إلى حساب دفتر الأستاذ المحدد للحصول على خصم نقدي تلقائياً إذا تمت تسوية فاتورة في الوقت المحدد.</span><span class="sxs-lookup"><span data-stu-id="f368e-104">Post to the ledger account that is specified for the cash discount automatically if an invoice is settled on time.</span></span>

<span data-ttu-id="f368e-105">ضع في الاعتبار السيناريو التالي:</span><span class="sxs-lookup"><span data-stu-id="f368e-105">Consider the following scenario:</span></span>

<span data-ttu-id="f368e-106">تقدم Adventure Works Cycles خصماً نقدياً إذا كان العميل يسدد الفواتير خلال مواعيد محددة.</span><span class="sxs-lookup"><span data-stu-id="f368e-106">Adventure Works Cycles offers a cash discount if a customer pays invoices within certain dates.</span></span>

<span data-ttu-id="f368e-107">قامت Adventure Works Cycles بإعداد الأكواد التالية:</span><span class="sxs-lookup"><span data-stu-id="f368e-107">Adventure Works Cycles has set up the following codes:</span></span>

-   <span data-ttu-id="f368e-108">5D10% - خصم نقدي بنسبة 10 بالمائة عند دفع المبلغ خلال خمسة أيام.</span><span class="sxs-lookup"><span data-stu-id="f368e-108">5D10% - Cash discount of 10 percent when the amount is paid within five days.</span></span>
-   <span data-ttu-id="f368e-109">10D5% - خصم نقدي بنسبة 5 بالمائة عند دفع المبلغ خلال عشرة أيام.</span><span class="sxs-lookup"><span data-stu-id="f368e-109">10D5% - Cash discount of five percent when the amount is paid within ten days.</span></span>
-   <span data-ttu-id="f368e-110">14D2% - خصم نقدي بنسبة 2 بالمائة عند دفع المبلغ خلال 14 يوماً.</span><span class="sxs-lookup"><span data-stu-id="f368e-110">14D2% - Cash discount of two percent when the amount is paid within 14 days.</span></span>

<span data-ttu-id="f368e-111">تتم الخصومات النقدية الثلاثة بشكل متسلسل عندما يقترب موعد الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="f368e-111">The three cash discounts occur sequentially as the cash discount date nears.</span></span> <span data-ttu-id="f368e-112">ومع ذلك، يُمنح خصم نقدي واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="f368e-112">However, only one cash discount is granted.</span></span>

<span data-ttu-id="f368e-113">لتحديد الخصومات النقدية التي تلي الكود 5D10%، يتم تحديد الكود 10D5% في قائمة **كود الخصم التالي**.</span><span class="sxs-lookup"><span data-stu-id="f368e-113">To specify the cash discounts following the 5D10% code, the 10D5% code is selected in the **Next discount code** list.</span></span> <span data-ttu-id="f368e-114">في الكود 10D5%، يتم تحديد الكود 14D2% في قائمة **كود الخصم التالي**.</span><span class="sxs-lookup"><span data-stu-id="f368e-114">On the 10D5% code, the 14D2% code is selected in the **Next discount code** list.</span></span> <span data-ttu-id="f368e-115">وأخيراً، على الكود 14D2%، تُترك قائمة **كود** **الخصم التالي** فارغة.</span><span class="sxs-lookup"><span data-stu-id="f368e-115">Finally, on the 14D2% code, the **Next discount** **code** list is left blank.</span></span> <span data-ttu-id="f368e-116">يمكنك تعيين خصومات نقدية للعملاء أو دفاتر اليومية أو أوامر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="f368e-116">You can assign cash discounts to customers, journals, or sales orders.</span></span>


<span data-ttu-id="f368e-117">**حسابات المقبوضات > إعداد المدفوعات > الخصومات النقدية**.</span><span class="sxs-lookup"><span data-stu-id="f368e-117">**Accounts receivable > Payments Setup > Cash discounts**</span></span>

![لقطة شاشة من صفحة الخصومات النقدية بتطبيقات Finance and Operations.](../media/cash-discount.png) 


<span data-ttu-id="f368e-119">في حقل **إدارة الخصومات النقدية** في صفحة **حسابات المقبوضات > الإعداد > محددات حسابات المقبوضات** وعلامة تبويب **التسوية**، حدد ما يجب القيام به مع الدفع بالزيادة أو بالنقصان في حاله عدم اقتطاع الخصم النقدي عند تسويه الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="f368e-119">In the **Cash-discount administration** field in the **Accounts receivable > Setup > Accounts receivable parameters** page and **Settlement** tab, select what to do with an overpayment or underpayment when a cash discount is not deducted when the invoice is settled.</span></span>

<span data-ttu-id="f368e-120">في حالة اختيار **غير محدد**، يتم ترحيل مبلغ الدفع بالنقصان إلى حساب الخصم النقدي للعميل.</span><span class="sxs-lookup"><span data-stu-id="f368e-120">If you select **Unspecific**, the underpayment amount is posted to the customer cash discount account.</span></span> <span data-ttu-id="f368e-121">إذا تم ترحيل الخصم النقدي القابل للتطبيق في نفس الشركة التي يوجد بها الدفع بالزيادة، فسوف تقوم إدارة الشؤون المالية بتعديل الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="f368e-121">If the applicable cash discount was posted in the same company as the overpayment, Finance will adjust the cash discount.</span></span>

<span data-ttu-id="f368e-122">إذا لم يتم ترحيل الخصم النقدي القابل للتطبيق في نفس الشركة التي يوجد بها الدفع بالزيادة، فسيتم ترحيله إلى حساب الخصم النقدي للنظام.</span><span class="sxs-lookup"><span data-stu-id="f368e-122">If the applicable cash discount was not posted in the same company as the overpayment, it is posted to the system cash discount account.</span></span> <span data-ttu-id="f368e-123">إذا كانت هناك خصومات نقدية متعددة بحيث تمت تسوية دفع المبلغ بالزيادة مقابل فواتير متعددة، فسيتم تعديل الخصم من الفاتورة الأخيرة إلى الخصم الأول.</span><span class="sxs-lookup"><span data-stu-id="f368e-123">If there are multiple cash discounts so that an overpayment was settled against multiple invoices, the adjustment to the discount is from the last invoice to the first discount.</span></span>

<span data-ttu-id="f368e-124">علامة تبويب **حسابات المقبوضات > إعداد > محددات حسابات المقبوضات > تسوية**</span><span class="sxs-lookup"><span data-stu-id="f368e-124">**Accounts receivable > Setup > Accounts receivable parameters > Settlement** tab</span></span>

![لقطة شاشة لصفحة محددات حسابات المقبوضات، مع تمييز علامة تبويب التسوية وإدارة الخصم النقدي.](../media/cash-discount-admin.png) 


<span data-ttu-id="f368e-126">في حالة اختيار **محدد**، يتم ترحيل مبلغ الدفع بالزيادة أو النقصان إلى حساب الخصم النقدي للعميل.</span><span class="sxs-lookup"><span data-stu-id="f368e-126">If you select **Specific,** the overpayment or underpayment amount is posted to the Customer cash discount account.</span></span>

<span data-ttu-id="f368e-127">لفهم هذين الخيارين بشكل أفضل، يمكنك النظر في المثال التالي:</span><span class="sxs-lookup"><span data-stu-id="f368e-127">To better understand these two options, consider the following example:</span></span>

<span data-ttu-id="f368e-128">يبلغ إجمالي فاتورة العميل 105.00 دولارات أمريكية، والخصم النقدي الذي يمكن الحصول عليه هو 10.50 دولارات أمريكية.</span><span class="sxs-lookup"><span data-stu-id="f368e-128">A customer's invoice total is USD 105.00, and the obtainable cash discount is USD 10.50.</span></span> <span data-ttu-id="f368e-129">مع الأخذ في الاعتبار الخصم النقدي، سيدفع العميل 94.50 دولاراً أمريكياً (105-10.50).</span><span class="sxs-lookup"><span data-stu-id="f368e-129">Considering the cash discount, the customer will pay USD 94.50 (105-10.50).</span></span>

<span data-ttu-id="f368e-130">ومع ذلك، فإن المبلغ الذي تتلقاه من العميل هو 95.00 دولاراً أمريكياً.</span><span class="sxs-lookup"><span data-stu-id="f368e-130">However, the amount they receive from the customer is USD 95.00.</span></span>

<span data-ttu-id="f368e-131">في حالة تعيين معلمة **إدارة الخصم النقدي** إلى **غير محدد**، تتم تسوية الفاتورة وترحيل فرق 0.50 دولار أمريكي إلى حساب دفتر الأستاذ الذي يتم تحديده لفروق الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="f368e-131">If the **Cash-discount administration** parameter is set to **Unspecific**, the invoice is settled, and the difference of USD 0.50 is posted to the ledger account that is specified for cash discount differences.</span></span>

<span data-ttu-id="f368e-132">في حالة تعيين معلمة **إدارة الخصم النقدي** إلى **محدد**، تتم تسوية الفاتورة وترحيل فرق 0.50 دولار أمريكي إلى حساب الخصم النقدي للعميل.</span><span class="sxs-lookup"><span data-stu-id="f368e-132">If the **Cash-discount administration** parameter is set to **Specific**, the invoice is settled, and the difference of USD 0.50 is posted to the customer's cash discount account.</span></span>

<span data-ttu-id="f368e-133">لتحديد أنه يتم حساب الخصم النقدي استناداً إلى المبلغ مضاف إليه ضريبة المبيعات، انتقل إلى صفحة **محددات دفتر الأستاذ العام**، وحدد علامة تبويب **ضريبة المبيعات**، ثم قم بتوسيع علامة التبويب السريعة **خيارات الضريبة**.</span><span class="sxs-lookup"><span data-stu-id="f368e-133">To specify that the cash discount is calculated based on the amount plus sales tax, go to the **General ledger parameters** page, select the **Sales tax** tab, and then expand the **Tax options** FastTab.</span></span> <span data-ttu-id="f368e-134">في هذا القسم، ستحتاج إلى تمكين **احتساب الخصم النقدي المفروض على المبلغ متضمناً ضريبة المبيعات** في منطقة **الخصم النقدي للعميل**.</span><span class="sxs-lookup"><span data-stu-id="f368e-134">In this section, you need to enable **Cash discount is calculated on amount including sales tax** in the **Customer cash discount** area.</span></span>

<span data-ttu-id="f368e-135">**دفتر الأستاذ العام > إعداد دفتر الأستاذ > محددات دفتر الأستاذ العام > ضريبة المبيعات**</span><span class="sxs-lookup"><span data-stu-id="f368e-135">**General ledger > Ledger setup > General ledger parameters > Sales tax**</span></span>

<span data-ttu-id="f368e-136">[![لقطة شاشة لعلامة تبويب ضريبة المبيعات، مع تمييز منطقة الخصم النقدي للعميل.](../media/customer-cash-discount.png)](../media/customer-cash-discount.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f368e-136">[![Screenshot of the Sales tax tab, with the Customer cash discount area highlighted.](../media/customer-cash-discount.png)](../media/customer-cash-discount.png#lightbox)</span></span>


