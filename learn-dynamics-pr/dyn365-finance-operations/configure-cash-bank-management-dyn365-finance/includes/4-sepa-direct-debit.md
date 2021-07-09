---
ms.openlocfilehash: 56fb28d88587dc619d668ddd1df2458cbcd46898
ms.sourcegitcommit: 39329122b3d8cf83af3522a38bd0fd4b383e1cc3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/13/2021
ms.locfileid: "6071007"
---
<span data-ttu-id="8dc83-101">تم إعداد منطقة التداول باليورو (سيبا) بواسطة المفوضية الأوروبية، والتي تقتضي أن تعتبر جميع عمليات الدفع الإلكترونية داخلية، بغض النظر عن البلد أو المنطقة التي يوجد فيها الفرد والشركة والمؤسسة والبنك.</span><span class="sxs-lookup"><span data-stu-id="8dc83-101">The Single Euro Payments Area (SEPA) is set up by the European Commission, and dictates that all electronic payments are considered domestic, regardless of the country or region where the individual, business, organization, and bank are located.</span></span> 

<span data-ttu-id="8dc83-102">ليس هناك فرق بين المدفوعات داخل الدولة والمدفوعات عبر الحدود.</span><span class="sxs-lookup"><span data-stu-id="8dc83-102">There is no difference between national and cross-border payments.</span></span> <span data-ttu-id="8dc83-103">تضم سيبا الدول الأعضاء في الاتحاد الأوروبي (EU) وعددها 28 دولة، بالإضافة إلى أيسلندا وليختنشتاين والنرويج وسويسرا وموناكو وسان مارينو.</span><span class="sxs-lookup"><span data-stu-id="8dc83-103">SEPA includes the 28 European Union (EU) member states, in addition to Iceland, Liechtenstein, Norway, Switzerland, Monaco, and San Marino.</span></span> <span data-ttu-id="8dc83-104">تساعد سيبا في إنشاء سوق واحد لحركات الدفع داخل المنطقة الاقتصادية الأوروبية (EEA).</span><span class="sxs-lookup"><span data-stu-id="8dc83-104">SEPA helps create a single market for payment transactions within the European Economic Area (EEA).</span></span> <span data-ttu-id="8dc83-105">وفي النهاية، من المتوقع أن تقوم سيبا بتقليل عدد تنسيقات الدفع التي يجب أن تعمل البنوك والشركات والأفراد من خلالها.</span><span class="sxs-lookup"><span data-stu-id="8dc83-105">Ultimately, SEPA is expected to reduce the number of payment formats that banks, businesses, and individuals must work with.</span></span>

<span data-ttu-id="8dc83-106">يتيح الدين المباشر لمنطقة التداول باليورو (سيبا) جمع أموال من الحساب البنكي للعميل، شريطة منح تفويض مُوقَع من العميل إلى الدائن.</span><span class="sxs-lookup"><span data-stu-id="8dc83-106">A Single Euro Payments Area (SEPA) direct debit lets a creditor collect funds from a customer's bank account, provided that the customer has granted a signed mandate to the creditor.</span></span> 

<span data-ttu-id="8dc83-107">ويوقع العميل تفويضاً يخول فيه الدائن لجمع مبلغ ويُعلم بنك العميل بدفع المبلغ.</span><span class="sxs-lookup"><span data-stu-id="8dc83-107">The mandate that the customer signs authorizes the creditor to collect a payment and instructs the customer's bank to pay the collection.</span></span> <span data-ttu-id="8dc83-108">تم تنظيم هذا الموضوع لعرض عملية إعداد تفويضات دين سيبا المباشر.</span><span class="sxs-lookup"><span data-stu-id="8dc83-108">This topic is organized to show the process for setting up SEPA direct debit mandates.</span></span> 

<span data-ttu-id="8dc83-109">تقوم ديون سيبا المباشرة بإنشاء أداة دفع للمرة الأولى يمكن استخدامها لكل من الديون المباشرة باليورو داخل الدول وعبر الحدود في دول أو مناطق سيبا البالغة 32.</span><span class="sxs-lookup"><span data-stu-id="8dc83-109">SEPA Direct Debits create, for the first time, a payment instrument that can be used for both national and cross-border euro direct debits throughout the 32 SEPA countries or regions.</span></span>

<span data-ttu-id="8dc83-110">يتوفر نظامان: نظام ديون سيبا المباشرة الأساسي ونظام ديون سيبا المباشرة بين متاجرة عمل-عمل (B2B).</span><span class="sxs-lookup"><span data-stu-id="8dc83-110">Two schemes are available: the SEPA Core Direct Debit Scheme and the SEPA Business to Business (B2B) Direct Debit Scheme.</span></span> <span data-ttu-id="8dc83-111">يستخدم كلا النظامين نفس تنسيق الملف.</span><span class="sxs-lookup"><span data-stu-id="8dc83-111">Both schemes use the same file format.</span></span>

