---
ms.openlocfilehash: 5ff3e789dc6e87231d4657e83ba9e1aef8ae1c06
ms.sourcegitcommit: c30d04e437514a1b7fe1d143dc8771662953312c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/03/2021
ms.locfileid: "6071025"
---
<span data-ttu-id="99435-101">من أجل التحقق من معالجة فواتير المورّد والتحكم فيها وتسهيل عملية الترحيل، توجد ميزات في "الحسابات الدائنة" يتم وضعها لتزويد المستخدمين بالأدوات المطلوبة لإدارة هذه العملية:</span><span class="sxs-lookup"><span data-stu-id="99435-101">In order to verify and control the processing of vendor invoices and to facilitate the posting process, there are features in Accounts payable that are in place to provide users with the tools to manage this process:</span></span>

- <span data-ttu-id="99435-102">يجب أن تكون إجماليات فاتورة المورد مطابقة للإجمالي المسجل قبل أن يتم إرسالها إلى سير العمل</span><span class="sxs-lookup"><span data-stu-id="99435-102">vendor invoice totals must match the registered total before it can be submitted to workflow</span></span>
- <span data-ttu-id="99435-103">خطوة في سير عمل فاتورة المورد لترحيل الفاتورة بمجرد أن تمر بمعايير سير العمل</span><span class="sxs-lookup"><span data-stu-id="99435-103">a step in the Vendor invoice workflow to post the invoice once it passes workflow criteria</span></span> 


## <a name="prohibit-submission-to-workflow-when-the-invoice-total-and-registered-invoice-total-are-not-equal"></a><span data-ttu-id="99435-104">منع الإرسال إلى سير العمل عند عدم تساوي إجمالي الفاتورة وإجمالي الفاتورة المسجلة</span><span class="sxs-lookup"><span data-stu-id="99435-104">Prohibit submission to workflow when the invoice total and registered invoice total are not equal</span></span>

<span data-ttu-id="99435-105">عند استخدام هذه الميزة، إذا تم تنشيط **سير عمل فاتورة المورد**، فإنه يتعذر إرسال الفاتورة إلى سير العمل إذا كانت الكمية المسجلة تختلف عن الكمية التي تمت فوترتها.</span><span class="sxs-lookup"><span data-stu-id="99435-105">With this feature, if you have the **Vendor invoice workflow** activated, an invoice cannot be submitted to workflow if the registered quantity differs from the invoiced quantity.</span></span> <span data-ttu-id="99435-106">وإذا كانت هذه هي الحالة، فسيتلقى الشخص الذي يقوم بإدخال الفاتورة رسالة خطأ تفيد بأنه يتعذر إرسال الفاتورة إلى سير العمل.</span><span class="sxs-lookup"><span data-stu-id="99435-106">If that is the case, the person who is entering the invoice will receive an error message that the invoice cannot be submitted to workflow.</span></span> 

<span data-ttu-id="99435-107">وفيما يأتي فيديو حول كيفية نجاح هذه العملية:</span><span class="sxs-lookup"><span data-stu-id="99435-107">Here is a video of how this process will work:</span></span>



> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4tFV3]
## <a name="vendor-invoice-batch-posting"></a><span data-ttu-id="99435-108">ترحيل دفعة فاتورة المورد</span><span class="sxs-lookup"><span data-stu-id="99435-108">Vendor invoice batch posting</span></span>
 
<span data-ttu-id="99435-109">لتقليل حالات التأخير بين فاتورة المورد الذي تتم الموافقة عليها في سير العمل وترحيل تلك الفاتورة، يمكنك اختيار إضافة الفاتورة إلى دُفعة لترحيلها في سير العمل نفسه.</span><span class="sxs-lookup"><span data-stu-id="99435-109">In order to minimize delays between a vendor invoice being approved in workflow and the posting of that invoice, you can choose to have the invoice be added to a batch for posting in the workflow itself.</span></span> 

<span data-ttu-id="99435-110">في لقطة الشاشة أدناه، يمكنك رؤية "سير عمل فاتورة المورد" مع إضافة هذه المهمة:</span><span class="sxs-lookup"><span data-stu-id="99435-110">In the screenshot below, you can see a Vendor invoice workflow with this task added:</span></span>

<span data-ttu-id="99435-111">**الحسابات الدائنة > الإعداد > سير عمل الحسابات الدائنة**</span><span class="sxs-lookup"><span data-stu-id="99435-111">**Accounts payable > Setup > Accounts payable workflow**</span></span>


![لقطة شاشة لسير عمل فاتورة المورد في Dynamics 365 Finance.](../media/vendor-invoice-workflow-ssm.png) 

