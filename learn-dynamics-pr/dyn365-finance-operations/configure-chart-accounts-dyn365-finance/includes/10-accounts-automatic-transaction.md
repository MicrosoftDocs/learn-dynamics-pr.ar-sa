---
ms.openlocfilehash: 9f090cb31e8ab88020f5b60e2ca95e87f9b062c6
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071056"
---
<span data-ttu-id="e0026-101">تكون الوحدات النمطية في Finance على درجة عالية من التكامل، لذا تتم معالجة العديد من عمليات الترحيل تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="e0026-101">The modules in Finance are highly integrated, so many postings are handled automatically.</span></span> <span data-ttu-id="e0026-102">وتوجد أوقات يتم فيها ترحيل إحدى الحركات لكن لا يوجد حساب دفتر أستاذ محدد لتلك الحركة.</span><span class="sxs-lookup"><span data-stu-id="e0026-102">There are times when a transaction is posted but there is no ledger account defined for that transaction.</span></span> 

<span data-ttu-id="e0026-103">على سبيل المثال، عند ترحيل فاتورة وتعيين الخصم، يتم ترحيل هذا المبلغ تلقائياً إلى حساب للخصومات.</span><span class="sxs-lookup"><span data-stu-id="e0026-103">For example, when an invoice is posted and a discount is given, this amount is posted automatically to an account for discounts.</span></span> <span data-ttu-id="e0026-104">ويجب إعداد الحساب المناسب لهذا النوع من الترحيل، من خلال حسابات النظام.</span><span class="sxs-lookup"><span data-stu-id="e0026-104">The appropriate account for that kind of posting must be set up, through system accounts.</span></span> <span data-ttu-id="e0026-105">ويمكن أن يكون فرقاً نقدياً أو حساب خطأ أو خصماً نقدياً.</span><span class="sxs-lookup"><span data-stu-id="e0026-105">It could be a penny difference, an error account, or a cash discount.</span></span> 

<span data-ttu-id="e0026-106">يمكنك تحديد حسابات للحركات التلقائية مثل الفروق التقريبية والإيرادات المحتجزة والخصومات.</span><span class="sxs-lookup"><span data-stu-id="e0026-106">You can specify accounts for automatic transactions such as rounding differences, retained earnings, and discounts.</span></span> 

<span data-ttu-id="e0026-107">**دفتر الأستاذ العام > إعداد الترحيل > حسابات للحركات التلقائية**</span><span class="sxs-lookup"><span data-stu-id="e0026-107">**General ledger > Posting setup > Accounts for automatic transactions**</span></span>
 
![لقطة شاشة للصفحة "حسابات الحركات التلقائية".](../media/account-auto-transaction.png)

<span data-ttu-id="e0026-109">بالنسبة إلى الكيان القانوني الذي تم إنشاؤه حديثاً، عندما تفتح الصفحة **حسابات الحركات التلقائية** للمرة الأولى، ستكون فارغة.</span><span class="sxs-lookup"><span data-stu-id="e0026-109">For a newly created legal entity, when you first open the **Accounts for automatic transactions** page, it will be blank.</span></span> <span data-ttu-id="e0026-110">ويمكنك تحديد **إنشاء أنواع افتراضية** في أعلى الصفحة لكي يتم إنشاء الإدخالات تلقائياً في الحقول **نوع الترحيل** و **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="e0026-110">You can select **Create default types** at the top of the page, to have entries automatically created in the **Posting type** and **Name** fields.</span></span> <span data-ttu-id="e0026-111">بعد ذلك، يجب عليك تحديد الحسابات الرئيسية المقابلة التي ترغب في تعيينها إلى قائمة الأنواع الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="e0026-111">Then, you must select the corresponding main accounts that you want to assign to the list of default types.</span></span>  

<span data-ttu-id="e0026-112">كما يمكنك إعداد حسابات أخرى لحركات تلقائية يدوياً.</span><span class="sxs-lookup"><span data-stu-id="e0026-112">You can also manually set up other accounts for automatic transactions.</span></span>  <span data-ttu-id="e0026-113">وتوجد قائمة منسدلة بأنواع الترحيل، إلى جانب أنه يمكنك إضافة المزيد إذا لزم الأمر.</span><span class="sxs-lookup"><span data-stu-id="e0026-113">There is a drop-down list of posting types, plus you can add more if needed.</span></span>  

<span data-ttu-id="e0026-114">**دفتر الأستاذ العام > إعداد الترحيل > حسابات للحركات التلقائية**</span><span class="sxs-lookup"><span data-stu-id="e0026-114">**General ledger > Posting setup > Accounts for automatic transactions**</span></span>

![لقطة شاشة للحقل "نوع الترحيل" في الصفحة "حسابات الحركات التلقائية".](../media/posting-types.png)

