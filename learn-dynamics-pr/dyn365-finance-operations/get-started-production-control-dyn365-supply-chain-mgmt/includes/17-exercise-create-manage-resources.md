---
ms.openlocfilehash: c9c855f70053c3a112595a13f45e90a377ac06ba
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6073866"
---
## <a name="scenario"></a><span data-ttu-id="1f720-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="1f720-101">Scenario</span></span>
<span data-ttu-id="1f720-102">اشترت شركة **USMF** روبوت تعبئة جديد لورشة تعبئة مكبر الصوت الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="1f720-102">Company **USMF** has bought a new packing robot for their speaker packing workshop.</span></span> <span data-ttu-id="1f720-103">سوف يقلل روبوت التعبئة من الحاجة إلى العمل اليدوي في ورشة تعبئة مكبرات الصوت.</span><span class="sxs-lookup"><span data-stu-id="1f720-103">The packing robot will reduce the need for manual labor in the speaker packing workshop.</span></span> <span data-ttu-id="1f720-104">لذلك، يمكن إعادة تعيين بعض العمال من هذه المجموعة لأداء أعمال أخرى حيث يصبح روبوت التعبئة الجديد جاهزاً للعمل بشكل كامل.</span><span class="sxs-lookup"><span data-stu-id="1f720-104">Therefore, some workers from this group can be reassigned to perform other work as the new packing robot becomes fully operational.</span></span>

## <a name="create-capabilities"></a><span data-ttu-id="1f720-105">إنشاء القدرات الإنتاجية</span><span class="sxs-lookup"><span data-stu-id="1f720-105">Create capabilities</span></span> 

1.  <span data-ttu-id="1f720-106">انتقل إلى **إدارة المؤسسة > الموارد > قدرات الموارد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-106">Go to **Organization administration > Resources > Resource capabilities**.</span></span>
2.  <span data-ttu-id="1f720-107">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-107">Select **New**.</span></span>
3.  <span data-ttu-id="1f720-108">أدخل **تجميع GTL** في حقل **القدرة** و **تجميع** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="1f720-108">Enter **GTL-Assembly** in the **Capability** field and **Assembly** in the **Description** field.</span></span>
4.  <span data-ttu-id="1f720-109">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-109">Select **New**.</span></span>
5.  <span data-ttu-id="1f720-110">أدخل **تعبئة GTL** في حقل **القدرة** و **تعبئة** في حقل **الوصف**.</span><span class="sxs-lookup"><span data-stu-id="1f720-110">Enter **GTL- Packing** in the **Capability** field and **Packing** in the **Description** field.</span></span>


## <a name="assign-resources-to-capability"></a><span data-ttu-id="1f720-111">تعيين الموارد للقدرة الإنتاجية</span><span class="sxs-lookup"><span data-stu-id="1f720-111">Assign resources to capability</span></span> ##

1.  <span data-ttu-id="1f720-112">حدد **تجميع GTL** من قائمة القدرات.</span><span class="sxs-lookup"><span data-stu-id="1f720-112">Select **GTL-Assembly** from the list of capabilities.</span></span>
1.  <span data-ttu-id="1f720-113">حدد **إضافة** من علامة التبويب السريعة **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-113">Select **Add** from the **Resources** FastTab.</span></span>
1.  <span data-ttu-id="1f720-114">حدد **5110**، عامل تجميع سماعات 1 في حقل **المورد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-114">Select **5110**, Assembly worker 1, in the **Resource** field.</span></span>
1.  <span data-ttu-id="1f720-115">في حقل **الأولوية**، أدخِل **1**.</span><span class="sxs-lookup"><span data-stu-id="1f720-115">Enter **1** in the **Priority** field.</span></span>
1.  <span data-ttu-id="1f720-116">اقبل **المستوى** الافتراضي بالقيمة 0.00.</span><span class="sxs-lookup"><span data-stu-id="1f720-116">Accept the default **Level** of 0.00.</span></span>
1.  <span data-ttu-id="1f720-117">كرر الخطوات من 2 إلى 5 للمورد **5111**.</span><span class="sxs-lookup"><span data-stu-id="1f720-117">Repeat steps 2 to 5 for resource **5111**.</span></span>
1.  <span data-ttu-id="1f720-118">قم بإغلاق صفحة **قدرات المورد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-118">Close the **Resource capabilities** page.</span></span>


## <a name="assign-capabilities-to-a-resource"></a><span data-ttu-id="1f720-119">تعيين القدرات الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="1f720-119">Assign capabilities to a resource</span></span> ##

1.  <span data-ttu-id="1f720-120">انتقل إلى **إدارة المؤسسة > الموارد > موارد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-120">Go to **Organization administration > Resources > Resources**.</span></span>
2.  <span data-ttu-id="1f720-121">حدد المورد **5111** في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="1f720-121">Select resource **5111** in the grid.</span></span>
3.  <span data-ttu-id="1f720-122">قم بتوسيع علامة التبويب السريعة **القدرات**.</span><span class="sxs-lookup"><span data-stu-id="1f720-122">Expand the **Capabilities** FastTab.</span></span>
4.  <span data-ttu-id="1f720-123">حدد **طريقة العرض > الكل**</span><span class="sxs-lookup"><span data-stu-id="1f720-123">Select **View > All**.</span></span>
5.  <span data-ttu-id="1f720-124">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="1f720-124">Select **Add**.</span></span>
6.  <span data-ttu-id="1f720-125">في حقل **القدرة الإنتاجية**، أدخل **تعبئة GTL**.</span><span class="sxs-lookup"><span data-stu-id="1f720-125">Enter **GTL-Packing** in the **Capability** field.</span></span>
7.  <span data-ttu-id="1f720-126">اقبل تاريخ **السريان** الافتراضي لتاريخ اليوم.</span><span class="sxs-lookup"><span data-stu-id="1f720-126">Accept the default **Effective** date of today's date.</span></span> 
8.  <span data-ttu-id="1f720-127">اقبل **المستوى** الافتراضي بالقيمة 0.00.</span><span class="sxs-lookup"><span data-stu-id="1f720-127">Accept the default **Level** of 0.00.</span></span>
9.  <span data-ttu-id="1f720-128">في حقل **الأولوية**، أدخل **2**.</span><span class="sxs-lookup"><span data-stu-id="1f720-128">Enter **2** in the **Priority** field.</span></span> 
10. <span data-ttu-id="1f720-129">حدد **حفظ**</span><span class="sxs-lookup"><span data-stu-id="1f720-129">Select **Save**</span></span>
11. <span data-ttu-id="1f720-130">أغلق صفحة **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="1f720-130">Close the **Resources** page.</span></span>

