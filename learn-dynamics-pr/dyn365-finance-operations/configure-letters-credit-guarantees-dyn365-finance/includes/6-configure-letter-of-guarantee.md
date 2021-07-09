---
ms.openlocfilehash: a24819c8289c9d02f2e920948dcb538d55867f35
ms.sourcegitcommit: 8e47fcb8fe1e706270b2967466a811bf85766c83
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "6071089"
---
<span data-ttu-id="ea674-101">يجب تنشيط خطاب الضمان كمستند بنكي قبل التمكن من البدء في الحركات التي تشتمل على خطابات اعتماد.</span><span class="sxs-lookup"><span data-stu-id="ea674-101">You must activate the letter of guarantee as a bank document before you can initiate transactions that involve letters of credit.</span></span>

1.  <span data-ttu-id="ea674-102">انتقل إلى **‏‫إدارة النقد والبنوك‬ > الإعداد > معلمات إدارة البنك والنقد**.</span><span class="sxs-lookup"><span data-stu-id="ea674-102">Go to **Cash and Bank Management > Setup > Cash and Bank Management parameters**.</span></span>
2.  <span data-ttu-id="ea674-103">قم بتوسيع علامة التبويب السريعة **المستند البنكي**.</span><span class="sxs-lookup"><span data-stu-id="ea674-103">Expand the **Bank document** FastTab.</span></span>
3.  <span data-ttu-id="ea674-104">قم بتعيين خيار **تمكين خطاب الضمان** إلى **نعم** لتنشيط خطاب الضمان.</span><span class="sxs-lookup"><span data-stu-id="ea674-104">Set the **Enable letter of guarantee** option to **Yes** to activate the letter of guarantee.</span></span>
4.  <span data-ttu-id="ea674-105">في الحقل **دفتر يومية الحركات** حدد الزر المنسدل لتحديد اسم دفتر يومية الحركة.</span><span class="sxs-lookup"><span data-stu-id="ea674-105">In the **Transaction journal** field, select the drop-down button to select the transaction journal name.</span></span>
5.  <span data-ttu-id="ea674-106">حدد علامة التبويب **التسلسلات الرقمية** ثم قم بتحديد كود تسلسل رقمي من أجل **رقم خطاب الضمان** ومراجع **حركة خطاب الضمان**.</span><span class="sxs-lookup"><span data-stu-id="ea674-106">Select the **Number sequences** tab, define a number sequence code for **Letter of guarantee number** and **Letter of guarantee transaction** references.</span></span>
6.  <span data-ttu-id="ea674-107">أغلق الصفحة لحفظ التغييرات التي أجريتها.</span><span class="sxs-lookup"><span data-stu-id="ea674-107">Close the page to save your changes.</span></span>


<span data-ttu-id="ea674-108">عند تعيين الحقل **نوع المستند البنكي** باعتباره **خطاب ضمان**، فسيتم عرض أمر المبيعات في قائمة خطابات الضمان في الوحدة النمطية لإدارة البنك والنقد.</span><span class="sxs-lookup"><span data-stu-id="ea674-108">When the **Bank document type** field is set as **Letter of guarantee**, the sales order is displayed in the list of letters of guarantee in the Cash and bank management module.</span></span> 

![لقطة شاشة لصفحة خطاب الضمان.](../media/letter-of-guarantee.png)

## <a name="set-up-bank-facilities-and-posting-profiles-for-letters-of-guarantee"></a><span data-ttu-id="ea674-110">إعداد ملفات تعريف الترحيل والتسهيلات البنكية لخطابات الضمان</span><span class="sxs-lookup"><span data-stu-id="ea674-110">Set up bank facilities and posting profiles for letters of guarantee</span></span> 

<span data-ttu-id="ea674-111">يتعين عليك إنشاء **تسهيل بنكي** و **ملف تعريف الترحيل** اللازم لمعالجة خطاب ضمان.</span><span class="sxs-lookup"><span data-stu-id="ea674-111">You need to create a **Bank facility** and **posting profile** that is necessary for processing a letter of guarantee.</span></span>

## <a name="create-a-bank-facility"></a><span data-ttu-id="ea674-112">إنشاء تسهيل بنكي</span><span class="sxs-lookup"><span data-stu-id="ea674-112">Create a bank facility</span></span> 

