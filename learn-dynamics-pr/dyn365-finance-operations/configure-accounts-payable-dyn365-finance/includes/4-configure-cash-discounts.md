---
ms.openlocfilehash: 2a7ba3ba11634d2a15817ae8be8f6b0abfbf5beb
ms.sourcegitcommit: e3f27696e7d66a3d06c8371b64691e113b3e91f4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "6071050"
---
<span data-ttu-id="77c62-101">شاهد هذا الفيديو للتعرف على كيفية تكوين الخصومات النقدية.</span><span class="sxs-lookup"><span data-stu-id="77c62-101">Watch this video to learn how to configure cash discounts.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE43VfZ]


## <a name="scenario"></a><span data-ttu-id="77c62-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="77c62-102">Scenario</span></span> 

<span data-ttu-id="77c62-103">تحصل USMF على خصم نقدي إذا كانت تسدد فواتير المورّد خلال مواعيد محددة.</span><span class="sxs-lookup"><span data-stu-id="77c62-103">USMF obtains a cash discount if it pays vendor invoices within certain dates.</span></span> <span data-ttu-id="77c62-104">تقوم USMF بإعداد الأكواد التالية:</span><span class="sxs-lookup"><span data-stu-id="77c62-104">USMF has set up the following codes:</span></span>

- <span data-ttu-id="77c62-105">5D10% - خصم نقدي بنسبة 10 بالمائة عند دفع المبلغ خلال خمسة أيام.</span><span class="sxs-lookup"><span data-stu-id="77c62-105">5D10% - Cash discount of 10 percent when the amount is paid within five days.</span></span>
- <span data-ttu-id="77c62-106">10D5% - خصم نقدي بنسبة 5 بالمائة عند دفع المبلغ خلال عشرة أيام.</span><span class="sxs-lookup"><span data-stu-id="77c62-106">10D5% - Cash discount of five percent when the amount is paid within ten days.</span></span>
- <span data-ttu-id="77c62-107">14D2% - خصم نقدي بنسبة 2 بالمائة عند دفع المبلغ خلال 14 يوماً.</span><span class="sxs-lookup"><span data-stu-id="77c62-107">14D2% - Cash discount of two percent when the amount is paid within 14 days.</span></span>

<span data-ttu-id="77c62-108">تتم الخصومات النقدية الثلاثة بشكل متسلسل عندما يقترب موعد الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="77c62-108">The three cash discounts occur sequentially as the cash discount date nears.</span></span> <span data-ttu-id="77c62-109">ومع ذلك، يُمنح خصم نقدي واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="77c62-109">However, only one cash discount is granted.</span></span>

- <span data-ttu-id="77c62-110">لتحديد الخصومات النقدية التي تلي الكود 5D10%، يتم تحديد الكود 10D5% في قائمة **كود الخصم التالي**.</span><span class="sxs-lookup"><span data-stu-id="77c62-110">To specify the cash discounts following the 5D10% code, the 10D5% code is selected in the **Next discount code** list.</span></span> 
- <span data-ttu-id="77c62-111">في الكود 10D5%، يتم تحديد الكود 14D2% في قائمة **كود الخصم التالي**.</span><span class="sxs-lookup"><span data-stu-id="77c62-111">For the 10D5% code, the 14D2% code is selected in the **Next discount code** list.</span></span> 
- <span data-ttu-id="77c62-112">وبالنسبة للكود 14D2%، تُترك قائمة **كود الخصم التالي** فارغة.</span><span class="sxs-lookup"><span data-stu-id="77c62-112">For the 14D2% code, the **Next discount code** is left blank.</span></span> <span data-ttu-id="77c62-113">يمكنك تعيين خصومات نقدية للموردين أو دفاتر اليومية أو أوامر الشراء.</span><span class="sxs-lookup"><span data-stu-id="77c62-113">You can assign cash discounts to vendors, journals, or purchase orders.</span></span>

