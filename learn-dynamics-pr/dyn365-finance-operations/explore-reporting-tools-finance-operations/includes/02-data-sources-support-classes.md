---
ms.openlocfilehash: 46d73e22d6123e356c91925c71ef36c1801399cb
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072302"
---
<span data-ttu-id="16c1b-101">تستخدم التقارير مصادر البيانات لسحب البيانات.</span><span class="sxs-lookup"><span data-stu-id="16c1b-101">Reports use data sources to pull data.</span></span> <span data-ttu-id="16c1b-102">SQL Server Reporting Services (SSRS) وPower BI هما أداتان لإعداد التقارير تستخدمان مصادر البيانات.</span><span class="sxs-lookup"><span data-stu-id="16c1b-102">SQL Server Reporting Services (SSRS) and Power BI are two reporting tools that use data sources.</span></span> <span data-ttu-id="16c1b-103">تغطي هذه الوحدة إنشاء مصادر البيانات وتعديلها لأداتي إعداد التقارير هاتين.</span><span class="sxs-lookup"><span data-stu-id="16c1b-103">This unit covers the creation and modification of data sources for these reporting tools.</span></span>

<span data-ttu-id="16c1b-104">تستخدم SSRS مجموعات البيانات التي يتم تعريفها بواسطة مصدر البيانات.</span><span class="sxs-lookup"><span data-stu-id="16c1b-104">SSRS uses data sets that are defined by a data source.</span></span> <span data-ttu-id="16c1b-105">يمكنك تعيين مصدر بيانات لتقرير SSRS من خلال Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="16c1b-105">You can assign a data source to an SSRS report through Visual Studio.</span></span> 


![رسم تخطيطي لمصادر البيانات التي يمكن تعيينها إلى تقرير S S R S.](../media/data-sources.png)

<span data-ttu-id="16c1b-107">في معلمات التقرير، يمكنك تحديد مصدر البيانات لمجموعة البيانات ونوع مصدر البيانات.</span><span class="sxs-lookup"><span data-stu-id="16c1b-107">In the report parameters, you can select the data source for the data set and the data source type.</span></span> <span data-ttu-id="16c1b-108">يمكن أن يكون نوع مصدر البيانات على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="16c1b-108">The data source type can be the following:</span></span> 

- <span data-ttu-id="16c1b-109">**الاستعلام** - نوع مصدر البيانات الاستعلام يستخدم استعلاماً موجوداً أو استعلاماً جديداً.</span><span class="sxs-lookup"><span data-stu-id="16c1b-109">**Query** - A query data source type uses an existing query or a new query.</span></span>

- <span data-ttu-id="16c1b-110">**منطق الأعمال** – استخدم هذا النوع للحصول على مصدر بيانات بخلاف تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="16c1b-110">**Business logic** – Use this type to get a data source other than Finance and Operations apps.</span></span> 

- <span data-ttu-id="16c1b-111">**فئة موفر بيانات التقارير** – يمكنك استخدام هذا النوع في حالة عدم إمكانية استخدام الاستعلام بمفرده.</span><span class="sxs-lookup"><span data-stu-id="16c1b-111">**Report data provider class** – You can use this type when a query cannot be used alone.</span></span> <span data-ttu-id="16c1b-112">في هذه الحالة، يلزم وجود منطق إضافي لتشغيل التقرير.</span><span class="sxs-lookup"><span data-stu-id="16c1b-112">In this case, additional logic is needed to run the report.</span></span> <span data-ttu-id="16c1b-113">إلى جانب فئة موفر بيانات التقارير (RDP)، يلزم وجود فئة عقد أيضاً لتعريف معلمات التقرير.</span><span class="sxs-lookup"><span data-stu-id="16c1b-113">Along with the RDP class, a contract class is also needed to define the report parameters.</span></span> 