1.  <span data-ttu-id="ea674-113">انتقل إلى **‏‫إدارة النقد والبنوك‬ > إعداد > التسهيلات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="ea674-113">Go to **Cash and bank management > Setup > Bank facilities**.</span></span>
2.  <span data-ttu-id="ea674-114">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="ea674-114">Select **New**.</span></span>
3.  <span data-ttu-id="ea674-115">في الحقل **مجموعة التسهيلات** أدخل اسم مجموعة التسهيلات البنكية لحركة خطاب الضمان.</span><span class="sxs-lookup"><span data-stu-id="ea674-115">In the **Facility group** field, enter the bank facility group name for the letter of guarantee transaction.</span></span>
4.  <span data-ttu-id="ea674-116">في حقل **الوصف** أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="ea674-116">In the **Description** field, type a value.</span></span>
5.  <span data-ttu-id="ea674-117">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea674-117">Select **Save**.</span></span>
6.  <span data-ttu-id="ea674-118">حدد علامة التبويب **أنواع التسهيلات**.</span><span class="sxs-lookup"><span data-stu-id="ea674-118">Select the **Facility types** tab.</span></span>
7.  <span data-ttu-id="ea674-119">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="ea674-119">Select **New**.</span></span>
8.  <span data-ttu-id="ea674-120">في الحقل **نوع التسهيلات** أدخل اسم نوع التسهيلات البنكية المرتبطة بإتفاقية التسهيلات البنكية.</span><span class="sxs-lookup"><span data-stu-id="ea674-120">In the **Facility type** field, enter the name of the bank facility type that is related to the bank facility agreement.</span></span>
9.  <span data-ttu-id="ea674-121">في حقل **الوصف** أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="ea674-121">In the **Description** field, type a value.</span></span>
10. <span data-ttu-id="ea674-122">في الحقل **مجموعة التسهيلات** حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="ea674-122">In the **Facility group** field, select the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="ea674-123">في القائمة، قم بالبحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="ea674-123">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="ea674-124">في الحقل **طبيعة التسهيلات** حدد خيارً.</span><span class="sxs-lookup"><span data-stu-id="ea674-124">In the **Facility nature** field, select an option.</span></span>
13. <span data-ttu-id="ea674-125">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea674-125">Select **Save**.</span></span>
14. <span data-ttu-id="ea674-126">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea674-126">Close the page.</span></span>


## <a name="set-up-a-bank-posting-profile"></a><span data-ttu-id="ea674-127">إعداد ملف تعريف ترحيل البنك</span><span class="sxs-lookup"><span data-stu-id="ea674-127">Set up a bank posting profile</span></span> 

1.  <span data-ttu-id="ea674-128">انتقل إلى **‏‫إدارة النقد والبنوك‬ > إعداد > ملف تعريف المستندات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="ea674-128">Go to **Cash and bank management > Setup > Bank documents posting profile**.</span></span>
 
    ![لقطة شاشة لصفحة ملف تعريف ترحيل المستندات البنكية.](../media/bank-document-posting-profile.png)  

2.  <span data-ttu-id="ea674-130">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="ea674-130">Select **New**.</span></span>
3.  <span data-ttu-id="ea674-131">في الحقل برقم **المجموعة/الحساب** حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="ea674-131">In the **Account/Group** number field, select the drop-down button to open the lookup.</span></span>
4.  <span data-ttu-id="ea674-132">في القائمة، قم بالبحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="ea674-132">In the list, find and select the desired record.</span></span>
5.  <span data-ttu-id="ea674-133">في الحقل **تسوية الحساب** حدد الحساب الرئيسي لإجراء التسوية.</span><span class="sxs-lookup"><span data-stu-id="ea674-133">In the **Settle account** field, select the main account for settlement.</span></span>
6.  <span data-ttu-id="ea674-134">في الحقل **حساب التكاليف** حدد الحساب الخاص بحركات المصروفات.</span><span class="sxs-lookup"><span data-stu-id="ea674-134">In the **Charges account** field, select the account for expense transactions.</span></span>
7.  <span data-ttu-id="ea674-135">في الحقل **حساب الهامش** حدد الحساب الخاص بحركة الهامش.</span><span class="sxs-lookup"><span data-stu-id="ea674-135">In the **Margin account** field, select the account for the margin transaction.</span></span>
8.  <span data-ttu-id="ea674-136">في الحقل **حساب التصفية** حدد حساب التصفية لحركة خطاب الضمان.</span><span class="sxs-lookup"><span data-stu-id="ea674-136">In the **Liquidation account** field, select the liquidation account for the letter of guarantee transaction.</span></span>
9.  <span data-ttu-id="ea674-137">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea674-137">Select **Save**.</span></span>
10. <span data-ttu-id="ea674-138">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea674-138">Close the page.</span></span>


## <a name="create-a-bank-facility-agreement"></a><span data-ttu-id="ea674-139">إنشاء إتفاقية تسهيل بنكي</span><span class="sxs-lookup"><span data-stu-id="ea674-139">Create a bank facility agreement</span></span> 

