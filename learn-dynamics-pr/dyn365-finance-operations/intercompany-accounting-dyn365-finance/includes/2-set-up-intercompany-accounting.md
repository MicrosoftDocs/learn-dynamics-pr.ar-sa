---
ms.openlocfilehash: 6013b2e406100b8a68b012de77adbae074ee5325
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6071139"
---
<span data-ttu-id="6b4e0-101">عند استخدام دفاتر اليومية للمحاسبة بين الشركات الشقيقة في Finance، فإن الحركات التي تم ترحيلها في إحدى الشركات ستؤدي إلى ترحيل الحركات ذات الصلة تلقائياً في الشركة الأخرى.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-101">When you use intercompany accounting daily journals in Finance, transactions posted in one company will cause the related transactions to post automatically in the other company.</span></span> 

<span data-ttu-id="6b4e0-102">توضح هذه الوحدة كيفية تكوين المحاسبة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-102">This unit explains how to configure Intercompany accounting.</span></span>

<span data-ttu-id="6b4e0-103">يجب إكمال الإعداد التالي لاستخدام المحاسبة بين الشركات الشقيقة:</span><span class="sxs-lookup"><span data-stu-id="6b4e0-103">The following setup must be completed to use intercompany accounting:</span></span>

1.  <span data-ttu-id="6b4e0-104">إنشاء الحسابات الرئيسية اللازمة في مخطط الحسابات.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-104">Create the necessary main accounts in the chart of accounts.</span></span>
2.  <span data-ttu-id="6b4e0-105">إعداد أسماء دفاتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-105">Set up journal names.</span></span>
3.  <span data-ttu-id="6b4e0-106">إعداد علاقات الترحيل بين الشركات.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-106">Set up the posting relationships between companies.</span></span>

<span data-ttu-id="6b4e0-107">شاهد هذا الفيديو للتعرف على كيفية إعداد المحاسبة بين الشركات الشقيقة في Finance:</span><span class="sxs-lookup"><span data-stu-id="6b4e0-107">Watch this video to learn how you can set up intercompany accounting in Finance:</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3TQTV]


## <a name="create-main-accounts"></a><span data-ttu-id="6b4e0-108">إنشاء حسابات رئيسية</span><span class="sxs-lookup"><span data-stu-id="6b4e0-108">Create main accounts</span></span> 

<span data-ttu-id="6b4e0-109">أولاً، تحتاج إلى إنشاء الحسابات الرئيسية بين الشركات الشقيقة لاستخدامها في إدخالات المحاسبة **مستحق إلى** و **مستحق من**.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-109">First, you need to create the intercompany main accounts to use for the **Due to** and **Due from** accounting entries.</span></span> <span data-ttu-id="6b4e0-110">نوصي باستخدام حسابات رئيسية فريدة لكل شركة لتبسيط التسوية والتخلص من إدخالات المحاسبة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-110">We recommend that you use unique main accounts for each company to simplify the reconciliation and elimination of intercompany accounting entries.</span></span> 

<span data-ttu-id="6b4e0-111">مخطط الحسابات هو إعداد عالمي، لذلك يمكن لجميع الشركات مشاركة مخطط حسابات واحد يحتوي على حسابات **مستحق إلى** و **مستحق من** الفريدة لكل شركة، أو يمكن أن يكون لكل شركة مخطط حسابات خاص بها.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-111">The chart of accounts is a global setup, so all companies could share one chart of accounts containing unique **Due to** and **Due from** accounts for each company, or each company could have their own chart of accounts.</span></span> 

<span data-ttu-id="6b4e0-112">يجب أن تشتمل الحسابات التي تم إنشاؤها في مخطط حسابات **مستحق إلى** و **مستحق من** على حقل **نوع الحساب الرئيسي** معيناً إلى **الميزانية العمومية** لكي يعمل الترحيل بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-112">The accounts that were created in the chart of accounts for **Due to** and **Due from** must have the **Main account type** field set to **Balance sheet** for the posting to work correctly.</span></span>

<span data-ttu-id="6b4e0-113">إذا كنت تستخدم شريكاً تجارياً أو بُعداً نظيراً لتحديد الطرف بين الشركات الشقيقة، فيمكنك تحديد هذا البعد كبُعد ثابت في الحساب الرئيسي المحدد في المحاسبة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-113">If you're using a trading partner or counterpart dimension to identify the intercompany party, you can define this dimension as a fixed dimension on the main account that is defined in intercompany accounting.</span></span> <span data-ttu-id="6b4e0-114">وصفحة **الحسابات الرئيسية** (**دفتر الأستاذ العام > مخطط الحسابات > الحسابات > الحسابات الرئيسية**) مبينة أدناه.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-114">The **Main accounts** page (**General ledger > Chart of accounts > Accounts > Main accounts**) is shown below.</span></span>


