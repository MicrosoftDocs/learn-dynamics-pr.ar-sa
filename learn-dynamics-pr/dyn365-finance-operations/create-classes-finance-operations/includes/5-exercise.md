---
ms.openlocfilehash: ba9e48e9ce4fa01db9dc8f9be69789abe4c37ebd
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072624"
---
## <a name="scenario"></a><span data-ttu-id="fbe7f-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="fbe7f-101">Scenario</span></span>
<span data-ttu-id="fbe7f-102">باعتبارك مطور تطبيقات Finance and Operations، تم تكليفك بمهمة إدراج سجلات عملاء في جدول شركة Fleet Management.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-102">As the Finance and Operations apps developer, you have been tasked with inserting customer records into a table for your Fleet Management company.</span></span> <span data-ttu-id="fbe7f-103">حيث تحتاج إلى إنشاء فئة قابلة للتشغيل وإضافة الكود الذي ستُدرج سجلين في جدول `FMCustomer`.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-103">You need to create a runnable class and add code that will insert two records into the `FMCustomer` table.</span></span>


## <a name="create-a-runnable-class"></a><span data-ttu-id="fbe7f-104">إنشاء فئة قابلة للتشغيل</span><span class="sxs-lookup"><span data-stu-id="fbe7f-104">Create a runnable class</span></span> 

1. <span data-ttu-id="fbe7f-105">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-105">Minimize the Internet Explorer window.</span></span>
1. <span data-ttu-id="fbe7f-106">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-106">Open Visual Studio.</span></span>
1. <span data-ttu-id="fbe7f-107">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-107">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
1. <span data-ttu-id="fbe7f-108">ابدأ في إنشاء مشروع جديد عن طريق فتح قائمة **الملف** وتحديد **مشروع > جديد**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-108">Start creating a new project by opening the **File** menu and selecting **New > Project**.</span></span>
1. <span data-ttu-id="fbe7f-109">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-109">In the **New Project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Installed**.</span></span>
1. <span data-ttu-id="fbe7f-110">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-110">On the middle pane, select **Finance Operations**.</span></span>
1. <span data-ttu-id="fbe7f-111">قم بتسمية المشروع **FleetManagementSecurityProject**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-111">Name the project **FleetManagementClassProject**.</span></span>
1. <span data-ttu-id="fbe7f-112">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-112">Select **OK**.</span></span>
1. <span data-ttu-id="fbe7f-113">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-113">Open the **Dynamics 365** menu in the ribbon.</span></span>
1. <span data-ttu-id="fbe7f-114">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-114">Select **Options**.</span></span>
1. <span data-ttu-id="fbe7f-115">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-115">Under the **Dynamics 365** node on the left pane, select  **Projects**.</span></span>
1. <span data-ttu-id="fbe7f-116">تأكد من تحديد خانتي الاختيار لكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-116">Ensure the check boxes are selected for **Organize projects by element type** and  **Synchronize database on build for newly created project**.</span></span>
1. <span data-ttu-id="fbe7f-117">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-117">Select **OK**.</span></span>
1. <span data-ttu-id="fbe7f-118">في **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementClassProject**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-118">In the **Solution Explorer**, right-click the project    **FleetManagementClassProject**.</span></span>
1. <span data-ttu-id="fbe7f-119">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-119">Select **Add > New Item**.</span></span>
1. <span data-ttu-id="fbe7f-120">في الجزء الأيمن، حدد **عناصر Dynamics 365** ثم حدد **الرمز**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-120">On the left pane, select **Dynamics 365 Items** and then select **Code**.</span></span>
1. <span data-ttu-id="fbe7f-121">في الجزء الأوسط، حدد **فئة قابلة للتشغيل (مهمة)**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-121">On the middle pane, select **Runnable Class (Job)**.</span></span>
1. <span data-ttu-id="fbe7f-122">أدخل **FMInsertCustomers** في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-122">Enter **FMInsertCustomers** in the **Name** field.</span></span>
1. <span data-ttu-id="fbe7f-123">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-123">Select **Add**.</span></span> <span data-ttu-id="fbe7f-124">سيتم فتح فئة **FMInsertCustomers** الآن في نافذة **مصمم الأكواد**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-124">The **FMInsertCustomers** class will now be open in the **Code designer** window.</span></span>

