---
ms.openlocfilehash: 22351494de50ff3e2fdb8e156e1075159b3b1439
ms.sourcegitcommit: 45337c216dae17eda3fd77996e054b20515eb8dc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "6072099"
---
<span data-ttu-id="37e6b-101">أنت مطور يجب عليه أن يقوم بإجراء تخصيص لأسلوب إدراج `CustTable`.</span><span class="sxs-lookup"><span data-stu-id="37e6b-101">You are a developer that must make a customization to the `CustTable` insert method.</span></span> <span data-ttu-id="37e6b-102">عند إنشاء العميل، إذا كان التقدير الائتماني للعميل أقل من 200، فيجب حظر العميل لجميع عمليات التسليم والفواتير.</span><span class="sxs-lookup"><span data-stu-id="37e6b-102">Upon customer creation, if the customer credit rating is less than 200, then the customer should be blocked for all delivery and invoicing.</span></span> <span data-ttu-id="37e6b-103">يجب أن تظهر مطالبة لتنبيه الشخص الذي يقوم بإدخال تفاصيل العميل.</span><span class="sxs-lookup"><span data-stu-id="37e6b-103">A prompt should appear to alert the person who is entering the customer details.</span></span> 
 
## <a name="before-you-begin"></a><span data-ttu-id="37e6b-104">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="37e6b-104">Before you begin</span></span>

<span data-ttu-id="37e6b-105">للحصول على أقصى استفادة من هذا التدريب، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في تطبيقات Finance and Operations والتي يتم تثبيتها باستخدام Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="37e6b-105">To get the most benefit from this exercise, we recommend that you have the standard sample data available in Finance and Operations apps installed by using Lifecycle Services (LCS).</span></span> <span data-ttu-id="37e6b-106">ستحتاج أيضاً إلى بيئة مطور وترخيص تجريبي أو دائم باستخدام Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="37e6b-106">You will also need a developer environment and trial or permanent license for using Visual Studio.</span></span>


## <a name="create-a-new-project"></a><span data-ttu-id="37e6b-107">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="37e6b-107">Create a new project</span></span>

1.  <span data-ttu-id="37e6b-108">افتح Visual Studio، الذي يعمل كمسؤول، وافتح قائمة **ملف**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-108">Open Visual Studio, running as an administrator, and open the **File** menu.</span></span>
2.  <span data-ttu-id="37e6b-109">حدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-109">Select **New > Project**.</span></span>
3.  <span data-ttu-id="37e6b-110">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **القوالب**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-110">In the **New Project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Templates**.</span></span>
4.  <span data-ttu-id="37e6b-111">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-111">On the middle pane, select **Finance Operations**.</span></span>
5.  <span data-ttu-id="37e6b-112">قم بتسمية مشروع **ChainOfCommand**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-112">Name the project **ChainOfCommand**.</span></span>
6.  <span data-ttu-id="37e6b-113">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-113">Select **OK**.</span></span>
7.  <span data-ttu-id="37e6b-114">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="37e6b-114">Open the **Dynamics 365** menu in the ribbon.</span></span>
8.  <span data-ttu-id="37e6b-115">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-115">Select **Options**.</span></span>
9.  <span data-ttu-id="37e6b-116">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع‏‎**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-116">Under the **Dynamics 365** node on the left pane, select    **Projects**.</span></span>
10. <span data-ttu-id="37e6b-117">حدد خانتي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً‏**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-117">Select the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project**.</span></span>
11. <span data-ttu-id="37e6b-118">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-118">Select **OK**.</span></span>
12. <span data-ttu-id="37e6b-119">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق اسم مشروعك وحدد **الخصائص**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-119">In the **Solution explorer**, right-click your project name and select **Properties**.</span></span>
13. <span data-ttu-id="37e6b-120">في صفحه الخصائص، قم بتغيير حقل **النموذج** إلى **Fleet Management**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-120">In the properties page, change the **Model** field to **Fleet Management**.</span></span>
14. <span data-ttu-id="37e6b-121">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-121">Select **OK**.</span></span> 
15. <span data-ttu-id="37e6b-122">تحتاج الآن للتأكد من أن لديك المراجع الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="37e6b-122">Now you need to ensure you have the correct references.</span></span> 
16. <span data-ttu-id="37e6b-123">انتقل إلى قائمة **Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-123">Go to the **Dynamics 365** menu.</span></span> 
17. <span data-ttu-id="37e6b-124">حدد **إدارة النماذج > تحديث معلمات النموذج**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-124">Select **Model management > Update model parameters**.</span></span> 
18. <span data-ttu-id="37e6b-125">في القائمة المنسدلة **اسم النموذج** حدد **Fleet Management**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-125">In the **Model name** dropdown, select **Fleet Management**.</span></span> 
19. <span data-ttu-id="37e6b-126">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-126">Select **Next**.</span></span> 
20. <span data-ttu-id="37e6b-127">في الصفحة **حزم المراجع المحددة**، تأكد من تحديد **الدليل** ومجموعة **التطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-127">In the **Selected references packages** page, ensure **Directory** and **Application** Suite are checked.</span></span> 
21. <span data-ttu-id="37e6b-128">بمجرد الانتهاء، حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-128">Once finished, select **Finish**.</span></span> 