<span data-ttu-id="e0026-116">عند ترحيل الحركة في Finance، قد تتلقى رسالة خطأ إذا لم يتم إعداد نوع ترحيل معين ويحتاج إليها دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="e0026-116">When you post a transaction in Finance, you might receive an error message if a specific posting type is not set up and the journal needs it.</span></span> <span data-ttu-id="e0026-117">على سبيل المثال، إذا كنت تستخدم إدخال دفتر اليومية لأول مرة لنوع حركة محدد لم يتم تكوينه في الصفحة **حسابات الحركات التلقائية**.</span><span class="sxs-lookup"><span data-stu-id="e0026-117">For example, if you are using a journal entry for the first time for a specific transaction type that has not been configured on the **Accounts for automatic transactions** page.</span></span>  

<span data-ttu-id="e0026-118">في الصفحة **حسابات الحركات التلقائية**، راجع المعايير الآتية:</span><span class="sxs-lookup"><span data-stu-id="e0026-118">On the **Accounts for automatic transactions** page, consider the following criteria:</span></span> 

- <span data-ttu-id="e0026-119">تحديد الحسابات الرئيسية للحركات التلقائية التي يتعذر إعدادها في مكان آخر في Finance.</span><span class="sxs-lookup"><span data-stu-id="e0026-119">Specify the main accounts for automatic transactions that cannot be set up elsewhere in Finance.</span></span>  
- <span data-ttu-id="e0026-120">توجد حسابات تلقائية أخرى تم إعدادها في كل وحدة نمطية، على سبيل المثال، ملفات تعريف الترحيل في الوحدتين النمطيتين "الحسابات المدينة" و"الحسابات الدائنة".</span><span class="sxs-lookup"><span data-stu-id="e0026-120">There are other automatic accounts set up in each module, for example, posting profiles in the Accounts receivable and Accounts payable modules.</span></span>  

<span data-ttu-id="e0026-121">يلزم وجود **حساب الخطأ والفرق النقدي** و **حسابات نتيجة نهاية العام** للحركات التلقائية.</span><span class="sxs-lookup"><span data-stu-id="e0026-121">The **Error account, Penny difference**, and **Year-end result** accounts for automatic transactions are required.</span></span> <span data-ttu-id="e0026-122">يتم إعداد الحسابات الأخرى للحركة التلقائية وفقاً لما إذا كان يتم استخدام هذه الوظيفة.</span><span class="sxs-lookup"><span data-stu-id="e0026-122">The other accounts for automatic transaction are set up depending on whether that functionality is used.</span></span> 

<span data-ttu-id="e0026-123">في حالة تطبيق تحديث على مثيل Finance، يمكن إضافة حسابات جديدة للحركات التلقائية.</span><span class="sxs-lookup"><span data-stu-id="e0026-123">If an update is applied to your instance of Finance, new accounts for automatic transactions can be added.</span></span> <span data-ttu-id="e0026-124">حدد دائماً **إنشاء أنواع افتراضية** بعد تطبيق التحديث للتأكد من أن لديك جميع أنواع الحسابات الافتراضية الأخيرة.</span><span class="sxs-lookup"><span data-stu-id="e0026-124">Always select **Create default types** after an update has been applied to make sure that you have all the latest default account types.</span></span>

<span data-ttu-id="e0026-125">لمقاطعة التحديثات مع ظهور رسالة خطأ عند استخدام حساب الخطأ في عملية الترحيل، حدد خانة الاختيار  **مقاطعة في حالة الحساب الخطأ** الموجودة في الصفحة **معلمات دفتر الأستاذ العام**.</span><span class="sxs-lookup"><span data-stu-id="e0026-125">To interrupt updates with an error message when the error account is used in the posting process, select the **Interrupt in case of error account** check box on the **General ledger parameters** page.</span></span>

<span data-ttu-id="e0026-126">لتسجيل خصم نقدي أو تغييره يدوياً في عملية التسوية، يجب إعداد حساب نظام الخصم النقدي.</span><span class="sxs-lookup"><span data-stu-id="e0026-126">To register or manually change a cash discount in the settlement process, a cash discount system account must be set up.</span></span> <span data-ttu-id="e0026-127">لعرض خصم على إجمالي مبلغ الفاتورة، يجب أن يقوم خصم فاتورة العميل أو خصم فاتورة المورد أو كليهما بإعداد حسابات للحركات التلقائية لأنواع ترحيل الخصم النقدي للعميل والمورد.</span><span class="sxs-lookup"><span data-stu-id="e0026-127">To offer a discount on the total invoice amount, a customer invoice discount, vendor invoice discount, or both must be set up accounts for automatic transactions for customer and vendor cash discount posting types.</span></span>



