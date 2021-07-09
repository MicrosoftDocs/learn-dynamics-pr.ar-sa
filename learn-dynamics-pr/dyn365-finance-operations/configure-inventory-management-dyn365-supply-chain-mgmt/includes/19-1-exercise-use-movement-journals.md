---
ms.openlocfilehash: 5b1af28339ad1b42af2c049029d410760b388a22
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073234"
---
## <a name="scenario"></a><span data-ttu-id="8505a-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="8505a-101">Scenario</span></span>
<span data-ttu-id="8505a-102">في **USMF**، تحتاج إلى تحديث المخزون الفعلي يدوياً باستخدام دفتر يومية حركة المخزون.</span><span class="sxs-lookup"><span data-stu-id="8505a-102">In **USMF**, you need to manually update the on-hand inventory by using an Inventory movement journal.</span></span> 

1.  <span data-ttu-id="8505a-103">انتقل إلى **إدارة المخزون > إدخالات دفتر اليومية > أصناف > حركة**.</span><span class="sxs-lookup"><span data-stu-id="8505a-103">Go to **Inventory management > Journal entries > Items > Movement**.</span></span>
2.  <span data-ttu-id="8505a-104">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="8505a-104">Select **New**.</span></span>
3.  <span data-ttu-id="8505a-105">في الحقل **اسم**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8505a-105">In the **Name** field, select the drop-down button to open the lookup.</span></span>
4.  <span data-ttu-id="8505a-106">حدد **Imov‎**.</span><span class="sxs-lookup"><span data-stu-id="8505a-106">Select **Imov**.</span></span> <span data-ttu-id="8505a-107">من الممارسات الجيدة استخدام قوالب مختلفة لأسماء دفتر اليومية لأغراض العمل المختلفة.</span><span class="sxs-lookup"><span data-stu-id="8505a-107">It’s a good practice to use different journal name templates for the different business purposes.</span></span>
5.  <span data-ttu-id="8505a-108">في الحقل **حساب مقابل**، حدد القيمة **140200**.</span><span class="sxs-lookup"><span data-stu-id="8505a-108">In the **Offset account** field, specify the value **140200**.</span></span> <span data-ttu-id="8505a-109">هذا هو الحساب المقابل الذي سيكون الحساب الافتراضي في سطور دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8505a-109">This is the offset account that will be the default account on the journal lines.</span></span> <span data-ttu-id="8505a-110">من الممكن تجاوز الإعداد الافتراضي لتعيين حسابات مقابلة مختلفة لكل سطر.</span><span class="sxs-lookup"><span data-stu-id="8505a-110">It’s possible to override the default to assign different offset accounts for each line.</span></span>
6.  <span data-ttu-id="8505a-111">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8505a-111">Select **OK**.</span></span>
7.  <span data-ttu-id="8505a-112">حدد **جديد** في علامة التبويب السريعة **سطور دفتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="8505a-112">Select **New** in the **Journal lines** FastTab.</span></span>
8.  <span data-ttu-id="8505a-113">في الحقل **رقم الصنف**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8505a-113">In the **Item number** field, select the drop-down button to open the lookup.</span></span>
9.  <span data-ttu-id="8505a-114">حدد عنصر **A0001**.</span><span class="sxs-lookup"><span data-stu-id="8505a-114">Select item **A0001**.</span></span>
10. <span data-ttu-id="8505a-115">حدد علامة التبويب **أبعاد المخزون** في القسم **تفاصيل السطر**.</span><span class="sxs-lookup"><span data-stu-id="8505a-115">Select the **Inventory dimensions** tab in the **Line Details** section.</span></span>
11. <span data-ttu-id="8505a-116">في الحقل **الموقع**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8505a-116">In the **Site** field, select the drop-down button to open the lookup.</span></span>
12. <span data-ttu-id="8505a-117">حدد الموقع **1**.</span><span class="sxs-lookup"><span data-stu-id="8505a-117">Select site **1**.</span></span>
13. <span data-ttu-id="8505a-118">في الحقل **مستودع**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8505a-118">In the **Warehouse** field, select the drop-down button to open the lookup.</span></span>
14. <span data-ttu-id="8505a-119">حدد المستودع **13**.</span><span class="sxs-lookup"><span data-stu-id="8505a-119">Select warehouse **13**.</span></span>
15. <span data-ttu-id="8505a-120">في الحقل **موقع**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8505a-120">In the **Location** field, select the drop-down button to open the lookup.</span></span>
16. <span data-ttu-id="8505a-121">حدد الموقع **13**.</span><span class="sxs-lookup"><span data-stu-id="8505a-121">Select location **13**.</span></span>
17. <span data-ttu-id="8505a-122">في الحقل **كمية**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="8505a-122">In the **Quantity** field, enter a number.</span></span>
18. <span data-ttu-id="8505a-123">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8505a-123">Select **Save**.</span></span>
19. <span data-ttu-id="8505a-124">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="8505a-124">Select **Post**.</span></span>
20. <span data-ttu-id="8505a-125">عيّن شريط التمرير **تحويل كافة أخطاء الترحيل إلى دفتر يومية جديد** على **لا**.</span><span class="sxs-lookup"><span data-stu-id="8505a-125">Set the **Transfer all posting errors to a new journal** slider to **No**.</span></span> <span data-ttu-id="8505a-126">إذا قمت بتمكين هذا الخيار، فسيتم نسخ أي سطور تفشل في الترحيل إلى دفتر يومية جديد.</span><span class="sxs-lookup"><span data-stu-id="8505a-126">If you enable this option, any lines that fail to post will be copied to a new journal.</span></span> <span data-ttu-id="8505a-127">يمكنك استخدام المعلومات الموجودة في السجل لتصحيح المشكلات ثم إعادة ترحيل السطور.</span><span class="sxs-lookup"><span data-stu-id="8505a-127">You can use the information in the log to correct the issues and then re-post the lines.</span></span>
21. <span data-ttu-id="8505a-128">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8505a-128">Select **OK**.</span></span>
22. <span data-ttu-id="8505a-129">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="8505a-129">Close all pages.</span></span>


