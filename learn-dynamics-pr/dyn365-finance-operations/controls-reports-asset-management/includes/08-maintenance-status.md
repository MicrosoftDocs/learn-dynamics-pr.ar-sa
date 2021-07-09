---
ms.openlocfilehash: a3215833cc5a608becda9001ba695e394ec5ba13
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072289"
---
<span data-ttu-id="e7aa1-101">في إدارة الأصول، يمكنك إجراء عمليات حسابية توفر مراجعة محددة بفترة معينة لطلبات الصيانة الجديدة والنشطة والمكتملة وأوامر العمل وأنشطة وقت تعطل الصيانة.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-101">In Asset Management, you can make calculations that provide a review that is defined by a specific period for new, active, and completed maintenance requests, work orders, and maintenance downtime activities.</span></span> <span data-ttu-id="e7aa1-102">يمكنك أيضاً رؤية عدد تقييمات الحالات المكتملة للفترة نفسها.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-102">You can also see the number of completed condition assessments for the same period.</span></span> 

<span data-ttu-id="e7aa1-103">استخدم العملية الحسابية الآتية للحصول على نظرة عامة حول حمل العمل الخاص بطلبات الصيانة الواردة والمكتملة وأوامر العمل.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-103">Use the following calculation to get an overview of your workload for incoming and completed maintenance requests and work orders.</span></span>

<span data-ttu-id="e7aa1-104">لإجراء عملية حسابية لحالة الصيانة، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="e7aa1-104">To make a maintenance status calculation, follow these steps:</span></span>

1.  <span data-ttu-id="e7aa1-105">انتقل إلى **إدارة الأصول > الاستعلامات > حالة الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-105">Go to **Asset management > Inquiries > Maintenance status**.</span></span>
2.  <span data-ttu-id="e7aa1-106">في مربع حوار **حالة العملية الحسابية**، حدد النطاق الزمني الذي تريد إجراء العملية الحسابية خلاله في الحقلين **تاريخ البدء** و **تاريخ الانتهاء**.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-106">In the **Calculate status** dialog box, select the time range that you want to make the calculation for in the **From date** and **To date** fields.</span></span>
4.  <span data-ttu-id="e7aa1-107">حقل **المستوى** يقوم بتعيين مدى تفاصيل بنود الصيانة التي تريدها لأماكن العمل.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-107">The **Level** field assigns how detailed you want the maintenance lines to be for functional locations.</span></span>
    - <span data-ttu-id="e7aa1-108">**1** = ستتم إضافة جميع المواقع مع بعضها في موقع عمل متعدد المستويات ويتم عرضها في موقع عمل من المستوى الأعلى.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-108">**1** = All locations in a multi-level functional location will be added together and shown in the top-level functional location.</span></span>
    - <span data-ttu-id="e7aa1-109">**0** = سيتم عرض جميع القيم التفصيلية لجميع البنود متعددة المستويات لموقع العمل.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-109">**0** = All detailed values of all multi-level lines of the functional location will be shown.</span></span>
3.  <span data-ttu-id="e7aa1-110">حدد **موافق** لبدء الحساب.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-110">Select **OK** to start the calculation.</span></span>
4.  <span data-ttu-id="e7aa1-111">يسمح لك زر **تجميع حسب** بتحديد مستوى التفاصيل المطلوب.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-111">The **Group by** buttons allow you to define the required detail level.</span></span> <span data-ttu-id="e7aa1-112">يتضمن زر **تجميع حسب** المحدد **تجميع حسب التاريخ** و **تجميع حسب موقع العمل** و **وتجميع حسب الأصل**.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-112">The selected **Group by** buttons include **Group by date**, **Group by functional location**, and **Group by asset**.</span></span> <span data-ttu-id="e7aa1-113">ضمن كل زر، يمكنك اختيار كيفية تحديدها.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-113">Under each button, you can choose how to define them.</span></span> <span data-ttu-id="e7aa1-114">على سبيل المثال، ضمن **تجميع حسب التاريخ**، يمكنك تحديد تجميع حسب **الأسبوع**.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-114">For example, under **Group by date**, you can select to group by **Week**.</span></span>
5.  <span data-ttu-id="e7aa1-115">حدد زر **تحديث** لتحديث العملية الحسابية في كل مرة تقوم فيها بإجراء تغييرات عن طريق تنشيط أو إلغاء تنشيط أزرار **تجميع حسب** أو بإجراء عملية حسابية لفترة جديدة.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-115">Select the **Update** button to update the calculation each time you make changes by activating or deactivating **Group by** buttons or by making a calculation for a new period.</span></span>
6.  <span data-ttu-id="e7aa1-116">حدد **الحالة** إذا كنت تريد إنشاء عملية حسابية لحالة صيانة جديدة.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-116">Select **Status** if you want to create a new maintenance status calculation.</span></span> 



<span data-ttu-id="e7aa1-117">**إدارة الأصول > الاستعلامات > حالة الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-117">**Asset management > Inquiries > Maintenance status**</span></span>
 
<span data-ttu-id="e7aa1-118">[![لقطة شاشة لصفحة "حالة الصيانة".](../media/maintenance-status-ss.png)](../media/maintenance-status-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="e7aa1-118">[![Screenshot of the Maintenance status page.](../media/maintenance-status-ss.png)](../media/maintenance-status-ss.png#lightbox)</span></span>


> [!NOTE]
> <span data-ttu-id="e7aa1-119">النتائج التي يتم عرضها في مساحة **حالة الصيانة** تتضمن فقط طلبات الصيانة وأوامر العمل التي لها بداية فعلية ووقت محدد.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-119">The results that are shown in the **Maintenance status** area include only those maintenance requests and work orders that have an actual start and time assigned.</span></span> <span data-ttu-id="e7aa1-120">قد يكون الحقلين **تاريخ الانتهاء** و **وقت الانتهاء** فارغين.</span><span class="sxs-lookup"><span data-stu-id="e7aa1-120">The **End date** and **End time** fields might be blank.</span></span>