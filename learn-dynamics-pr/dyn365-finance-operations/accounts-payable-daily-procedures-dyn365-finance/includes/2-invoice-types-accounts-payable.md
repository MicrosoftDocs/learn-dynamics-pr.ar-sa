---
ms.openlocfilehash: 0bbcfc2e9c543bb9f6afdcd6565f63ce609f56ed
ms.sourcegitcommit: 4ecdf5debbb9e9098084bff71834755f0976db57
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2021
ms.locfileid: "6071149"
---
<span data-ttu-id="de7c6-101">يختلف إجراء معالجة الفواتير الواردة من شركة إلى أخرى، اعتماداً على حجم الشركة وهيكلها وتنظيمها.</span><span class="sxs-lookup"><span data-stu-id="de7c6-101">The procedure for handling incoming invoices varies from company to company, depending on the company's size, structure, and organization.</span></span> <span data-ttu-id="de7c6-102">عادةً ما تكون الفواتير بإحدى الحالات التالية.</span><span class="sxs-lookup"><span data-stu-id="de7c6-102">The invoices are typically one of the following statuses.</span></span>

- <span data-ttu-id="de7c6-103">مسجلة</span><span class="sxs-lookup"><span data-stu-id="de7c6-103">Registered</span></span>
- <span data-ttu-id="de7c6-104">تمت الموافقة عليها</span><span class="sxs-lookup"><span data-stu-id="de7c6-104">Approved</span></span>
- <span data-ttu-id="de7c6-105">مدفوعة</span><span class="sxs-lookup"><span data-stu-id="de7c6-105">Paid</span></span>

<span data-ttu-id="de7c6-106">يدعم Dynamics 365 Finance عدة أساليب لإدارة الفواتير الواردة لتلبية إجراءات الشركة المختلفة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-106">Dynamics 365 Finance supports several methods of managing incoming invoices to cater to different company procedures.</span></span> <span data-ttu-id="de7c6-107">يحتوي النظام على دفتر يومية فواتير مختلف وفقاً لاحتياجات الشركة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-107">The system has a different invoice journal depending on the company’s needs.</span></span>
<span data-ttu-id="de7c6-108">تتوفر الأنواع التالية من الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-108">The following types of invoices are available.</span></span>

- <span data-ttu-id="de7c6-109">تسجيل الفاتورة والموافقة عليها</span><span class="sxs-lookup"><span data-stu-id="de7c6-109">Invoice register and approval</span></span> 
- <span data-ttu-id="de7c6-110">دفتر يومية الفواتير</span><span class="sxs-lookup"><span data-stu-id="de7c6-110">Invoice journal</span></span>
- <span data-ttu-id="de7c6-111">فواتير المورّد</span><span class="sxs-lookup"><span data-stu-id="de7c6-111">Vendor invoices</span></span>

<span data-ttu-id="de7c6-112">دعنا نراجع كل نوع من أنواع الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-112">Let's review each of the invoice types.</span></span> 

## <a name="invoice-register"></a><span data-ttu-id="de7c6-113">سجل الفواتير</span><span class="sxs-lookup"><span data-stu-id="de7c6-113">Invoice register</span></span> 

<span data-ttu-id="de7c6-114">الغرض من دفتر يومية سجل الفواتير هو التسجيل المسبق للفواتير عند وصولها إلى الشركة وتحويلها إلى مجموعة فواتير للموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="de7c6-114">The purpose of the invoice register journal is to pre-register invoices when they arrive at the company and transfer them to an invoice pool for approval.</span></span> <span data-ttu-id="de7c6-115">في دفتر يومية سجل الفواتير، يقوم الموظف بتسجيل المعلومات التالية.</span><span class="sxs-lookup"><span data-stu-id="de7c6-115">In the invoice register journal, an employee registers the following information.</span></span>

