---
ms.openlocfilehash: 68be1f77760a6602dadf3bb36408e96e4ea28ce5
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071069"
---
<span data-ttu-id="2cc33-101">تشرح هذه الوحدة كيفية تكوين مكونات الائتمان والتحصيلات.</span><span class="sxs-lookup"><span data-stu-id="2cc33-101">This unit explains how to configure credit and collections components.</span></span>

## <a name="set-up-aging-period-definitions"></a><span data-ttu-id="2cc33-102">إعداد تعريفات فترة التأخر</span><span class="sxs-lookup"><span data-stu-id="2cc33-102">Set up aging period definitions</span></span> 
 
<span data-ttu-id="2cc33-103">يمكنك استخدام صفحة **تعريفات فترة التقادم** لتحليل استحقاق حسابات العملاء وحسابات الموردين، بناءً على التاريخ الذي تدخله.</span><span class="sxs-lookup"><span data-stu-id="2cc33-103">You can use the **Aging period definitions** page to analyze the maturity of customer accounts and vendor accounts, based on a date that you enter.</span></span> <span data-ttu-id="2cc33-104">يتم استخدام التاريخ الذي تم إدخاله، جنباً إلى جنب مع الوحدة ومعلومات الفاصل الزمني التي تدخلها في علامة التبويب **الفترات** في هذه الصفحة، لحساب الفاصل الزمني لكل **فترة تقادم** (رأس العمود) في صفحة **تعريف فترة التقادم**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-104">The date entered, together with the unit and interval information that you enter on the **Periods** tab in this page, is used to calculate a date interval for each **Aging period** (column header) in the **Aging period definition** page.</span></span>

<span data-ttu-id="2cc33-105">تتوافق كل فترة تقادم تقوم بإعدادها لتعريف فترة التقادم مع عمود في صفحة القائمة أو في الصفحة أو التقرير عند إجراء التحليل.</span><span class="sxs-lookup"><span data-stu-id="2cc33-105">Each aging period that you set up for the aging period definition corresponds to a column on the list page or in the page or report when the analysis is performed.</span></span>

<span data-ttu-id="2cc33-106">يتم عرض فترات التقادم في صفحة القائمة، أو في الصفحة أو التقرير، بالترتيب الذي قمت بتعيينها به.</span><span class="sxs-lookup"><span data-stu-id="2cc33-106">The aging periods are shown on the list page, or in the page or report, in the order in which you set them.</span></span> <span data-ttu-id="2cc33-107">تحتاج إلى استخدام تعريفات فترة التقادم لإنشاء لقطات تقادم العملاء.</span><span class="sxs-lookup"><span data-stu-id="2cc33-107">You need to use aging period definitions to create customer aging snapshots.</span></span> <span data-ttu-id="2cc33-108">تُستخدم لقطات التقادم لعرض المعلومات في صفحة **التحصيلات** وفي صفحات القائمة ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="2cc33-108">The aging snapshots are used to display information in the **Collections** page and in related list pages.</span></span>

<span data-ttu-id="2cc33-109">يحدد تعريف فترة التقادم الأعمدة التي تظهر في صفحات قوائم **الأرصدة القديمة وأنشطة التحصيلات**، و **حالات التحصيلات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-109">An aging period definition defines the columns that appear on the **Aged balances, Collections activities**, and **Collections cases** list pages.</span></span> <span data-ttu-id="2cc33-110">كما تحدد الفترات التي تظهر في صفحة التحصيلات.</span><span class="sxs-lookup"><span data-stu-id="2cc33-110">It also defines the periods that appear on the Collections page.</span></span> 

<span data-ttu-id="2cc33-111">إذا تم إعداد وعاء العملاء، فسيتم استخدام تعريف فترة التقادم للوعاء.</span><span class="sxs-lookup"><span data-stu-id="2cc33-111">If a customer pool is set up, the aging period definition for the pool is used.</span></span> 

