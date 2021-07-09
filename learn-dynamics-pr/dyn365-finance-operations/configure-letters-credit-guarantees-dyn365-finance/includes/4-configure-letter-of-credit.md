---
ms.openlocfilehash: bbfc089880665dd3b6cc28ee194ed81e15132bed
ms.sourcegitcommit: 8e47fcb8fe1e706270b2967466a811bf85766c83
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "6071092"
---
<span data-ttu-id="9bf02-101">قبل استيراد خطابات الاعتماد، يجب إكمال إعداد التسهيلات البنكية وملفات تعريف الترحيل واتفاقية تسهيلات بنكية وتفاصيل بنكية للمورّد.</span><span class="sxs-lookup"><span data-stu-id="9bf02-101">Before importing the letters of credit, you must complete the setup for bank facilities, posting profiles, a bank facility agreement, and vendor bank details.</span></span>

<span data-ttu-id="9bf02-102">لا يمكن أن تحتوي اتفاقيات التسهيلات على تواريخ متداخلة.</span><span class="sxs-lookup"><span data-stu-id="9bf02-102">Facility agreements cannot have overlapping dates.</span></span> 

<span data-ttu-id="9bf02-103">فعلى سبيل المثال، إذا كانت إحدى الاتفاقيات تمتد من 01 يناير 2019 إلى 31 أغسطس 2019، فلا يمكنك إبرام اتفاقية تسهيل أخرى في بداية أو نهاية تلك الفترة.</span><span class="sxs-lookup"><span data-stu-id="9bf02-103">For example, if an agreement extends from January 01, 2019 to August 31, 2019, you cannot create another facility agreement that begins or ends within that period.</span></span>

<span data-ttu-id="9bf02-104">تعرض الصورة التالية مجموعات التسهيلات في صفحة **التسهيلات البنكية** في **إدارة النقد والبنوك > إعداد**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-104">The following image shows the facility groups on the **Bank facilities** page in **Cash and bank management > Setup**.</span></span>
 

![لقطة شاشة لمجموعات التسهيلات في صفحة التسهيلات البنكية.](../media/bank-facilities.png)

## <a name="activate-the-letter-of-credit-as-a-bank-document"></a><span data-ttu-id="9bf02-106">تنشيط خطاب الاعتماد كمستند بنكي</span><span class="sxs-lookup"><span data-stu-id="9bf02-106">Activate the letter of credit as a bank document</span></span> 

<span data-ttu-id="9bf02-107">تنشيط خطاب الاعتماد كمستند بنكي قبل البدء في الحركات التي تنطوي على خطابات اعتماد.</span><span class="sxs-lookup"><span data-stu-id="9bf02-107">Activate the letter of credit as a bank document before you initiate transactions that involve letters of credit.</span></span>

1.  <span data-ttu-id="9bf02-108">انتقل إلى **‏‫إدارة النقد والبنوك‬ > الإعداد > معلمات إدارة البنك والنقد**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-108">Go to **Cash and Bank Management > Setup > Cash and Bank Management parameters**.</span></span>
2.  <span data-ttu-id="9bf02-109">قم بتوسيع علامة التبويب السريعة **المستند البنكي**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-109">Expand the **Bank document** FastTab.</span></span>
3.  <span data-ttu-id="9bf02-110">قمّ بتعيين خيار **تمكين استيراد خطاب الاعتماد** إلى **نعم** لتنشيط خطاب الاعتماد.</span><span class="sxs-lookup"><span data-stu-id="9bf02-110">Set the **Enable import letter of credit** option to **Yes** to activate the letter of credit.</span></span>
4.  <span data-ttu-id="9bf02-111">أغلق الصفحة لحفظ التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="9bf02-111">Close the page to save your changes.</span></span>

<span data-ttu-id="9bf02-112">عند تعيين حقل **نوع المستند البنكي** باعتباره **خطاب اعتماد**، فسيتم عرض أمر الشراء في قائمة خطابات الاعتماد في الوحدة النمطية لإدارة النقد والبنوك.</span><span class="sxs-lookup"><span data-stu-id="9bf02-112">When the **Bank document type** field is set as **Letter of credit**, the purchase order is displayed in the list of letters of credit in the Cash and bank management module.</span></span> 

<span data-ttu-id="9bf02-113">**إدارة النقد والبنوك > إعداد > محددات إدارة النقد والبنوك**
![لقطة شاشة لصفحة محددات إدارة النقد والبنوك.](../media/enable-letter-of-credit.png)</span><span class="sxs-lookup"><span data-stu-id="9bf02-113">**Cash and bank management > Setup > Cash and bank management parameters**
![Screenshot of the Cash and bank management parameters page.](../media/enable-letter-of-credit.png)</span></span> 



