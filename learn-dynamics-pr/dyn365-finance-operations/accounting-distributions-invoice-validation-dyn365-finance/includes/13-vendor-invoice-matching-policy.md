---
ms.openlocfilehash: 7312fd76aeefc0e2070ce58a82e5d0e5e853f6e0
ms.sourcegitcommit: 31f8966c7ff800511bc1374faf4606bac94e4dde
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/27/2020
ms.locfileid: "6070984"
---
> [!NOTE]
> <span data-ttu-id="95272-101">يجب إكمال المعمل السابق قبل البدء بهذا المعمل.</span><span class="sxs-lookup"><span data-stu-id="95272-101">You must complete the previous lab before starting this one.</span></span>

## <a name="scenario"></a><span data-ttu-id="95272-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="95272-102">Scenario</span></span>
<span data-ttu-id="95272-103">ستقوم بإنشاء فاتورة مورد من أمر شراء وعرض نتائج مطابقة أمر الشراء والاستلام والفاتورة (المطابقة ثلاثية الاتجاهات).</span><span class="sxs-lookup"><span data-stu-id="95272-103">You will create a vendor invoice from a purchase order and view the results of matching the purchase order, receipt, and invoice (three-way matching).</span></span>

## <a name="create-a-purchase-order-and-change-the-line-matching-policy"></a><span data-ttu-id="95272-104">إنشاء أمر شراء وتغيير سياسة مطابقة السطر</span><span class="sxs-lookup"><span data-stu-id="95272-104">Create a purchase order and change the line matching policy</span></span> 

