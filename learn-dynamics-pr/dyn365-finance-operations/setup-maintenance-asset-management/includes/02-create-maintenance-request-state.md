---
ms.openlocfilehash: 78abc4516d6f60176e83f4481579c8508bada759
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071348"
---
<span data-ttu-id="27c25-101">تحدد حالات دورة حياة طلب الصيانة المراحل المختلفة التي يمكن أن يمر بها طلب الصيانة، مثل **جديد**، أو **نشط**، أو **قيد التقدم**، أو **مرفوض**، أو **مُقفل**.</span><span class="sxs-lookup"><span data-stu-id="27c25-101">Maintenance request lifecycle states define the various stages that a maintenance request can go through, such as **New**, **Active**, **In Progress**, **Rejected**, or **Closed**.</span></span> <span data-ttu-id="27c25-102">يمكن تعريف حالات دورة الحياة هذه وإنشاؤها لتناسب احتياجات مؤسستك وعمليات سير إجراءات العمل على أفضل وجه.</span><span class="sxs-lookup"><span data-stu-id="27c25-102">These lifecycle states can be defined and created to best fit your organization’s needs and process flows.</span></span>

<span data-ttu-id="27c25-103">لكي يتمكن المستخدمون من إنشاء طلبات صيانة، يجب عليهم أولاً إنشاء حالات دورة حياة طلب الصيانة وتكوينها في إدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="27c25-103">For users to create maintenance requests, they must first create and configure maintenance request lifecycle states in Asset Management.</span></span> <span data-ttu-id="27c25-104">يستعرض القسم التالي خطوات إنشاء حالات دورة حياة طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="27c25-104">The following section goes through the steps to create your maintenance request lifecycle states.</span></span>

## <a name="set-up-maintenance-request-lifecycle-states"></a><span data-ttu-id="27c25-105">إعداد حالات دورة حياة طلب الصيانة</span><span class="sxs-lookup"><span data-stu-id="27c25-105">Set up maintenance request lifecycle states</span></span>
<span data-ttu-id="27c25-106">لبدء استخدام طلبات الصيانة، يجب أولاً إعداد حالة دورة حياة طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="27c25-106">To begin using maintenance requests, you must first set up a maintenance request lifecycle state.</span></span> <span data-ttu-id="27c25-107">يوضح هذا الإجراء خطوة بخطوة كيفية إنشاء حالة دورة حياة **نشط**.</span><span class="sxs-lookup"><span data-stu-id="27c25-107">This step-by-step procedure shows how to create a lifecycle state of **Active**.</span></span>

1.  <span data-ttu-id="27c25-108">انتقل إلى **‏‫إدارة الأصول‬ > إعداد > ‏‫طلبات صيانة‬ > حالات دورة الحياة**.</span><span class="sxs-lookup"><span data-stu-id="27c25-108">Go to **Asset Management > Setup > Maintenance requests > Lifecycle states**.</span></span>
2.  <span data-ttu-id="27c25-109">حدد **جديد** لإنشاء حالة دورة حياة طلب صيانة جديدة.</span><span class="sxs-lookup"><span data-stu-id="27c25-109">Select **New** to create a new maintenance request lifecycle state.</span></span>
3.  <span data-ttu-id="27c25-110">في حقل **حالة دورة الحياة**، أدخل معرّفاً لحالة دورة الحياة على النحو **نشط**.</span><span class="sxs-lookup"><span data-stu-id="27c25-110">In the **Lifecycle state** field, enter an ID for the lifecycle state as **Active**.</span></span>
4.  <span data-ttu-id="27c25-111">في حقل **الاسم**، أدخل اسماً وصفياً، مثل **طلب صيانة نشط**.</span><span class="sxs-lookup"><span data-stu-id="27c25-111">In the **Name** field, enter a descriptive name, such as **Active maintenance request**.</span></span>
<span data-ttu-id="27c25-112">في علامة التبويب السريعة **تفاصيل**، يملأ حقل نماذج دورة الحياة تلقائياً عدد نماذج دورة حياة طلب الصيانة التي تستخدم حالة دورة الحياة هذه.</span><span class="sxs-lookup"><span data-stu-id="27c25-112">On the **Details** FastTab, the Lifecycle models field automatically populates the number of maintenance request lifecycle models that use this lifecycle state.</span></span>
    > [!NOTE] 
    > <span data-ttu-id="27c25-113">عندما تقوم بتكوين حالة دورة حياة جديدة أول مرة، سيكون هذا الحقل فارغاً حتى تتم إضافة هذه الحالة إلى نموذج دورة الحياة.</span><span class="sxs-lookup"><span data-stu-id="27c25-113">When you are initially configuring a new lifecycle state, this field will be blank until this state is added to a lifecycle model.</span></span>

5.  <span data-ttu-id="27c25-114">في علامة التبويب السريعة **عام**، قم بتعيين شريط التبديل **نشط** إلى **‎نعم** إذا كان يجب أن يكون طلب الصيانة نشطاً في حالة دورة الحياة هذه.</span><span class="sxs-lookup"><span data-stu-id="27c25-114">On the **General** FastTab, set the **Active** toggle bar to **Yes** if a maintenance request should be active in this lifecycle state.</span></span>
6.  <span data-ttu-id="27c25-115">قم بتعيين شريط التبديل **تعيين الانتهاء الفعلي** إلى **نعم** إذا كان سيتم تسجيل تاريخ الانتهاء الفعلي ووقته تلقائياً في طلب الصيانة الذي يوجد في حالة دورة الحياة هذه.</span><span class="sxs-lookup"><span data-stu-id="27c25-115">Set the **Set actual end** toggle bar to **Yes** if an actual end date and time is to be automatically recorded on a maintenance request that is in this lifecycle state.</span></span>
7.  <span data-ttu-id="27c25-116">حدد **نعم** في شريط التبديل **إنشاء أمر عمل** إذا كان من الممكن إنشاء أمر عمل من طلب صيانة في حالة دورة الحياة هذه.</span><span class="sxs-lookup"><span data-stu-id="27c25-116">Select **Yes** on the **Create work order** toggle bar if a work order can be created from a maintenance request in this lifecycle state.</span></span>
8.  <span data-ttu-id="27c25-117">حدد **لا** في شريط التبديل **‏‫حذف** للاحتفاظ بالبيانات التاريخية.</span><span class="sxs-lookup"><span data-stu-id="27c25-117">Select **No** on the **Delete** toggle bar to keep the historical data.</span></span> 
9.  <span data-ttu-id="27c25-118">حدد **حفظ** لحفظ السجل.</span><span class="sxs-lookup"><span data-stu-id="27c25-118">Select **Save** to save the record.</span></span>

 
<span data-ttu-id="27c25-119">شاهد الفيديو التالي للتعرف على كيفية إعداد حالة دورة حياة طلب الصيانة.</span><span class="sxs-lookup"><span data-stu-id="27c25-119">Watch the following video to learn how to set up a maintenance request lifecycle state.</span></span>
 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4oJAj]

