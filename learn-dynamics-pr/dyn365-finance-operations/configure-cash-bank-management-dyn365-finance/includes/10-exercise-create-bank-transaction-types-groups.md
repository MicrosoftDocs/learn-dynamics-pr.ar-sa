---
ms.openlocfilehash: 4f8d9db43f80f6f55893417f189d0652978a1ccf
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070960"
---
## <a name="scenario"></a><span data-ttu-id="32c54-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="32c54-101">Scenario</span></span>

<span data-ttu-id="32c54-102">يجب أن يقوم مسؤول الدفاتر في USMF بإنشاء نوع حركة بنكية لعمليات السحب النقدي.</span><span class="sxs-lookup"><span data-stu-id="32c54-102">The bookkeeper at USMF, must create a bank transaction type for cash withdrawals.</span></span> <span data-ttu-id="32c54-103">كما تريد USMF خياراً لتحليل إجمالي الرسوم المدفوعة لكل بنك.</span><span class="sxs-lookup"><span data-stu-id="32c54-103">USMF also wants the option to analyze the total charges paid to each bank.</span></span> <span data-ttu-id="32c54-104">وسيقوم مسؤول الدفاتر بإنشاء مجموعة حركات بنكية إضافية للرسوم البنكية ورسوم الفائدة.</span><span class="sxs-lookup"><span data-stu-id="32c54-104">The bookkeeper will create an additional bank transaction group for bank fees and interest charges.</span></span>

<span data-ttu-id="32c54-105">فاتبع الخطوات الآتية لمساعدته.</span><span class="sxs-lookup"><span data-stu-id="32c54-105">Follow the steps to help them.</span></span>

1.  <span data-ttu-id="32c54-106">إنشاء نوع حركة بنكية لعمليات السحب النقدي.</span><span class="sxs-lookup"><span data-stu-id="32c54-106">Create a bank transaction type for cash withdrawals.</span></span>
2.  <span data-ttu-id="32c54-107">إنشاء مجموعة حركات بنكية للرسوم البنكية.</span><span class="sxs-lookup"><span data-stu-id="32c54-107">Create a bank transaction group for bank charges.</span></span>
3.  <span data-ttu-id="32c54-108">تحديد معلمات البنك والنقد</span><span class="sxs-lookup"><span data-stu-id="32c54-108">Define cash and bank parameters</span></span>


## <a name="create-a-bank-transaction-type-for-cash-withdrawals"></a><span data-ttu-id="32c54-109">إنشاء نوع حركة بنكية لعمليات السحب النقدي</span><span class="sxs-lookup"><span data-stu-id="32c54-109">Create a bank transaction type for cash withdrawals</span></span>

1.  <span data-ttu-id="32c54-110">انتقل إلى **‏‫إدارة النقد والبنوك‬**، ثم قم بتوسيع **الإعداد**، ثم انقر على **أنواع الحركات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="32c54-110">Go to **Cash and bank management**, expand **Setup**, and then click **Bank transaction types**.</span></span>
2.  <span data-ttu-id="32c54-111">حدد الزر **جديد** لإدخال سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="32c54-111">Select the **New** button to insert a new record.</span></span>
3.  <span data-ttu-id="32c54-112">في الحقل **نوع الحركة البنكية**، أدخل **20**.</span><span class="sxs-lookup"><span data-stu-id="32c54-112">In the **Bank transaction type** field, enter **20**.</span></span>
4.  <span data-ttu-id="32c54-113">أدخل اسم **السحب النقدي** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="32c54-113">Enter the name **Cash Withdrawal** in the **Name** field.</span></span>
5.  <span data-ttu-id="32c54-114">اكتب **110110** في الحقل **الحساب الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="32c54-114">Type **110110** in the **Main account** field.</span></span>
6.  <span data-ttu-id="32c54-115">أغلق الصفحة **أنواع الحركات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="32c54-115">Close the **Bank transaction types** page.</span></span>


## <a name="create-a-bank-transaction-group-for-bank-charges"></a><span data-ttu-id="32c54-116">إنشاء مجموعة حركات بنكية للرسوم البنكية.</span><span class="sxs-lookup"><span data-stu-id="32c54-116">Create a bank transaction group for bank charges.</span></span> 

