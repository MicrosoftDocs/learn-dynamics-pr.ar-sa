---
ms.openlocfilehash: 71ca064cbb9d198c3bc153dd484b920cf62a71f1
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071968"
---
<span data-ttu-id="ec3a7-101">تتكامل تطبيقات Finance and Operations أيضاً مع Microsoft Power Platform.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-101">Finance and Operations apps also integrates with Microsoft Power Platform.</span></span>
<span data-ttu-id="ec3a7-102">يدعم Power Automate هذا التكامل عبر الموصلات الخاصة به، في حين يصل Power BI وPower Apps إلى كيانات البيانات العامة التي يتم تخزينها في قاعدة بيانات تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-102">Power Automate supports this integration through its connectors, whereas Power BI and Power Apps access public data entities that are stored in the Finance and Operations apps database.</span></span> 

## <a name="connect-to-power-automate"></a><span data-ttu-id="ec3a7-103">الاتصال بـ Power Automate</span><span class="sxs-lookup"><span data-stu-id="ec3a7-103">Connect to Power Automate</span></span>

<span data-ttu-id="ec3a7-104">اتبع الخطوات التالية للبحث عن موصلات Power Automate لتطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-104">Follow these steps to find Power Automate connectors for Finance and Operations apps.</span></span> 

1.  <span data-ttu-id="ec3a7-105">في Power Automate، حدد رمز الترس لقائمة الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-105">In Power Automate, select the gear icon for the settings menu.</span></span>
2.  <span data-ttu-id="ec3a7-106">في القائمة المنسدلة، حدد **اتصالات**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-106">In the drop-down menu, select **Connections**.</span></span> <span data-ttu-id="ec3a7-107">اتصالات تطبيقات Finance and Operations، المدرجة كـ **Dynamics 365 for Fin & Ops** من بين قائمة الاتصالات المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-107">Finance and Operations apps connections, listed as **Dynamics 365 for Fin & Ops**, are among the list of available connections.</span></span>

    <span data-ttu-id="ec3a7-108">[![لقطة الشاشة هذه من Power Automate وتُظهر إضافة تطبيقات Finance and Operations كاتصال في صفحة إدارة اتصالاتك.](../media/flow.png)](../media/flow.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec3a7-108">[![This screenshot is from Power Automate and shows adding Finance and Operations apps as a connection in the Manage your connections page.](../media/flow.png)](../media/flow.png#lightbox)</span></span>

4.  <span data-ttu-id="ec3a7-109">عند تحديد الاتصال المناسب، حدد **إنشاء اتصال** وقم بإعداد الاتصال عن طريق إدخال بيانات الاعتماد الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-109">When you have selected the appropriate connection, select **Create Connection** and set up the connection by entering your credentials.</span></span> <span data-ttu-id="ec3a7-110">سيظهر الاتصال في **الاتصالات الخاصة بي** عندما تقوم بإعداده.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-110">The connection will appear in **My Connections** when you have set it up.</span></span>

## <a name="connect-to-power-bi-desktop"></a><span data-ttu-id="ec3a7-111">الاتصال بـ Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="ec3a7-111">Connect to Power BI Desktop</span></span>
  
<span data-ttu-id="ec3a7-112">اتبع الخطوات التالية لتوصيل Power BI Desktop بتطبيقات Finance and Operations:</span><span class="sxs-lookup"><span data-stu-id="ec3a7-112">Follow these steps to connect Power BI Desktop to Finance and Operations apps.</span></span> 

1.  <span data-ttu-id="ec3a7-113">حدد  **الحصول على البيانات** من شريط  **الصفحة الرئيسية** .</span><span class="sxs-lookup"><span data-stu-id="ec3a7-113">Select **Get Data** from the **Home** ribbon.</span></span>
2.  <span data-ttu-id="ec3a7-114">حدد الفئة **أخرى** .</span><span class="sxs-lookup"><span data-stu-id="ec3a7-114">Select the **Other** category.</span></span>
3.  <span data-ttu-id="ec3a7-115">حدد **موجز OData**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-115">Select **OData Feed**.</span></span>

    <span data-ttu-id="ec3a7-116">[![تعرض لقطة الشاشة هذه من تطبيقات Power BI Desktop شاشة الحصول على البيانات للاتصال بموجز OData.](../media/power-bi.png)](../media/power-bi.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec3a7-116">[![This screenshot from the Power BI Desktop app shows the Get Data screen to connect to an OData Feed.](../media/power-bi.png)](../media/power-bi.png#lightbox)</span></span>
4.  <span data-ttu-id="ec3a7-117">انقر على **اتصال**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-117">Click **Connect**.</span></span>
5.  <span data-ttu-id="ec3a7-118">أدخل معلومات الاتصال في الصفحة التي تظهر، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-118">Enter connection information into the page that appears, and then select  **OK**.</span></span>
5.  <span data-ttu-id="ec3a7-119">حدد البيانات التي تحتاج إليها ثم حدد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-119">Select the data that you need and then select **Load**.</span></span>

## <a name="connect-to-power-apps"></a><span data-ttu-id="ec3a7-120">الاتصال بـ Power Apps</span><span class="sxs-lookup"><span data-stu-id="ec3a7-120">Connect to Power Apps</span></span>

<span data-ttu-id="ec3a7-121">اتبع الخطوات التالية لتوصيل تطبيقات  Finance and Operations في Power Apps:</span><span class="sxs-lookup"><span data-stu-id="ec3a7-121">Follow these steps to connect to Finance and Operations apps in Power Apps.</span></span>


1.  <span data-ttu-id="ec3a7-122">عند إنشاء تطبيق Power Apps جديد، حدد الخيار **بدء من البيانات**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-122">When creating a new Power Apps app, select the **Start from data** option.</span></span> 
2.  <span data-ttu-id="ec3a7-123">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-123">Select **Create**.</span></span>
3.  <span data-ttu-id="ec3a7-124">في صفحة **نشاء تطبيق**، انقر على السهم المواجه لليمين لعرض مزيد من خيارات الاتصال.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-124">In the **Create an app** page, click the right facing arrow to show more connection options.</span></span> 
4.  <span data-ttu-id="ec3a7-125">انقر على **اتصال جديد.**</span><span class="sxs-lookup"><span data-stu-id="ec3a7-125">Click **New connection.**</span></span> 
5.  <span data-ttu-id="ec3a7-126">حدد خيار **Dynamics 365 for Fin & Ops**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-126">Select the **Dynamics 365 for Fin & Ops** option.</span></span>
6.  <span data-ttu-id="ec3a7-127">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-127">Select **Create**.</span></span> 
7.  <span data-ttu-id="ec3a7-128">ستحتاج الآن إلى تحديد المثيل (بيئات تطبيقات Finance and Operations) والجدول (كيان بيانات) الذي تريد الاتصال به.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-128">You will now need to select the instance (Finance and Operations apps environments) and Table (data entity) that you want to connect to.</span></span> <span data-ttu-id="ec3a7-129">تحتاج إلى التأكد من أنك مستخدم مسؤول للبيئة التي تحددها وأن لديك أذونات للوصول إلى الجدول (كيان البيانات) الذي تحدده.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-129">You need to ensure you are an admin user for the environment you select and you have permissions to access the table (data entity) you are selecting.</span></span> 

     <span data-ttu-id="ec3a7-130">[![تعرض لقطة شاشة Power Apps تحديد مصادر البيانات في الشريط وتوصيل بيانات تطبيقات Finance and Operations ](../media/power-apps.png)](../media/power-apps.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec3a7-130">[![This Power Apps screenshot shows selecting Data sources in the ribbon and connecting to Finance and Operations apps data.](../media/power-apps.png)](../media/power-apps.png#lightbox)</span></span>
  


   
