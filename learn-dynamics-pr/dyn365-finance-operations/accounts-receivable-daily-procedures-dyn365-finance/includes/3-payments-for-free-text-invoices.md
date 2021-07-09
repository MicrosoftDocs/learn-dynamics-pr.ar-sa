---
ms.openlocfilehash: 2395b35c6dfbbb53cba7b8b6b81beaee4ab5690d
ms.sourcegitcommit: 886a6c468bde328603d5f79e74282140631ec884
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/05/2021
ms.locfileid: "6071036"
---
## <a name="set-up-and-process-recurring-invoices"></a><span data-ttu-id="0d7d7-101">إعداد ومعالجة الفواتير المتكررة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-101">Set up and process recurring invoices</span></span> 

<span data-ttu-id="0d7d7-102">يتم استخدام الفواتير المتكررة ذات النص الحر عندما تتم محاسبة العميل على أساس متكرر.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-102">Recurring free text invoices are used when a customer is to be billed on a recurring basis.</span></span>

<span data-ttu-id="0d7d7-103">لإنشاء فاتورة ذات نص حر متكرر، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0d7d7-103">To create a recurring free text invoice, follow these steps:</span></span>

1.  <span data-ttu-id="0d7d7-104">إنشاء قالب فاتورة نص حر.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-104">Create a free text invoice template.</span></span>
2.  <span data-ttu-id="0d7d7-105">تعيين القالب إلى عميل.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-105">Assign the template to a customer.</span></span>
3.  <span data-ttu-id="0d7d7-106">إنشاء وترحيل الفاتورة المتكررة.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-106">Generate and post the recurring invoice.</span></span>

<span data-ttu-id="0d7d7-107">يمكنك استخدام الفواتير المتكررة إذا كنت تقوم بفوترة العملاء بنفس المبلغ على أساس منتظم.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-107">You can use recurring invoices if you invoice customers for the same amount on a regular basis.</span></span>

## <a name="create-a-recurring-free-text-invoice-template"></a><span data-ttu-id="0d7d7-108">إنشاء قالب فاتورة ذات نص حر</span><span class="sxs-lookup"><span data-stu-id="0d7d7-108">Create a recurring free text invoice template</span></span>

<span data-ttu-id="0d7d7-109">لفوترة العملاء لنفس الخدمات بشكل منتظم، يتعين عليك تحديد قالب فاتورة ذات نص حر يمكن إعادة استخدامه لإنشاء الفواتير.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-109">To invoice customers for the same services on a regular basis, you need to define a free text invoice template that can be reused to create the invoices.</span></span> <span data-ttu-id="0d7d7-110">يحتوي هذا القالب على المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="0d7d7-110">This template contains the following information:</span></span>

-   <span data-ttu-id="0d7d7-111">معلومات العنوان، مثل مجموعات الضرائب، وشروط الدفع، وطريقة الدفع</span><span class="sxs-lookup"><span data-stu-id="0d7d7-111">Header information, such as tax groups, terms of payment, and the method of payment</span></span>
-   <span data-ttu-id="0d7d7-112">معلومات البند، مثل وصف الخدمة وحسابات الإيراد وسعر الوحدة ومبلغ الفاتورة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-112">Line information, such as the service description, revenue accounts, unit price, and invoice amount</span></span>
-   <span data-ttu-id="0d7d7-113">تكاليف الشحن أو المعالجة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-113">Charges for shipping or handling</span></span>
-   <span data-ttu-id="0d7d7-114">التوزيعات المحاسبية، مع معلومات البعد المالي، مثل مراكز التكلفة ووحدات الأعمال</span><span class="sxs-lookup"><span data-stu-id="0d7d7-114">Accounting distributions, together with financial dimension information, such as cost centers and business units</span></span>


<span data-ttu-id="0d7d7-115">بشكل أساسي، تقوم بإنشاء فاتورة بأكملها وتحفظها كقالب.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-115">Essentially, you're creating an entire invoice and saving it as a template.</span></span> <span data-ttu-id="0d7d7-116">يمكنك إعداد القوالب باستخدام صفحة  **إنشاء فواتير متكررة** .</span><span class="sxs-lookup"><span data-stu-id="0d7d7-116">You can set up the templates by using the **Generate recurring invoices** page.</span></span>