<span data-ttu-id="99435-113">في لقطة الشاشة هذه، يمكنك عرض محفوظات سير العمل وعملية الترحيل التي حدثت.</span><span class="sxs-lookup"><span data-stu-id="99435-113">In this screenshot, you can see the workflow history and the posting process that has taken place.</span></span> 

<span data-ttu-id="99435-114">[ ![لقطة شاشة لمحفوظات سير العمل وعملية الترحيل في Dynamics 365 Finance.](../media/workflow-history-ssm.png) ](../media/workflow-history-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="99435-114">[ ![Screenshot of the workflow history and posting process in Dynamics 365 Finance.](../media/workflow-history-ssm.png) ](../media/workflow-history-ssm.png#lightbox)</span></span>

<span data-ttu-id="99435-115">وأخيراً، بعد ترحيل الدُفعة، تظهر الفاتورة في الصفحة **فواتير المورّد المفتوحة**:</span><span class="sxs-lookup"><span data-stu-id="99435-115">And then finally, after the batch posting, the invoice appears in the **Open vendor invoices** page:</span></span>

<span data-ttu-id="99435-116">**الحسابات الدائنة > الفواتير > فواتير المورّد المفتوحة**</span><span class="sxs-lookup"><span data-stu-id="99435-116">**Accounts payable > Invoices > Open vendor invoices**</span></span>

<span data-ttu-id="99435-117">[ ![لقطة شاشة للصفحة "الفواتير المفتوحة" مع سهم واحد في Dynamics 365 Finance.](../media/open-invoices-ssm.png) ](../media/open-invoices-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="99435-117">[ ![Screenshot of the Open invoices page with one row in Dynamics 365 Finance.](../media/open-invoices-ssm.png) ](../media/open-invoices-ssm.png#lightbox)</span></span>

   
## <a name="update-the-invoice-quantities-to-match-product-receipt-quantities-in-workflow"></a><span data-ttu-id="99435-118">تحديث كميات الفواتير لمطابقة كميات إيصال المنتج في سير العمل</span><span class="sxs-lookup"><span data-stu-id="99435-118">Update the invoice quantities to match product receipt quantities in workflow</span></span>

<span data-ttu-id="99435-119">تتطلب بعض عمليات الأعمال استلام جميع البضائع والخدمات من المورد قبل إمكانية إنشاء فاتورة.</span><span class="sxs-lookup"><span data-stu-id="99435-119">Some business processes require that all goods and services are received from a vendor before an invoice can be created.</span></span> <span data-ttu-id="99435-120">وللقيام بذلك، يوجد خيار تشغيل ميزة **تحديث كميات الفواتير لمطابقة كميات إيصال المنتج في سير العمل** الموجودة في مساحة العمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="99435-120">To accomplish this, there is the option to turn on the **Update the invoice quantities to match product receipt quantities in the workflow** feature in the **Feature management** workspace.</span></span> 

<span data-ttu-id="99435-121">وتتيح هذه الميزة للمستخدمين المرونة في تحديث كمية الفاتورة داخل عملية سير العمل، بدلاً من استلام خطأ سير العمل.</span><span class="sxs-lookup"><span data-stu-id="99435-121">This feature enables users the flexibility to update the invoice quantity within the workflow process, rather than receiving a workflow error.</span></span> <span data-ttu-id="99435-122">وعند طرح خطأ ما، فإنه يتطلب من المستخدم تحديث الكمية المستلمة، ثم بدء عملية الفاتورة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="99435-122">When an error is thrown, it requires the user to update the received quantity, then begin the invoice process over.</span></span> <span data-ttu-id="99435-123">وتعمل هذه الميزة على منع حدوث أخطاء الترحيل وإهدار وقت المستخدم وجهده.</span><span class="sxs-lookup"><span data-stu-id="99435-123">This feature prevents posting errors and the user's wasted time and effort.</span></span>

<span data-ttu-id="99435-124">لمعرفة المزيد عن الإعداد والتكوين المطلوب لهذه الميزة، راجع [تسجيل فاتورة المورد ومطابقتها بالكمية المستلمة](https://docs.microsoft.com/dynamics365/finance/accounts-payable/tasks/record-vendor-invoice-match-against-received-quantity/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="99435-124">To learn more about the setup and configuration that is required for this feature, see [Record vendor invoice and match against received quantity](https://docs.microsoft.com/dynamics365/finance/accounts-payable/tasks/record-vendor-invoice-match-against-received-quantity/?azure-portal=true).</span></span>