- <span data-ttu-id="de7c6-116">حساب المورد</span><span class="sxs-lookup"><span data-stu-id="de7c6-116">Vendor account</span></span>
- <span data-ttu-id="de7c6-117">رقم الفاتورة</span><span class="sxs-lookup"><span data-stu-id="de7c6-117">Invoice number</span></span>
- <span data-ttu-id="de7c6-118">المبلغ</span><span class="sxs-lookup"><span data-stu-id="de7c6-118">Amount</span></span>
- <span data-ttu-id="de7c6-119">الشخص الذي وافق على الفاتورة</span><span class="sxs-lookup"><span data-stu-id="de7c6-119">The person who approves the invoice</span></span> 

<span data-ttu-id="de7c6-120">يقوم نفس الموظف بالتحقق من صحة دفتر اليومية وإرساله إلى الحسابات المحددة في ملف تعريف الترحيل.</span><span class="sxs-lookup"><span data-stu-id="de7c6-120">The same employee validates and posts the journal to the accounts specified in the posting profile.</span></span> <span data-ttu-id="de7c6-121">عادةً ما تكون الحسابات معلقة حيث تتطلب المبالغ الموافقة اليدوية وإعادة التصنيف من قِبل الشخص المحدد في بند دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="de7c6-121">Usually, the accounts are pending accounts where the amounts require manual approval and reclassification by the person specified in the journal line.</span></span>

<span data-ttu-id="de7c6-122">لأسباب أمنية، يمكن لمستخدم واحد فقط في كل مرة إدخال بنود في دفتر يومية.</span><span class="sxs-lookup"><span data-stu-id="de7c6-122">For security reasons, only one user at a time can enter lines in a journal.</span></span> 

<span data-ttu-id="de7c6-123">بعد إدخال جميع بنود دفتر يومية الفاتورة، انقر على زر **ترحيل** لترحيل دفترة يومية الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-123">After you enter all the invoice journal lines, click the **Post** button to post the invoice journal.</span></span> <span data-ttu-id="de7c6-124">للوصول إلى صفحة **سجل الفواتير**، انتقل إلى **الحسابات الدائنة > الفواتير > سجل الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="de7c6-124">To access the **Invoice register** page, navigate to **Accounts payable > Invoices > Invoice register**.</span></span>

![لقطة شاشة لصفحة سجل الفواتير في Dynamics 365 Finance.](../media/invoice-register.png)


<span data-ttu-id="de7c6-126">تتوفر خيارات الترحيل التالية عند التعامل مع سجلات الفواتير في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="de7c6-126">The following posting options are available when working with invoice registers in the application.</span></span>

- <span data-ttu-id="de7c6-127">**الترحيل والنقل** – قم بترحيل البنود التي لا تحتوي على أخطاء، وانقل البنود التي بها أخطاء إلى دفتر يومية جديد.</span><span class="sxs-lookup"><span data-stu-id="de7c6-127">**Post and transfer** – Post lines that do not have errors, and transfer lines that have errors to a new journal.</span></span>
- <span data-ttu-id="de7c6-128">**ترحيل** - قم بترحيل البنود المحددة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-128">**Post** - Post the selected lines.</span></span> <span data-ttu-id="de7c6-129">في حالة وجود خطأ، لا يتم ترحيل أي بنود ويتم عرض رسالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="de7c6-129">If an error exists, no lines are posted and an error message is displayed.</span></span>

<span data-ttu-id="de7c6-130">عند ترحيل بنود دفتر اليومية، فإنك تقوم بنقلها إلى وعاء فواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-130">When posting the journal lines, you transfer them to an invoice pool.</span></span> <span data-ttu-id="de7c6-131">في دفتر يومية الموافقة على الفواتير، يمكنك نقلها من وعاء الفواتير إلى دفتر يومية الموافقة على الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-131">In an invoice approval journal, you can transfer them from the invoice pool into the invoice approval journal.</span></span>

## <a name="invoice-pool-and-approval-journal"></a><span data-ttu-id="de7c6-132">وعاء الفواتير ودفتر يومية الموافقة</span><span class="sxs-lookup"><span data-stu-id="de7c6-132">Invoice pool and approval journal</span></span> 

