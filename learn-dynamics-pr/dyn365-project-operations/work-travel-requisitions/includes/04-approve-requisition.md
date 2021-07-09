---
ms.openlocfilehash: 048c49a197c42e752f3b63ba53703ec8f231029c
ms.sourcegitcommit: 87b2596ffaa2b3239b7034d89fa9c0deeab4212d
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2020
ms.locfileid: "6072805"
---
<span data-ttu-id="0ebe7-101">عند إرسال طلب سفر إلى سير العمل، فستتم إعادة توجيهه بشكل منهجي إلى المعتمِد المحدد استناداً إلى القواعد التي تم تحديدها عند إنشاء سير العمل.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-101">When a travel request is sent to the workflow, it is systematically forwarded to the identified approver based on the rules that were defined when the workflow was created.</span></span>

<span data-ttu-id="0ebe7-102">إذا كنت معتمداً في سير عمل طلب السفر، فسيتم إعلامك عندما يتطلب الطلب انتباهك.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-102">If you are an approver in the travel requisition workflow, you will be notified when a request requires your attention.</span></span> <span data-ttu-id="0ebe7-103">قد تحتوي بعض مهام سير العمل على قرارات مشروطة تم إنشاؤها بناءً على تكوين سير العمل.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-103">Some workflows might have conditional decisions that are created based on the workflow configuration.</span></span> <span data-ttu-id="0ebe7-104">قد يحتوي سير العمل أيضاً على مستويات متعددة من الاعتماد المطلوب.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-104">The workflow might also have various levels of required approval.</span></span> <span data-ttu-id="0ebe7-105">وفي هذه الحالات، عندما يقوم المعتمد الأول باعتماد سير العمل، يتم إرساله إلى المعتمد التالي، وهكذا.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-105">In these cases, when the first approver has approved the workflow, it is then sent to the next approver, and so on.</span></span> <span data-ttu-id="0ebe7-106">إذا قام أي معتمد بإرجاع طلب سفر، فستتم إعادة تشغيل التدفق، وسيحتاج منشئ سير العمل إلى إجراء تصحيحات وفقاً لما ينصح به المعتمِد الذي أبدى الرفض.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-106">If any approver returns a travel requisition, the flow is restarted, and the workflow originator will need to make corrections as advised by the rejecting approver.</span></span> 

<span data-ttu-id="0ebe7-107">يمكن عرض الإعلامات على لوحة المعلومات ضمن **عناصر عمل تم تعيينها إلي**.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-107">Notifications can be viewed on your dashboard under **Work items assigned to me**.</span></span> 

![لقطة شاشة لقسم "عناصر عمل تم تعيينها إلي" في لوحة المعلومات.](../media/work-items-assigned-to-me-ss.png)
 
<span data-ttu-id="0ebe7-109">لاعتماد طلب سفر، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0ebe7-109">To approve a travel requisition, follow these steps:</span></span>

1.  <span data-ttu-id="0ebe7-110">في لوحة المعلومات، حدد ارتباطاً تشعبياً في القسم **عناصر عمل تم تعيينها إلي**.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-110">On your dashboard, select a hyperlink in the **Work items assigned to me** section.</span></span> <span data-ttu-id="0ebe7-111">سيتم فتح صفحة **عناصر عمل تم تعيينها إلي**.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-111">The **Work items assigned to me** page will open.</span></span>
2.  <span data-ttu-id="0ebe7-112">حدد طلب السفر القابل للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-112">Select the applicable travel requisition.</span></span>
3.  <span data-ttu-id="0ebe7-113">عند إتمام المراجعة، حدد **سير العمل**، ثم حدد أحد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="0ebe7-113">When your review is complete, select **Workflow** and then select one of the following options:</span></span>
    - <span data-ttu-id="0ebe7-114">**اعتماد** – يقوم باعتماد طلب السفر بالكامل.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-114">**Approve** – Approves the entire travel requisition.</span></span> 
    - <span data-ttu-id="0ebe7-115">**إرجاع** – إرجاع طلب السفر إلى العامل الذي قدمه.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-115">**Return** – Returns the travel requisition to the worker who submitted it.</span></span> <span data-ttu-id="0ebe7-116">يمكنك تحديد هذا الخيار إذا كانت المعلومات غير مكتملة أو إذا كانت لديك أسئلة حول التقرير.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-116">You would select this option if the information is incomplete or if you have questions about the report.</span></span>
    - <span data-ttu-id="0ebe7-117">**تفويض** – يقوم بتعيين طلب السفر إلى مستخدم آخر للاعتماد.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-117">**Delegate** – Assigns the travel requisition to another user for approval.</span></span> 
    - <span data-ttu-id="0ebe7-118">**عرض السجل** – يفتح صفحة "تفاصيل محفوظات سير العمل"، حيث يمكنك عرض المحفوظات والتفاصيل الخاصة بالطلب في عملية الاعتماد.</span><span class="sxs-lookup"><span data-stu-id="0ebe7-118">**View history** – Opens the Workflow history details page, where you can view the history and details of the requisition in the approval process.</span></span>

<span data-ttu-id="0ebe7-119">[![لقطة شاشة لعملية كيفية اعتماد طلب سفر.](../media/approve-travel-requisition-ss.png)](../media/approve-travel-requisition-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0ebe7-119">[![Screenshot of the process of how to approve a travel requisition.](../media/approve-travel-requisition-ss.png)](../media/approve-travel-requisition-ss.png#lightbox)</span></span>
 