## <a name="generate-the-recurring-invoices"></a><span data-ttu-id="0d7d7-117">إنشاء الفواتير المتكررة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-117">Generate the recurring invoices</span></span>

<span data-ttu-id="0d7d7-118">تحتوي صفحة  **إنشاء الفواتير المتكررة** على مهمة تعالج قوالب الفواتير المتكررة، حيث يمكنك تحديد تاريخ الفاتورة والقالب لإنشاء الفواتير منها.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-118">The **Generate recurring invoices** page contains a task that processes recurring invoice templates, where you specify the invoice date and the template to generate the invoices from.</span></span> <span data-ttu-id="0d7d7-119">سيتم إنشاء الفواتير وتعيين رقم معرف تكرار فردي لكل مجموعة من مجموعات الفواتير التي تمت معالجتها.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-119">Invoices will be generated and assigned a single recurrence ID number for each group of invoices that is processed.</span></span>

## <a name="assign-a-free-text-invoice-template-to-a-customer-and-enter-recurrence-details"></a><span data-ttu-id="0d7d7-120">‏‫تعيين قالب فاتورة ذات نص حر إلى عميل وإدخال تفاصيل التكرار</span><span class="sxs-lookup"><span data-stu-id="0d7d7-120">Assign a free text invoice template to a customer and enter recurrence details</span></span>

<span data-ttu-id="0d7d7-121">بعد إنشاء القالب، تحتاج إلى تعيين القالب إلى العملاء الذين ترغب في فوترتهم.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-121">After the template is created, you need to assign the template to the customers that you want to invoice.</span></span> <span data-ttu-id="0d7d7-122">بالإضافة إلى ذلك، يجب تحديد متى وعدد المرات التي سيتم فيها استخدام الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-122">Additionally, you should specify when and how often the invoice will be used.</span></span> <span data-ttu-id="0d7d7-123">يمكنك تعيين القوالب في علامة التبويب  **الفاتورة** في صفحة  **العملاء** .</span><span class="sxs-lookup"><span data-stu-id="0d7d7-123">You can assign the templates on the **Invoice** tab of the **Customers** page.</span></span> <span data-ttu-id="0d7d7-124">أضف القالب إلى القائمة، ثم قم بتحديث المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="0d7d7-124">Add the template to the list, and update the following information:</span></span>

-   <span data-ttu-id="0d7d7-125">تاريخ البدء، واختياريأً، تاريخ الانتهاء للفوترة المتكررة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-125">The start date and, optionally, the end date for the recurring billing</span></span>
-   <span data-ttu-id="0d7d7-126">تكرار الفاتورة المتكررة (على سبيل المثال، كل يوم أو مرة كل شهر)</span><span class="sxs-lookup"><span data-stu-id="0d7d7-126">The frequency of the recurring billing (for example, every day or once a month)</span></span>
-   <span data-ttu-id="0d7d7-127">الحد الأقصى لمبلغ الفوترة (إذا كانت هذه المعلومات مطلوبة)</span><span class="sxs-lookup"><span data-stu-id="0d7d7-127">The maximum billing amount (if this information is required)</span></span>

![لقطة شاشة لعلامة التبويب "الفاتورة" في صفحة "العملاء".](../media/customers-invoice-tab.png)

<span data-ttu-id="0d7d7-129">يمكن أن يكون للعميل قوالب متعددة لها تكرارات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-129">A customer can have multiple templates that have different frequencies.</span></span>

## <a name="post-recurring-free-text-invoices"></a><span data-ttu-id="0d7d7-130">ترحيل الفواتير ذات النص الحر والمتكررة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-130">Post recurring free text invoices</span></span>

<span data-ttu-id="0d7d7-131">بعد إنشاء الفواتير المتكررة، تظهر معرفات تكرار الفاتورة في مهمة ترحيل في صفحة  **الفواتير المتكررة** .</span><span class="sxs-lookup"><span data-stu-id="0d7d7-131">After recurring invoices are generated, the invoice recurrence IDs appear in a posting task on the **Recurring invoices** page.</span></span>

![لقطة شاشة تبرز علامة التبويب "خيارات" في صفحة ترحيل الفواتير المتكررة.](../media/post-recurring-invoices.png)

