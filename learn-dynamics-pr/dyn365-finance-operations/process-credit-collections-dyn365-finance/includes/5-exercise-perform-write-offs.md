---
ms.openlocfilehash: 43514c9b3e001b2cd83bce4e18bfb6841f689955
ms.sourcegitcommit: 7d4cc5f2048fa309552e39da447684b1d06d0772
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/13/2021
ms.locfileid: "6071144"
---
## <a name="scenario"></a><span data-ttu-id="57df7-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="57df7-101">Scenario</span></span>

<span data-ttu-id="57df7-102">يحتوي هذا التدريب العملي على العديد من طرق لتنفيذ عمليات شطب العملاء.</span><span class="sxs-lookup"><span data-stu-id="57df7-102">This lab contains several methods to perform write-offs for customers.</span></span>

## <a name="write-off-a-customer-balance-from-the-aged-balances-page"></a><span data-ttu-id="57df7-103">شطب رصيد عميل من صفحة الأرصدة القديمة</span><span class="sxs-lookup"><span data-stu-id="57df7-103">Write off a customer balance from the Aged balances page</span></span> 

<span data-ttu-id="57df7-104">كمندوب تحصيلات في شركة **USMF**، تحتاج إلى إنشاء دفتر يومية شطب لأن شركة Birch لا تنوي دفع الرصيد بسبب حدوث خلل بالمنتجات التي تم شحنها إليها.</span><span class="sxs-lookup"><span data-stu-id="57df7-104">As a collection agent in company **USMF**, you need to create a write-off journal because the Birch company is not going to pay the balance due to defect with the products that were shipped to them.</span></span>

1.  <span data-ttu-id="57df7-105">الانتقال إلى شركة USMF</span><span class="sxs-lookup"><span data-stu-id="57df7-105">Go to company USMF</span></span>
2.  <span data-ttu-id="57df7-106">انتقل إلى **الائتمان والتحصيلات > التحصيلات > الأرصدة القديمة**.</span><span class="sxs-lookup"><span data-stu-id="57df7-106">Go to **Credit and collections > Collections > Aged balances**.</span></span>
3.  <span data-ttu-id="57df7-107">حدد الصف الذي تريد شطبه من حساب العميل.</span><span class="sxs-lookup"><span data-stu-id="57df7-107">Select the row for the customer that you want to write off.</span></span> <span data-ttu-id="57df7-108">علي سبيل المثال، حدد البند الذي يحتوي على **شركة Birch**.</span><span class="sxs-lookup"><span data-stu-id="57df7-108">For example, select the line with **Birch Company** on it.</span></span>
4.  <span data-ttu-id="57df7-109">في جزء الإجراءات **تحصيل**، حدد **شطب**.</span><span class="sxs-lookup"><span data-stu-id="57df7-109">In the **Collect** Action Pane, select **Write off**.</span></span>
6.  <span data-ttu-id="57df7-110">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="57df7-110">Select **OK**.</span></span>
7.  <span data-ttu-id="57df7-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="57df7-111">Close the page.</span></span>
8.  <span data-ttu-id="57df7-112">انتقل إلى **دفتر الأستاذ العام > إدخالات دفتر اليومية > دفاتر اليومية العامة**.</span><span class="sxs-lookup"><span data-stu-id="57df7-112">Go to **General ledger > Journal entries > General journals**.</span></span>
9.  <span data-ttu-id="57df7-113">حدد رقم دفعة دفتر اليومية لدفتر اليومية الذي يحتوي على عملية الشطب الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="57df7-113">Select the journal batch number for the journal that contains your write-off.</span></span> <span data-ttu-id="57df7-114">يتم إنشاء سطر واحد لعكس رصيد العميل.</span><span class="sxs-lookup"><span data-stu-id="57df7-114">One line is created to reverse the customer balance.</span></span> <span data-ttu-id="57df7-115">يتم إنشاء سطر واحد أو أكثر لترحيل الشطب إلى حساب الشطب.</span><span class="sxs-lookup"><span data-stu-id="57df7-115">One or more lines are created to post the write-off to the write-off account.</span></span>
10. <span data-ttu-id="57df7-116">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="57df7-116">Close all pages.</span></span>

<span data-ttu-id="57df7-117">تعرض هذه الصورة صفحة **الأرصدة القديمة** في **عمليات التحصيل والائتمان > التحصيلات**</span><span class="sxs-lookup"><span data-stu-id="57df7-117">This image shows the **Aged balances** page in **Credit and collections > Collections**</span></span>

