---
ms.openlocfilehash: e25da7e724c96fde78f2e673def72f261eca425b
ms.sourcegitcommit: 3b7930e46f1a732939d8d75f99df7bf1f7ccc2ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "6072367"
---
<span data-ttu-id="1b211-101">بعد الانتهاء من إدخال المعلومات الخاصة بالإيجار، يجب إنشاء جدول الإيجار.</span><span class="sxs-lookup"><span data-stu-id="1b211-101">After you've finished entering information for the lease, you need to generate the lease schedule.</span></span> <span data-ttu-id="1b211-102">عند إنشاء الجدول، ستقوم الجداول بتنفيذ ثلاثة إجراءات:</span><span class="sxs-lookup"><span data-stu-id="1b211-102">When you generate the schedule, the schedules will implement three actions:</span></span> 

- <span data-ttu-id="1b211-103">إنشاء دفاتر استناداً إلى مجموعة الإيجار.</span><span class="sxs-lookup"><span data-stu-id="1b211-103">Create books based on the lease group.</span></span>
- <span data-ttu-id="1b211-104">إنشاء الجداول (المدفوعات والالتزامات والإهلاك والمصروفات).</span><span class="sxs-lookup"><span data-stu-id="1b211-104">Create schedules (payment, liability, depreciation, and expense).</span></span>
- <span data-ttu-id="1b211-105">حساب أصول حق الاستخدام الأولية والالتزامات الأولية.</span><span class="sxs-lookup"><span data-stu-id="1b211-105">Calculate initial right-of-use assets and initial liabilities.</span></span> 

<span data-ttu-id="1b211-106">على سبيل المثال، عند حساب فترة الإيجار بالأشهر، يقوم النظام بالبحث عن الفرق بين تاريخ البدء وتاريخ الانتهاء لسطر جدول دفعات معين.</span><span class="sxs-lookup"><span data-stu-id="1b211-106">For example, when calculating the lease term in months, the system finds the difference between the start date and the end date for a specific payment schedule line.</span></span> <span data-ttu-id="1b211-107">ثم ينتقل إلى سطر جدول الدفعات التالي ويبحث عن الفرق مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="1b211-107">It then moves to the next payment schedule line and finds the difference again.</span></span> <span data-ttu-id="1b211-108">وفي النهاية، يقوم النظام بجمع كافة المبالغ لتحديد فترة الإيجار بالأشهر.</span><span class="sxs-lookup"><span data-stu-id="1b211-108">Finally, the system sums all amounts to determine the lease term in months.</span></span>

<span data-ttu-id="1b211-109">لإنشاء جدول إيجار، انتقل إلى صفحة **ملخص الإيجار** وحدد **إنشاء جداول**.</span><span class="sxs-lookup"><span data-stu-id="1b211-109">To create a lease schedule, go to the **Lease summary** page and select **Create schedules**.</span></span>


 
![لقطة شاشة لصفحة "إنشاء الجداول".](../media/create-schedules.png)

<span data-ttu-id="1b211-111">سوف تتلقى رسالة بأنه تم إنشاء جدول دفعات الإيجار وجدول إطفاء الدين للالتزام وجدول الإهلاك وجدول المصروفات للإيجار.</span><span class="sxs-lookup"><span data-stu-id="1b211-111">You will receive a message that the Payment schedule, Liability amortization schedule, Depreciation schedule, and Expense schedule are created for the lease.</span></span>

<span data-ttu-id="1b211-112">اتبع الخطوات الآتية لعرض جداول الإيجار التي تم إنشاؤها وتأكيدها:</span><span class="sxs-lookup"><span data-stu-id="1b211-112">Follow these steps to view and confirm the generated lease schedules:</span></span>

1.  <span data-ttu-id="1b211-113">حدد علامة التبويب **الدفاتر** ثم حدد الدفتر الذي قمت بإنشاء جدول له.</span><span class="sxs-lookup"><span data-stu-id="1b211-113">Select the **Books** tab and then select the book that you created a schedule for.</span></span>
2.  <span data-ttu-id="1b211-114">في جزء الإجراءات، ضمن **الجداول**، حدد **جداول الدفعات**.</span><span class="sxs-lookup"><span data-stu-id="1b211-114">In the Action Pane, under **Schedules**, select **Payment schedules**.</span></span>
3.  <span data-ttu-id="1b211-115">إذا كان يلزم إجراء تغييرات، فلا يزال بإمكانك تغيير كل مبلغ دفعة ودفعة متغيرة.</span><span class="sxs-lookup"><span data-stu-id="1b211-115">If changes are required, you can still change each payment amount and variable payment.</span></span> <span data-ttu-id="1b211-116">يتم حساب التزامات الإيجار استناداً إلى جدول الدفعات المعدل.</span><span class="sxs-lookup"><span data-stu-id="1b211-116">The lease liability is calculated based on the modified payment schedule.</span></span>
4.  <span data-ttu-id="1b211-117">بعد مراجعة الجدول، حدد **تأكيد الجدول**.</span><span class="sxs-lookup"><span data-stu-id="1b211-117">After you have reviewed the schedule, select **Confirm schedule**.</span></span> <span data-ttu-id="1b211-118">بعد تأكيد الجدول، يصبح عقد الإيجار غير متوفر للتحرير.</span><span class="sxs-lookup"><span data-stu-id="1b211-118">After the schedule is confirmed, the lease is no longer available for editing.</span></span>

<span data-ttu-id="1b211-119">في جزء **الجدول**، إذا كنت تريد عرض مصروفات الفائدة المحسوبة، فحدد صفحة **جدول إطفاء الدين للالتزام**.</span><span class="sxs-lookup"><span data-stu-id="1b211-119">In the **Schedule** pane, if you want to view the calculated interest expenses, select the **Liability amortization schedule** page.</span></span> <span data-ttu-id="1b211-120">لعرض الإهلاك الثابت المحسوب، افتح الصفحة **جدول إهلاك الأصول**.</span><span class="sxs-lookup"><span data-stu-id="1b211-120">To view calculated straight-line depreciation, open the **Asset depreciation schedule** page.</span></span> 

