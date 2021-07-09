---
ms.openlocfilehash: 5b955253ef0791e84dc6472808ea22b94ee89360
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070863"
---
<span data-ttu-id="12b52-101">على الرغم من قيام معظم العملاء بدفع فواتيرهم في الموعد، فإنه يجب أن تكون قادراً على معالجة الفواتير التي لم يتم دفعها بحلول تاريخ الاستحقاق.</span><span class="sxs-lookup"><span data-stu-id="12b52-101">Although most customers pay their invoices on time, you need to be able to process invoices that are not paid by their due date.</span></span>

<span data-ttu-id="12b52-102">يشرح هذا الموضوع كيفية إدارة العملاء المتخلفين عن السداد عن طريق تكوين الوحدة النمطية لعمليات التحصيل والائتمان في Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="12b52-102">This topic explains how to manage delinquent customers by configuring the Credit and collections module in Dynamics 365 Finance.</span></span> <span data-ttu-id="12b52-103">لاستخدام الوحدة النمطية لعمليات التحصيل والائتمان، يجب عليك بالفعل إكمال تكوين الوحدة النمطية للحسابات المدينة.</span><span class="sxs-lookup"><span data-stu-id="12b52-103">To use the Credit and collections module, you should already have completed the configuration of accounts receivable module.</span></span>

<span data-ttu-id="12b52-104">سوف تتعرف في هذه الوحدة على كيفية:</span><span class="sxs-lookup"><span data-stu-id="12b52-104">In this module, you will learn how to:</span></span>

- <span data-ttu-id="12b52-105">تكوين مكونات عمليات التحصيل والائتمان.</span><span class="sxs-lookup"><span data-stu-id="12b52-105">Configure credit and collections components.</span></span>
- <span data-ttu-id="12b52-106">تكوين تقارير التقادم وأوعيه العملاء ووكلاء التحصيلات وتعريفات فترات التقادم.</span><span class="sxs-lookup"><span data-stu-id="12b52-106">Configure aging reports, customer pools, collection agents, and aging period definitions.</span></span>
- <span data-ttu-id="12b52-107">إعداد الفوائد وإدارتها.</span><span class="sxs-lookup"><span data-stu-id="12b52-107">Set up and manage interests.</span></span>
- <span data-ttu-id="12b52-108">إعداد خطابات التحصيل وإدارتها.</span><span class="sxs-lookup"><span data-stu-id="12b52-108">Set up and manage collection letters.</span></span>
 
## <a name="terminology"></a><span data-ttu-id="12b52-109">المصطلحات</span><span class="sxs-lookup"><span data-stu-id="12b52-109">Terminology</span></span> 

<span data-ttu-id="12b52-110">تقدم القائمة التالية عدة بنود ومفاهيم يتم تضمينها في إدارة عمليات التحصيل والائتمان.</span><span class="sxs-lookup"><span data-stu-id="12b52-110">The following list introduces several terms and concepts that are included in the credit and collections management process.</span></span>

- <span data-ttu-id="12b52-111">**وكيل التحصيل** – شخص يعمل مع العملاء للتأكد من تحصيل المدفوعات في الوقت المناسب.</span><span class="sxs-lookup"><span data-stu-id="12b52-111">**Collection agent** – A person who works with customers to make sure that payments are collected in a timely manner.</span></span>
- <span data-ttu-id="12b52-112">**النشاط** – تمثل الأنشطة الإجراءات التي قد يتخذها وكيل التحصيل.</span><span class="sxs-lookup"><span data-stu-id="12b52-112">**Activity** – Activities represent actions that a collection agent may take.</span></span> <span data-ttu-id="12b52-113">وهذه الأنشطة هي نفسها الأنواع المستخدمة في الوحدة النمطية المبيعات والتسويق.</span><span class="sxs-lookup"><span data-stu-id="12b52-113">These activities are the same types that are used in the Sales and Marketing module.</span></span>
    - <span data-ttu-id="12b52-114">**المهمة** – الإجراء الذي يجب القيام به في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="12b52-114">**Task** – An action that must be done in the future.</span></span>
    - <span data-ttu-id="12b52-115">**الإجراء** – إجراء تم إكماله.</span><span class="sxs-lookup"><span data-stu-id="12b52-115">**Action** – An action that was completed.</span></span>
    - <span data-ttu-id="12b52-116">**الموعد** – موعد في المستقبل لم يتم إكماله.</span><span class="sxs-lookup"><span data-stu-id="12b52-116">**Appointment** – An appointment in the future that is not completed.</span></span>
    - <span data-ttu-id="12b52-117">**الحدث** – حدث قد تم بالفعل.</span><span class="sxs-lookup"><span data-stu-id="12b52-117">**Event** – An event that has already occurred.</span></span>
- <span data-ttu-id="12b52-118">**وعاء العملاء** – استعلام يعرّف مجموعة من العملاء الذين سيتم عرضهم وإدارتهم.</span><span class="sxs-lookup"><span data-stu-id="12b52-118">**Customer pool** – A query that defines a group of customers who will be displayed and managed.</span></span>
- <span data-ttu-id="12b52-119">**لقطة التأخر** – حساب أرصدة المتقادمة لمجموعة من العملاء في نقطة زمنية.</span><span class="sxs-lookup"><span data-stu-id="12b52-119">**Aging snapshot** – A calculation of the aged balances for a group of customers at a point in time.</span></span>
- <span data-ttu-id="12b52-120">**تعريف فترة التأخر** - تتقادم حركات العميل المفتوحة عادةً استناداً إلى عدد الأيام المتأخرة عن تاريخ الاستحقاق.</span><span class="sxs-lookup"><span data-stu-id="12b52-120">**Aging period definition** – Open customer transactions are typically aged based on the number of days that they are overdue.</span></span> <span data-ttu-id="12b52-121">يمثل نطاقاً من أيام التقادم فترة.</span><span class="sxs-lookup"><span data-stu-id="12b52-121">A range of aging days represents a period.</span></span> <span data-ttu-id="12b52-122">يمكن استخدام العديد من فترات التأخر لفهم توزيع الحركات المتأخرة بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="12b52-122">Several aging periods can be used to better understand the distribution of overdue transactions.</span></span>

