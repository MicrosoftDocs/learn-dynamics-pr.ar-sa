---
ms.openlocfilehash: 7f11f3fcc10e53773eb0e7b82e1fea1fab1635d5
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070206"
---
<span data-ttu-id="f5226-101">يمكنك ضبط تكرار تحميل المعاملة (الوظيفة P) من القنوات بشكل متكرر بحيث تظهر الحركات من القنوات في الوقت الحقيقي تقريباً.</span><span class="sxs-lookup"><span data-stu-id="f5226-101">You can set the recurrence for transaction upload (the P-job) from the channels so frequently that transactions from the channels appear near real-time.</span></span> <span data-ttu-id="f5226-102">ومع ذلك، عندما تكون الحركات في Commerce Headquarters‏ (HQ)، لن يتحقق المخزون والبيانات المالية.</span><span class="sxs-lookup"><span data-stu-id="f5226-102">However, when the transactions are in Commerce Headquarters (HQ), the inventory and financials will not be realized.</span></span> <span data-ttu-id="f5226-103">قد تحدث مشكلات أيضاً في البيانات التي لم يتم تحديدها بعد.</span><span class="sxs-lookup"><span data-stu-id="f5226-103">Issues might also occur in the data that have yet to be identified.</span></span>

<span data-ttu-id="f5226-104">عندما تكون الحركات في النظام، يمكنك استخدام بديل لترحيل كشف حساب نهاية اليوم الموضح سابقاً.</span><span class="sxs-lookup"><span data-stu-id="f5226-104">When the transactions are in the system, you can use an alternative to the previously described end of day statement posting.</span></span> <span data-ttu-id="f5226-105">باستخدام ميزة تسمى **الترحيل القائم على الخلاصة النقطية**، يمكنك تقسيم عمليات نشر البيان الفردي إلى عبارتين:</span><span class="sxs-lookup"><span data-stu-id="f5226-105">By using a feature named **Trickle feed-based posting**, you can split the single statement posting processes into two statements:</span></span> 

- <span data-ttu-id="f5226-106">تعاملي</span><span class="sxs-lookup"><span data-stu-id="f5226-106">Transactional</span></span>
- <span data-ttu-id="f5226-107">مالي</span><span class="sxs-lookup"><span data-stu-id="f5226-107">Financial</span></span>

<span data-ttu-id="f5226-108">ستنشئ عملية كشف الحركات (المستندة إلى التغذية المستمرة) أوامر المبيعات والفواتير والمدفوعات على مدار اليوم.</span><span class="sxs-lookup"><span data-stu-id="f5226-108">The transactional statement process (trickle feed-based) will create sales orders, invoices, and payments throughout the day.</span></span> <span data-ttu-id="f5226-109">تتيح هذه العملية الاعتراف بالإيرادات والمدفوعات ليتم تحقيقها عند إجراء الحركات، بدلاً من ترحيل كشف الحساب في نهاية اليوم.</span><span class="sxs-lookup"><span data-stu-id="f5226-109">This process allows the recognition of revenue and payments to be realized as the transactions are brought in, as opposed to an end of day statement posting.</span></span> 

<span data-ttu-id="f5226-110">تدعم عملية القوائم المالية طريقة الإقفال **التحول**.</span><span class="sxs-lookup"><span data-stu-id="f5226-110">The financial statement process supports the **Shift** closing method.</span></span> <span data-ttu-id="f5226-111">تعالج هذه العملية التسوية المالية وتنشئ دفاتر يومية لمبالغ التباين بين المبالغ المحسوبة والمعاملات لمدفوعات نوع عطاء المتجر وحركات إدارة النقد الأخرى.</span><span class="sxs-lookup"><span data-stu-id="f5226-111">This process handles financial reconciliation and creates journals for the discrepancy amounts between counted and transactional amounts for the store tender type payments and the other cash management transactions.</span></span>

<span data-ttu-id="f5226-112">تنشئ العملية أوامر المبيعات وفواتير المبيعات ودفاتر يومية الدفع والخصم وحركات مصروفات الدخل.</span><span class="sxs-lookup"><span data-stu-id="f5226-112">The process creates sales orders, sales invoices, payment and discount journals, and income expense transactions.</span></span> <span data-ttu-id="f5226-113">لتحقيق رؤية في الوقت الفعلي تقريباً، يجب تشغيل المعاملة بعد تكرار تحميل المعاملة (وظيفة P) للقنوات.</span><span class="sxs-lookup"><span data-stu-id="f5226-113">To achieve near real-time visibility, the transaction should be run after the recurrence for transaction upload (P-job) for the channels.</span></span> <span data-ttu-id="f5226-114">ليست هناك حاجة لوظيفة دُفعة **ترحيل المخزون**.</span><span class="sxs-lookup"><span data-stu-id="f5226-114">The **Post inventory** batch job is not needed.</span></span> 


