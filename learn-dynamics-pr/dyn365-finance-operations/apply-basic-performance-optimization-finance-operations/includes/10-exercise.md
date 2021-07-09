---
ms.openlocfilehash: bf3c65d487e950d6a341bc3082cf206fd09ed977
ms.sourcegitcommit: 977539219691830a564399fa637ced040d24475e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "6072561"
---

## <a name="scenario"></a><span data-ttu-id="d7845-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="d7845-101">Scenario</span></span>
<span data-ttu-id="d7845-102">تم تكليف مطور تطبيقات Finance and Operations بإنشاء مهمة لتحديث تفاوت "السعر" إلى 2 بالمائة لجميع الأصناف الموجودة في مجموعة منتجات التلفزيون.</span><span class="sxs-lookup"><span data-stu-id="d7845-102">The Finance and Operations apps developer has been tasked with creating a job to update the Price tolerance to 2 percent for all items in the Television product group.</span></span>


## <a name="create-a-new-project"></a><span data-ttu-id="d7845-103">إنشاء مشروع جديد</span><span class="sxs-lookup"><span data-stu-id="d7845-103">Create a new project</span></span>

1. <span data-ttu-id="d7845-104">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d7845-104">Minimize the Internet Explorer window.</span></span> 
2. <span data-ttu-id="d7845-105">افتح Visual Studio</span><span class="sxs-lookup"><span data-stu-id="d7845-105">Open Visual Studio.</span></span>
3. <span data-ttu-id="d7845-106">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="d7845-106">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
4. <span data-ttu-id="d7845-107">افتح القائمة **ملف** وحدد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="d7845-107">Open the **File** menu and select **New > Project**.</span></span>
5. <span data-ttu-id="d7845-108">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.</span><span class="sxs-lookup"><span data-stu-id="d7845-108">In the **New Project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Installed**.</span></span>
6. <span data-ttu-id="d7845-109">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="d7845-109">On the middle pane, select **Finance Operations**.</span></span>
7. <span data-ttu-id="d7845-110">قم بتسمية المشروع **PriceToleranceUpdateJob**.</span><span class="sxs-lookup"><span data-stu-id="d7845-110">Name the project **PriceToleranceUpdateJob**.</span></span>
8. <span data-ttu-id="d7845-111">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d7845-111">Select **OK**.</span></span>
9. <span data-ttu-id="d7845-112">لضمان الرجوع إلى مجموعة التطبيقات الصحيحة، انتقل إلى قائمة **Dynamics 365**</span><span class="sxs-lookup"><span data-stu-id="d7845-112">To ensure the correct applications suite is referenced, go to the **Dynamics 365** menu</span></span>
10. <span data-ttu-id="d7845-113">حدد **إدارة النماذج > تحديث معلمات النموذج**</span><span class="sxs-lookup"><span data-stu-id="d7845-113">Select **Model Management > Update model parameters**</span></span>
11. <span data-ttu-id="d7845-114">حدد نموذج **FleetManagement** من القائمة المنسدلة **اسم النموذج**.</span><span class="sxs-lookup"><span data-stu-id="d7845-114">Select the **FleetManagement** model from the **Model name** dropdown list.</span></span> 
12. <span data-ttu-id="d7845-115">حدد **التالي**، ثم تأكد من تحديد **ApplicationSuite** في القائمة المنسدلة **الحزم المشار إليها**.</span><span class="sxs-lookup"><span data-stu-id="d7845-115">Select **Next**, then ensure **ApplicationSuite** is selected in the **Referenced packages** dropdown.</span></span> 
13. <span data-ttu-id="d7845-116">حدد **التالي** ثم **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="d7845-116">Select **Next** then **Finish**.</span></span>
14. <span data-ttu-id="d7845-117">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="d7845-117">Open the **Dynamics 365** menu in the ribbon again.</span></span>
15. <span data-ttu-id="d7845-118">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="d7845-118">Select **Options**.</span></span>
16. <span data-ttu-id="d7845-119">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="d7845-119">Under the **Dynamics 365** node on the left pane, select **Projects**.</span></span>
17. <span data-ttu-id="d7845-120">تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **ومزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="d7845-120">Ensure the check boxes for **Organize projects by element type** and **Synchronize database on build for newly created project** are selected.</span></span>
18. <span data-ttu-id="d7845-121">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d7845-121">Select **OK**.</span></span>


