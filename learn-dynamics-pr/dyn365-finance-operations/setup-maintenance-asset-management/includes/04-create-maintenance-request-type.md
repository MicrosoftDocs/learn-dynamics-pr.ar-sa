---
ms.openlocfilehash: 02d8cafaed805f9a3299117fe6dd211dc5069a62
ms.sourcegitcommit: 7d4cc5f2048fa309552e39da447684b1d06d0772
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/13/2021
ms.locfileid: "6072487"
---
<span data-ttu-id="c7c10-101">تساعد أنواع طلب الصيانة في تحديد طلبات الصيانة وتصنيفها وتصفيتها.</span><span class="sxs-lookup"><span data-stu-id="c7c10-101">Maintenance request types help to define, categorize, and filter maintenance requests.</span></span> <span data-ttu-id="c7c10-102">يمكنك إعداد نوع طلب لتحديد طلب الصيانة الوقائية، مثل تغيير الحزام المجدول بانتظام مقابل طلب تصحيحي، مثل عطل أو إصلاح عطل.</span><span class="sxs-lookup"><span data-stu-id="c7c10-102">You can set up a request type to define a preventive maintenance request such as a regularly-scheduled belt change versus a corrective request such as a breakdown or fault repair.</span></span> <span data-ttu-id="c7c10-103">يمكن بعد ذلك إقران نوع طلب الصيانة بنموذج دورة حياة طلب الصيانة، والذي بدوره يحدد تدفق حالات دورة الحياة التي يمر بها الطلب.</span><span class="sxs-lookup"><span data-stu-id="c7c10-103">A maintenance request type can then be associated to a maintenance request lifecycle model, which in turn defines the flow of the lifecycle states that the request will go through.</span></span> 

## <a name="example"></a><span data-ttu-id="c7c10-104">مثال</span><span class="sxs-lookup"><span data-stu-id="c7c10-104">Example</span></span>
<span data-ttu-id="c7c10-105">قررت مزرعة مونسون للمخللات والمعلبات أنها بحاجة إلى إعداد أنواع الطلبات التالية لمؤسستها: التصنيف، والتفتيش، والصيانة الوقائية، والطلب المرفوض، والملاحظات.</span><span class="sxs-lookup"><span data-stu-id="c7c10-105">Munson’s Pickles and Preserves Farm has determined that they need to set up the following request types for their organization: Breakdown, Inspection, Preventive, Rejected, and Notes.</span></span> <span data-ttu-id="c7c10-106">يبدأ هذا الإجراء بإنشاء نوع طلب "تصنيف".</span><span class="sxs-lookup"><span data-stu-id="c7c10-106">This procedure starts by creating a Breakdown request type.</span></span>

1.  <span data-ttu-id="c7c10-107">انتقل إلى  **إدارة الأصول > الإعداد > طلبات الصيانة > أنواع طلبات الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="c7c10-107">Go to  **Asset Management > Setup > Maintenance requests > Maintenance request types**.</span></span> 
2.  <span data-ttu-id="c7c10-108">حدد **جديد** لإنشاء نوع طلب صيانة جديد.</span><span class="sxs-lookup"><span data-stu-id="c7c10-108">Select **New** to create a new maintenance request type.</span></span>
3.  <span data-ttu-id="c7c10-109">في الحقل **نوع طلب الصيانة** أدخل معرفاً لنوع طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="c7c10-109">In the **Maintenance request type** field, enter an ID for the maintenance request type.</span></span> <span data-ttu-id="c7c10-110">في هذا المثال، أدخل **تصنيف**.</span><span class="sxs-lookup"><span data-stu-id="c7c10-110">In this example, enter **Breakdown**.</span></span> 
4.  <span data-ttu-id="c7c10-111">في الحقل  **الاسم** ، أدخل اسماً وصفياً، مثل **طلب إصلاح الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="c7c10-111">In the  **Name** field, enter a descriptive name such as **Repair maintenance request**.</span></span> 
5.  <span data-ttu-id="c7c10-112">في علامة التبويب السريعة **عام**، في القائمة المنسدلة **نموذج دورة حياة طلب الصيانة**، حدد نموذج دورة حياة طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="c7c10-112">On the **General** FastTab, in the **Maintenance request lifecycle model** drop-down menu, select a maintenance request lifecycle model.</span></span> <span data-ttu-id="c7c10-113">حدد **قيد التقدم**.</span><span class="sxs-lookup"><span data-stu-id="c7c10-113">Select **In Progress**.</span></span>
6.  <span data-ttu-id="c7c10-114">في الحقل **نوع أمر العمل** حدد نوع أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="c7c10-114">In the **Work order type** field, select a work order type.</span></span> <span data-ttu-id="c7c10-115">عند تحويل طلب صيانة إلى أمر عمل، يحصل أمر العمل تلقائياً على نوع أمر العمل المرتبط بنوع طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="c7c10-115">When a maintenance request is converted to a work order, the work order automatically gets the work order type that is related to the maintenance request type.</span></span> 

    <span data-ttu-id="c7c10-116">**إدارة الأصول > الإعداد > طلبات الصيانة > أنواع طلبات الصيانة**</span><span class="sxs-lookup"><span data-stu-id="c7c10-116">**Asset Management > Setup > Maintenance requests > Maintenance request types**</span></span>

    ![لقطة شاشة لصفحة "أنواع طلبات الصيانة".](../media/maintenance-request-types-ssm.png)

> [!NOTE]
> <span data-ttu-id="c7c10-118">لا يمكن تغيير نوع طلب الصيانة في حالة إنشاء الطلب.</span><span class="sxs-lookup"><span data-stu-id="c7c10-118">The Maintenance request type cannot be changed when the request has been created.</span></span>