- <span data-ttu-id="16c1b-114">**موفر تعداد** – يمكن استخدام موفر تعداد AX عندما تكون معلمة التقرير من نوع التعداد لتصفية طريقة عرض التقرير.</span><span class="sxs-lookup"><span data-stu-id="16c1b-114">**Enum provider** – An AX enum provider can be used when the report parameter is an Enum type to filter the report view.</span></span>  

<span data-ttu-id="16c1b-115">إذا كنت بحاجة إلى تعديل مصدر بيانات، فستحتاج إلى توسيع الجداول أو فئات موفر بيانات التقارير (RDP) لإجراء التعديلات.</span><span class="sxs-lookup"><span data-stu-id="16c1b-115">If you need to modify a data source, you will need to extend the tables or RDP classes to make modifications.</span></span>

<span data-ttu-id="16c1b-116">يمكن لـ Power BI الاتصال بمصادر البيانات، بدءاً من الملفات، وقواعد البيانات، ومجموعات بيانات Power BI وتدفقات البيانات الخاصة به الأخرى، وقواعد بيانات Azure، والخدمات عبر الإنترنت، ووصولاً إلى عناوين URL على الويب.</span><span class="sxs-lookup"><span data-stu-id="16c1b-116">Power BI can connect to data sources, ranging from files, databases, other Power BI datasets and data flows, Azure databases, online services, and even web URLs.</span></span> 

![رسم تخطيطي لمصادر البيانات التي يمكن لـ Power B I الاتصال بها.](../media/power-bi-data.png)

<span data-ttu-id="16c1b-118">استخدم الإجراء التالي للاتصال بمصدر بيانات لإنشاء تقرير Power BI.</span><span class="sxs-lookup"><span data-stu-id="16c1b-118">Use the following procedure to connect to a data source to create a Power BI report.</span></span>

1.  <span data-ttu-id="16c1b-119">في شريط الأدوات Power BI، حدد الزر **إحضار البيانات**.</span><span class="sxs-lookup"><span data-stu-id="16c1b-119">In the Power BI toolbar, select the **Get Data** button.</span></span> <span data-ttu-id="16c1b-120">يتم عرض مصادر البيانات الأكثر شيوعاً، ولكن يمكنك تحديد المزيد للوصول إلى القائمة بأكملها.</span><span class="sxs-lookup"><span data-stu-id="16c1b-120">The most common data sources are displayed, but you can select more to get access to the entire list.</span></span>

2.  <span data-ttu-id="16c1b-121">بعد تحديد مصدر البيانات، حدد **اتصال**.</span><span class="sxs-lookup"><span data-stu-id="16c1b-121">After you have selected the data source, select **Connect**.</span></span>

3.  <span data-ttu-id="16c1b-122">يتم عرض نافذة اتصال يمكنك من خلالها تحديد اتصال البيانات وإدخال أية بيانات اعتماد مطلوبة.</span><span class="sxs-lookup"><span data-stu-id="16c1b-122">A connection window is displayed where you can specify the data connection and enter any required credentials.</span></span> <span data-ttu-id="16c1b-123">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="16c1b-123">Select **OK**.</span></span>

4.  <span data-ttu-id="16c1b-124">ستظهر صفحة **‏‏المتصفح**.</span><span class="sxs-lookup"><span data-stu-id="16c1b-124">The **Navigator** page will appear.</span></span> <span data-ttu-id="16c1b-125">يمكنك إما تحديد الزر **تحميل** لتحميل جميع البيانات، وإما تحديد **تحرير** لتعديل الاستعلام.</span><span class="sxs-lookup"><span data-stu-id="16c1b-125">You can either select the **Load** button to load all the data, or you can select **Edit** to modify the query.</span></span>

<span data-ttu-id="16c1b-126">عند الانتهاء من هذه الخطوات، سيتم توصيل Power BI بمصدر بيانات يمكنك استخدامه لإنشاء التقارير ومؤثرات عرض البيانات.</span><span class="sxs-lookup"><span data-stu-id="16c1b-126">When you have completed these steps, Power BI will be connected to a data source that you can use to create reports and data visualizations.</span></span>