<span data-ttu-id="2cc33-112">إذا لم يتم إعداد أوعية العملاء، فسيتم استخدام تعريف فترة التقادم الافتراضي المحدد في صفحة **معلمات حسابات المقبوضات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-112">If no customer pools are set up, the default aging period definition that is specified on the **Accounts receivable parameters** page is used.</span></span> 

<span data-ttu-id="2cc33-113">إذا لم يتم تحديد تعريف افتراضي لفترة التقادم، فسيتم استخدام تعريف فترة التقادم الأولى في صفحة **الائتمان والتحصيلات > الإعداد > تعريفات فترة التقادم**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-113">If no default aging period definition is specified, the first aging period definition on the **Credit and collections > Setup > Aging period definitions** page is used.</span></span>
 
![لقطة شاشة لصفحة تعريفات فترة التقادم.](../media/aging-period-definition.png)

## <a name="create-a-customer-aging-snapshot"></a><span data-ttu-id="2cc33-115">قم بإنشاء لقطة تأخر العميل</span><span class="sxs-lookup"><span data-stu-id="2cc33-115">Create a customer aging snapshot</span></span> 

<span data-ttu-id="2cc33-116">توفر اللقطات القديمة وصولاً سريعاً إلى معلومات التقادم لموظفي التحصيلات باستخدام صفحة **الأرصدة القديمة** في **الائتمان والتحصيلات > التحصيلات > الأصدة القديمة**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-116">Aging snapshots provide quick access to aging information for collections personnel by using the **Aged balances** list page in **Credit and collections >  Collections > Aged balances**.</span></span> <span data-ttu-id="2cc33-117">تتضمن هذه الصفحة رموزاً بجوار حقل **رصيد المبلغ المستحق** الذي يتيح للمستخدمين التعرف بسرعة على الحسابات وحالة تقادمها.</span><span class="sxs-lookup"><span data-stu-id="2cc33-117">This page includes icons next to the **Amount due balance** field that enable users to quickly identify accounts and their aging status.</span></span>