<span data-ttu-id="de7c6-133">بعد ترحيل بنود سجل الفواتير، يتم عرض الترحيلات في وعاء الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-133">After you post the lines of the invoice register, the postings display in the invoice pool.</span></span>

<span data-ttu-id="de7c6-134">لعرض الترحيلات في وعاء الفواتير، انتقل إلى **الحسابات الدائنة > الفواتير > وعاء الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="de7c6-134">To view the postings in the invoice pool, go to **Accounts payable > Invoices > Invoice pool**.</span></span>

<span data-ttu-id="de7c6-135">يعرض وعاء الفواتير المعلومات المرتبطة بالفواتير في انتظار الموافقة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-135">The invoice pool displays relevant information about the invoices awaiting approval.</span></span>

### <a name="scenario"></a><span data-ttu-id="de7c6-136">السيناريو</span><span class="sxs-lookup"><span data-stu-id="de7c6-136">Scenario</span></span>

<span data-ttu-id="de7c6-137">في أبريل، يقوم موظف الحسابات الدائنة بتسجيل فاتورة وارده في سجل الفواتير وترحيل التسجيل.</span><span class="sxs-lookup"><span data-stu-id="de7c6-137">April, the Accounts payable clerk, registers an incoming invoice in the invoice register and posts the registration.</span></span> <span data-ttu-id="de7c6-138">يرسل أبريل الفاتورة الفعلية إلى فيليس، مدير الحسابات، للموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="de7c6-138">April sends the physical invoice to Phyllis, the Accounting manager, for approval.</span></span> <span data-ttu-id="de7c6-139">يوافق فيليس على الفاتورة بتوقيع أو ختم ويعيد الفاتورة إلى أبريل.</span><span class="sxs-lookup"><span data-stu-id="de7c6-139">Phyllis approves the invoice with a signature or a stamp and returns the invoice to April.</span></span> <span data-ttu-id="de7c6-140">يقوم أبريل بتسجيل الموافقة وترحيلها في دفتر يومية الموافقة على الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-140">April registers and posts the approval in the invoice approval journal.</span></span> <span data-ttu-id="de7c6-141">الفاتورة جاهزه الآن ليتم دفعها.</span><span class="sxs-lookup"><span data-stu-id="de7c6-141">The invoice is now ready to be paid.</span></span>

<span data-ttu-id="de7c6-142">يحتفظ وعاء الفواتير بالفواتير الناشئة من أمر الشراء والتي تنشأ بدورها من سجل الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-142">The invoice pool holds invoices originating from a purchase order that, in turn originate from an invoice register.</span></span> <span data-ttu-id="de7c6-143">انتقل إلى **الحسابات الدائنة > الفواتير > وعاء الفواتير** ثم حدد زر **أمر الشراء** لتحديد أوامر الشراء والموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="de7c6-143">Go to **Accounts payable > Invoices > Invoice pool** then select the **Purchase order** button to select and approve the purchase orders.</span></span>
 
![لقطة شاشة لصفحة وعاء الفواتير في Dynamics 365 Finance.](../media/invoice-pool.png)


<span data-ttu-id="de7c6-145">يمكنك استخدام **الحسابات الدائنة > الفواتير > الموافقة على الفواتير** لمشاهدة جميع الفواتير المسجلة المعينة لك، ثم حدد فاتورة واحدة أو فواتير متعددة أو كل الفواتير لإضافتها إلى دفتر يومية الموافقة على الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-145">You can use **Accounts payable > Invoices > Invoice approval** to see all registered invoices assigned to you, and then select one, multiple, or all to add to the invoice approval journal.</span></span> 

<span data-ttu-id="de7c6-146">يجب عليك بعد ذلك التحقق من حسابات المصروفات لكل إيصال ثم ترحيل دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="de7c6-146">You should then verify the expense accounts for each voucher and then post the journal.</span></span>