## <a name="add-code-to-insert-customer-records"></a><span data-ttu-id="fbe7f-125">إضافة كود لإدراج سجلات العملاء</span><span class="sxs-lookup"><span data-stu-id="fbe7f-125">Add code to insert customer records</span></span> 

1. <span data-ttu-id="fbe7f-126">في نافذة **مصمم الأكواد**، قم بإدراج سطر فارغ بين السطرين 6 و7 باستخدام مفتاح **Enter** وقم بإزالة الشُرط المائلة (///).</span><span class="sxs-lookup"><span data-stu-id="fbe7f-126">In the **Code designer** window, insert a blank line between lines 6 and 7 by using the **Enter** key and remove the slashes (///).</span></span>
2. <span data-ttu-id="fbe7f-127">أدخل الكود التالي في السطر 7:</span><span class="sxs-lookup"><span data-stu-id="fbe7f-127">Enter the following code on line 7:</span></span>

    ```xpp
       FMCustomer FMCustomer;
    ```

3. <span data-ttu-id="fbe7f-128">في نافذة **مصمم الأكواد**، قم بإدراج سطر فارغ بين الأقواس المتعرجة في السطرين 9 و10 باستخدام مفتاح **Enter**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-128">In the **Code designer** window, insert a blank line between the curly braces on lines 9 and 10 by using the **Enter** key.</span></span>
4. <span data-ttu-id="fbe7f-129">انسخ الكود التالي والصقه في المساحة الخالية في السطر 10:</span><span class="sxs-lookup"><span data-stu-id="fbe7f-129">Copy and paste the following code into the blank space on line 10:</span></span>

    ```xpp
       FMInsertCustomers FMInsertCustomers = new  FMInsertCustomers();
       FMInsertCustomers.run();
    ``` 

5. <span data-ttu-id="fbe7f-130">وفي السطر 13، انسخ الكود التالي والصقه:</span><span class="sxs-lookup"><span data-stu-id="fbe7f-130">On line 13, copy and paste the following code:</span></span>

    ```xpp
          public void run()
         {
          this.insertRecords();
         }
         private void insertRecords()
         {
             ttsBegin;

                FMCustomer.FirstName = "John";
                FMCustomer.LastName = "Smith";
                FMCustomer.Email = "johnsmith@contoso.com";

                FMCustomer.insert();

                FMCustomer.clear();
                FMCustomer.FirstName = "Sally";
                FMCustomer.LastName = "Smith";
                FMCustomer.Email = "sallysmith@contoso.com";

                FMCustomer.insert();

             ttsCommit;
        }
    ```

6. <span data-ttu-id="fbe7f-131">في **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق فئة `FMInsertCustomers`.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-131">In the **Solution Explorer**, right-click the `FMInsertCustomers` class.</span></span>
7. <span data-ttu-id="fbe7f-132">حدد **تعيين ككائن بدء التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-132">Select **Set as Startup Object**.</span></span>
8. <span data-ttu-id="fbe7f-133">قم بتنفيذ بناء بالنقر بزر الماوس الأيمن فوق مشروع **FleetManagementClassProject** في نافذة **مستكشف الحلول** ثم حدد **البناء**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-133">Perform a build by right-clicking the project **FleetManagementClassProject** in the **Solution Explorer** and then selecting **Build**.</span></span>
9. <span data-ttu-id="fbe7f-134">قم بتشغيل الفئة دون التصحيح بتحديد القائمة **تصحيح**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-134">Run the class without debugging by selecting the **Debug** menu.</span></span> <span data-ttu-id="fbe7f-135">حدد **ابدأ بدون تصحيح**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-135">Select **Start Without Debugging**.</span></span> <span data-ttu-id="fbe7f-136">يمكنك أيضا استخدام اختصار لوحة المفاتيح **Ctrl + F5**.</span><span class="sxs-lookup"><span data-stu-id="fbe7f-136">You can also use the keyboard shortcut **Ctrl + F5**.</span></span>



