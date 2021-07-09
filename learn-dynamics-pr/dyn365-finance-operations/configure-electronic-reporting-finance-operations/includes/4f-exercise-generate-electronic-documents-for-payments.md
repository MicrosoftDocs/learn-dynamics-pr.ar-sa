---
ms.openlocfilehash: 27fd9265ecb304bd7092470761b873b1eb8967b6
ms.sourcegitcommit: 92dc7d01a500c2ef16f130203f4ebfe1a7950200
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "6072026"
---
## <a name="scenario"></a><span data-ttu-id="2ecc1-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="2ecc1-101">Scenario</span></span>

<span data-ttu-id="2ecc1-102">بصفتك المدير المالي لشركة **USMF‎**، فأنت بحاجة إلى إعداد التقارير الإلكترونية نظراً لمتطلبات محلية.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-102">As the Finance manager for the company **USMF**, you need to set up Electronic reporting due to a local requirement.</span></span> <span data-ttu-id="2ecc1-103">لقد قام فريقك الفني بإعداد التنسيق، والآن تحتاج إلى اختباره، من خلال إنشاء ملف للتأكد من أنه يطابق ما هو مطلوب.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-103">Your technical team has set up the format, and now you need to test it, by creating a file to see that it matches what is needed.</span></span> 

## <a name="verify-file-format-is-set-up"></a><span data-ttu-id="2ecc1-104">تحقق من إعداد تنسيق الملف</span><span class="sxs-lookup"><span data-stu-id="2ecc1-104">Verify file format is set up</span></span>

1. <span data-ttu-id="2ecc1-105">في شركة **USMF‎** انتقل إلى **‏الحسابات الدائنة‏‎ > إعداد الدفع > طرق الدفع**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-105">In company **USMF** go to **Accounts payable > Payment setup > Methods of payment**.</span></span>
2. <span data-ttu-id="2ecc1-106">ضع المؤشر في شريط التنقل الأيسر على **إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-106">Place your cursor in the left navigation bar on **Electronic**.</span></span>
3. <span data-ttu-id="2ecc1-107">حدد علامة التبويب السريعة **تنسيقات الملف**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-107">Select the **File formats** FastTab.</span></span>
4. <span data-ttu-id="2ecc1-108">إذا لم يكن **تنسيق التصدير** **NACHA (US)**، فحدده.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-108">If the **Export format** is not **NACHA (US)**, then select it.</span></span>
5. <span data-ttu-id="2ecc1-109">حدد **حفظ**، ثم أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-109">**Save** and close the page.</span></span>

## <a name="test-the-format-of-generated-payment-files"></a><span data-ttu-id="2ecc1-110">قم باختبار تنسيق ملفات الدفع التي تم إنشاؤها</span><span class="sxs-lookup"><span data-stu-id="2ecc1-110">Test the format of generated payment files</span></span>

1.  <span data-ttu-id="2ecc1-111">انتقل إلى **الحسابات الدائنة > المدفوعات > دفتر يومية دفع المورد**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-111">Go to **Accounts payable > Payments > Vendor payment journal**.</span></span>
2.  <span data-ttu-id="2ecc1-112">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-112">Select **New**.</span></span>
3.  <span data-ttu-id="2ecc1-113">في حقل **الاسم**، حدد **VendPay‎**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-113">In the **Name** field, select **VendPay**.</span></span>
4.  <span data-ttu-id="2ecc1-114">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-114">Select **Save**.</span></span>
5.  <span data-ttu-id="2ecc1-115">حدد **البنود**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-115">Select **Lines**.</span></span>
6.  <span data-ttu-id="2ecc1-116">في حقل **الشركة**، أدخل **DEMF**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-116">In the **Company** field, enter **DEMF**.</span></span>
7.  <span data-ttu-id="2ecc1-117">في حقل **الحساب**، حدد القيمة **DE-01001**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-117">In the **Account** field, specify the value **DE-01001**.</span></span>
8.  <span data-ttu-id="2ecc1-118">في حقل **الوصف**، أدخل **الدفع**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-118">In the **Description** field, enter **Payment**.</span></span>
9.  <span data-ttu-id="2ecc1-119">في حقل **المدين**، أدخل **175**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-119">In the **Debit** field, enter **175**.</span></span>
10. <span data-ttu-id="2ecc1-120">حدد علامة التبويب **الدفع**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-120">Select the **Payment** tab.</span></span>
11. <span data-ttu-id="2ecc1-121">في حقل **طريقة الدفع**، حدد **إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-121">In the **Method of payment** field, select the **Electronic**.</span></span>
12. <span data-ttu-id="2ecc1-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-122">Select **Save**.</span></span>
13. <span data-ttu-id="2ecc1-123">حدد **إنشاء مدفوعات**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-123">Select **Generate payments**.</span></span>
14. <span data-ttu-id="2ecc1-124">في حقل **طريقة الدفع**، حدد **إلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-124">In the **Method of payment** field, select **Electronic**.</span></span>
15. <span data-ttu-id="2ecc1-125">في حقل **الحساب البنكي**، حدد **USMF OPER**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-125">In the **Bank account** field, select **USMF OPER**.</span></span>
15. <span data-ttu-id="2ecc1-126">حدد زر الخيار الموجود في **تنسيق التصدير**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-126">Select the radio button on **Export format**.</span></span>
16. <span data-ttu-id="2ecc1-127">حدد **تنسيق التصدير** الخاص بـ **NACHA (US)**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-127">Select the **Export format** of **NACHA (US)**.</span></span>
17. <span data-ttu-id="2ecc1-128">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-128">Select **OK**.</span></span>
15. <span data-ttu-id="2ecc1-129">لاحظ **اسم الملف** تم إنشاؤه.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-129">Note the **File name** created.</span></span> <span data-ttu-id="2ecc1-130">(رقم الدُفعة متبوعاً بالبنك، إلخ).</span><span class="sxs-lookup"><span data-stu-id="2ecc1-130">(The batch number followed by the bank, etc.).</span></span>
17. <span data-ttu-id="2ecc1-131">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-131">Select **OK**.</span></span> <span data-ttu-id="2ecc1-132">ستشاهد رسالة في أسفل الشاشة تطلب منك فتح الملف أو حفظه.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-132">You will see a message at the bottom of the screen asking you to open or save the file.</span></span> 
18. <span data-ttu-id="2ecc1-133">حدد **فتح**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-133">Select **Open**.</span></span> <span data-ttu-id="2ecc1-134">سترى الملف الإلكتروني في **المفكرة**.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-134">You will see the electronic file in **Notepad**.</span></span>
19. <span data-ttu-id="2ecc1-135">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-135">Close the page.</span></span>