1.  <span data-ttu-id="95272-105">في الشركة **USMF**، انتقل إلى **الحسابات الدائنة > أوامر الشراء > أوامر الشراء التي تم استلامها ولم تتم فوترتها**.</span><span class="sxs-lookup"><span data-stu-id="95272-105">In the company **USMF**, go to **Accounts payable > Purchase orders > Purchase orders received but not invoiced**.</span></span>
2.  <span data-ttu-id="95272-106">حدد أمر الشراء الذي قمت بإنشائه وملاحظته في التمرين السابق.</span><span class="sxs-lookup"><span data-stu-id="95272-106">Select the purchase order that you created and noted in the previous exercise.</span></span>
3.  <span data-ttu-id="95272-107">في جزء الإجراء، حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="95272-107">On the Action Pane, select **Invoice**.</span></span>
4.  <span data-ttu-id="95272-108">حدد **فاتورة**.</span><span class="sxs-lookup"><span data-stu-id="95272-108">Select **Invoice**.</span></span>
5.  <span data-ttu-id="95272-109">في الحقل **الرقم**، تحقق من حفظ القيمة **RainInv1** من التمرين 1.</span><span class="sxs-lookup"><span data-stu-id="95272-109">In the **Number** field, verify the value **RainInv1** is saved from exercise 1.</span></span> <span data-ttu-id="95272-110">ويمكن تعديله.</span><span class="sxs-lookup"><span data-stu-id="95272-110">This can be modified.</span></span>
6.  <span data-ttu-id="95272-111">في الحقل وصف الفاتورة، اكتب **العرض التوضيحي لمطابقة الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="95272-111">In the Invoice description field, type **Invoice matching demo**.</span></span>
7.  <span data-ttu-id="95272-112">في حقل **تاريخ الفاتورة**، أدخل تاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="95272-112">In the **Invoice date** field, enter today’s date.</span></span> 
8.  <span data-ttu-id="95272-113">ضمن علامة التبويب السريعة **البنود**، أدخل "1200" في الحقل **سعر الوحدة**.</span><span class="sxs-lookup"><span data-stu-id="95272-113">Under the **Lines** FastTab, enter '1200' in the **Unit price** field.</span></span>
9.  <span data-ttu-id="95272-114">حدد **إضافة سطر**.</span><span class="sxs-lookup"><span data-stu-id="95272-114">Select **Add line**.</span></span>
10. <span data-ttu-id="95272-115">في الحقل **رقم الصنف**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="95272-115">In the **Item number** field, select the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="95272-116">في القائمة، ابحث عن خدمات تثبيت **رقم الصنف** S0001.</span><span class="sxs-lookup"><span data-stu-id="95272-116">In the list, find the **item number** S0001 installation services.</span></span>
12. <span data-ttu-id="95272-117">لاحظ حقل **حالة المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="95272-117">Note the **Match status** field.</span></span> <span data-ttu-id="95272-118">لم يتم اجراء المطابقة.</span><span class="sxs-lookup"><span data-stu-id="95272-118">The matching has not been performed.</span></span>
13. <span data-ttu-id="95272-119">حدد **تحديث حالة المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="95272-119">Select **Update match status**.</span></span> <span data-ttu-id="95272-120">لاحظ حقل **حالة المطابقة**، الحالة هي **فشل**.</span><span class="sxs-lookup"><span data-stu-id="95272-120">Note the **Match status** field, the status is **Failed**.</span></span>
14. <span data-ttu-id="95272-121">في جزء الإجراء، حدد **مراجعة**.</span><span class="sxs-lookup"><span data-stu-id="95272-121">On the Action Pane, select **Review**.</span></span>
15. <span data-ttu-id="95272-122">حدد **تفاصيل المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="95272-122">Select **Matching details**.</span></span> <span data-ttu-id="95272-123">لا تلزم مطابقة السطر الجديد مع الخدمات لذلك تبقى الحالة **لم يتم التنفيذ**.</span><span class="sxs-lookup"><span data-stu-id="95272-123">The new line with services does not need to be matched so the status stays **Not performed**.</span></span> <span data-ttu-id="95272-124">ويحتوي A0001 أيضاً على اختلاف في السعر.</span><span class="sxs-lookup"><span data-stu-id="95272-124">Also, A0001 has a price discrepancy.</span></span>
16. <span data-ttu-id="95272-125">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="95272-125">Close the page.</span></span> 
17. <span data-ttu-id="95272-126">حدد بند الفاتورة للصنف A0001 الذي قمت باستلامه.</span><span class="sxs-lookup"><span data-stu-id="95272-126">Select the invoice line for item A0001 that you have received.</span></span> <span data-ttu-id="95272-127">تمت مطابقة السطر مع إيصال استلام المنتجات لكن هناك عدم تطابق في الكمية أو السعر، لذلك فشلت المطابقة.</span><span class="sxs-lookup"><span data-stu-id="95272-127">The line with the product receipt was matched but there is a mismatch of quantity or price, so it fails.</span></span>
18. <span data-ttu-id="95272-128">في حقل **سعر الوحدة**، أدخِل **12**.</span><span class="sxs-lookup"><span data-stu-id="95272-128">In the **Unit price** field, enter **12**.</span></span> 
19. <span data-ttu-id="95272-129">حدد **تحديث حالة المطابقة**.</span><span class="sxs-lookup"><span data-stu-id="95272-129">Select **Update match status**.</span></span> 
20. <span data-ttu-id="95272-130">والآن بعد تطابق سعر الوحدة، يتم تحديث الحقل **حالة المطابقة** إلى **ناجح**.</span><span class="sxs-lookup"><span data-stu-id="95272-130">Now that the unit price matches, the **Match status** field is updated to **Passed**.</span></span> <span data-ttu-id="95272-131">إذا كانت السياسة الخاصة بك تسمح بالاختلافات أو إذا كانت عملية المطابقة هي تحذير فقط، فلا يزال بإمكانك ترحيل الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="95272-131">If your policy allows discrepancies or if matching is only a warning, you can still post the invoice.</span></span>
21. <span data-ttu-id="95272-132">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="95272-132">Select **Post**.</span></span>
22. <span data-ttu-id="95272-133">يتم إغلاق الصفحة تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="95272-133">The page automatically closes.</span></span>
23. <span data-ttu-id="95272-134">لاحظ ان أمر الشراء لم يعد مدرجاً في الصفحة **أوامر الشراء التي تم استلامها ولم تتم فوترتها** نظرا لأنه قد تم ترحيله الآن.</span><span class="sxs-lookup"><span data-stu-id="95272-134">Note that the purchase order is no longer listed on the **Purchase orders received but not invoiced** page because it has been now posted.</span></span>