## <a name="create-a-runnable-class"></a><span data-ttu-id="d7845-122">إنشاء فئة قابلة للتشغيل</span><span class="sxs-lookup"><span data-stu-id="d7845-122">Create a runnable class</span></span> 

1. <span data-ttu-id="d7845-123">في النافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **PriceToleranceUpdateJob**.</span><span class="sxs-lookup"><span data-stu-id="d7845-123">In the **Solution Explorer** window, right-click the **PriceToleranceUpdateJob** project.</span></span>
2. <span data-ttu-id="d7845-124">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="d7845-124">Select **Add > New Item**.</span></span>
3. <span data-ttu-id="d7845-125">في الجزء الأيمن، حدد **عناصر Dynamics 365** ثم حدد **الرمز**.</span><span class="sxs-lookup"><span data-stu-id="d7845-125">On the left pane, select **Dynamics 365 Items** and then select **Code**.</span></span>
4. <span data-ttu-id="d7845-126">في الجزء الأوسط، حدد **فئة قابلة للتشغيل (مهمة)**.</span><span class="sxs-lookup"><span data-stu-id="d7845-126">On the middle pane, select **Runnable class (Job)**.</span></span>
5. <span data-ttu-id="d7845-127">أدخل **PriceToleranceUpdate** في الحقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="d7845-127">Enter **PriceToleranceUpdate** in the **Name** field.</span></span>
6. <span data-ttu-id="d7845-128">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="d7845-128">Select **Add**.</span></span>
7. <span data-ttu-id="d7845-129">سيتم الآن فتح الفئة القابلة للتشغيل **PriceToleranceUpdate** في النافذة "مصمم العناصر".</span><span class="sxs-lookup"><span data-stu-id="d7845-129">The **PriceToleranceUpdate** runnable class will now be open in the element designer window.</span></span>
8. <span data-ttu-id="d7845-130">قم بإزالة الكود الموجود في النافذة "مصمم العناصر"، ثم قم بإدخال الكود الآتي سطراً بسطر:</span><span class="sxs-lookup"><span data-stu-id="d7845-130">Remove the code present in Element designer window and then enter the following code line by line:</span></span>
   
   ```xpp
   class PriceToleranceUpdate
   {
        Public static void main(Args _args)
        {
        InventTable inventTable;
        InventItemGroupItem inventItemGroupItem;
                UPDATE_RECORDSET inventTable
                SETTING
                     ItemPriceToleranceGroupId = "2%"
                JOIN inventItemGroupItem
                      Where inventItemGroupItem.Itemid == inventTable.itemid
                      && inventItemGroupItem.ItemGroupId == 'Television';
       }
   }
   ```
9. <span data-ttu-id="d7845-131">احفظ الفئة القابلة للتشغيل.</span><span class="sxs-lookup"><span data-stu-id="d7845-131">Save the runnable class.</span></span>
10. <span data-ttu-id="d7845-132">انقر بزر الماوس الأيمن فوق مشروع **PriceToleranceUpdateJob** وحدد **بناء**.</span><span class="sxs-lookup"><span data-stu-id="d7845-132">Right-click the **PriceToleranceUpdateJob** project and select **Build**.</span></span>
11. <span data-ttu-id="d7845-133">انقر بزر الماوس الأيمن فوق الفئة القابلة للتشغيل **PriceToleranceUpdate** وحدد **تعيين ككائن بدء التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="d7845-133">Right-click the **PriceToleranceUpdate** runnable class and select **Set as Startup Object**.</span></span>
12. <span data-ttu-id="d7845-134">من شريط الأدوات، حدد الخيار **تصحيح الأخطاء > البدء دون تصحيح الأخطاء** لتشغيل الفئة.</span><span class="sxs-lookup"><span data-stu-id="d7845-134">From the toolbar, select the option **Debug > Start Without Debugging** to run the class.</span></span>



