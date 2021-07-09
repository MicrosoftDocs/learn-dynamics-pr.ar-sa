---
ms.openlocfilehash: 4b9023fcd2a687227e95194f01c77d3a6c87c62a
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070843"
---
<span data-ttu-id="8af2c-101">يمكنك إعداد قيود على الشركة ونوع الحساب وقيمة المقطع.</span><span class="sxs-lookup"><span data-stu-id="8af2c-101">You can set up restrictions on the company, account type, and segment values.</span></span> 

<span data-ttu-id="8af2c-102">على سبيل المثال، باستخدام عنصر تحكم دفتر اليومية لاسم دفتر يومية، يمكنك السماح فقط باستخدام دفتر اليومية لإجراء عمليات التسوية.</span><span class="sxs-lookup"><span data-stu-id="8af2c-102">For example, by using the journal control for a journal name, you can only allow the journal to be used for adjustments.</span></span> <span data-ttu-id="8af2c-103">في هذه الحالة، يمكنك تحديد أن يكون نوع حساب **دفتر الأستاذ** فقط صالحاً لجميع الشركات أو شركة معينة.</span><span class="sxs-lookup"><span data-stu-id="8af2c-103">In this case, you can specify that only the **Ledger** account type is valid across all companies or a specific company.</span></span> 

<span data-ttu-id="8af2c-104">يمكن تحديد واحد أو أكثر من أنواع الحسابات التالية في عنصر تحكم دفتر اليومية:</span><span class="sxs-lookup"><span data-stu-id="8af2c-104">One or more of the following accounts types can be selected in the journal control:</span></span>

- <span data-ttu-id="8af2c-105">**الكل** - يتضمن كافة أنواع الحسابات.</span><span class="sxs-lookup"><span data-stu-id="8af2c-105">**All** - Includes all account types.</span></span>
- <span data-ttu-id="8af2c-106">**دفتر الأستاذ** - حدد نوع الحساب هذا إذا كنت تريد استخدام قيمة محددة أو نطاق من القيم للحسابات الرئيسية أو الأبعاد المالية المحددة في بنية الحساب المحدد فقط.</span><span class="sxs-lookup"><span data-stu-id="8af2c-106">**Ledger** - Select this account type if you want to use a specific value or a range of values for the main accounts, or financial dimensions defined in the selected account structure only.</span></span> <span data-ttu-id="8af2c-107">دفتر الأستاذ وجميع الأنواع هما الخياران الوحيدان اللذان يسمحان لك بتحديد قيم المقطع (الأبعاد المالية) الصالحة لدفتر اليومية المحدد.</span><span class="sxs-lookup"><span data-stu-id="8af2c-107">The Ledger and All types are the only two options that allow you to select which segment values (financial dimensions) are valid for the selected journal.</span></span>
- <span data-ttu-id="8af2c-108">**البنك**</span><span class="sxs-lookup"><span data-stu-id="8af2c-108">**Bank**</span></span>
- <span data-ttu-id="8af2c-109">**العميل**</span><span class="sxs-lookup"><span data-stu-id="8af2c-109">**Customer**</span></span>
- <span data-ttu-id="8af2c-110">**المورّد**</span><span class="sxs-lookup"><span data-stu-id="8af2c-110">**Vendor**</span></span>
- <span data-ttu-id="8af2c-111">**الأصول الثابتة**</span><span class="sxs-lookup"><span data-stu-id="8af2c-111">**Fixed assets**</span></span>
- <span data-ttu-id="8af2c-112">**المشروع**</span><span class="sxs-lookup"><span data-stu-id="8af2c-112">**Project**</span></span>

<span data-ttu-id="8af2c-113">بعد الانتهاء من إعداد عنصر تحكم دفتر اليومية على اسم دفتر اليومية، فعند استخدام اسم دفتر اليومية، يتحقق عنصر التحكم في دفتر اليومية أولاً من صحة أنواع الحسابات بالإضافة إلى أي قيم محددة لأي حسابات أو شرائح (الأبعاد المالية).</span><span class="sxs-lookup"><span data-stu-id="8af2c-113">After you’ve completed the setup of the journal control on a journal name, when you use the journal name, the journal control first checks the validity of the account types as well as any values defined for either accounts or segments (financial dimensions).</span></span> <span data-ttu-id="8af2c-114">إذا فشل التحقق من الصحة عند الترحيل، فستتلقى خطأ.</span><span class="sxs-lookup"><span data-stu-id="8af2c-114">If the validation fails upon posting, you will receive an error.</span></span>

<span data-ttu-id="8af2c-115">شاهد هذا الفيديو للتعرف على كيف يمكنك استخدام التحكم في دفتر اليومية لاسم دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="8af2c-115">Watch this video to learn how you can use journal control for a journal name.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE48hLn]

<span data-ttu-id="8af2c-116">لإعداد عنصر تحكم دفتر اليومية، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8af2c-116">To set up a journal control, follow these steps:</span></span>

1. <span data-ttu-id="8af2c-117">انتقل إلى **دفتر الأستاذ العام > إعداد دفتر اليومية > أسماء دفاتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="8af2c-117">Go to **General ledger > Journal setup > Journal names**.</span></span>
1. <span data-ttu-id="8af2c-118">في القائمة، قم بالبحث عن سجل وحدده.</span><span class="sxs-lookup"><span data-stu-id="8af2c-118">In the list, find and select a record.</span></span>
2.  <span data-ttu-id="8af2c-119">**عنصر التحكم في دفتر اليومية**.</span><span class="sxs-lookup"><span data-stu-id="8af2c-119">**Journal control**.</span></span>
1. <span data-ttu-id="8af2c-120">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="8af2c-120">Select **Add**.</span></span>
1. <span data-ttu-id="8af2c-121">في الحقل **حسابات الشركة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8af2c-121">In the **Company accounts** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="8af2c-122">في القائمة، قم بالبحث عن سجل وحدده.</span><span class="sxs-lookup"><span data-stu-id="8af2c-122">In the list, find and select a record.</span></span>
1. <span data-ttu-id="8af2c-123">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="8af2c-123">Select **Add**.</span></span>
1. <span data-ttu-id="8af2c-124">في الحقل **بنية الحساب**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8af2c-124">In the **Account structure** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="8af2c-125">في القائمة، قم بالبحث عن سجل وحدده.</span><span class="sxs-lookup"><span data-stu-id="8af2c-125">In the list, find and select a record.</span></span>
1. <span data-ttu-id="8af2c-126">في الحقل **مقطع**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8af2c-126">In the **Segment** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="8af2c-127">في القائمة، حدد بعداً مالياً.</span><span class="sxs-lookup"><span data-stu-id="8af2c-127">In the list, select a financial dimension.</span></span>
1. <span data-ttu-id="8af2c-128">في الحقل **من القيمة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8af2c-128">In the **From value** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="8af2c-129">في القائمة، قم بالبحث عن سجل وحدده.</span><span class="sxs-lookup"><span data-stu-id="8af2c-129">In the list, find and select a record.</span></span>
1. <span data-ttu-id="8af2c-130">في الحقل **إلى القيمة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="8af2c-130">In the **To value** field, select the drop-down button to open the lookup.</span></span>
1. <span data-ttu-id="8af2c-131">في القائمة، قم بالبحث عن سجل وحدده.</span><span class="sxs-lookup"><span data-stu-id="8af2c-131">In the list, find and select a record.</span></span>