## <a name="create-a-direct-debit-mandate-for-a-customer"></a><span data-ttu-id="8dc83-112">إنشاء تفويض دين مباشر لعميل</span><span class="sxs-lookup"><span data-stu-id="8dc83-112">Create a direct debit mandate for a customer</span></span>
<span data-ttu-id="8dc83-113">تصف الخطوات التالية كيفية:</span><span class="sxs-lookup"><span data-stu-id="8dc83-113">The steps below describe how to:</span></span>

-   <span data-ttu-id="8dc83-114">إنشاء تفويض دين مباشر لعميل.</span><span class="sxs-lookup"><span data-stu-id="8dc83-114">Create a direct debit mandate for a customer.</span></span>
-   <span data-ttu-id="8dc83-115">تحديد طريقة الدفع الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="8dc83-115">Define the electronic payment method.</span></span>
-   <span data-ttu-id="8dc83-116">إضافة تفويض دين مباشر لعميل.</span><span class="sxs-lookup"><span data-stu-id="8dc83-116">Add a direct debit mandate to a customer.</span></span>

### <a name="create-a-bank-account"></a><span data-ttu-id="8dc83-117">إنشاء حساب بنكي</span><span class="sxs-lookup"><span data-stu-id="8dc83-117">Create a bank account</span></span>
1.  <span data-ttu-id="8dc83-118">انتقل إلى **الوحدات النمطية > حسابات المقبوضات > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-118">Go to **Modules > Accounts receivable > Customers > All customers**.</span></span>
2.  <span data-ttu-id="8dc83-119">في القائمة، حدد أحد السجلات.</span><span class="sxs-lookup"><span data-stu-id="8dc83-119">In the list, select a record.</span></span> 
3.  <span data-ttu-id="8dc83-120">في جزء الإجراء، حدد **عميل**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-120">On the Action Pane, select **Customer**.</span></span>
4.  <span data-ttu-id="8dc83-121">حدد **الحسابات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-121">Select **Bank accounts**.</span></span>
5.  <span data-ttu-id="8dc83-122">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-122">Select **New**.</span></span>
6.  <span data-ttu-id="8dc83-123">في حقل **الحساب البنكي**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-123">In the **Bank account** field, enter a value.</span></span>
7.  <span data-ttu-id="8dc83-124">في حقل **الاسم**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-124">In the **Name** field, enter a value.</span></span>
8.  <span data-ttu-id="8dc83-125">في حقل **IBAN**‬، أدخل رقم IBAN الذي زودتك به مؤسستك البنكية.</span><span class="sxs-lookup"><span data-stu-id="8dc83-125">In the **IBAN** field, enter the IBAN number provided by your banking institution.</span></span>
9.  <span data-ttu-id="8dc83-126">في حقل **العملة**، أدخل قيمةً.</span><span class="sxs-lookup"><span data-stu-id="8dc83-126">In the **Currency** field, enter a value.</span></span>
10. <span data-ttu-id="8dc83-127">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-127">Select **Save**.</span></span>
11. <span data-ttu-id="8dc83-128">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-128">Close the page.</span></span>
12. <span data-ttu-id="8dc83-129">انتقل إلى **الوحدات النمطية > إدارة النقد والبنوك > الحسابات البنكية > الحسابات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-129">Go to **Modules > Cash and bank management > Bank accounts > Bank accounts**.</span></span>
13. <span data-ttu-id="8dc83-130">في القائمة، قم بالبحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="8dc83-130">In the list, find and select the desired record.</span></span>
14. <span data-ttu-id="8dc83-131">في القائمة، حدد الارتباط في الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="8dc83-131">In the list, select the link in the selected row.</span></span>
15. <span data-ttu-id="8dc83-132">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-132">Select **Edit**.</span></span>
16. <span data-ttu-id="8dc83-133">قُم بتوسيع علامة التبويب السريعة **تعريف إضافي**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-133">Expand the **Additional identification** FastTab.</span></span>
17. <span data-ttu-id="8dc83-134">في حقل **مُعرّف الدين المباشر**، أدخل قيمةً.</span><span class="sxs-lookup"><span data-stu-id="8dc83-134">In the **Direct debit ID** field, enter a value.</span></span>
18. <span data-ttu-id="8dc83-135">في حقل **IBAN**‬، أدخل رقم IBAN الذي زودتك به مؤسستك البنكية.</span><span class="sxs-lookup"><span data-stu-id="8dc83-135">In the **IBAN** field, enter the IBAN number provided by your banking institution.</span></span>
19. <span data-ttu-id="8dc83-136">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-136">Close the page.</span></span>

