---
ms.openlocfilehash: 80648dafc51ffccec3559ed5c7b669438b1be701
ms.sourcegitcommit: 45337c216dae17eda3fd77996e054b20515eb8dc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "6072102"
---
<span data-ttu-id="b83e8-101">هناك أداة أخرى يمكن للمطورين استخدامها لاختبار الأداء وتشخيص مشكلات الأداء وهي SQL Profiler.</span><span class="sxs-lookup"><span data-stu-id="b83e8-101">Another tool developers can use to test performance and diagnose performance issues is the SQL Profiler.</span></span> <span data-ttu-id="b83e8-102">يمكنك الوصول إلى أداة Profiler من خلال SQL Server Management Studio.</span><span class="sxs-lookup"><span data-stu-id="b83e8-102">You access the Profiler through the SQL Server management studio.</span></span> <span data-ttu-id="b83e8-103">يمكنك من هنا استغلال إمكانيات التتبع من جانب الخادم لأداة SQL Server Profiler لتصدير تعريف تتبع يمكنك استخدامه لإنشاء مجموعة تستخدم نوع مُجمع Generic SQL Trace.</span><span class="sxs-lookup"><span data-stu-id="b83e8-103">Here you can exploit the server-side trace capabilities of the SQL Server Profiler to export a trace definition that you can use to create a collection that uses the Generic SQL Trace collector type.</span></span> 
> [!NOTE]
> <span data-ttu-id="b83e8-104">ولا يمكن استخدام هذه الأداة إلا على مثيلات الطبقة 1 من Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b83e8-104">This tool can only be used on tier 1 Dynamics 365 instances</span></span>

<span data-ttu-id="b83e8-105">هناك العديد من الأسباب التي تجعلك ترغب في استخدام أداة SQL Profiler.</span><span class="sxs-lookup"><span data-stu-id="b83e8-105">There are many reasons why you would want to use the SQL Profiler.</span></span> <span data-ttu-id="b83e8-106">على سبيل المثال، قد تحتاج إلى رؤية جميع الاستعلامات طويلة المدى على نظام خادم SQL، وليس فقط الاستعلامات طويلة المدى في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="b83e8-106">For example, you may need to see all the long-running queries on the SQL server system, not just the long-running queries in Finance and Operations apps.</span></span> 

<span data-ttu-id="b83e8-107">للوصول إلى SQL Profiler واستخدامه، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b83e8-107">To access and use the SQL Profiler, follow these steps:</span></span>

1.  <span data-ttu-id="b83e8-108">في SQL Server Management Studio، افتح **SQL Server Profiler** من قائمة **أدوات**.</span><span class="sxs-lookup"><span data-stu-id="b83e8-108">In SQL Server Management Studio, open **SQL Server Profiler** from the **Tools** menu.</span></span> 
2.  <span data-ttu-id="b83e8-109">الاتصال بقاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="b83e8-109">Connect to the database.</span></span> 
3.  <span data-ttu-id="b83e8-110">في نوافذ **خصائص التتبع**، قم بتسمية التتبع.</span><span class="sxs-lookup"><span data-stu-id="b83e8-110">In the **Trace Properties** windows, name your trace.</span></span> 
4.  <span data-ttu-id="b83e8-111">عندما تحدد كل الخصائص، حدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="b83e8-111">When you have specified all properties, select **Run**.</span></span> 
5.  <span data-ttu-id="b83e8-112">أثناء تشغيل تتبع SQL Profile، يمكنك تنفيذ العملية أو العمليات التي تهمك.</span><span class="sxs-lookup"><span data-stu-id="b83e8-112">While the SQL Profile trace is running, you perform the process or processes that are of concern.</span></span> <span data-ttu-id="b83e8-113">على سبيل المثال، قد يعاني المستخدمون من البطء عند إضافة البيانات إلى SalesTable.</span><span class="sxs-lookup"><span data-stu-id="b83e8-113">For example, users may be experiencing slowness when adding data to the SalesTable.</span></span> <span data-ttu-id="b83e8-114">وفي هذه الحالة، ستطلب من المستخدم أداء المهمة أثناء تشغيل التتبع.</span><span class="sxs-lookup"><span data-stu-id="b83e8-114">In this case, you will ask the user to perform the task, while the trace is running.</span></span> 
6.  <span data-ttu-id="b83e8-115">عند اكتمال العملية، أوقف التتبع من خلال تحديد زر **إيقاف** في القائمة.</span><span class="sxs-lookup"><span data-stu-id="b83e8-115">When the process is complete, stop the trace by selecting the **Stop** button in the menu.</span></span> 
7.  <span data-ttu-id="b83e8-116">يمكنك الآن تحليل التتبع بمراجعة نتائج التتبع.</span><span class="sxs-lookup"><span data-stu-id="b83e8-116">Now you can analyze the trace by reviewing the trace results.</span></span> <span data-ttu-id="b83e8-117">تُظهر لقطة الشاشة التالية كيف يبدو التتبع عند إيقافه.</span><span class="sxs-lookup"><span data-stu-id="b83e8-117">The following screenshot shows what the trace looks like when it is stopped.</span></span>  
    

    <span data-ttu-id="b83e8-118">[![لقطة شاشة لنافذة التتبع الخاص بي عند إيقاف التتبع](../media/my-trace.png)](../media/my-trace.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b83e8-118">[![Screenshot of My Trace window when a trace is stopped](../media/my-trace.png)](../media/my-trace.png#lightbox)</span></span>
