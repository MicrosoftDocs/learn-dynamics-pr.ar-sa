---
ms.openlocfilehash: 0ee05c81fc4b501c9dca25203bfa82488bee0104
ms.sourcegitcommit: 0af0a6f1739b0e2a5ec60989ffbf8aa131de41c3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/08/2021
ms.locfileid: "6072244"
---
<span data-ttu-id="17d82-101">نظراً لأن القدرة الإنتاجية توضح الطلب الموضوع على نظام، يمكنك تشغيل الحساب استناداً إلى المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="17d82-101">Because capacity load shows the demand that is placed on a system, you can run a calculation based on the following information:</span></span>

- <span data-ttu-id="17d82-102">بنود جدول الصيانة</span><span class="sxs-lookup"><span data-stu-id="17d82-102">Maintenance schedule lines</span></span>
- <span data-ttu-id="17d82-103">أوامر العمل التي لم تتم جدولتها بعد</span><span class="sxs-lookup"><span data-stu-id="17d82-103">Work orders that have not yet been scheduled</span></span>
- <span data-ttu-id="17d82-104">أوامر العمل المجدولة</span><span class="sxs-lookup"><span data-stu-id="17d82-104">Scheduled work orders</span></span>

<span data-ttu-id="17d82-105">هناك ثلاث طرق للوصول إلى صفحة **‏‫حساب القدرة الإنتاجية‬**:</span><span class="sxs-lookup"><span data-stu-id="17d82-105">Three ways to access the **Calculate capacity load** page are:</span></span>

- <span data-ttu-id="17d82-106">**إدارة الأصول > الاستعلامات > القدرة الإنتاجية**</span><span class="sxs-lookup"><span data-stu-id="17d82-106">**Asset Management > Inquiries > Capacity load**</span></span>
- <span data-ttu-id="17d82-107">**إدارة الأصول > عام > أوعية أوامر العمل > ‏‫كافة أوعية أوامر العمل / أوعية أوامر العمل النشطة** > تحديد وعاء أمر العمل في القائمة > زر **القدرة الإنتاجية**</span><span class="sxs-lookup"><span data-stu-id="17d82-107">**Asset Management > Common > Work order pools > All work order pools / Active work order pools** > select a work order pool in the list > **Capacity load** button</span></span>
- <span data-ttu-id="17d82-108">**إدارة الأصول > عام > أنشطة وقت تعطل الصيانة > جميع أنشطة وقت تعطل الصيانة / أنشطة وقت تعطل الصيانة النشطة** > تحديد نشاط صيانة من القائمة > زر **القدرة الإنتاجية**.</span><span class="sxs-lookup"><span data-stu-id="17d82-108">**Asset management > Common > Maintenance downtime activities > All maintenance downtime activities / Active maintenance downtime activities** > select a maintenance activity from the list > **Capacity load** button.</span></span>

<span data-ttu-id="17d82-109">بعد اتباع المسار الذي تختاره، ‏‫يتم فتح مربع الحوار **‏‫حساب القدرة الإنتاجية‬**.</span><span class="sxs-lookup"><span data-stu-id="17d82-109">After you have followed your path of choice, the **Calculate capacity load** dialog box opens.</span></span>