1.  <span data-ttu-id="ea674-140">انتقل إلى **‏‫إدارة النقد والبنوك‬ > خطابات الضمان > اتفاقيات التسهيلات البنكية**.</span><span class="sxs-lookup"><span data-stu-id="ea674-140">Go to **Cash and bank management > Letters of guarantee > Bank facility agreements**.</span></span>
2.  <span data-ttu-id="ea674-141">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="ea674-141">Select **New**.</span></span>
3.  <span data-ttu-id="ea674-142">في الحقل **رقم الاتفاقية** أدخل رقم اتفاقية البنك الخاص بالحركة.</span><span class="sxs-lookup"><span data-stu-id="ea674-142">In the **Agreement number** field, enter the bank agreement number for the transaction.</span></span>
4.  <span data-ttu-id="ea674-143">في الحقل **حساب البنك** حدد رقم الحساب البنكي الذي يُفتح من أجله خطاب الضمان.</span><span class="sxs-lookup"><span data-stu-id="ea674-143">In the **Bank account** field, select the bank account number for which the letter of guarantee is open.</span></span>
5.  <span data-ttu-id="ea674-144">في القائمة، انقر على الارتباط في الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="ea674-144">In the list, click the link in the selected row.</span></span>
6.  <span data-ttu-id="ea674-145">في الحقل **تاريخ البدء** أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="ea674-145">In the **Start date** field, enter a date and time.</span></span>
7.  <span data-ttu-id="ea674-146">في الحقل **تاريخ الإنهاء** أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="ea674-146">In the **End date** field, enter a date and time.</span></span>
8.  <span data-ttu-id="ea674-147">قم بتبديل توسيع القسم **عام**.</span><span class="sxs-lookup"><span data-stu-id="ea674-147">Toggle the expansion of the **General** section.</span></span>
9.  <span data-ttu-id="ea674-148">حدد **إضافة سطر**.</span><span class="sxs-lookup"><span data-stu-id="ea674-148">Select **Add line**.</span></span>
10. <span data-ttu-id="ea674-149">في الحقل **نوع التسهيلات** حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="ea674-149">In the **Facility type** field, select the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="ea674-150">في القائمة، قم بالبحث عن السجل المطلوب وحدده.</span><span class="sxs-lookup"><span data-stu-id="ea674-150">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="ea674-151">في القائمة، انقر على الارتباط في الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="ea674-151">In the list, click the link in the selected row.</span></span>
13. <span data-ttu-id="ea674-152">في الحقل **الحد** أدخل المبلغ الذي تم التفاوض عليه مع البنك.</span><span class="sxs-lookup"><span data-stu-id="ea674-152">In the **Limit** field, enter the amount negotiated with the bank.</span></span>
14. <span data-ttu-id="ea674-153">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea674-153">Select **Save**.</span></span>
15. <span data-ttu-id="ea674-154">قم بتبديل توسيع القسم **خطاب الضمان**.</span><span class="sxs-lookup"><span data-stu-id="ea674-154">Toggle the expansion of the **Letter of guarantee** section.</span></span>
16. <span data-ttu-id="ea674-155">في الحقل **أسلوب الحساب** حدد خيارً.</span><span class="sxs-lookup"><span data-stu-id="ea674-155">In the **Calculation method** field, select an option.</span></span>
<span data-ttu-id="ea674-156">أدخل تفاصيل النسبة المئوية وطريقه الحساب لـ **الهامش النقدي** أو **عمولة الإصدار** أو **عمولة المد أو زيادة عمولة القيمة** أو **خفض عمولة القيمة** كما هو مناسب.</span><span class="sxs-lookup"><span data-stu-id="ea674-156">Enter the calculation method and percentage details for the **Cash margin**, **Issuance commission**, **Extension commission, Increase value commission**, or **Decrease value commission**, as appropriate.</span></span>
17. <span data-ttu-id="ea674-157">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea674-157">Select **Save**.</span></span>




## <a name="extend-a-bank-facility-agreement"></a><span data-ttu-id="ea674-158">تمديد اتفاقية التسهيلات البنكية</span><span class="sxs-lookup"><span data-stu-id="ea674-158">Extend a bank facility agreement</span></span> 

1.  <span data-ttu-id="ea674-159">حدد **توسيع** لفتح مربع الحوار المنسدل.</span><span class="sxs-lookup"><span data-stu-id="ea674-159">Select **Extend** to open the drop-down dialog box.</span></span>
2.  <span data-ttu-id="ea674-160">في الحقل **رقم الاتفاقية الجديد** اكتب قيمةً.</span><span class="sxs-lookup"><span data-stu-id="ea674-160">In the **New agreement number** field, type a value.</span></span>
3.  <span data-ttu-id="ea674-161">في الحقل **تاريخ الإنهاء** أدخل تاريخاً ووقتاً.</span><span class="sxs-lookup"><span data-stu-id="ea674-161">In the **End date** field, enter a date and time.</span></span>
4.  <span data-ttu-id="ea674-162">حدد **تمديد**.</span><span class="sxs-lookup"><span data-stu-id="ea674-162">Select **Extend**.</span></span>
5.  <span data-ttu-id="ea674-163">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ea674-163">Select **Save**.</span></span>
6.  <span data-ttu-id="ea674-164">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="ea674-164">Close the page.</span></span>