### <a name="define-the-electronic-payment-method"></a><span data-ttu-id="8dc83-137">تحديد طريقة الدفع الإلكترونية</span><span class="sxs-lookup"><span data-stu-id="8dc83-137">Define the electronic payment method</span></span>
1.  <span data-ttu-id="8dc83-138">في جزء التنقل، انتقل إلى **الوحدات النمطية > حسابات المقبوضات > إعداد المدفوعات > طرق الدفع**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-138">In the Navigation pane, go to **Modules > Accounts receivable > Payments setup > Methods of payment**.</span></span>
2.  <span data-ttu-id="8dc83-139">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-139">Select **New**.</span></span>
3.  <span data-ttu-id="8dc83-140">في حقل **طريقة الدفع**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-140">In the **Method of payment** field, enter a value.</span></span>
4.  <span data-ttu-id="8dc83-141">في حقل **الوصف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-141">In the **Description** field, enter a value.</span></span>
5.  <span data-ttu-id="8dc83-142">في حقل **نوع الدفع**، أدخل أو حدد **دفع إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-142">In the **Payment type** field, enter or select **Electronic payment**.</span></span> <span data-ttu-id="8dc83-143">يجب أن يكون **الدفع الإلكتروني** نوع الدفع لطريقة دفع تفويض الدين المباشر.</span><span class="sxs-lookup"><span data-stu-id="8dc83-143">The payment type for a direct debit mandate method of payment must be **Electronic payment**.</span></span>
6.  <span data-ttu-id="8dc83-144">حدد **نعم** في حقل **مطلوب تفويض**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-144">Select **Yes** in the **Require mandate** field.</span></span>
7.  <span data-ttu-id="8dc83-145">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-145">Close the page.</span></span>

### <a name="add-a-direct-debit-mandate-to-a-customer"></a><span data-ttu-id="8dc83-146">إضافة تفويض دين مباشر لعميل</span><span class="sxs-lookup"><span data-stu-id="8dc83-146">Add a direct debit mandate to a customer</span></span>
1.  <span data-ttu-id="8dc83-147">انتقل إلى **الوحدات النمطية > حسابات المقبوضات > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-147">Go to **Modules > Accounts receivable > Customers > All customers**.</span></span>
2.  <span data-ttu-id="8dc83-148">في القائمة، حدد أحد السجلات.</span><span class="sxs-lookup"><span data-stu-id="8dc83-148">In the list, select a record.</span></span> 
3.  <span data-ttu-id="8dc83-149">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-149">Select **Edit**.</span></span>
4.  <span data-ttu-id="8dc83-150">قُم بتوسيع علامة التبويب السريعة **القيم الافتراضية للدفع**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-150">Expand the **Payment defaults** FastTab.</span></span>
5.  <span data-ttu-id="8dc83-151">في حقل **طريقة الدفع**، أدخل أو حدد قيمةً.</span><span class="sxs-lookup"><span data-stu-id="8dc83-151">In the **Method of payment** field, enter or select a value.</span></span>
6.  <span data-ttu-id="8dc83-152">قُم بتوسيع علامة التبويب السريعة **القيم الافتراضية للدفع**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-152">Expand the **Payment defaults** FastTab.</span></span>
7.  <span data-ttu-id="8dc83-153">قُم بتوسيع علامة التبويب السريعة **تفويضات الدين المباشر**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-153">Expand the **Direct debit mandates** FastTab.</span></span>
8.  <span data-ttu-id="8dc83-154">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-154">Select **Add**.</span></span>
9.  <span data-ttu-id="8dc83-155">في الحقل **حساب البنك**، أدخل أو حدد قيمة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-155">In the **Bank account** field, enter or select a value.</span></span>
10. <span data-ttu-id="8dc83-156">في حقل **الحساب البنكي للدائن**، أدخل أو حدد قيمةً.</span><span class="sxs-lookup"><span data-stu-id="8dc83-156">In the **Creditor bank account** field, enter or select a value.</span></span>
11. <span data-ttu-id="8dc83-157">في حقل **تكرار الدفع**، أدخل عدد الدفعات التي تتوقع معالجتها لهذا التفويض.</span><span class="sxs-lookup"><span data-stu-id="8dc83-157">In the **Payment frequency** field, enter the number of payments that you expect to process for this mandate.</span></span>
12. <span data-ttu-id="8dc83-158">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-158">Select **OK**.</span></span>
13. <span data-ttu-id="8dc83-159">حدد **طباعة**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-159">Select **Print**.</span></span>
14. <span data-ttu-id="8dc83-160">حدد **تقرير التفويض**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-160">Select **Mandate report**.</span></span>
15. <span data-ttu-id="8dc83-161">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-161">Close the page.</span></span>
16. <span data-ttu-id="8dc83-162">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-162">Select **Edit**.</span></span>
17. <span data-ttu-id="8dc83-163">في حقل **تاريخ التوقيع**، أدخل تاريخاً.</span><span class="sxs-lookup"><span data-stu-id="8dc83-163">In the **Signature date** field, enter a date.</span></span>
18. <span data-ttu-id="8dc83-164">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-164">Select **Yes**.</span></span>
19. <span data-ttu-id="8dc83-165">أدخل موقع توقيع التفويض.</span><span class="sxs-lookup"><span data-stu-id="8dc83-165">Enter the location where the mandate was signed.</span></span>
20. <span data-ttu-id="8dc83-166">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8dc83-166">Select **OK**.</span></span>
21. <span data-ttu-id="8dc83-167">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="8dc83-167">Close the page.</span></span>