<span data-ttu-id="2cc33-118">[![لقطة شاشة لصفحة الأرصدة القديمة تعرض الرموز بجوار حقل رصيد المبلغ المستحق.](../media/aged-balances.png)](../media/aged-balances.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="2cc33-118">[![Screenshot of the Aged balances page showing icons next to the Amount due balance field.](../media/aged-balances.png)](../media/aged-balances.png#lightbox)</span></span>


<span data-ttu-id="2cc33-119">يجب إنشاء لقطة تقادم قبل أن تتمكن من عرض المعلومات في صفحة **الائتمان والتحصيلات > التحصيلات > الارصدة القديمة**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-119">An aging snapshot must be created before you can view information on the **Credit and collections > Collections > Aged balances** page.</span></span>

<span data-ttu-id="2cc33-120">انتقل إلى **الائتمان والتحصيلات > المهام الدورية > أرصدة العملاء القديمة** لتحديث لقطة تقادم العميل.</span><span class="sxs-lookup"><span data-stu-id="2cc33-120">Go to **Credit and collections > Periodic tasks > Age customer balances** to update the customer aging snapshot.</span></span>
 
![لقطة شاشة لإنشاء لقطة تقادم العميل.](../media/aging-snapshot.png)

<span data-ttu-id="2cc33-122">لكل عميل، تحتوي لقطة التقادم على العناصر التالية.</span><span class="sxs-lookup"><span data-stu-id="2cc33-122">For each customer, an aging snapshot contains the following elements.</span></span>

- <span data-ttu-id="2cc33-123">رأس لقطة تقادم</span><span class="sxs-lookup"><span data-stu-id="2cc33-123">An aging snapshot header</span></span>
- <span data-ttu-id="2cc33-124">واحد أو أكثر من رؤوس لقطات تقادم الشركات</span><span class="sxs-lookup"><span data-stu-id="2cc33-124">One or more company aging snapshot headers</span></span>
- <span data-ttu-id="2cc33-125">سجلات تفصيلية لكل فترة تقادم في تعريف فترة التقادم</span><span class="sxs-lookup"><span data-stu-id="2cc33-125">Detail records for each aging period in the aging period definition</span></span>

<span data-ttu-id="2cc33-126">أنشئ سجلات لقطات تقادم لجميع العملاء أو للعملاء في وعاء العملاء.</span><span class="sxs-lookup"><span data-stu-id="2cc33-126">Create aging snapshot records for all customers or for the customers in a customer pool.</span></span>
 
## <a name="optional---set-up-customer-pools"></a><span data-ttu-id="2cc33-127">اختياري - إعداد أوعية العملاء</span><span class="sxs-lookup"><span data-stu-id="2cc33-127">Optional - Set up customer pools</span></span> 

<span data-ttu-id="2cc33-128">يمكنك إعداد أوعية العملاء لتمثيل مجموعات العملاء.</span><span class="sxs-lookup"><span data-stu-id="2cc33-128">You can set up customer pools to represent groups of customers.</span></span> 

<span data-ttu-id="2cc33-129">يمكنك استخدام مجموعات العملاء كعوامل تصفية لمعلومات العميل التي تظهر في صفحة **الائتمان والتحصيلات > التحصيلات > إعداد > أوعية العملاء** أو عند إنشاء لقطات التقادم.</span><span class="sxs-lookup"><span data-stu-id="2cc33-129">You can use customer pools as filters for the customer information that appears on **Credit and collections > Collections > Setup > Customer pools** page, or when you create aging snapshots.</span></span>
  
![لقطة شاشة لصفحة أوعية العملاء تعرض علامة التبويب السريعة معايير أوعية العملاء.](../media/customer-pools.png)

<span data-ttu-id="2cc33-131">فيما يلي أمثلة يمكن استخدامها لأوعية العملاء.</span><span class="sxs-lookup"><span data-stu-id="2cc33-131">The following are examples that might be used for customer pools.</span></span>

- <span data-ttu-id="2cc33-132">العملاء الذين لديهم أرصدة تزيد على مبلغ محدد</span><span class="sxs-lookup"><span data-stu-id="2cc33-132">Customers who have balances over a specified amount</span></span>
- <span data-ttu-id="2cc33-133">العملاء في دول أو مناطق أو ضواحي محددة</span><span class="sxs-lookup"><span data-stu-id="2cc33-133">Customers in specific countries, regions, or districts</span></span>
- <span data-ttu-id="2cc33-134">أنواع العملاء</span><span class="sxs-lookup"><span data-stu-id="2cc33-134">Types of customers</span></span>
- <span data-ttu-id="2cc33-135">العملاء مجمعين حسب الحجم أو الكم أو تكرار الأوامر</span><span class="sxs-lookup"><span data-stu-id="2cc33-135">Customers grouped by size, volume, or frequency of ordering</span></span>
 
## <a name="optional----create-a-collection-agent"></a><span data-ttu-id="2cc33-136">اختياري - إنشاء وكيل تحصيل</span><span class="sxs-lookup"><span data-stu-id="2cc33-136">Optional -  Create a collection agent</span></span> 

<span data-ttu-id="2cc33-137">إذا قام العديد من الأشخاص في مؤسستك بعمل التحصيلات، فيمكنك إعداد فريق التحصيلات.</span><span class="sxs-lookup"><span data-stu-id="2cc33-137">If multiple people in your organization do collections work, you can set up a collections team.</span></span> <span data-ttu-id="2cc33-138">يمكنك تحديد الفريق في صفحة **معلمات حسابات المقبوضات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-138">You can select the team on the **Accounts receivable parameters** page.</span></span> 
 
![لقطة شاشة لصفحة معلمات حسابات المقبوضات.](../media/ar-parameters.png)

<span data-ttu-id="2cc33-140">قبل أن يتمكن العمال من إنشاء أنشطة أو إرسال رسائل بريد إلكتروني باستخدام صفحة **التحصيلات**، تحتاج إلى التحقق من تحيدد مفتاح تكوين **مزامنة Microsoft Outlook**، وأن مزامنة Outlook معدة لهؤلاء العمال.</span><span class="sxs-lookup"><span data-stu-id="2cc33-140">Before workers can create activities or send email messages by using the **Collections** page, you need to verify that the **Microsoft Outlook synchronization** configuration key is selected, and that Outlook synchronization is set up for those workers.</span></span>

<span data-ttu-id="2cc33-141">إذا لم تقم بإنشاء فريق تحصيل، فسيتم إنشاء فريق تلقائياً عندما تقوم بإعداد وكلاء التحصيل في صفحة **الائتمان والتحصيلات > الإعداد > وكلاء التحصيل**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-141">If you don't create a collections team, a team is created automatically when you set up collection agents on the **Credit and collections > Setup > Collection agents** page.</span></span>
  
![لقطة شاشة لصفحة وكلاء التحصيل.](../media/collection-agents.png)

<span data-ttu-id="2cc33-143">استخدم صفحة **وكلاء التحصيل** لإعداد الموظفين والمقاولين كوكلاء تحصيل وتعيين أوعية العملاء لهم اختيارياً.</span><span class="sxs-lookup"><span data-stu-id="2cc33-143">Use the **Collection agents** page to set up employees and contractors as collections agents and optionally assign customer pools to them.</span></span> <span data-ttu-id="2cc33-144">وكيل التحصيل هو الشخص الذي يعمل مع العملاء للتأكد من تحصيل المدفوعات في الوقت المناسب.</span><span class="sxs-lookup"><span data-stu-id="2cc33-144">A collection agent is a person who works with customers to make sure that payments are collected in a timely manner.</span></span>

<span data-ttu-id="2cc33-145">إذا قام العديد من الأشخاص في مؤسستك بعمل المجموعات، فيمكنك إعداد وكلاء التحصيل، الذين تم إعدادهم كمستخدمين في صفحة **علاقات المستخدمين**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-145">If multiple people in your organization do collections work, you can set up collection agents, who are set up as users on the **User relations** page.</span></span> 

<span data-ttu-id="2cc33-146">يمكنك تعيين أوعية العملاء (استعلامات العملاء) لوكلاء التحصيل لمساعدة الوكلاء في تنظيم عملهم.</span><span class="sxs-lookup"><span data-stu-id="2cc33-146">You can assign customer pools (customer queries) to collection agents to help the agents organize their work.</span></span> <span data-ttu-id="2cc33-147">تتم إضافة وكلاء التحصيل إلى الفريق الذي تم تحديده في صفحة **معلمات حسابات المقبوضات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-147">The collection agents are added to the team that is selected on the **Accounts receivable parameters** page.</span></span> <span data-ttu-id="2cc33-148">إذا لم يتم تحديد فريق في تلك الصفحة، فسيتم إنشاء فريق جديد يسمى التحصيلات تلقائياً، وتتم إضافة وكلاء التحصيل إلى هذا الفريق.</span><span class="sxs-lookup"><span data-stu-id="2cc33-148">If a team isn't selected on that page, a new team that is named Collections is automatically created, and the collection agents are added to that team.</span></span>

## <a name="set-up-a-collections-case-category"></a><span data-ttu-id="2cc33-149">إعداد فئة حالة التحصيلات</span><span class="sxs-lookup"><span data-stu-id="2cc33-149">Set up a collections case category</span></span> 

<span data-ttu-id="2cc33-150">إذا كنت تخطط لاستخدام الحالات لتنظيم عمل التحصيلات، فقم بإعداد فئة حالة لها نوع فئة التحصيلات.</span><span class="sxs-lookup"><span data-stu-id="2cc33-150">If you plan to use cases to organize your collections work, set up a case category that has the Collections category type.</span></span> <span data-ttu-id="2cc33-151">انتقل إلى **إدارة المؤسسة > الإعداد > الحالات > فئات الحالات** لإنشاء فئة حالة تحصيل.</span><span class="sxs-lookup"><span data-stu-id="2cc33-151">Go to **Organization administration > Setup > Cases > Case categories** to create a collection case category.</span></span>
  
<span data-ttu-id="2cc33-152">[![رسم متحرك يوضح كيفية التنقل إلى صفحة فئات الحالات.](../media/case-category.gif)](../media/case-category.gif#lightbox)</span><span class="sxs-lookup"><span data-stu-id="2cc33-152">[![Animation showing how to navigate to the Case categories page.](../media/case-category.gif)](../media/case-category.gif#lightbox)</span></span>

<span data-ttu-id="2cc33-153">هذا الإعداد مطلوب فقط إذا كنت تريد استخدام وظيفة الحالة في صفحة **الائتمان والتحصيلات > التحصيلات > حالات التحصيلات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-153">This setup is required only if you want to use the case functionality on the **Credit and collections > Collections > Collections cases** page.</span></span>

## <a name="set-up-email-and-address-settings-for-collections-customer-contacts"></a><span data-ttu-id="2cc33-154">إعداد إعدادات البريد الإلكتروني والعنوان لجهات اتصال عملاء التحصيلات</span><span class="sxs-lookup"><span data-stu-id="2cc33-154">Set up email and address settings for collections customer contacts</span></span> 

<span data-ttu-id="2cc33-155">قم بإعداد عناوين البريد الإلكتروني لجهات اتصال العملاء إذا كنت تريد إرسال رسائل بريد إلكتروني إلى جهات الاتصال هذه من صفحة **التحصيلات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-155">Set up email addresses for customer contacts if you want to send email messages to those contacts from the **Collections** page.</span></span> <span data-ttu-id="2cc33-156">يتم استخدام جهة اتصال التحصيلات كجهة اتصال افتراضية في صفحة **التحصيلات**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-156">The collections contact is used as the default contact on the **Collections** page.</span></span> <span data-ttu-id="2cc33-157">يمكنك إعداد عنوان كشف حساب للعميل إذا كان يجب على البيانات استخدام عنوان آخر غير العنوان الأساسي.</span><span class="sxs-lookup"><span data-stu-id="2cc33-157">You can set up a statement address for a customer if statements should use an address other than the primary address.</span></span>

<span data-ttu-id="2cc33-158">في علامة التبويب السريعة **الائتمان والتحصيلات** لأحد العملاء، في حقل **جهة اتصال التحصيلات**، حدد الشخص في مؤسسة العميل الذي يعمل مع وكيل التحصيل الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="2cc33-158">On the **Credit and Collections** FastTab for a customer, in the **Collections contact** field, select the person in the customer organization who works with your collection agent.</span></span> <span data-ttu-id="2cc33-159">يتم استخدام هذا الشخص كجهة اتصال افتراضية في صفحة **التحصيلات**، ويتم إرسال رسائل البريد الإلكتروني إليه.</span><span class="sxs-lookup"><span data-stu-id="2cc33-159">This person is used as the default contact on the **Collections** page, and email messages are sent to him or her.</span></span>

<span data-ttu-id="2cc33-160">إذا لم يتم تحديد جهة اتصال تحصيلات للعميل، فسيتم استخدام جهة الاتصال الأساسية للعميل.</span><span class="sxs-lookup"><span data-stu-id="2cc33-160">If a collections contact isn't specified for a customer, the primary contact for the customer is used.</span></span> <span data-ttu-id="2cc33-161">إذا لم يتم تحديد جهة اتصال أساسية، فسيتم إرسال رسائل البريد الإلكتروني إلى العنوان الأول المدرج في صفحة **جهات الاتصال**.</span><span class="sxs-lookup"><span data-stu-id="2cc33-161">If a primary contact isn't specified, email messages are sent to the first address that is listed on the **Contacts** page.</span></span>


