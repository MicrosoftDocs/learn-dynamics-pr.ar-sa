---
ms.openlocfilehash: d32e35e496806a6128e654f86056c5f82e347f51
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070870"
---
<span data-ttu-id="b6951-101">في هذا التمرين، ستقوم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="b6951-101">In this exercise, you will:</span></span>

1.  <span data-ttu-id="b6951-102">قم بإنشاء فاتورة من أمر مبيعات.</span><span class="sxs-lookup"><span data-stu-id="b6951-102">Create an invoice from a sales order.</span></span>
2.  <span data-ttu-id="b6951-103">قم بدمج الأوامر في فاتورة واحدة.</span><span class="sxs-lookup"><span data-stu-id="b6951-103">Combine orders into a single invoice.</span></span>
3.  <span data-ttu-id="b6951-104">قم بترحيل الفواتير الموجودة في إحدى الدفعات.</span><span class="sxs-lookup"><span data-stu-id="b6951-104">Post invoices in a batch.</span></span>

## <a name="create-an-invoice-from-a-sales-order"></a><span data-ttu-id="b6951-105">إنشاء فاتورة من أمر مبيعات</span><span class="sxs-lookup"><span data-stu-id="b6951-105">Create an invoice from a sales order</span></span> 

1.  <span data-ttu-id="b6951-106">في شركة USMF، انتقل إلى **الحسابات المدينة > الأوامر > أوامر المبيعات المشحونة وغير المفوترة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-106">In company USMF, go to **Accounts receivable > Orders > Shipped but not invoiced sales orders**.</span></span>
2.  <span data-ttu-id="b6951-107">حدد أمر مبيعات في القائمة.</span><span class="sxs-lookup"><span data-stu-id="b6951-107">Select a sales order in the list.</span></span>
3.  <span data-ttu-id="b6951-108">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-108">On the Action Pane, select **Invoice**.</span></span>
4.  <span data-ttu-id="b6951-109">حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-109">Select **Invoice**.</span></span> <span data-ttu-id="b6951-110">لاحظ أن أمر المبيعات هذا يحتوي على العديد من إيصالات التعبئة المرتبطة به.</span><span class="sxs-lookup"><span data-stu-id="b6951-110">Note that this sales order has multiple packing slips associated with it.</span></span> <span data-ttu-id="b6951-111">وهو سيعرض فقط الكلمة بدلاً من رقم إيصال التعبئة.</span><span class="sxs-lookup"><span data-stu-id="b6951-111">It will only show the word instead of the packing slip number.</span></span>
5.  <span data-ttu-id="b6951-112">قم بتوسيع القسم **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="b6951-112">Expand the **Parameters** section.</span></span> <span data-ttu-id="b6951-113">يجب تعيين الترحيل إلى **نعم** لترحيل الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b6951-113">Posting must be set to **Yes** to post the invoice.</span></span> <span data-ttu-id="b6951-114">يمكنك أيضاً إيقاف تشغيل الترحيل وطباعة الفاتورة فقط.</span><span class="sxs-lookup"><span data-stu-id="b6951-114">You can also turn off posting and just print the invoice.</span></span> <span data-ttu-id="b6951-115">ومع ذلك، يمكنك تحقيق نفس النتيجة عن طريق إنشاء فاتورة مبدئية بدلاً من الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="b6951-115">However, you can accomplish the same result by creating a pro forma invoice instead of an invoice.</span></span> <span data-ttu-id="b6951-116">يُستخدم هذا الخيار للوظائف الدفعية.</span><span class="sxs-lookup"><span data-stu-id="b6951-116">This option is used for batch jobs.</span></span> <span data-ttu-id="b6951-117">ويتم تشغيل الاستعلام عند تشغيل الوظيفة الدفعية.</span><span class="sxs-lookup"><span data-stu-id="b6951-117">The query is run when the batch job is run.</span></span>
6.  <span data-ttu-id="b6951-118">في الحقل **طباعة**، حدد **بعد**.</span><span class="sxs-lookup"><span data-stu-id="b6951-118">In the **Print** field, select **After**.</span></span>
7.  <span data-ttu-id="b6951-119">حدد **نعم** للقيام بـ **طباعة الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-119">Select **Yes** for **Print invoice**.</span></span>
    <span data-ttu-id="b6951-120">يمكن لإدارة الطباعة طباعة نسخ متعددة من الفاتورة وكذلك إرسال الفاتورة عبر البريد الإلكتروني كملف PDF.</span><span class="sxs-lookup"><span data-stu-id="b6951-120">Print management can print multiple copies of the invoice and also send the invoice by email as a PDF file.</span></span>
8.  <span data-ttu-id="b6951-121">في الحقل **طباعة التكاليف**، حدد **تلخيص**.</span><span class="sxs-lookup"><span data-stu-id="b6951-121">In the **Print charges** field, select **Summarize**.</span></span>
9.  <span data-ttu-id="b6951-122">في الحقل **فحص الحد الائتماني**، حدد **الرصيد**.</span><span class="sxs-lookup"><span data-stu-id="b6951-122">In the **Check credit limit** field, select **Balance**.</span></span>
10. <span data-ttu-id="b6951-123">حدد **إلغاء**.</span><span class="sxs-lookup"><span data-stu-id="b6951-123">Select **Cancel**.</span></span>