## <a name="set-up-the-bank-facilities-and-posting-profiles"></a><span data-ttu-id="9bf02-114">إعداد التسهيلات البنكية وملفات تعريف الترحيل</span><span class="sxs-lookup"><span data-stu-id="9bf02-114">Set up the bank facilities and posting profiles</span></span> 

<span data-ttu-id="9bf02-115">يمكنك إعداد أنواع التسهيلات البنكية ومجموعات التسهيلات البنكية في صفحة **التسهيلات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-115">You can set up bank facility types and bank facility groups on the **Bank facilities** page.</span></span> <span data-ttu-id="9bf02-116">بعد إعداد ملف تعريف الترحيل البنكي، يمكنك إبرام اتفاقيات تسهيلات.</span><span class="sxs-lookup"><span data-stu-id="9bf02-116">After the bank posting profile is set up, you can create facility agreements.</span></span>

1.  <span data-ttu-id="9bf02-117">حدد **‏إدارة النقد والبنوك > إعداد > التسهيلات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-117">Select **Cash and bank management > Setup > Bank facilities**.</span></span>
2.  <span data-ttu-id="9bf02-118">في الارتباط **مجموعات التسهيلات**، حدد **جديد** لإنشاء مجموعة تسهيلات بنكية جديدة.</span><span class="sxs-lookup"><span data-stu-id="9bf02-118">On the **Facility groups** link, select **New** to create a new bank facility group.</span></span>
3.  <span data-ttu-id="9bf02-119">في حقلي **مجموعة التسهيلات** و **الوصف**، أدخل اسم مجموعة التسهيلات البنكية ووصفها.</span><span class="sxs-lookup"><span data-stu-id="9bf02-119">In the **Facility group** and **Description** fields, enter the bank facility group name and description.</span></span>
4.  <span data-ttu-id="9bf02-120">حدد الارتباط **أنواع التسهيلات**، ثم حدد **جديد** لإنشاء نوع تسهيل جديد.</span><span class="sxs-lookup"><span data-stu-id="9bf02-120">Select the **Facility types** link, and then select **New** to create a new facility type.</span></span>
5.  <span data-ttu-id="9bf02-121">أدخل كوداً فريداً في حقل **نوع التسهيلات**، ثمّ في حقلي **مجموعة التسهيلات** و **طبيعة التسهيلات**، حدد مجموعة التسهيلات البنكية وطبيعتها.</span><span class="sxs-lookup"><span data-stu-id="9bf02-121">Enter a unique code in the **Facility type** field, and then in the **Facility group** and **Facility nature** fields, select the group and nature of the bank facility.</span></span>
6.  <span data-ttu-id="9bf02-122">أغلق الصفحة لحفظ التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="9bf02-122">Close the page to save your changes.</span></span>
7.  <span data-ttu-id="9bf02-123">حدد **‏إدارة النقد والبنوك > إعداد > المستندات البنكية > ملف تعريف ترحيل المستندات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-123">Select **Cash and bank management > Setup > Bank documents > Bank documents posting profile**.</span></span>
8.  <span data-ttu-id="9bf02-124">في الحقل **تسوية الحساب** حدد الحساب الرئيسي لإجراء التسوية.</span><span class="sxs-lookup"><span data-stu-id="9bf02-124">In the **Settle account** field, select the main account for settlement.</span></span> <span data-ttu-id="9bf02-125">يُستخدم هذا الحساب عند حساب تقدير التدفقات النقدية.</span><span class="sxs-lookup"><span data-stu-id="9bf02-125">This account is used when you are calculating the cash flow forecast.</span></span>
9.  <span data-ttu-id="9bf02-126">في الحقل **حساب التكاليف** حدد الحساب الخاص بحركات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="9bf02-126">In the **Charges account** field, select the account for expense transactions.</span></span>
10. <span data-ttu-id="9bf02-127">في الحقل **حساب الهامش** حدد الحساب الخاص بحركة الهامش.</span><span class="sxs-lookup"><span data-stu-id="9bf02-127">In the **Margin account** field, select the account for the margin transaction.</span></span> <span data-ttu-id="9bf02-128">يتم خصم هذا الحساب عند ترحيل الهامش الافتتاحي وقيده عند ترحيل الدفع.</span><span class="sxs-lookup"><span data-stu-id="9bf02-128">This account is debited when the opening margin is posted and credited when the payment is posted.</span></span> <span data-ttu-id="9bf02-129">يعتبر الهامش دفعة مقدمة للبنك الذي تم تسويتها بواسطة البنك عند إجراء المشتري للتسوية النهائية.</span><span class="sxs-lookup"><span data-stu-id="9bf02-129">A margin is an advance payment to the bank that is adjusted by the bank when the final settlement is made by the buyer.</span></span>  
11. <span data-ttu-id="9bf02-130">أغلق الصفحة لحفظ التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="9bf02-130">Close the page to save your changes.</span></span>

 <span data-ttu-id="9bf02-131">**‏إدارة النقد والبنوك > إعداد > التسهيلات البنكية > أنواع التسهيلات**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-131">**Cash and bank management > Setup > Bank facilities > Facility types**</span></span> 

