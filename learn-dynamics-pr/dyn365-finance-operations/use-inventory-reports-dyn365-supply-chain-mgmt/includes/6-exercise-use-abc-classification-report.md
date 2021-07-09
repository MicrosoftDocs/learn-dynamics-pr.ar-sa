---
ms.openlocfilehash: cb54816bd1dfa3d15d552277292cdddb514d56b6
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073383"
---
<span data-ttu-id="22d01-101">يطلب منك مديرك في شركة USMF إجراء بعض سيناريوهات تصنيف ABC الاختبارية على المخزون لشهر يناير 2016.</span><span class="sxs-lookup"><span data-stu-id="22d01-101">You are asked by your manager at the USMF company to do some test ABC classification scenarios on inventory for January 2016.</span></span> <span data-ttu-id="22d01-102">يُطلب منك تشغيل تقريري تصنيف ABC يعرضان سيناريوهات مختلفة، مع التفاصيل التالية:</span><span class="sxs-lookup"><span data-stu-id="22d01-102">You are asked to run two ABC classification reports that will show different scenarios, with the following details:</span></span>

- <span data-ttu-id="22d01-103">تصنيفات الإيرادات، بنسبة 80 بالمائة (A) و15 بالمائة (B) و5 بالمائة (C)</span><span class="sxs-lookup"><span data-stu-id="22d01-103">Revenue classifications, with 80 percent (A), 15 percent (B), and 5 percent (C)</span></span>
- <span data-ttu-id="22d01-104">تصنيفات القيم، بنسبة 20 بالمائة (A) و15 بالمائة (B) و5 بالمائة (C)</span><span class="sxs-lookup"><span data-stu-id="22d01-104">Value classifications, with 20 percent (A), 60 percent (B), and 20 percent (C)</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="22d01-105">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="22d01-105">Before you begin</span></span> 

<span data-ttu-id="22d01-106">للحصول على أقصى استفادة من هذا التدريب وغيره من التدريبات الأخرى في هذه الوحدة، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Dynamics 365 Supply Chain Management والتي يتم تثبيتها باستخدام Lifecycle Services ‏(LCS).</span><span class="sxs-lookup"><span data-stu-id="22d01-106">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data available in Dynamics 365 Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span> 

<span data-ttu-id="22d01-107">لتشغيل تقرير تصنيف ABC الذي يستخدم تصنيفات الإيرادات؛ 80 بالمائة (A) و15 بالمائة (B) و5 بالمائة (C)، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="22d01-107">To run the ABC classification report that uses Revenue classifications; 80 percent (A), 15 percent (B), and 5 percent (C), follow these steps:</span></span> 

1.  <span data-ttu-id="22d01-108">انتقل إلى **إدارة المخزون > الاستعلامات والتقارير > تقارير قيم المخزون > تصنيف ABC**.</span><span class="sxs-lookup"><span data-stu-id="22d01-108">Go to **Inventory management > Inquiries and reports > Inventory value reports > ABC classification**.</span></span>
2.  <span data-ttu-id="22d01-109">في حقل **من التاريخ**، اكتب **01/01/16**.</span><span class="sxs-lookup"><span data-stu-id="22d01-109">In the **From date** field, type **01/01/16**.</span></span>
3.  <span data-ttu-id="22d01-110">في حقل **إلى التاريخ**، اكتب **01/31/16**.</span><span class="sxs-lookup"><span data-stu-id="22d01-110">In the **To date** field, type **01/31/16**.</span></span>
4.  <span data-ttu-id="22d01-111">في حقل **A: الأعلى**، اكتب **80**.</span><span class="sxs-lookup"><span data-stu-id="22d01-111">In the **A: Highest** field, type **80**.</span></span>
5.  <span data-ttu-id="22d01-112">في حقل **B: متوسط**، اكتب **15**.</span><span class="sxs-lookup"><span data-stu-id="22d01-112">In the **B: Middle** field, type **15**.</span></span>
6.  <span data-ttu-id="22d01-113">في حقل **C: الأقل**، اكتب **5**.</span><span class="sxs-lookup"><span data-stu-id="22d01-113">In the **C: Lowest** field, type **5**.</span></span>
7.  <span data-ttu-id="22d01-114">في حقل **نماذج ABC**، حدد السهم، ثم حدد **الإيراد**.</span><span class="sxs-lookup"><span data-stu-id="22d01-114">In the **ABC Models** field, select the arrow, and then select **Revenue**.</span></span>
8.  <span data-ttu-id="22d01-115">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="22d01-115">Select **OK**.</span></span> <span data-ttu-id="22d01-116">تتم طباعة تقرير تصنيف ABC على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="22d01-116">The ABC classification report prints to the screen.</span></span>
9.  <span data-ttu-id="22d01-117">أغلق التقرير.</span><span class="sxs-lookup"><span data-stu-id="22d01-117">Close the report.</span></span>


<span data-ttu-id="22d01-118">لتشغيل تقرير تصنيف ABC الذي يستخدم تصنيفات القيم؛ 20 بالمائة (A) و15 بالمائة (B) و5 بالمائة (C)، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="22d01-118">To run the ABC classification report that uses Value classifications; 20 percent (A), 60 percent (B), and 20 percent (C), follow these steps:</span></span>

1.  <span data-ttu-id="22d01-119">انتقل إلى **إدارة المخزون > الاستعلامات والتقارير > تقارير قيم المخزون > تصنيف ABC**.</span><span class="sxs-lookup"><span data-stu-id="22d01-119">Go to **Inventory management > Inquiries and reports > Inventory value reports > ABC classification**.</span></span>
2.  <span data-ttu-id="22d01-120">في حقل **من التاريخ**، اكتب **01/01/16**.</span><span class="sxs-lookup"><span data-stu-id="22d01-120">In the **From date** field, type **01/01/16**.</span></span>
3.  <span data-ttu-id="22d01-121">في حقل **إلى التاريخ**، اكتب **01/31/16**.</span><span class="sxs-lookup"><span data-stu-id="22d01-121">In the **To date** field, type **01/31/16**.</span></span>
4.  <span data-ttu-id="22d01-122">في حقل **A: الأعلى**، اكتب **20**.</span><span class="sxs-lookup"><span data-stu-id="22d01-122">In the **A: Highest** field, type **20**.</span></span>
5.  <span data-ttu-id="22d01-123">في حقل **B: متوسط**، اكتب **60**.</span><span class="sxs-lookup"><span data-stu-id="22d01-123">In the **B: Middle** field, type **60**.</span></span>
6.  <span data-ttu-id="22d01-124">في حقل **C: الأقل**، اكتب **20**.</span><span class="sxs-lookup"><span data-stu-id="22d01-124">In the **C: Lowest** field, type **20**.</span></span>
7.  <span data-ttu-id="22d01-125">في حقل **نماذج ABC**، حدد السهم، ثم حدد **القيمة**.</span><span class="sxs-lookup"><span data-stu-id="22d01-125">In the **ABC Models** field, select the arrow, and then select **Value**.</span></span>
8.  <span data-ttu-id="22d01-126">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="22d01-126">Select **OK**.</span></span> 
9.  <span data-ttu-id="22d01-127">تتم طباعة تقرير تصنيف ABC على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="22d01-127">The ABC classification report prints to the screen.</span></span>
10. <span data-ttu-id="22d01-128">أغلق التقرير.</span><span class="sxs-lookup"><span data-stu-id="22d01-128">Close the report.</span></span>