## <a name="create-an-extension-of-a-method-in-the-custtable-class"></a><span data-ttu-id="37e6b-129">إنشاء امتداد لأسلوب في فئة CustTable</span><span class="sxs-lookup"><span data-stu-id="37e6b-129">Create an extension of a method in the CustTable class</span></span>


1.  <span data-ttu-id="37e6b-130">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **ChainOfCommand**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-130">In the **Solution Explorer** window, right-click the project **ChainOfCommand**.</span></span>
2.  <span data-ttu-id="37e6b-131">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-131">Select **Add > New Item**.</span></span>
3.  <span data-ttu-id="37e6b-132">في الجزء الأيمن، حدد **عناصر ‎Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-132">In the left pane, select **Dynamics 365 Items**.</span></span>
4.  <span data-ttu-id="37e6b-133">في الجزء الأوسط، حدد **الفئة**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-133">Select **Class** in the middle pane.</span></span>
5.  <span data-ttu-id="37e6b-134">أدخل **CustTable_Extension** باعتباره الاسم.</span><span class="sxs-lookup"><span data-stu-id="37e6b-134">Enter **CustTable_Extension** as the name.</span></span>
6.  <span data-ttu-id="37e6b-135">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="37e6b-135">Select **Add**.</span></span>
7.  <span data-ttu-id="37e6b-136">في فئة **CustTable_Extension** أضف الكود التالي لتعيين الحقل **الفوترة والتسليم قيد الانتظار** إلى **الكل** لعرض رسالة بعد الإدراج.</span><span class="sxs-lookup"><span data-stu-id="37e6b-136">In the **CustTable_Extension** class, add the following code to set the field **Invoicing and Delivery on hold** to **All** and to display a message after the insert.</span></span>
```xpp
[ExtensionOf(tableStr(CustTable))]
final class CustTable_Extension
{
    public void insert(DirPartyType _partyType, Name _name,boolean _updateCRM)
   {
        if (str2Int(this.creditRating) < 200)
        {
            this.blocked = CustVendorBlocked::All;
            info("The customer has been placed on hold due to low credit rating. Please review.");
        }
        next insert();       
   } 
}
```
8.  <span data-ttu-id="37e6b-137">**احفظ** الفئة.</span><span class="sxs-lookup"><span data-stu-id="37e6b-137">**Save** the class.</span></span>
9.  <span data-ttu-id="37e6b-138">**أنشئ** المشروع.</span><span class="sxs-lookup"><span data-stu-id="37e6b-138">**Build** the project.</span></span>