![لقطة شاشة لأنواع التسهيلات في صفحة التسهيلات البنكية.](../media/facility-types.png)  



## <a name="create-a-bank-facility-agreement"></a><span data-ttu-id="9bf02-133">إنشاء إتفاقية تسهيل بنكي</span><span class="sxs-lookup"><span data-stu-id="9bf02-133">Create a bank facility agreement</span></span> 

<span data-ttu-id="9bf02-134">يمكنك إبرام اتفاقيات تسهيلات بنكية تسجل التسهيلات المختلفة التي يقدمها البنك.</span><span class="sxs-lookup"><span data-stu-id="9bf02-134">You can create bank facility agreements that record various facilities that are provided by the bank.</span></span> <span data-ttu-id="9bf02-135">يمكن استخدام المستندات البنكية في الحركات فقط بعد إنشاء اتفاقيات التسهيلات.</span><span class="sxs-lookup"><span data-stu-id="9bf02-135">Bank documents can be used in transactions only after facility agreements are created.</span></span> <span data-ttu-id="9bf02-136">يعين البنك حداً لخطاب الاعتماد، والذي تتم إعادة حسابه في كل مره يتم فيها تسجيل حركة خطاب الاعتماد.</span><span class="sxs-lookup"><span data-stu-id="9bf02-136">The bank assigns a limit for the letter of credit, which is recalculated every time a letter of credit transaction is recorded.</span></span>

<span data-ttu-id="9bf02-137">عندما تنتهي اتفاقية التسهيلات، يمكنك إنشاء إصدار جديد من الاتفاقية بتواريخ بداية ونهاية جديدة، بتمديد مدة الاتفاقية القديمة.</span><span class="sxs-lookup"><span data-stu-id="9bf02-137">When a facility agreement ends, you can create a new version of the agreement, with new starting and ending dates, by extending the old agreement.</span></span>

1.  <span data-ttu-id="9bf02-138">انتقل إلى **‏‫إدارة النقد والبنوك > خطابات الاعتماد > اتفاقيات التسهيلات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-138">Go to **Cash and bank management > Letters of credit > Bank facility agreements**.</span></span>
2.  <span data-ttu-id="9bf02-139">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-139">Select **New**.</span></span>
3.  <span data-ttu-id="9bf02-140">في حقل **رقم الاتفاقية**، أدخل رقم الاتفاقية وفقاً للاتفاقية مع البنك.</span><span class="sxs-lookup"><span data-stu-id="9bf02-140">In the **Agreement number** field, enter the agreement number according to the agreement with the bank.</span></span>
4.  <span data-ttu-id="9bf02-141">في حقل **الحساب البنكي**، أدخل رقم الحساب في بنك الإصدار.</span><span class="sxs-lookup"><span data-stu-id="9bf02-141">In the **Bank account** field, enter the account number at the issuing bank.</span></span>
5.  <span data-ttu-id="9bf02-142">في الحقل **تاريخ البدء** أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="9bf02-142">In the **Start date** field, enter a date and time.</span></span>
6.  <span data-ttu-id="9bf02-143">في الحقل **تاريخ الإنهاء** أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="9bf02-143">In the **End date** field, enter a date and time.</span></span>
7.  <span data-ttu-id="9bf02-144">قُم بتوسيع قسم **‎‏‫عام** أو طيه.</span><span class="sxs-lookup"><span data-stu-id="9bf02-144">Expand or collapse the **General** section.</span></span>
8.  <span data-ttu-id="9bf02-145">حدد **إضافة سطر**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-145">Select **Add line**.</span></span>
9.  <span data-ttu-id="9bf02-146">في الحقل **نوع التسهيلات** حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="9bf02-146">In the **Facility type** field, select the drop-down button to open the lookup.</span></span>
10. <span data-ttu-id="9bf02-147">في القائمة، قم بالبحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="9bf02-147">In the list, find and select the desired record.</span></span> <span data-ttu-id="9bf02-148">يعرض حقل **المبلغ المستخدم** المبلغ المستخدم حالياً لخطاب الاعتماد.</span><span class="sxs-lookup"><span data-stu-id="9bf02-148">The **Amount used** field displays the amount that is currently used for the letter of credit.</span></span>
11. <span data-ttu-id="9bf02-149">في حقل **الحد**، أدخل مبلغ التسهيل الذي تم التفاوض عليه مع البنك.</span><span class="sxs-lookup"><span data-stu-id="9bf02-149">In the **Limit** field, enter the facility amount that was negotiated with the bank.</span></span>
12. <span data-ttu-id="9bf02-150">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-150">Select **Save**.</span></span>
13. <span data-ttu-id="9bf02-151">في صفحة **اتفاقيات التسهيلات البنكية**، حدد اتفاقية التسهيلات التي لم تعد نشطة.</span><span class="sxs-lookup"><span data-stu-id="9bf02-151">In the **Bank facility agreements** page, select the facility agreement that is no longer active.</span></span>
14. <span data-ttu-id="9bf02-152">حدد **توسيع** لفتح مربع الحوار المنسدل.</span><span class="sxs-lookup"><span data-stu-id="9bf02-152">Select **Extend** to open the drop-down dialog box.</span></span>
 
    
<span data-ttu-id="9bf02-153">**‏إدارة النقد والبنوك > خطابات الاعتماد > اتفاقيات التسهيلات البنكية > تمديد**</span><span class="sxs-lookup"><span data-stu-id="9bf02-153">**Cash and bank management > Letters of credit > Bank facility agreements > Extend**</span></span>

