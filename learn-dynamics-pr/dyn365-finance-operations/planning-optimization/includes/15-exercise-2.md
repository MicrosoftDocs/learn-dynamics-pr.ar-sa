---
ms.openlocfilehash: b9f3b0f2344676b8def24cc1ffc01a7775811e46
ms.sourcegitcommit: 01f8d224bf1e548ba0cbe53b3e2150c43302c125
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "6072098"
---
> [!NOTE]
> <span data-ttu-id="41533-101">لإكمال هذا المعمل، يجب تثبيت الوظيفة الإضافية تحسين التخطيط في البيئة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="41533-101">To complete this lab, the Planning Optimization add-in must be installed in your own environment.</span></span> 

## <a name="scenario"></a><span data-ttu-id="41533-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="41533-102">Scenario</span></span>
<span data-ttu-id="41533-103">في هذا التمرين، سيتم تشغيل تحسين التخطيط واعتماد أمر شراء مخطط.</span><span class="sxs-lookup"><span data-stu-id="41533-103">In this exercise, Planning Optimization will be run and a planned purchase order will be approved.</span></span> <span data-ttu-id="41533-104">وبعد ذلك، عند تشغيل تحسين التخطيط مره أخرى، تبقى الأوامر المعتمدة كما هي وستتم إعادة حساب الباقي.</span><span class="sxs-lookup"><span data-stu-id="41533-104">Then, when you run Planning Optimization again, the approved orders will remain the same and the rest will be re-calculated.</span></span> 

1.  <span data-ttu-id="41533-105">في شركة **USMF**، انتقل **التخطيط الرئيسي > التخطيط الرئيسي > الأوامر المخططة**.</span><span class="sxs-lookup"><span data-stu-id="41533-105">In company **USMF**, go to **Master planning > Master planning > Planned orders**.</span></span>
2.  <span data-ttu-id="41533-106">حدد الخطة المسماة **DynPlan**.</span><span class="sxs-lookup"><span data-stu-id="41533-106">Select the plan named **DynPlan**.</span></span>
3.  <span data-ttu-id="41533-107">قم بتصفية **رقم الصنف** إلى **T0003**.</span><span class="sxs-lookup"><span data-stu-id="41533-107">Filter the **Item number** to **T0003**.</span></span>
4.  <span data-ttu-id="41533-108">بالنسبة لكافة أوامر الشراء المخططة الثلاثة، قم بتمييزها بالحالة **معتمدة**، والتي يمكن إجراؤها بإحدى الطريقتين التاليتين:</span><span class="sxs-lookup"><span data-stu-id="41533-108">For all three planned purchase orders, mark them as **Approved**, which can be done in one of two ways:</span></span>
    - <span data-ttu-id="41533-109">في العمود **الحالة**، حدد كل قائمة منسدلة ثم حدد **معتمدة**.</span><span class="sxs-lookup"><span data-stu-id="41533-109">In the **Status** column, select each drop-down menu and then select **Approved**.</span></span>
    - <span data-ttu-id="41533-110">حدد كل أمر في القائمة، ثم قم بتحديد **اعتماد** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="41533-110">Select each order in the list and then select **Approve** in the Action Pane.</span></span>
5.  <span data-ttu-id="41533-111">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="41533-111">Close the page.</span></span>
6.  <span data-ttu-id="41533-112">انتقل إلى مساحة عمل **التخطيط الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="41533-112">Go to the **Master planning** workspace.</span></span>
7.  <span data-ttu-id="41533-113">في لوحة **التخطيط الرئيسي**، حدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="41533-113">In the **Master planning** tile, select **Run**.</span></span> 
8.  <span data-ttu-id="41533-114">في مربع الحوار، حدد **الخطة الرئيسية** DynPlan ولا تقم بتمكين التأكيد التلقائي.</span><span class="sxs-lookup"><span data-stu-id="41533-114">In the dialog box, select **Master plan** DynPlan and do not enable auto-firming.</span></span>
9.  <span data-ttu-id="41533-115">تأكد من عدم وجود أية عوامل تصفية في علامة التبويب السريعة **السجلات المطلوب تضمينها**.</span><span class="sxs-lookup"><span data-stu-id="41533-115">Ensure that no filters are in the **Records to include** FastTab.</span></span> 
10. <span data-ttu-id="41533-116">حدد **موافق** لتشغيل تحسين التخطيط.</span><span class="sxs-lookup"><span data-stu-id="41533-116">Select **OK** to run Planning Optimization.</span></span>
11. <span data-ttu-id="41533-117">حدد لوحة **الأوامر المخططة** والخطة التي تسمى **DynPlan**.</span><span class="sxs-lookup"><span data-stu-id="41533-117">Select the **Planned orders** tile and the plan named **DynPlan**.</span></span> 
12. <span data-ttu-id="41533-118">لاحظ أن **تاريخ الأمر** سيكون هو تاريخ اليوم في معظم الأوامر المخططة.</span><span class="sxs-lookup"><span data-stu-id="41533-118">Note that the **Order date** will be today’s date on most planned orders.</span></span>
13. <span data-ttu-id="41533-119">قم بتصفية **رقم الصنف** إلى **T0003**.</span><span class="sxs-lookup"><span data-stu-id="41533-119">Filter the **Item number** to **T0003**.</span></span>
14. <span data-ttu-id="41533-120">لاحظ **تاريخ الأمر**.</span><span class="sxs-lookup"><span data-stu-id="41533-120">Note the **Order date**.</span></span> <span data-ttu-id="41533-121">ولكنه لم يتغير لأنه بالحالة **معتمد** ويبقى كما هو.</span><span class="sxs-lookup"><span data-stu-id="41533-121">It did not change because it was in **Approved** status and remains the same.</span></span> 