<span data-ttu-id="0d7d7-133">يمكنك عرض جميع الفواتير الخاصة بمعرف التكرار عن طريق تحديد الارتباط.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-133">You can view all invoices for a recurrence ID by selecting the link.</span></span>
<span data-ttu-id="0d7d7-134">أثناء مراجعه الفواتير الخاصة بمعرف التكرار، يمكن حذف الفواتير الفردية.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-134">During your review of the invoices for the recurrence ID, you can delete individual invoices.</span></span> <span data-ttu-id="0d7d7-135">ستتم إعادة تعيين إعدادات تكرار العميل لهذا القالب بحيث يمكن إعادة إنشائها لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-135">The customer's recurrence settings will be reset for that template so that it can be regenerated later.</span></span> <span data-ttu-id="0d7d7-136">يمكنك ترحيل فاتورة واحدة أو عدد من الفواتير أو كلها لمعرف التكرار.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-136">You can post one, many, or all of the invoices for a recurrence ID.</span></span> <span data-ttu-id="0d7d7-137">في حالة تمكين مهام سير العمل، حدد  **إرسال** قبل ترحيل الفواتير.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-137">If workflows are enabled, select **Submit** before you post the invoices.</span></span>

## <a name="print-recurring-free-text-invoices"></a><span data-ttu-id="0d7d7-138">طباعة الفواتير ذات النص الحر والمتكررة</span><span class="sxs-lookup"><span data-stu-id="0d7d7-138">Print recurring free text invoices</span></span>

<span data-ttu-id="0d7d7-139">بعد ترحيل الفواتير المتكررة، يمكنك طباعه الفواتير من قائمة **الفواتير ذات النص الحر**.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-139">After recurring invoices are posted, you can print the invoices from the **Free text invoice** list page.</span></span> <span data-ttu-id="0d7d7-140">يمكنك طباعة الفواتير التي تم تحديدها، أو يمكنك تحديد مجموعة من الفواتير لطباعتها.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-140">You can print the invoices that are selected, or you can select a range of invoices to print.</span></span>


## <a name="subledger-journals-for-free-text-invoices"></a><span data-ttu-id="0d7d7-141">دفاتر يومية دفتر الأستاذ الفرعي للفواتير ذات النص الحر</span><span class="sxs-lookup"><span data-stu-id="0d7d7-141">Subledger journals for free text invoices</span></span> 

<span data-ttu-id="0d7d7-142">قبل أن تقوم بترحيل فاتورة ذات نص حر، يمكنك عرض الإدخال المحاسبي الكامل للفاتورة، والذي يتضمن الخصومات والائتمانات، للتحقق من ترحيل الفاتورة إلى الحسابات الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-142">Before you post a free text invoice, you can view the full accounting entry of the invoice, which includes debits and credits, to verify that the invoice is being posted to the correct accounts.</span></span> <span data-ttu-id="0d7d7-143">يُطلق على طريقة العرض هذه للإدخال المحاسبي الكامل اسم دفتر يومية دفتر الأستاذ الفرعي.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-143">This view of the full accounting entry is called a subledger journal.</span></span>

<span data-ttu-id="0d7d7-144">إذا كان إدخال دفتر اليومية في دفتر الأستاذ الفرعي غير صحيح عند معاينته قبل تسجيل الفاتورة ذات النص الحر في دفتر اليومية، فلا يمكنك تغيير إدخال دفتر اليومية في دفتر الأستاذ الفرعي.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-144">If the subledger journal entry is incorrect when you preview it before journalizing the free text invoice, you can't change the subledger journal entry.</span></span> <span data-ttu-id="0d7d7-145">بدلاً من ذلك، يجب عليك تغيير التوزيعات المحاسبية أو ملف تعريف الترحيل.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-145">Instead, you must change the accounting distributions or the posting profile.</span></span> <span data-ttu-id="0d7d7-146">تستخدم التوزيعات المحاسبية لتحديد جانب واحد من الإدخال المحاسبي، الخصم والائتمان.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-146">The accounting distributions are used to define one side of the accounting entry, the debit or the credit.</span></span> <span data-ttu-id="0d7d7-147">يتم إنشاء مقاصة إدخال حساب دفتر اليومية لدفتر الأستاذ الفرعي من ملفات تعريف الترحيل، مثل من حساب العميل أو الضريبة.</span><span class="sxs-lookup"><span data-stu-id="0d7d7-147">The offsetting subledger journal account entry is created from the posting profiles, such as from the customer account or the tax.</span></span>