![لقطة شاشة لصفحة الأرصدة القديمة مع تمييز دفاتر اليومية والشطب.](../media/writeoff-journal.png)

## <a name="write-off-an-invoice-using-the-open-customer-invoices-page"></a><span data-ttu-id="57df7-119">شطب فاتورة باستخدام صفحة "فتح فواتير العملاء"</span><span class="sxs-lookup"><span data-stu-id="57df7-119">Write off an invoice using the Open customer invoices page</span></span> 

1.  <span data-ttu-id="57df7-120">انتقل إلى **الحسابات المدينة > الفواتير > فتح فواتير العملاء‬‏‫**.</span><span class="sxs-lookup"><span data-stu-id="57df7-120">Go to **Accounts receivable > Invoices > Open customer invoices**.</span></span>
2.  <span data-ttu-id="57df7-121">حدد سطر فاتورة.</span><span class="sxs-lookup"><span data-stu-id="57df7-121">Select the line for an invoice.</span></span> <span data-ttu-id="57df7-122">على سبيل المثال، حدد السطر **CIV-000715**.</span><span class="sxs-lookup"><span data-stu-id="57df7-122">For example, select the line for **CIV-000715**.</span></span>
3.  <span data-ttu-id="57df7-123">في جزء الإجراء، حدد **الفاتورة > تحصيل**.</span><span class="sxs-lookup"><span data-stu-id="57df7-123">On the Action Pane, select **Invoice > Collect**.</span></span>
4.  <span data-ttu-id="57df7-124">حدد **شطب**.</span><span class="sxs-lookup"><span data-stu-id="57df7-124">Select **Write off.**</span></span>
5.  <span data-ttu-id="57df7-125">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="57df7-125">Select **OK**.</span></span>
6.  <span data-ttu-id="57df7-126">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="57df7-126">Close the page.</span></span>

<span data-ttu-id="57df7-127">تعرض هذه الصورة صفحة **فتح فواتير العملاء** في **الحسابات المدينة > الفواتير**</span><span class="sxs-lookup"><span data-stu-id="57df7-127">This image shows the **Open customer invoices** page in **Accounts receivable > Invoices**</span></span>

![لقطة شاشة لصفحة "فتح فواتير العملاء".](../media/writeoff-invoice-opencusts.png)

## <a name="write-off-a-customer-balance-using-the-customer-page"></a><span data-ttu-id="57df7-129">شطب رصيد عميل باستخدام صفحة العميل</span><span class="sxs-lookup"><span data-stu-id="57df7-129">Write off a customer balance using the Customer page</span></span> 

1.  <span data-ttu-id="57df7-130">انتقل إلى **الحسابات المدينة > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="57df7-130">Go to **Accounts receivable > Customers > All customers.**</span></span>
2.  <span data-ttu-id="57df7-131">حدد حساب عميل.</span><span class="sxs-lookup"><span data-stu-id="57df7-131">Select a customer account.</span></span> <span data-ttu-id="57df7-132">على سبيل المثال، حدد **US-001** (Contoso Retail San Diego).</span><span class="sxs-lookup"><span data-stu-id="57df7-132">For example, select **US-001** (Contoso Retail San Diego).</span></span>
3.  <span data-ttu-id="57df7-133">في جزء الإجراء، حدد **تجميع**.</span><span class="sxs-lookup"><span data-stu-id="57df7-133">On the Action Pane, select **Collect**.</span></span>
4.  <span data-ttu-id="57df7-134">حدد **شطب**.</span><span class="sxs-lookup"><span data-stu-id="57df7-134">Select **Write off**.</span></span>
5.  <span data-ttu-id="57df7-135">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="57df7-135">Select **OK**.</span></span>
6.  <span data-ttu-id="57df7-136">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="57df7-136">Close the page.</span></span>

<span data-ttu-id="57df7-137">تعرض هذه الصورة صفحة **كافة العملاء** في **الحسابات المدينة > العملاء**</span><span class="sxs-lookup"><span data-stu-id="57df7-137">This image shows the **All customers** page in **Accounts receivable > Customers**</span></span>

![لقطة شاشة لطريقة عرض كافة العملاء مع تمييز أرصدة العملاء والشطب.](../media/writeoff-custbalance.png)