## <a name="combine-orders-into-a-single-invoice"></a><span data-ttu-id="b6951-124">دمج الأوامر في فاتورة واحدة</span><span class="sxs-lookup"><span data-stu-id="b6951-124">Combine orders into a single invoice</span></span> 

1.  <span data-ttu-id="b6951-125">انتقل إلى **الحسابات المدينة > الأوامر > جميع أوامر المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="b6951-125">Go to **Accounts receivable > Orders > All sales orders**.</span></span>
2.  <span data-ttu-id="b6951-126">حدد موقع عميل لديه فواتير متعددة مفتوحة.</span><span class="sxs-lookup"><span data-stu-id="b6951-126">Locate a customer that has multiple invoices open.</span></span>
3.  <span data-ttu-id="b6951-127">حدد أمر مبيعات مفتوح.</span><span class="sxs-lookup"><span data-stu-id="b6951-127">Select an open sales order.</span></span>
4.  <span data-ttu-id="b6951-128">حدد أمر مبيعات آخر مفتوح لنفس العميل.</span><span class="sxs-lookup"><span data-stu-id="b6951-128">Select another open sales order for the same customer.</span></span>
5.  <span data-ttu-id="b6951-129">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-129">On the Action Pane, select **Invoice**.</span></span>
6.  <span data-ttu-id="b6951-130">حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-130">Select **Invoice**.</span></span>
7.  <span data-ttu-id="b6951-131">قم بتوسيع القسم **المعلمات**.</span><span class="sxs-lookup"><span data-stu-id="b6951-131">Expand the **Parameters** section.</span></span>
8.  <span data-ttu-id="b6951-132">في الحقل **الكمية**، حدد **الكل**.</span><span class="sxs-lookup"><span data-stu-id="b6951-132">In the **Quantity** field, select **All**.</span></span> <span data-ttu-id="b6951-133">لاحظ أنه تم إدراج فاتورتين في القسم نظرة عامة.</span><span class="sxs-lookup"><span data-stu-id="b6951-133">Note that two invoices are listed in the overview section.</span></span> <span data-ttu-id="b6951-134">الآن، يمكنك دمجهما في فاتورة واحدة.</span><span class="sxs-lookup"><span data-stu-id="b6951-134">Now, you can merge them into a single invoice.</span></span>
9.  <span data-ttu-id="b6951-135">في **حقل تحديث الملخص لـ**، حدد **حساب الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-135">In the **Summary update for field**, select **Invoice account**.</span></span>
10. <span data-ttu-id="b6951-136">حدد **ترتيب** لدمج أوامر المبيعات في فاتورة واحدة.</span><span class="sxs-lookup"><span data-stu-id="b6951-136">Select **Arrange** to merge the sales orders into a single invoice.</span></span>
    <span data-ttu-id="b6951-137">يتم الآن دمج أمري المبيعات في فاتورة واحدة.</span><span class="sxs-lookup"><span data-stu-id="b6951-137">The two sales orders are now merged into a single invoice.</span></span>
11. <span data-ttu-id="b6951-138">حدد **إلغاء**.</span><span class="sxs-lookup"><span data-stu-id="b6951-138">Select **Cancel**.</span></span>
12. <span data-ttu-id="b6951-139">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="b6951-139">Select **Yes**.</span></span>

## <a name="post-invoices-in-a-batch"></a><span data-ttu-id="b6951-140">ترحيل الفواتير الموجودة في إحدى الدفعات</span><span class="sxs-lookup"><span data-stu-id="b6951-140">Post invoices in a batch</span></span> 

1.  <span data-ttu-id="b6951-141">انتقل إلى **الحسابات المدينة > الفواتير > فوترة الدُفعة >الفاتورة‬‏‫**.</span><span class="sxs-lookup"><span data-stu-id="b6951-141">Go to **Accounts receivable > Invoices > Batch invoicing > Invoice**.</span></span>
2.  <span data-ttu-id="b6951-142">حدد الخيار **تحديد**.</span><span class="sxs-lookup"><span data-stu-id="b6951-142">Select the **Select** option.</span></span>
3.  <span data-ttu-id="b6951-143">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b6951-143">Select **OK**.</span></span>
4.  <span data-ttu-id="b6951-144">حدد **دُفعة**.</span><span class="sxs-lookup"><span data-stu-id="b6951-144">Select **Batch**.</span></span>
5.  <span data-ttu-id="b6951-145">حدد **نعم** لتشغيل معالجة الدُفعة.</span><span class="sxs-lookup"><span data-stu-id="b6951-145">Select **Yes** to turn on batch processing.</span></span>
6.  <span data-ttu-id="b6951-146">حدد **تكرار**.</span><span class="sxs-lookup"><span data-stu-id="b6951-146">Select **Recurrence**.</span></span>
7.  <span data-ttu-id="b6951-147">حدد **الأيام**.</span><span class="sxs-lookup"><span data-stu-id="b6951-147">Select **Days**.</span></span>
8.  <span data-ttu-id="b6951-148">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b6951-148">Select **OK**.</span></span>
9.  <span data-ttu-id="b6951-149">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b6951-149">Select **OK**.</span></span>
10. <span data-ttu-id="b6951-150">حدد **إلغاء**.</span><span class="sxs-lookup"><span data-stu-id="b6951-150">Select **Cancel**.</span></span>
11. <span data-ttu-id="b6951-151">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="b6951-151">Select **Yes**.</span></span>