![لقطة شاشة لتوسيع مربع الحوار المنسدل للاتفاقيات البنكية.](../media/extend-1.png) 

15. <span data-ttu-id="9bf02-155">في الحقل **رقم الاتفاقية الجديد** اكتب قيمةً.</span><span class="sxs-lookup"><span data-stu-id="9bf02-155">In the **New agreement number** field, type a value.</span></span>
16. <span data-ttu-id="9bf02-156">في الحقل **تاريخ الإنهاء** أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="9bf02-156">In the **End date** field, enter a date and time.</span></span>
17. <span data-ttu-id="9bf02-157">حدد **تمديد**.</span><span class="sxs-lookup"><span data-stu-id="9bf02-157">Select **Extend**.</span></span>
18. <span data-ttu-id="9bf02-158">القيمة الموجودة في حقل **تاريخ البدء** للاتفاقية الممتدة هي اليوم الذي يلي تاريخ انتهاء الاتفاقية المحددة.</span><span class="sxs-lookup"><span data-stu-id="9bf02-158">The value in the **Start date** field of the extended agreement is the day after the selected agreement’s end date.</span></span> 
19. <span data-ttu-id="9bf02-159">يُعين حقل **المبلغ المستخدم** إلى صفر لأن هذه الاتفاقية تم إبرامها حديثاً.</span><span class="sxs-lookup"><span data-stu-id="9bf02-159">The **Amount used** field is set to zero because this is a newly created agreement.</span></span>
20. <span data-ttu-id="9bf02-160">أغلق الصفحة لحفظ التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="9bf02-160">Close the page to save your changes.</span></span>

![لقطة شاشة لصفحة اتفاقيات التسهيلات البنكية.](../media/bank-facility-agreements.png)

## <a name="set-up-vendor-bank-accounts"></a><span data-ttu-id="9bf02-162">إعداد الحسابات البنكية للموردين</span><span class="sxs-lookup"><span data-stu-id="9bf02-162">Set up vendor bank accounts</span></span> 

<span data-ttu-id="9bf02-163">يجب تحديد الحسابات البنكية للموردين حتى يتم تسجيل حركات خطاب الاعتماد بشكل ملائم.</span><span class="sxs-lookup"><span data-stu-id="9bf02-163">Vendor bank accounts must be specified for vendors to have the letter of credit transactions recorded appropriately.</span></span>

<span data-ttu-id="9bf02-164">لمعرفة كيفية إعداد حسابات المورّدين، انتقل إلى [تكوين الحسابات الدائنة‏‎ في Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/configure-accounts-payable-in-dynamics-365-finance-ops//?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="9bf02-164">To learn how to set up vendor accounts, go to [Configure Accounts payable in Dynamics 365 Finance ](https://docs.microsoft.com/learn/modules/configure-accounts-payable-in-dynamics-365-finance-ops//?azure-portal=true).</span></span> 