<span data-ttu-id="77c62-114">**الحسابات الدائنة > إعداد المدفوعات > الخصومات النقدية**.</span><span class="sxs-lookup"><span data-stu-id="77c62-114">**Accounts payable > Payment setup > Cash discounts**</span></span>
 
<span data-ttu-id="77c62-115">[![لقطة شاشة لصفحة الخصومات النقدية مع تمييز كود الخصم التالي.](../media/cash-discount.png)](../media/cash-discount.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="77c62-115">[![Screenshot of the Cash discounts page with Next discount code highlighted.](../media/cash-discount.png)](../media/cash-discount.png#lightbox)</span></span>

## <a name="cash-discount-administration-field-setup"></a><span data-ttu-id="77c62-116">إعداد حقل إدارة الخصم النقدي</span><span class="sxs-lookup"><span data-stu-id="77c62-116">Cash-discount administration field setup</span></span> 

<span data-ttu-id="77c62-117">انتقل إلى صفحة **الحسابات الدائنة > إعداد > محددات الحسابات الدائنة**، في علامة تبويب **التسوية** في حقل **إدارة الخصم النقدي**، وحدد ما ترغب في القيام به مع الدفع بالزيادة أو بالنقصان في حاله عدم اقتطاع الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="77c62-117">Go to **Accounts payable > Setup > Accounts payable parameters** page, on the **Settlement** tab, in the **Cash-discount administration** field, and select what you want to do with an overpayment or underpayment when a cash discount is not deducted.</span></span> <span data-ttu-id="77c62-118">يجب إعداد محددة الحسابات الدائنة‏‎ هذه بشكل صحيح قبل تسوية الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="77c62-118">This Accounts payable parameter must be set up correctly before an invoice is settled.</span></span> 

<span data-ttu-id="77c62-119">في حالة اختيار **غير محدد**، يتم ترحيل مبلغ الدفع بالنقصان إلى حساب الخصم النقدي للمورِّد.</span><span class="sxs-lookup"><span data-stu-id="77c62-119">If you select **Unspecific**, the underpayment amount is posted to the vendor cash discount account.</span></span> <span data-ttu-id="77c62-120">إذا تم ترحيل الخصم النقدي القابل للتطبيق في نفس الشركة التي يوجد بها الدفع بالزيادة، فسوف تقوم إدارة الشؤون المالية بتعديل الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="77c62-120">If the applicable cash discount was posted in the same company as the overpayment, Finance will adjust the cash discount.</span></span> 

<span data-ttu-id="77c62-121">إذا لم يتم ترحيل الخصم النقدي القابل للتطبيق في نفس الشركة التي يوجد بها الدفع بالزيادة، فسيتم ترحيله إلى حساب الخصم النقدي للنظام.</span><span class="sxs-lookup"><span data-stu-id="77c62-121">If the applicable cash discount was not posted in the same company as the overpayment, it is posted to the system cash discount account.</span></span> <span data-ttu-id="77c62-122">إذا كانت هناك خصومات نقدية متعددة بحيث تمت تسوية دفع المبلغ بالزيادة مقابل فواتير متعددة، فسيتم تعديل الخصم من الفاتورة الأخيرة إلى الخصم الأول.</span><span class="sxs-lookup"><span data-stu-id="77c62-122">If there are multiple cash discounts so that an overpayment was settled against multiple invoices, the adjustment to the discount is from the last invoice to the first discount.</span></span>
 
![لقطة شاشة لصفحة محددات الحسابات الدائنة‏‎، مع تمييز القائمة المنسدلة لإدارة الخصم النقدي.](../media/cash-discount-admin.png)

<span data-ttu-id="77c62-124">في حالة اختيار **محدد**، يتم ترحيل مبلغ الدفع بالزيادة أو النقصان إلى حساب الخصم النقدي للمورد.</span><span class="sxs-lookup"><span data-stu-id="77c62-124">If you select **Specific**, the overpayment or underpayment amount is posted to the vendor cash discount account.</span></span>

<span data-ttu-id="77c62-125">لفهم هذين الخيارين بشكل أفضل، يمكنك النظر في المثال التالي:</span><span class="sxs-lookup"><span data-stu-id="77c62-125">To better understand these two options, consider the following example:</span></span>

<span data-ttu-id="77c62-126">يبلغ إجمالي فاتورة مورد 105.00 دولارات أمريكية، والخصم النقدي الذي يمكن الحصول عليه هو 10.50 دولارات أمريكية.</span><span class="sxs-lookup"><span data-stu-id="77c62-126">A vendor's invoice total is 105.00 USD, and the obtainable cash discount is 10.50 USD.</span></span> <span data-ttu-id="77c62-127">مع الأخذ في الاعتبار الخصم النقدي، سيدفع المورد 94.50 دولاراً أمريكياً (105-10.50).</span><span class="sxs-lookup"><span data-stu-id="77c62-127">Considering the cash discount, the vendor will be paid 94.50 USD (105-10.50).</span></span>

<span data-ttu-id="77c62-128">ومع ذلك، فإن المبلغ المدفوع بالفعل للمورد هو 95.00 دولاراً أمريكياً.</span><span class="sxs-lookup"><span data-stu-id="77c62-128">However, the amount actually paid to the vendor is 95.00 USD.</span></span>

<span data-ttu-id="77c62-129">في حالة تعيين معلمة **إدارة الخصم النقدي** على **غير محدد**، تتم تسوية الفاتورة، ويتم ترحيل فرق 0.50 دولار أمريكي إلى حساب دفتر الأستاذ المحدد لفروق الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="77c62-129">If the **Cash-discount administration** parameter is set to **Unspecific**, the invoice is settled, and the difference of 0.50 USD is posted to the ledger account specified for cash discount differences.</span></span>

<span data-ttu-id="77c62-130">في حالة تعيين معلمة **إدارة الخصم النقدي** إلى **محدد**، تتم تسوية الفاتورة وترحيل فرق 0.50 دولار أمريكي إلى حساب الخصم النقدي للمورِّد.</span><span class="sxs-lookup"><span data-stu-id="77c62-130">If the **Cash-discount administration** parameter is set to **Specific**, the invoice is settled, and the difference of 0.50 USD is posted to the vendor's cash discount account.</span></span>

<span data-ttu-id="77c62-131">لتحديد أنه يتم حساب الخصم النقدي استناداً إلى المبلغ مضافاً إليه ضريبة المبيعات، انتقل إلى صفحة **دفتر الأستاذ العام > الإعداد > محددات دفتر الأستاذ العام**، وحدد علامة تبويب **ضريبة المبيعات**، ثم قم بتوسيع علامة التبويب السريعة **خيارات الضريبة**.</span><span class="sxs-lookup"><span data-stu-id="77c62-131">To specify that the cash discount is calculated based on the amount plus sales tax, go to **General ledger > Setup > General ledger parameters**, and then select the **Sales tax** tab. Expand the **Tax options** FastTab.</span></span> 

<span data-ttu-id="77c62-132">تحتاج إلى تمكين خيار **احتساب الخصم النقدي المفروض على المبلغ متضمناً ضريبة المبيعات** في منطقة **الخصم النقدي للمورد**.</span><span class="sxs-lookup"><span data-stu-id="77c62-132">You need to enable the **Cash discount is calculated on amount including sales tax** option in the **Vendor cash discount** area.</span></span> 


<span data-ttu-id="77c62-133">[![لقطة شاشة لعلامة تبويب ضريبة المبيعات، مع تمييز منطقه الخصم النقدي للمورد.](../media/vendor-cash-discount.png)](../media/vendor-cash-discount.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="77c62-133">[![Screenshot of the  Sales tax tab with the Vendor cash discount area hightlighted.](../media/vendor-cash-discount.png)](../media/vendor-cash-discount.png#lightbox)</span></span>