![لقطة شاشة لصفحة الحسابات الرئيسية توضح مكان تحديد حساب المستحق إلى أو المستحق من.](../media/main-accounts.png)

## <a name="set-up-journal-names"></a><span data-ttu-id="6b4e0-116">إعداد أسماء دفاتر اليومية</span><span class="sxs-lookup"><span data-stu-id="6b4e0-116">Set up journal names</span></span> 

<span data-ttu-id="6b4e0-117">بعد ذلك، سوف تحدد اسم دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-117">Next, you will define a journal name.</span></span> <span data-ttu-id="6b4e0-118">يجب إعداد أسماء دفتر اليومية في كل كيان قانوني.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-118">The journal names must be set up in each legal entity.</span></span> <span data-ttu-id="6b4e0-119">على سبيل المثال، قم بتعيين حقل **نوع دفتر اليومية** إلى **يومي** في صفحة **أسماء دفاتر اليومية** (**دفتر الأستاذ العام > إعداد دفتر اليومية > أسماء دفتر الأستاذ**).</span><span class="sxs-lookup"><span data-stu-id="6b4e0-119">For example, set the **Journal type** field to **Daily** on the **Journal names** page (**General ledger > Journal setup > Journal names**).</span></span> <span data-ttu-id="6b4e0-120">نوصي باستخدام اسم دفتر يومية محدد للمحاسبة بين الشركات الشقيقة واستخدام نفس اسم دفتر اليومية في جميع الكيانات القانونية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-120">We recommend that you use a specific journal name for intercompany accounting and to use the same journal name in all legal entities.</span></span> 


![لقطة شاشة لعلامة التبويب "عام" في صفحة أسماء دفاتر اليومية.](../media/journal-name.png)

## <a name="set-up-posting-relationships-between-the-companies"></a><span data-ttu-id="6b4e0-122">إعداد علاقات الترحيل بين الشركات</span><span class="sxs-lookup"><span data-stu-id="6b4e0-122">Set up posting relationships between the companies</span></span> 

<span data-ttu-id="6b4e0-123">عندما يتم إعداد الحسابات في مخطط الحسابات ودفاتر اليومية، يمكنك إعداد علاقات الترحيل بين الشركات.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-123">When accounts in the Chart of accounts and the journals are set up, you can set up the posting relationships between the companies.</span></span>

<span data-ttu-id="6b4e0-124">تُستخدم صفحة **المحاسبة بين الشركات الشقيقة** لإنشاء أزواج الكيانات القانونية التي يمكنها التعامل مع بعضها البعض.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-124">The **Intercompany accounting** page is used to create the legal entity pairs that can transact with each other.</span></span> <span data-ttu-id="6b4e0-125">تتم مشاركة إعداد المحاسبة بين الشركات الشقيقة، بحيث يكون الإعداد مرئياً من داخل جميع الكيانات القانونية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-125">The Intercompany accounting setup is shared, so the setup is visible from within all legal entities.</span></span> 

<span data-ttu-id="6b4e0-126">عند إنشاء زوج كيان قانوني جديد، تأكد من أنك على دراية بالكيان القانوني الذي يتم تعريفه على أنه الشركة المنشئة مقابل الشركة الوجهة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-126">When creating a new legal entity pair, ensure that you are aware of which legal entity is defined as the originating company versus the destination company.</span></span> <span data-ttu-id="6b4e0-127">عند إدخال الحركات بين الشركات الشقيقة، تحدد المعاملة الكيان القانوني الذي يقوم ببدء أو إنشاء الحركة استناداً إلى الشركة النشطة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-127">When entering intercompany transactions, the transaction determines which legal entity is initiating or originating the transaction based on the active company.</span></span> 

