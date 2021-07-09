---
ms.openlocfilehash: e62611a330aaa3f3c3b599148a8c3fd39a2839cf
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073473"
---
<span data-ttu-id="85ca3-101">كمساعد جديد لمصمم المنتج في شركة **USMF**، تتم مطالبتك بإنشاء قائمة مكونات صنف بسيطة لخزانة خفيفة جديدة.</span><span class="sxs-lookup"><span data-stu-id="85ca3-101">As a new assistant to the Product designer at the **USMF** company, you are asked to create a simple BOM for a new Light cabinet.</span></span> <span data-ttu-id="85ca3-102">استخدم المواصفات التالية ووافق على قائمة مكونات الصنف باستخدام الموظف 000020، جوليا فونديربورك، والمعلمات التالية:</span><span class="sxs-lookup"><span data-stu-id="85ca3-102">Use the following specifications and approve the BOM by using employee 000020, Julia Funderburk, and the following parameters:</span></span>

-   <span data-ttu-id="85ca3-103">**الاسم**: خزانة خفيفة</span><span class="sxs-lookup"><span data-stu-id="85ca3-103">**Name**: Light Cabinet</span></span>
-   <span data-ttu-id="85ca3-104">**مجموعة الصنف**: الصوت</span><span class="sxs-lookup"><span data-stu-id="85ca3-104">**Item group**: Audio</span></span>
-   <span data-ttu-id="85ca3-105">**الموقع**: ‏1</span><span class="sxs-lookup"><span data-stu-id="85ca3-105">**Site**: 1</span></span>
-   <span data-ttu-id="85ca3-106">**الصنف**:</span><span class="sxs-lookup"><span data-stu-id="85ca3-106">**Item**:</span></span>
    -   <span data-ttu-id="85ca3-107">حاوية M0005</span><span class="sxs-lookup"><span data-stu-id="85ca3-107">M0005 Enclosure</span></span>
    -   <span data-ttu-id="85ca3-108">أعمدة الربط M0006</span><span class="sxs-lookup"><span data-stu-id="85ca3-108">M0006 Binding posts</span></span>
    -   <span data-ttu-id="85ca3-109">رغوة تخميد السماعة P0002</span><span class="sxs-lookup"><span data-stu-id="85ca3-109">P0002 Speaker Damping Foam</span></span>
-   <span data-ttu-id="85ca3-110">**الكمية** لكل صنف: 1</span><span class="sxs-lookup"><span data-stu-id="85ca3-110">**Quantity** for each item: 1</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="85ca3-111">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="85ca3-111">Before you begin</span></span> 

<span data-ttu-id="85ca3-112">للحصول على أقصى استفادة من هذا التدريب وغيره من التدريبات الأخرى في هذه الوحدة، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Supply Chain Management والتي يتم تثبيتها باستخدام Lifecycle Services ‏(LCS).</span><span class="sxs-lookup"><span data-stu-id="85ca3-112">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data available in Dynamics 365 Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span>

1.  <span data-ttu-id="85ca3-113">في USMF، انتقل إلى **إدارة معلومات المنتج > قوائم مكونات الأصناف والمعادلات > قوائم مكونات الأصناف**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-113">In USMF, go to **Product information management > Bills of materials and formulas > Bills of materials**.</span></span>
2.  <span data-ttu-id="85ca3-114">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-114">Select **New**.</span></span>
3.  <span data-ttu-id="85ca3-115">في حقل **الاسم**، أدخل **خزانة خفيفة**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-115">In the **Name** field, enter **Light Cabinet**.</span></span>
4.  <span data-ttu-id="85ca3-116">في حقل **الموقع**، أدخل أو حدد **1**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-116">In the **Site** field, enter or select **1**.</span></span>
5.  <span data-ttu-id="85ca3-117">في حقل **مجموعة الصنف**، أدخِل **الصوت** أو حدده.</span><span class="sxs-lookup"><span data-stu-id="85ca3-117">In the **Item group** field, enter or select **Audio**.</span></span>
6.  <span data-ttu-id="85ca3-118">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-118">Select **Save**.</span></span>
7.  <span data-ttu-id="85ca3-119">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-119">Select **New**.</span></span>
8.  <span data-ttu-id="85ca3-120">في حقل **رقم البند**، أدخِل **M0005**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-120">In the **Item number** field, enter **M0005**.</span></span>
9.  <span data-ttu-id="85ca3-121">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-121">Select **New**.</span></span>
10. <span data-ttu-id="85ca3-122">في حقل **رقم البند**، أدخِل **M0006**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-122">In the **Item number** field, enter **M0006**.</span></span>
11. <span data-ttu-id="85ca3-123">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-123">Select **New**.</span></span>
12. <span data-ttu-id="85ca3-124">في حقل **رقم البند**، أدخِل **P0002**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-124">In the **Item number** field, enter **P0002**.</span></span>
13. <span data-ttu-id="85ca3-125">حدد **موافقة**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-125">Select **Approval**.</span></span>
14. <span data-ttu-id="85ca3-126">حدد **000020، ‏Julia Funderburk**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-126">Select **000020, Julia Funderburk**.</span></span>
15. <span data-ttu-id="85ca3-127">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-127">Select **OK**.</span></span>
16. <span data-ttu-id="85ca3-128">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="85ca3-128">Select **Save**.</span></span>
17. <span data-ttu-id="85ca3-129">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="85ca3-129">Close all pages.</span></span>