1.  <span data-ttu-id="32c54-117">انتقل إلى **‏‫إدارة النقد والبنوك‬**، ثم قم بتوسيع **الإعداد**، ثم انقر على **مجموعات الحركات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="32c54-117">Go to **Cash and bank management**, expand **Setup**, and then click **Bank transaction groups**.</span></span>
2.  <span data-ttu-id="32c54-118">حدد الزر **جديد** لإدخال سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="32c54-118">Select the **New** button to insert a new record.</span></span>
3.  <span data-ttu-id="32c54-119">في الحقل **مجموعات الحركات البنكية**، أدخل **80**.</span><span class="sxs-lookup"><span data-stu-id="32c54-119">In the **Bank transaction groups** field, enter **80**.</span></span>
4.  <span data-ttu-id="32c54-120">أدخل **الرسوم البنكية** في الحقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="32c54-120">Enter **Bank Charges** in the **Description** field.</span></span>
5.  <span data-ttu-id="32c54-121">من الصفحة **مجموعات الحركات البنكية**، حدد علامة التبويب السريعة **النوع**.</span><span class="sxs-lookup"><span data-stu-id="32c54-121">From the **Bank transaction groups** page, Select the **Type** FastTab.</span></span>
6.  <span data-ttu-id="32c54-122">حدد السهم **نوع الحركة البنكية** وحدد نوع الحركة البنكية **07** في **الرسوم**.</span><span class="sxs-lookup"><span data-stu-id="32c54-122">Select the **Bank transaction type** arrow and select the bank transaction type of **07** for **Fees**.</span></span> 
7.  <span data-ttu-id="32c54-123">تحقق من ملء الحقل **الاسم** تلقائياً باسم **نوع الحركة البنكية**.</span><span class="sxs-lookup"><span data-stu-id="32c54-123">Verify that the **Name** field is automatically populated with the **Bank transaction type** name.</span></span>
8.  <span data-ttu-id="32c54-124">حدد الزر **إضافة** لإدخال سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="32c54-124">Select the **Add** button to insert a new record.</span></span>
9.  <span data-ttu-id="32c54-125">حدد السهم **نوع الحركة البنكية** وحدد نوع الحركة البنكية **08** في **رسوم الفائدة**.</span><span class="sxs-lookup"><span data-stu-id="32c54-125">Select the **Bank transaction type** arrow and select the bank transaction type of **08** for **Interest charges**.</span></span> 
10. <span data-ttu-id="32c54-126">يتم ملء الحقل **الاسم** تلقائياً باسم **نوع الحركة البنكية**.</span><span class="sxs-lookup"><span data-stu-id="32c54-126">The **Name** field is automatically populated with the **Bank transaction type** name.</span></span>
11. <span data-ttu-id="32c54-127">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="32c54-127">Close the page.</span></span>


## <a name="define-cash-and-bank-parameters"></a><span data-ttu-id="32c54-128">تحديد معلمات البنك والنقد</span><span class="sxs-lookup"><span data-stu-id="32c54-128">Define cash and bank parameters</span></span> 

1.  <span data-ttu-id="32c54-129">انتقل إلى **‏‫إدارة النقد والبنوك‬**، ثم قم بتوسيع **الإعداد**، ثم انقر على **معلمات إدارة النقد والبنوك**.</span><span class="sxs-lookup"><span data-stu-id="32c54-129">Go to **Cash and bank management**, expand **Setup**, and then click **Cash and bank management parameters**.</span></span>
2.  <span data-ttu-id="32c54-130">حدد الارتباط **عام** إذا لم يتم تحديده تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="32c54-130">Select the **General** link if it is not automatically selected.</span></span>
3.  <span data-ttu-id="32c54-131">حدد **نوع الحركة البنكية** المستخدم في **الأرصدة غير الكافية**‏ (NSF) من القائمة **NSF**.</span><span class="sxs-lookup"><span data-stu-id="32c54-131">Select the **Bank transaction type** that is used for **NOT SUFFICIENT FUNDS** (NSF) from the **NSF** list.</span></span>
4.  <span data-ttu-id="32c54-132">حدد شريط التمرير **السماح بالشيكات للحسابات البنكية أو حسابات دفتر الأستاذ** لتحديد ما إذا كان من الممكن طباعة شيك لحساب بنكي أو حساب دفتر أستاذ.</span><span class="sxs-lookup"><span data-stu-id="32c54-132">Select the **Allow checks for bank or ledger accounts** slider to indicate whether a check can be printed for a bank or ledger account.</span></span>
5.  <span data-ttu-id="32c54-133">حدد مربع التمرير **السماح بإعادة استخدام الشيك** لتوضيح ما إذا كان من الممكن إعادة استخدام رقم الشيك في حالة طباعة الشيك بشكل غير صحيح أو عدم استخدام مخزون الشيك.</span><span class="sxs-lookup"><span data-stu-id="32c54-133">Select the **Allow check reuse** slider to indicate whether a check number can be reused if the check was printed incorrectly or the check stock was not used.</span></span>
6.  <span data-ttu-id="32c54-134">لطلب أكواد السبب للحركات البنكية، حدد شريط تمرير واحد أو أكثر في **متطلبات كود السبب** في **طلب أسباب عمليات إلغاء الدفع** و **طلب أسباب عمليات إلغاء الدفع بإيصال الإيداع**.</span><span class="sxs-lookup"><span data-stu-id="32c54-134">To require reason codes for bank transactions, select one or more of the sliders in the **Reason code requirements** for **Require reasons for payment reversals** and **Require reasons for deposit slip payment cancellations**.</span></span>
7.  <span data-ttu-id="32c54-135">أغلق الصفحة</span><span class="sxs-lookup"><span data-stu-id="32c54-135">Close the page</span></span>





