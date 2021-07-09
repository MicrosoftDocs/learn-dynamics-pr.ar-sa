---
ms.openlocfilehash: a937c39db8677ad9f8e141d4322599e8b9419c79
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072609"
---
## <a name="scenario"></a><span data-ttu-id="2bcc4-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="2bcc4-101">Scenario</span></span>

<span data-ttu-id="2bcc4-102">باعتبارك مطور تطبيقات Finance and Operations، طلبت منك شركة Fleet Management إنشاء كيان بيانات لاستخدامه في عمليات تكامل البيانات.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-102">As the Finance and Operations apps developer, you have been asked by the Fleet Management company to create a data entity to use for data integrations.</span></span>

## <a name="create-a-new-project"></a><span data-ttu-id="2bcc4-103">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="2bcc4-103">Create a new project</span></span>

1.  <span data-ttu-id="2bcc4-104">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-104">Minimize the Internet Explorer window.</span></span> 
2.  <span data-ttu-id="2bcc4-105">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-105">Open Visual Studio.</span></span>
3.  <span data-ttu-id="2bcc4-106">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-106">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
2.  <span data-ttu-id="2bcc4-107">قم بإنشاء مشروع جديد عن طريق فتح قائمة **الملف** وتحديد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-107">Create a new project by opening the **File** menu and selecting **New > Project**.</span></span>
3.  <span data-ttu-id="2bcc4-108">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-108">In the **New Project** dialog box, ensure that **Dynamics 365** is selected in the left pane under **Installed**.</span></span>
4.  <span data-ttu-id="2bcc4-109">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-109">On the middle pane, select **Finance Operations**.</span></span>
5.  <span data-ttu-id="2bcc4-110">قم بتسمية المشروع **FleetManagementEntityProject2**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-110">Name the project **FleetManagementEntityProject2**.</span></span>
6.  <span data-ttu-id="2bcc4-111">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-111">Select **OK**.</span></span>
7.  <span data-ttu-id="2bcc4-112">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-112">Open the **Dynamics 365** menu in the ribbon.</span></span>
8.  <span data-ttu-id="2bcc4-113">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-113">Select **Options**.</span></span>
9.  <span data-ttu-id="2bcc4-114">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-114">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
10. <span data-ttu-id="2bcc4-115">تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **ومزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-115">Ensure the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project** are selected.</span></span>
11. <span data-ttu-id="2bcc4-116">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-116">Select **OK**.</span></span>

## <a name="create-a-data-entity"></a><span data-ttu-id="2bcc4-117">إنشاء كيان بيانات</span><span class="sxs-lookup"><span data-stu-id="2bcc4-117">Create a data entity</span></span>

1.  <span data-ttu-id="2bcc4-118">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementEntityProject2**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-118">In the **Solution Explorer** window, right-click your **FleetManagementEntityProject2** project.</span></span>
13. <span data-ttu-id="2bcc4-119">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-119">Select **Add > New Item**.</span></span>
14. <span data-ttu-id="2bcc4-120">في الجزء الأيسر، حدد **عناصر Dynamics 365** ثم حدد **نموذج البيانات**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-120">On the left pane, select **Dynamics 365 Items** and then select **Data Model**.</span></span>
15. <span data-ttu-id="2bcc4-121">في الجزء الأوسط، حدد **كيان البيانات**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-121">On the middle pane, select **Data Entity**.</span></span>
16. <span data-ttu-id="2bcc4-122">أدخل **FMMyDataEntity** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-122">Enter **FMMyDataEntity** in the **Name** field.</span></span>
17. <span data-ttu-id="2bcc4-123">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-123">Select **Add**.</span></span> <span data-ttu-id="2bcc4-124">سيتم فتح معالج **كيان البيانات**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-124">The **Data Entity Wizard** will open.</span></span>
18. <span data-ttu-id="2bcc4-125">في القائمة المنسدلة **مصدر البيانات الأساسي**، حدد الجدول **FMCustomer**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-125">In the **Primary datasource** drop-down menu, select the **FMCustomer** table.</span></span>
19. <span data-ttu-id="2bcc4-126">حدد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="2bcc4-126">Specify the following options:</span></span>
    -   <span data-ttu-id="2bcc4-127">فئة الكيان - **الرئيسي**</span><span class="sxs-lookup"><span data-stu-id="2bcc4-127">Entity category - **Master**</span></span>
    -   <span data-ttu-id="2bcc4-128">حدد خانة الاختيار **لتمكين واجهة برمجة التطبيقات (API) العامة**</span><span class="sxs-lookup"><span data-stu-id="2bcc4-128">Select the check box for **Enable public API**</span></span>
    -   <span data-ttu-id="2bcc4-129">حدد خانة الاختيار **لتمكين إمكانيات إدارة البيانات**</span><span class="sxs-lookup"><span data-stu-id="2bcc4-129">Select the check box for **Enable data management capabilities**</span></span>
    -   <span data-ttu-id="2bcc4-130">ترك جميع الحقول الأخرى كما هي</span><span class="sxs-lookup"><span data-stu-id="2bcc4-130">Leave all other fields as-is</span></span>
20. <span data-ttu-id="2bcc4-131">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-131">Select **Next**.</span></span>
21. <span data-ttu-id="2bcc4-132">حدد كيان البيانات وحدد الحقول التي سيتم تضمينها في هذا الكيان.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-132">Define your data entity and specify the fields that will be included in this entity.</span></span>
22. <span data-ttu-id="2bcc4-133">حدد كل الحقول.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-133">Select all fields.</span></span>
23. <span data-ttu-id="2bcc4-134">حدد خانة الاختيار **لتحويل التسميات إلى أسماء حقول**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-134">Select the check box for **Convert labels to field names**.</span></span>
24. <span data-ttu-id="2bcc4-135">حدد **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-135">Select **Finish**.</span></span> <span data-ttu-id="2bcc4-136">ستشاهد كيان البيانات الجديد في مشروعك، بالإضافة إلى جدول تشغيل مرحلي وامتيازات الأمان.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-136">You will see your new data entity in your project, along with a staging table and security privileges.</span></span>
25. <span data-ttu-id="2bcc4-137">قم بتنفيذ بناء بالنقر بزر الماوس الأيمن فوق مشروع **FleetManagementEntityProject2** في نافذة **مستكشف الحلول** ثم حدد **البناء**.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-137">Perform a build by right-clicking the project  **FleetManagementEntityProject2** in **Solution Explorer** and then selecting **Build**.</span></span>

<span data-ttu-id="2bcc4-138">قد يظهر لك خطأ نظراً لأنه يجب إيقاف تشغيل خادم الدُفعة في البيئة.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-138">You may see an error because the batch server needs to be turned off in the environment.</span></span> <span data-ttu-id="2bcc4-139">ومع ذلك، لا يؤثر هذا على البناء ويتم إنشاء وحدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="2bcc4-139">However, this does not affect the build and the data entity is created.</span></span>


