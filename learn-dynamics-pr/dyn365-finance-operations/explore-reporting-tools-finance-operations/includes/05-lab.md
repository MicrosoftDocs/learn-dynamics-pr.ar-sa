---
ms.openlocfilehash: be57b5da47d268d0571401ccd1a11f23c6e6f15a
ms.sourcegitcommit: 0484f01637a384540476f9c6e45ba64bd86526a8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/19/2021
ms.locfileid: "6072125"
---
## <a name="scenario"></a><span data-ttu-id="ff643-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="ff643-101">Scenario</span></span>

<span data-ttu-id="ff643-102">إذا أردت تمكين إطار عمل أذونات الجدول لجدول محدد في شجره مكونات البرنامج (AOT).</span><span class="sxs-lookup"><span data-stu-id="ff643-102">You want to enable the Table Permissions Framework for a specific table in the Application Object Tree (AOT).</span></span>

## <a name="enable-the-aosauthorization-property"></a><span data-ttu-id="ff643-103">تمكين الخاصية تفويض Application Object Server‏ (AOSAuthorization)</span><span class="sxs-lookup"><span data-stu-id="ff643-103">Enable the AOSAuthorization property</span></span>

1.  <span data-ttu-id="ff643-104">قم بتصغير نافذة Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ff643-104">Minimize the Internet Explorer window.</span></span>
2.  <span data-ttu-id="ff643-105">افتح Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="ff643-105">Open Visual Studio.</span></span>
3.  <span data-ttu-id="ff643-106">حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.</span><span class="sxs-lookup"><span data-stu-id="ff643-106">Select **Yes** in the **Do you want to allow this app to make changes to your device?** window.</span></span>
4.  <span data-ttu-id="ff643-107">ابدأ في إنشاء مشروع جديد عن طريق فتح قائمة **الملف** وتحديد **مشروع > جديد**.</span><span class="sxs-lookup"><span data-stu-id="ff643-107">Start creating a new project by opening the **File** menu and selecting **New > Project**.</span></span>
5.  <span data-ttu-id="ff643-108">في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **القوالب**.</span><span class="sxs-lookup"><span data-stu-id="ff643-108">In the **New Project** dialog box, ensure that **Dynamics 365** is selected on the left pane under **Templates**.</span></span>
6.  <span data-ttu-id="ff643-109">في الجزء الأوسط، حدد **العمليات المالية**.</span><span class="sxs-lookup"><span data-stu-id="ff643-109">On the middle pane, select **Finance  Operations**.</span></span>
7.  <span data-ttu-id="ff643-110">قم بتسمية المشروع **FleetManagementSecurityProject**.</span><span class="sxs-lookup"><span data-stu-id="ff643-110">Name the project **FleetManagementClassProject**.</span></span>
8.  <span data-ttu-id="ff643-111">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ff643-111">Select **OK**.</span></span>
9.  <span data-ttu-id="ff643-112">افتح القائمة **Dynamics 365** في الشريط.</span><span class="sxs-lookup"><span data-stu-id="ff643-112">Open the **Dynamics 365** menu in the ribbon.</span></span>
10. <span data-ttu-id="ff643-113">حدد **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="ff643-113">Select **Options**.</span></span>
11. <span data-ttu-id="ff643-114">ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="ff643-114">Under the **Dynamics 365** node on the left pane, select  **Projects**.</span></span>
12. <span data-ttu-id="ff643-115">تأكد من تحديد خانتي الاختيار لكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.</span><span class="sxs-lookup"><span data-stu-id="ff643-115">Ensure the check boxes are selected for **Organize projects by element type** and **Synchronize database on build for newly created project**.</span></span>
13. <span data-ttu-id="ff643-116">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ff643-116">Select **OK**.</span></span>
5.  <span data-ttu-id="ff643-117">انقر بزر الماوس الأيمن فوق مشروع في مستكشف الحلول.</span><span class="sxs-lookup"><span data-stu-id="ff643-117">Right-click your project in the Solution Explorer.</span></span>
6.  <span data-ttu-id="ff643-118">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="ff643-118">Select **Add > New item**.</span></span>
7.  <span data-ttu-id="ff643-119">في الجزء الأيمن، حدد **نموذج البيانات** ثم حدد **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="ff643-119">On the left pane, select **Data Model** and then select **Table**.</span></span>
8.  <span data-ttu-id="ff643-120">قم بتسمية الجدول **جدولي**.</span><span class="sxs-lookup"><span data-stu-id="ff643-120">Name the table **MyTable**.</span></span>
9.  <span data-ttu-id="ff643-121">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="ff643-121">Select **Add**.</span></span>
10. <span data-ttu-id="ff643-122">مع فتح **جدولي** في المصمم، انقر بزر الماوس الأيمن فوق العقدة الرئيسية للجدول وحدد **الخصائص**.</span><span class="sxs-lookup"><span data-stu-id="ff643-122">With **MyTable** open in the designer, right-click the main node of the table and select **Properties**.</span></span>
11. <span data-ttu-id="ff643-123">في النافذة **الخصائص**، ابحث عن خاصية **تفويض AOS**.</span><span class="sxs-lookup"><span data-stu-id="ff643-123">In the **Properties** window, find the **AOS Authorization**  property.</span></span> <span data-ttu-id="ff643-124">وبشكلٍ افتراضي، يتم تعيين هذه الخاصية إلى **بلا**.</span><span class="sxs-lookup"><span data-stu-id="ff643-124">This property is set to **None** by default.</span></span>
12. <span data-ttu-id="ff643-125">حدد الرمز المنسدل في خاصيه "تفويض AOS"، حيث سترى ستة خيارات:</span><span class="sxs-lookup"><span data-stu-id="ff643-125">Select the drop-down icon in the AOS Authorization property, where you will see six options:</span></span>
    - <span data-ttu-id="ff643-126">بلا</span><span class="sxs-lookup"><span data-stu-id="ff643-126">None</span></span>
    - <span data-ttu-id="ff643-127">إنشاء حذف</span><span class="sxs-lookup"><span data-stu-id="ff643-127">CreateDelete</span></span>
    - <span data-ttu-id="ff643-128">تحديث حذف</span><span class="sxs-lookup"><span data-stu-id="ff643-128">UpdateDelete</span></span>
    - <span data-ttu-id="ff643-129">إنشاء تحديث حذف</span><span class="sxs-lookup"><span data-stu-id="ff643-129">CreateUpdateDelete</span></span>
    - <span data-ttu-id="ff643-130">إنشاء قراءة تحديث حذف</span><span class="sxs-lookup"><span data-stu-id="ff643-130">CreateReadUpdateDelete</span></span>
    - <span data-ttu-id="ff643-131">قراءة</span><span class="sxs-lookup"><span data-stu-id="ff643-131">Read</span></span>
13. <span data-ttu-id="ff643-132">حدد **إنشاء قراءة تحديث حذف**.</span><span class="sxs-lookup"><span data-stu-id="ff643-132">Select **CreateReadUpdateDelete**.</span></span>
14. <span data-ttu-id="ff643-133">حدد **حفظ جدولي**.</span><span class="sxs-lookup"><span data-stu-id="ff643-133">Select **Save MyTable**.</span></span>