<span data-ttu-id="6b4e0-128">على سبيل المثال، تم إعداد المحاسبة بين الشركات الشقيقة لـ USMF (الأصلية) وAdventure Works Cycles (الوجهة).</span><span class="sxs-lookup"><span data-stu-id="6b4e0-128">For example, the intercompany accounting is set up for USMF (originating) and Adventure Works Cycles (destination).</span></span> <span data-ttu-id="6b4e0-129">إذا كان المستخدم نشطاً في Adventure Works Cycles ودخل حركة بين الشركات الشقيقة مع USMF، فلن يتم ترحيل الحركة لأن المحاسبة بين الشركات الشقيقة محددة فقط لأن USMF هو المنشئ.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-129">If a user is active in Adventure Works Cycles and enters an intercompany transaction with USMF, the transaction will not post because the intercompany accounting is only defined for USMF being the originator.</span></span> <span data-ttu-id="6b4e0-130">إذا كان بإمكان أي من الشركتين إنشاء حركة، فستحتاج إلى إنشاء زوج كيان قانوني ثانٍ للإعداد المتبادل.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-130">If either company can originate a transaction, you will need to create a second legal entity pair for the reciprocal setup.</span></span>

<span data-ttu-id="6b4e0-131">حدد **حساب الخصم (مستحق إلى)** و **حساب الائتمان (مستحق من)** لكل من الكيان القانوني المنشأ والوجهة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-131">Select the **Debit account (Due to)** and **Credit account (Due from)** for both the originating and destination legal entity.</span></span> 

<span data-ttu-id="6b4e0-132">حدد **اسم دفتر اليومية** الذي سيتم استخدامه عند إنشاء الحركة في الشركة الوجهة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-132">Define which **Journal name** will be used when the transaction is created in the destination company.</span></span> <span data-ttu-id="6b4e0-133">إن دفتر اليومية للشركة المنشأ معروف بالفعل لأنه يتم تحديده من قبل المستخدم عند إنشاء الحركة بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-133">The journal for the originating company is already known because it's selected by the user when creating the intercompany transaction.</span></span>

<span data-ttu-id="6b4e0-134">وأخيراً، حدد الكيان القانوني الذي سيتلقى المحاسبة عن المبالغ الداعمة، مثل الخصم النقدي أو المكاسب/الخسائر المحققة للمدفوعات المركزية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-134">Finally, select which legal entity will receive the accounting for supporting amounts, such as cash discount or realized gains/losses for centralized payments.</span></span>

<span data-ttu-id="6b4e0-135">يمكن بسهولة إعداد علاقة متبادلة في صفحة **المحاسبة بين الشركات الشقيقة** (**دفتر الأستاذ العام > إعداد الترحيل > المحاسبة بين الشركات الشقيقة**) باستخدام الزر **إنشاء علاقة متبادلة** بعد إنشاء أول زوج من الكيانات القانونية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-135">A reciprocal relationship can easily be set up on the **Intercompany accounting** page (**General ledger > Posting setup > Intercompany accounting**) by using the **Create reciprocal relationship** button after the first legal entity pair is created.</span></span> <span data-ttu-id="6b4e0-136">عندما يتم إنشاء الزوج المتبادل، يتم نسخ معلومات الشركة الوجهة إلى الشركة المنشأ والعكس صحيح.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-136">When the reciprocal pair is created, the information for the destination company is copied to the originating company and vice versa.</span></span> 

![لقطة شاشة لصفحة المحاسبة بين الشركات الشقيقة.](../media/intercompany1.png)


<span data-ttu-id="6b4e0-138">سيبقى دفتر اليومية المحدد للشركة الوجهة.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-138">The journal defined for the destination company will remain.</span></span> <span data-ttu-id="6b4e0-139">تستخدم معظم المؤسسات نفس اصطلاح التسمية لأسماء دفاتر اليومية الخاصة بهم، لذا فإن اسم دفتر اليومية يكون نفس الشيء.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-139">Most organizations use the same naming convention for their journal names, so the journal name is the same.</span></span> <span data-ttu-id="6b4e0-140">إذا كان اسم دفتر اليومية مختلفاً، فسيظهر تحذير في الحقل لإعلامك بعدم وجود دفتر اليومية، ويمكن تحديد دفتر يومية مختلف.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-140">If the journal name is different, a warning will appear on the field to notify you that the journal doesn't exist, and a different journal can be selected.</span></span>

<span data-ttu-id="6b4e0-141">بغض النظر عن اتجاه الترحيل بين حسابات الشركات، يجب أن يكون لدى كلتا الشركتين حسابات بين الشركات الشقيقة تم إعدادها لحسابات الشركة الأخرى.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-141">Regardless of the direction of posting between company accounts, both companies must have intercompany accounts set up for the other company accounts.</span></span> <span data-ttu-id="6b4e0-142">ستؤدي أي أخطاء في الإعداد إلى حدوث أخطاء في محاكاة الترحيل والترحيل في دفاتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="6b4e0-142">Any errors in the setup will cause errors in Simulate posting and Post in the journals.</span></span>