<span data-ttu-id="17d82-110">[![لقطة شاشة لمربع الحوار "حساب القدرة الإنتاجية".](../media/calculate-capacity-load-ss.png)](../media/calculate-capacity-load-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="17d82-110">[![Screenshot of the Calculate capacity load dialog box.](../media/calculate-capacity-load-ss.png)](../media/calculate-capacity-load-ss.png#lightbox)</span></span>

1.  <span data-ttu-id="17d82-111">أدخل الإطار الزمني لحساب القدرة الإنتاجية في حقلي **تاريخ/وقت البدء** و **تاريخ/وقت الانتهاء**.</span><span class="sxs-lookup"><span data-stu-id="17d82-111">Enter the time frame for the capacity load calculation in the **Start date/time** and **End date/time** fields.</span></span> <span data-ttu-id="17d82-112">على سبيل المثال، إذا كنت تريد التحقق من القدرة الإنتاجية لشهر يناير.</span><span class="sxs-lookup"><span data-stu-id="17d82-112">For example, you want to check the capacity load for the month of January.</span></span> <span data-ttu-id="17d82-113">أدخل **1 يناير 2020** في حقل **‬‏‫تاريخ/وقت البدء** و **31 يناير 2020** في حقل **‬‏‫تاريخ/وقت الانتهاء‬‏‫**.</span><span class="sxs-lookup"><span data-stu-id="17d82-113">Enter **1 January 2020** in the **Start date/time** field and **31 January 2020** in the **End date/time** field.</span></span> 
2.  <span data-ttu-id="17d82-114">بالإضافة إلى الإطار الزمني المحدد، يمكنك إضافة بنود جدول الصيانة ومهام أوامر العمل إلى المعادلة عن طريق تحديد **نعم** على أزرار التبديل الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="17d82-114">In addition to a specific time frame, you can add maintenance schedule lines and work order jobs to the equation by selecting **Yes** on their respective toggle buttons.</span></span>
3.  <span data-ttu-id="17d82-115">يتيح لك حقل **المستوى** تحديد مستوى التفاصيل لبنود القدرة الإنتاجية حسب موقع العمل.</span><span class="sxs-lookup"><span data-stu-id="17d82-115">The **Level** field lets you define the level of detail for capacity load lines by functional location.</span></span> <span data-ttu-id="17d82-116">على سبيل المثال، ضع في اعتبارك سيناريو يكون فيه لديك موقع عمل متعدد المستويات.</span><span class="sxs-lookup"><span data-stu-id="17d82-116">For example, consider the scenario where you have a multi-level functional location.</span></span> <span data-ttu-id="17d82-117">إذا قمت بإدخال **1** في الحقل، فستظهر بنود جدول الصيانة وأوامر العمل لموقع العمل هذا في المستوى الأعلى.</span><span class="sxs-lookup"><span data-stu-id="17d82-117">If you enter **1** in the field, then the maintenance schedule lines and work orders for that functional location will appear at the top level.</span></span> <span data-ttu-id="17d82-118">إذا قمت بإدخال **0** في الحقل، فستظهر جميع بنود جدول الصيانة وأوامر العمل لجميع مواقع العمل.</span><span class="sxs-lookup"><span data-stu-id="17d82-118">If you enter **0** in the field, you will see all maintenance schedule lines and work orders for all functional locations.</span></span>
4.  <span data-ttu-id="17d82-119">عند الانتهاء، حدد **موافق** لبدء الحساب وسيظهر التقرير.</span><span class="sxs-lookup"><span data-stu-id="17d82-119">When you are done, select **OK** to start the calculation and the report will appear.</span></span>
5.  <span data-ttu-id="17d82-120">في علامة التبويب **القدرة الإنتاجية**، يمكنك تحديد خيارات متنوعة لإضافة مزيد من المعلومات إلى التقرير.</span><span class="sxs-lookup"><span data-stu-id="17d82-120">On the **Capacity load** tab, you can select various options to add more information to the report.</span></span> <span data-ttu-id="17d82-121">يمكنك إكمال هذه المهمة حسب الأصل، ونوع الأصل، وموقع العمل، وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="17d82-121">You can complete this task by asset, asset type, functional location, and so on.</span></span>

<span data-ttu-id="17d82-122">‏‫تعرض الصورة التالية تقرير القدرة الإنتاجية مع توضيح بعض خيارات التجميع.</span><span class="sxs-lookup"><span data-stu-id="17d82-122">The following image shows the capacity load report with some of the grouping options highlighted.</span></span>

<span data-ttu-id="17d82-123">**إدارة الأصول > الاستعلامات > القدرة الإنتاجية**</span><span class="sxs-lookup"><span data-stu-id="17d82-123">**Asset Management > Inquiries > Capacity load**</span></span>

<span data-ttu-id="17d82-124">[![لقطة شاشة لتقرير القدرة الإنتاجية مع توضيح خيارات التجميع.](../media/capacity-load-planning2-ssm.png)](../media/capacity-load-planning2-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="17d82-124">[![Screenshot of a Capacity load report with grouping options highlighted.](../media/capacity-load-planning2-ssm.png)](../media/capacity-load-planning2-ssm.png#lightbox)</span></span>  


> [!NOTE]
> <span data-ttu-id="17d82-125">إذا كان تركيزك مقتصراً تماماً على أوامر العمل المجدولة‬، فانتقل إلى **حساب القدرة الإنتاجية** في أوامر العمل المجدولة.</span><span class="sxs-lookup"><span data-stu-id="17d82-125">If your focus is strictly related to scheduled work orders, go to **Calculate capacity load** on scheduled work orders.</span></span>

<span data-ttu-id="17d82-126">يوضح الفيديو التالي كيفية إعداد حساب القدرة الإنتاجية.</span><span class="sxs-lookup"><span data-stu-id="17d82-126">The following video describes how to set up the capacity calculation.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4oJXG]


