---
ms.openlocfilehash: 250ce04e697eeea8f1595b715adc5a9dde9daf3d
ms.sourcegitcommit: e41ecaf7321ad74c447820357c8a21e7d6725302
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/04/2021
ms.locfileid: "6071003"
---
<span data-ttu-id="21b5a-101">توضح لك الخطوات الآتية كيفية استخدام سجل الفواتير لتسجيل الفواتير ثم استخدام دفتر يومية الموافقة لتحديث حسابات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="21b5a-101">The following steps show you how to use the invoice register to record invoices and then use the approval journal to update the expense accounts.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="21b5a-102">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="21b5a-102">Before you begin</span></span> ##
<span data-ttu-id="21b5a-103">لتحقيق أقصى استفادة من هذا التمرين والتمارين الأخرى الواردة في هذه الوحدة، نوصي بأن يكون لديك بيانات النماذج القياسية المتوفرة في Dynamics 365 Finance التي تم تثبيتها عبر Lifecycle services.</span><span class="sxs-lookup"><span data-stu-id="21b5a-103">To get the most out of this exercise and the other exercises that are included with this module, we recommend that you have the standard sample data available in Dynamics 365 Finance that is installed via Lifecycle services.</span></span>
 

## <a name="create-and-post-an-invoice"></a><span data-ttu-id="21b5a-104">إنشاء فاتورة وترحيلها</span><span class="sxs-lookup"><span data-stu-id="21b5a-104">Create and post an invoice</span></span> 

1.  <span data-ttu-id="21b5a-105">في **USMF**، انتقل إلى **الحسابات الدائنة > الفواتير > سجل الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-105">In **USMF**, go to **Accounts payable > Invoices > Invoice register**.</span></span>
2.  <span data-ttu-id="21b5a-106">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-106">Select **New**.</span></span>
3.  <span data-ttu-id="21b5a-107">حدد اسم سجل الفاتورة الذي تود استخدامه.</span><span class="sxs-lookup"><span data-stu-id="21b5a-107">Select the name of the invoice register that you want to use.</span></span>
4.  <span data-ttu-id="21b5a-108">حدد **بنود** لفتح السجل وإدخال بنود المصروفات.</span><span class="sxs-lookup"><span data-stu-id="21b5a-108">Select **Lines** to open the register and enter expense lines.</span></span>
5.  <span data-ttu-id="21b5a-109">حدد مُورِّداً.</span><span class="sxs-lookup"><span data-stu-id="21b5a-109">Select a vendor.</span></span> <span data-ttu-id="21b5a-110">على سبيل المثال، أدخل أو حدد **US-104**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-110">For example, enter or select **US-104**.</span></span>
6.  <span data-ttu-id="21b5a-111">في حقل **الفاتورة**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="21b5a-111">In the **Invoice** field, enter a value.</span></span>
7.  <span data-ttu-id="21b5a-112">في حقل **الوصف**، أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="21b5a-112">In the **Description** field, enter a value.</span></span>
8.  <span data-ttu-id="21b5a-113">في حقل **الائتمان**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="21b5a-113">In the **Credit** field, enter a number.</span></span>
9.  <span data-ttu-id="21b5a-114">في حقل **موافق عليه بواسطة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="21b5a-114">In the **Approved by** field, select the drop-down button to open the lookup.</span></span>
10. <span data-ttu-id="21b5a-115">ميِّز المُوافِق وحدد **تحديد** لتحديد هذا المُوافِق.</span><span class="sxs-lookup"><span data-stu-id="21b5a-115">Highlight an approver and select **Select** to select that approver.</span></span>
11. <span data-ttu-id="21b5a-116">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-116">select **Post**.</span></span>
12. <span data-ttu-id="21b5a-117">قم بإغلاق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="21b5a-117">Close all pages.</span></span>


## <a name="approve-an-invoice"></a><span data-ttu-id="21b5a-118">الموافقة على فاتورة</span><span class="sxs-lookup"><span data-stu-id="21b5a-118">Approve an invoice</span></span> 

1.  <span data-ttu-id="21b5a-119">انتقل إلى **الحسابات الدائنة > الفواتير > الموافقة على الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-119">Go to **Accounts payable > Invoices > Invoice approval**.</span></span>
2.  <span data-ttu-id="21b5a-120">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-120">Select **New**.</span></span>
3.  <span data-ttu-id="21b5a-121">حدد اسم دفتر يومية الموافقة على الفواتير الذي تود استخدامه.</span><span class="sxs-lookup"><span data-stu-id="21b5a-121">Select the name of the invoice approval journal that you want to use.</span></span>
4.  <span data-ttu-id="21b5a-122">حدد **البنود** لعرض صفحة يمكنك من خلالها تحديد الفواتير التي تود الموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="21b5a-122">Select **Lines** to display a page where you will be able to select the invoices that you want to approve.</span></span>
5.  <span data-ttu-id="21b5a-123">حدد **البحث عن إيصالات** لعرض جميع الفواتير الجاهزة للموافقة عليها.</span><span class="sxs-lookup"><span data-stu-id="21b5a-123">Select **Find Vouchers** to display all the invoices that are ready for approval.</span></span>
6.  <span data-ttu-id="21b5a-124">حدد الفاتورة التي قمت بإنشائها.</span><span class="sxs-lookup"><span data-stu-id="21b5a-124">Select the invoice that you created.</span></span>
7.  <span data-ttu-id="21b5a-125">حدد **تحديد**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-125">Select **Select**.</span></span> <span data-ttu-id="21b5a-126">تُنقل الإيصالات التي حددتها أعلاه إلى هذه القائمة بعد تحديدها.</span><span class="sxs-lookup"><span data-stu-id="21b5a-126">The vouchers that you selected above are moved to this list after you select them.</span></span>
8.  <span data-ttu-id="21b5a-127">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-127">Select **OK**.</span></span>
9.  <span data-ttu-id="21b5a-128">حدد حقل **الحساب** لإضافة حساب مصروفات إلى الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="21b5a-128">Select the **Account** field to add an expense account to the invoice.</span></span>
10. <span data-ttu-id="21b5a-129">أدخل رقم الحساب وأغلق الحقل.</span><span class="sxs-lookup"><span data-stu-id="21b5a-129">Enter an account number and tab off the field.</span></span> <span data-ttu-id="21b5a-130">على سبيل المثال، أدخل **600120**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-130">For example, enter **600120**.</span></span>
11. <span data-ttu-id="21b5a-131">حدد **ترحيل**.</span><span class="sxs-lookup"><span data-stu-id="21b5a-131">Select **Post**.</span></span>
12. <span data-ttu-id="21b5a-132">حدد **إيصال** لعرض القيود التي تم ترحيلها.</span><span class="sxs-lookup"><span data-stu-id="21b5a-132">Select **Voucher** to view the entries that were posted.</span></span> <span data-ttu-id="21b5a-133">يتم إلغاء حساب الموافقة قيد الانتظار على الفاتورة واستبداله بحساب المصروفات الفعلية.</span><span class="sxs-lookup"><span data-stu-id="21b5a-133">The Invoice pending approval account is reversed and replaced with the actual expense account.</span></span>