<span data-ttu-id="de7c6-147">بالقيام بذلك، يعكس Finance الحركات في وعاء الفواتير، ثم يقوم بتحديث حساب ملخص المورد، الذي تم تعيينه في ملف تعريف الترحيل لحساب المورد الذي تم تعيينه لإيصال مسجل.</span><span class="sxs-lookup"><span data-stu-id="de7c6-147">By doing this, Finance reverses the transactions in the invoice pool, and then updates the vendor summary account, which was assigned in the posting profile for the vendor account that was assigned to a registered voucher.</span></span>

<span data-ttu-id="de7c6-148">[![لقطة شاشة لصفحة الموافقة على الفواتير في Dynamics 365 Finance.](../media/invoice-approval.png)](../media/invoice-approval.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="de7c6-148">[![Screenshot of the Invoice pproval page in Dynamics 365 Finance.](../media/invoice-approval.png)](../media/invoice-approval.png#lightbox)</span></span>


## <a name="invoice-journal"></a><span data-ttu-id="de7c6-149">دفتر يومية الفواتير</span><span class="sxs-lookup"><span data-stu-id="de7c6-149">Invoice journal</span></span> 

<span data-ttu-id="de7c6-150">يمكنك إدخال الفواتير مباشرة في دفتر يومية الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-150">You can enter invoices directly into the invoice journal.</span></span> <span data-ttu-id="de7c6-151">بشكل افتراضي، يوافق المستخدم الذي قام بتسجيل الدخول والذي يقوم بإدخال بنود دفتر اليومية على الفواتير.</span><span class="sxs-lookup"><span data-stu-id="de7c6-151">By default, the user who is logged in and who enters the journal lines approves the invoices.</span></span> 

<span data-ttu-id="de7c6-152">تم تصميم دفتر يومية الفواتير للمستخدمين لإدخال الفواتير التي يتلقونها من الموردين غير المرتبطين بأوامر الشراء.</span><span class="sxs-lookup"><span data-stu-id="de7c6-152">The invoice journal is designed for users to enter the invoices they receive from vendors that are not related to purchase orders.</span></span> <span data-ttu-id="de7c6-153">ستكون هذه عادةً للسلع باهظة الثمن وغير المخزنة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-153">These would typically be for expensed, non-stocked goods.</span></span> <span data-ttu-id="de7c6-154">بمجرد أن يقوم المستخدم بإدخال الفواتير الواردة، يمكن للمستخدم الترحيل.</span><span class="sxs-lookup"><span data-stu-id="de7c6-154">As soon as the user enters the incoming invoices, the user can post.</span></span> <span data-ttu-id="de7c6-155">يمكنك عرض واستخدام دفتر يومية الفاتورة بالانتقال إلى **الحسابات الدائنة > الفواتير > دفتر يومية الفواتير**</span><span class="sxs-lookup"><span data-stu-id="de7c6-155">You can view and use the invoice journal by going to **Accounts payable > Invoices > Invoice journal**</span></span>

![لقطة شاشة لصفحة دفتر يومية الفواتير في Dynamics 365 Finance.](../media/invoice-journal.png)


<span data-ttu-id="de7c6-157">[![لقطة شاشة لبنود الفاتورة في صفحة دفتر يومية فاتورة المورد في Dynamics 365 Finance.](../media/invoice-journal-lines.png)](../media/invoice-journal-lines.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="de7c6-157">[![Screenshot of the Invoice lines on the Vendor invoice journal page in Dynamics 365 Finance.](../media/invoice-journal-lines.png)](../media/invoice-journal-lines.png#lightbox)</span></span>

### <a name="scenario"></a><span data-ttu-id="de7c6-158">السيناريو</span><span class="sxs-lookup"><span data-stu-id="de7c6-158">Scenario</span></span>

<span data-ttu-id="de7c6-159">يقوم أبريل، موظف الحسابات الدائنة في Contoso، بفدخال الفاتورة مباشرةً في دفتر يومية جديد للفواتير، ثم يوافق على دفتر اليومية ويقوم بترحيله.</span><span class="sxs-lookup"><span data-stu-id="de7c6-159">April, the Accounts payable clerk at Contoso, enters the invoice directly into a new invoice journal, and then approves and posts the journal.</span></span> <span data-ttu-id="de7c6-160">الفاتورة جاهزه الآن ليتم دفعها.</span><span class="sxs-lookup"><span data-stu-id="de7c6-160">Now the invoice is ready to be paid.</span></span>

<span data-ttu-id="de7c6-161">يمكنك معرفة المزيد حول كيفية استخدام دفتر يومية الفواتير في هذا الفيديو.</span><span class="sxs-lookup"><span data-stu-id="de7c6-161">You can learn more about how to use the invoice journal in this video.</span></span>
<span data-ttu-id="de7c6-162">&nbsp;</span><span class="sxs-lookup"><span data-stu-id="de7c6-162">&nbsp;</span></span>
> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3ZYKR]


## <a name="accrued-purchases-excluding-sales-tax-report"></a><span data-ttu-id="de7c6-163">عمليات الشراء المستحقة باستثناء تقرير ضريبة المبيعات</span><span class="sxs-lookup"><span data-stu-id="de7c6-163">Accrued purchases excluding sales tax report</span></span>
<span data-ttu-id="de7c6-164">يعرض تقرير **المشتريات المستحقة** تفاصيل حول إيصالات استلام المنتج التي تم إدخالها وترحيلها، ولكن لم يتم تحرير فواتير بها، اعتباراً من تاريخ الانقطاع الذي تحدده.</span><span class="sxs-lookup"><span data-stu-id="de7c6-164">The **Accrued purchases** report displays details about the product receipts that are entered and posted, but not invoiced, as of the cutoff date that you specify.</span></span> <span data-ttu-id="de7c6-165">يحتوي التقرير على البيانات التي يمكنك استخدامها لتسوية واحد أو أكثر من حسابات الشراء المستحقة.</span><span class="sxs-lookup"><span data-stu-id="de7c6-165">The report contains data that you can use to reconcile one or more accrued purchase accounts.</span></span> 

<span data-ttu-id="de7c6-166">يتم عرض تفاصيل الفاتورة في التقرير عندما يكون أحد الشروط التالية صحيحاً:</span><span class="sxs-lookup"><span data-stu-id="de7c6-166">Invoice details are displayed on the report when one of the following conditions is true:</span></span>

- <span data-ttu-id="de7c6-167">يكون تاريخ حركة الاستلام قبل أو يساوي تاريخ الانقطاع، ويكون تاريخ حركة الفاتورة بعد تاريخ الانقطاع.</span><span class="sxs-lookup"><span data-stu-id="de7c6-167">The receipt transaction date is before or equal to the cutoff date, and the invoice transaction date is after the cutoff date.</span></span>
- <span data-ttu-id="de7c6-168">يكون تاريخ حركة الفاتورة قبل أو يساوي تاريخ الانقطاع، ويكون تاريخ حركة الإيصال بعد تاريخ الانقطاع.</span><span class="sxs-lookup"><span data-stu-id="de7c6-168">The invoice transaction date is before or equal to the cutoff date, and the receipt transaction date is after the cutoff date.</span></span>

<span data-ttu-id="de7c6-169">يُمكّنك حقل **تاريخ الانقطاع لتضمين الإيصالات المصححة** لإنشاء التقرير بناءً على تاريخ المحاسبة أو تاريخ الإصدار.</span><span class="sxs-lookup"><span data-stu-id="de7c6-169">The **Cutoff date for including corrected receipts** field enables you to generate the report based on the accounting date or the version date.</span></span> <span data-ttu-id="de7c6-170">تتيح هذه المرونة لموظفي الحسابات الدائنة تسوية وحساب معلومات المشتريات المستحقة بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="de7c6-170">This flexibility enables Accounts payable clerks to better reconcile and account for information for accrued purchases.</span></span>

![لقطة شاشة للمشتريات المستحقة باستثناء الاستعلام عن تقرير ضريبة المبيعات.](../media/accrued-purchases-report-ss.png)

