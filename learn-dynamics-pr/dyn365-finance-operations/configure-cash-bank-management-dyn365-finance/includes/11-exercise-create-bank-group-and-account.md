---
ms.openlocfilehash: 7af6e8f7bb0d8e6fc04178a02040ee5d3fa7ffa9
ms.sourcegitcommit: 39329122b3d8cf83af3522a38bd0fd4b383e1cc3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/13/2021
ms.locfileid: "6071010"
---
## <a name="scenario"></a><span data-ttu-id="4ae6d-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="4ae6d-101">Scenario</span></span>

<span data-ttu-id="4ae6d-102">قامت شركة **USMF** بفتح حساب بنكي جديد.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-102">The **USMF** company has opened a new bank account.</span></span> <span data-ttu-id="4ae6d-103">سيعمل الحساب البنكي بشكل أساسي بالدولار الكندي (CAD)، ولكنه قد يعمل بعملات أخرى.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-103">The bank account will operate primarily in Canadian dollars (CAD), but might operate in other currencies.</span></span> <span data-ttu-id="4ae6d-104">يجب أن يقوم مسؤول الدفاتر بإنشاء مجموعة بنكية جديدة وحساب بنكي جديد في Finance لهذا البنك.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-104">The bookkeeper, must create a new bank group and new bank account in Finance for this bank.</span></span> <span data-ttu-id="4ae6d-105">ولا تتوفر له معلومات عنوان للحساب البنكي، لكن لديه المواصفات التالية.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-105">They don't have address information for the bank account, but do have the following specifications.</span></span>

<span data-ttu-id="4ae6d-106">للمجموعة البنكية:</span><span class="sxs-lookup"><span data-stu-id="4ae6d-106">For the bank group:</span></span>

- <span data-ttu-id="4ae6d-107">اسم المجموعة البنكية **RBCA** للبنك Royal Bank of Canada.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-107">The bank group name is **RBCA** for Royal Bank of Canada.</span></span>
- <span data-ttu-id="4ae6d-108">رقم توجيه المجموعة البنكية هو **8117**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-108">The bank group routing number is **8117**.</span></span>

<span data-ttu-id="4ae6d-109">للحساب البنكي:</span><span class="sxs-lookup"><span data-stu-id="4ae6d-109">For the bank account:</span></span>

- <span data-ttu-id="4ae6d-110">اسم الحساب البنكي هو حساب بنكي بالدولار الكندي.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-110">The bank account name is Bank Account CAD.</span></span>
- <span data-ttu-id="4ae6d-111">يعد الحساب البنكي جزءاً من البنك Royal Bank of Canada.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-111">The bank account is part of the Royal Bank of Canada group.</span></span>
- <span data-ttu-id="4ae6d-112">يجب أن تستخدم عمليات الترحيل حساب ميزانية جديداً يسمى حساب بنكي - دولار كندي.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-112">Postings should use a new balance account called Bank account - CAD.</span></span>

## <a name="create-a-new-account-for-cash-in-bank---cad-to-the-chart-of-accounts"></a><span data-ttu-id="4ae6d-113">إنشاء حساب جديد للنقدية في البنك - الدولار الكندي إلى دليل الحسابات</span><span class="sxs-lookup"><span data-stu-id="4ae6d-113">Create a new account for Cash in bank - CAD to the Chart of accounts</span></span> 

1.  <span data-ttu-id="4ae6d-114">انتقل إلى **دفتر الأستاذ العام > دليل الحسابات > الحسابات > الحسابات الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-114">Go to **General ledger > Chart of accounts > Accounts > Main accounts**.</span></span>
2.  <span data-ttu-id="4ae6d-115">تحقق من أن لديك الحساب 110115 – الحساب البنكي بالدولار الكندي.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-115">Verify that you do have the account 110115 – Bank Account CAD.</span></span> <span data-ttu-id="4ae6d-116">(في حالة وجودها، قم بالتخطي إلى المهمة الفرعية "إنشاء المجموعة البنكية الجديدة وتعيين الدولار الكندي (CAD) إليها".)</span><span class="sxs-lookup"><span data-stu-id="4ae6d-116">(If it exists, skip to the “Create the new bank group and assign the Canadian dollar (CAD) to it” subtask.)</span></span>
3.  <span data-ttu-id="4ae6d-117">حدد **جديد** لإنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-117">Select **New** to create a new record.</span></span>
4.  <span data-ttu-id="4ae6d-118">في الحقل **الحساب الرئيسي**، أدخل **110115**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-118">In the **Main account** field, enter **110115**.</span></span>
5.  <span data-ttu-id="4ae6d-119">في حقل **الاسم**، أدخِل **الحساب البنكي - الدولار الكندي**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-119">In the **Name** field, enter **Bank Account – CAD**.</span></span>
6.  <span data-ttu-id="4ae6d-120">حدد **الأصل** في الحقل **نوع الحساب الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-120">Select **Asset** in the **Main account type** field.</span></span>
7.  <span data-ttu-id="4ae6d-121">حدد السهم في حقل **العملة الافتراضية**، ثم انقر على **دولار كندي**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-121">Select the arrow in the **Default Currency** field, and then click **CAD**.</span></span>
8.  <span data-ttu-id="4ae6d-122">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-122">Close the page.</span></span>

## <a name="create-the-new-bank-group-and-assign-the-canadian-dollar-cad-to-it"></a><span data-ttu-id="4ae6d-123">إنشاء المجموعة البنكية الجديدة وتعيين الدولار الكندي (CAD) إليها</span><span class="sxs-lookup"><span data-stu-id="4ae6d-123">Create the new bank group and assign the Canadian dollar (CAD) to it</span></span> 

1.  <span data-ttu-id="4ae6d-124">انتقل إلى **‏‫إدارة النقد والبنوك‬ > إعداد > المجموعات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-124">Go to **Cash and bank management > Setup > Bank groups**.</span></span>
2.  <span data-ttu-id="4ae6d-125">حدد **جديد** لإنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-125">Select **New** to create a new record.</span></span>
3.  <span data-ttu-id="4ae6d-126">في الحقل **مجموعات بنكية**، أدخل **RBCA**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-126">In the **Bank groups** field, enter **RBCA**.</span></span>
4.  <span data-ttu-id="4ae6d-127">أدخِل **8117** في حقل **رقم التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-127">Enter **8117** in the **Routing number** field.</span></span>
5.  <span data-ttu-id="4ae6d-128">في الحقل **الاسم**، أدخل **Royal Bank of Canada**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-128">In the **Name** field, enter **Royal Bank of Canada**.</span></span>
6.  <span data-ttu-id="4ae6d-129">حدد علامة التبويب السريعة **عام**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-129">Select the **General** FastTab.</span></span>
7.  <span data-ttu-id="4ae6d-130">من قائمة **العملة** حدد **دولار كندي**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-130">From the **Currency** list, select **CAD**.</span></span>
8.  <span data-ttu-id="4ae6d-131">قم بإغلاق صفحة **المجموعات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="4ae6d-131">Close the **Bank groups** page.</span></span>





