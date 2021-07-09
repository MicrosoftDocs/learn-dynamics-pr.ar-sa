---
ms.openlocfilehash: c0b9aa65b000227341e71400f3fec1a8d3b9b5f8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070168"
---
<span data-ttu-id="b232c-101">لأداء التمارين في هذه الوحدة، يجب عليك استخدام البيانات التجريبية للكيان القانوني USRT والوصول إلى منشئ موقع التجارة الإلكترونية من خلال LCS.</span><span class="sxs-lookup"><span data-stu-id="b232c-101">To perform the exercises in this module, you should use the demo data of the USRT legal entity and have access to the e-Commerce site builder through LCS.</span></span> 

## <a name="scenario"></a><span data-ttu-id="b232c-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="b232c-102">Scenario</span></span>

<span data-ttu-id="b232c-103">بصفتك مدير المنتجات في شركة Fabrikam، فأنت تريد تمكين ظهور تقييمات المنتجات في نقطة البيع بالتجزئة (Retail POS) في المتاجر الفعلية لشركة Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="b232c-103">As the product manager at Fabrikam, you want to enable product ratings to be visible in the Retail POS in Fabrikam’s physical stores.</span></span> 

<span data-ttu-id="b232c-104">لمزامنة تقييمات المنتجات من خلال وظيفة دفعية وتعقب حالة الوظيفة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b232c-104">To sync product ratings through the batch job and track job status, follow these steps:</span></span>

1.  <span data-ttu-id="b232c-105">انتقل إلى **Retail وCommerce > إعداد المركز الرئيسي > جدولة التجارة > وظيفة مزامنة تقييمات المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="b232c-105">Go to **Retail and Commerce > Headquarters setup > Commerce scheduler > Sync product ratings job**.</span></span> 
2.  <span data-ttu-id="b232c-106">قم بتوسيع قسم **تشغيل في الخلفية**.</span><span class="sxs-lookup"><span data-stu-id="b232c-106">Expand the **Run in the background** section.</span></span> 
3.  <span data-ttu-id="b232c-107">حدد **تكرار**.</span><span class="sxs-lookup"><span data-stu-id="b232c-107">Select **Recurrence**.</span></span> 
4.  <span data-ttu-id="b232c-108">في الحقل **وحدة النمط**، أدخل **أسابيع**.</span><span class="sxs-lookup"><span data-stu-id="b232c-108">In the **PatternUnit** field, enter **Weeks**.</span></span> 
5.  <span data-ttu-id="b232c-109">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b232c-109">Select **OK**.</span></span>
6.  <span data-ttu-id="b232c-110">حدد **نعم** في الحقل **معالجة الدفعة**.</span><span class="sxs-lookup"><span data-stu-id="b232c-110">Select **Yes** in the **Batch processing** field.</span></span> 
7.  <span data-ttu-id="b232c-111">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b232c-111">Select **OK**.</span></span> 
8.  <span data-ttu-id="b232c-112">انتقل إلى **Retail وCommerce > الاستعلامات والتقارير > وظائف دفعية**.</span><span class="sxs-lookup"><span data-stu-id="b232c-112">Go to **Retail and Commerce > Inquiries and reports > Batch jobs**.</span></span> 
9.  <span data-ttu-id="b232c-113">استخدم **عامل التصفية السريع** للعثور على السجلات.</span><span class="sxs-lookup"><span data-stu-id="b232c-113">Use the **Quick Filter** to find records.</span></span> <span data-ttu-id="b232c-114">على سبيل المثال، قم بتصفية الحقل **وصف الوظيفة** بقيمة **اسحب تصنيفات المنتج**.</span><span class="sxs-lookup"><span data-stu-id="b232c-114">For example, filter on the **Job description** field with a value of **Pull product ratings**.</span></span>
10. <span data-ttu-id="b232c-115">في جزء الإجراء، حدد **وظيفة دفعية**.</span><span class="sxs-lookup"><span data-stu-id="b232c-115">On the Action Pane, select **Batch job**.</span></span> 
11. <span data-ttu-id="b232c-116">حدد **عرض الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="b232c-116">Select **View tasks**.</span></span> 
12. <span data-ttu-id="b232c-117">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="b232c-117">Close the page.</span></span> 
13. <span data-ttu-id="b232c-118">في جزء الإجراء، حدد **وظيفة دفعية**.</span><span class="sxs-lookup"><span data-stu-id="b232c-118">On the Action Pane, select **Batch job**.</span></span> 
14. <span data-ttu-id="b232c-119">حدد **سجل الوظائف الدفعية**.</span><span class="sxs-lookup"><span data-stu-id="b232c-119">Select **Batch job history**.</span></span>
15. <span data-ttu-id="b232c-120">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="b232c-120">Close the page.</span></span> 
16. <span data-ttu-id="b232c-121">انتقل إلى **Retail وCommerce > إعداد المركز الرئيسي > المعلمات > معلمات Commerce**.</span><span class="sxs-lookup"><span data-stu-id="b232c-121">Go to **Retail and Commerce > Headquarters setup > Parameters > Commerce parameters**.</span></span> 
17. <span data-ttu-id="b232c-122">حدد علامة التبويب **معلمات التكوين**.</span><span class="sxs-lookup"><span data-stu-id="b232c-122">Select the **Configuration parameters** tab.</span></span> 
18. <span data-ttu-id="b232c-123">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="b232c-123">Select **New**.</span></span>
19. <span data-ttu-id="b232c-124">في الحقل **الاسم**، أدخل **التصنيفات والمراجعات**.</span><span class="sxs-lookup"><span data-stu-id="b232c-124">In the **Name** field, enter **RatingsAndReviews**.</span></span>
20. <span data-ttu-id="b232c-125">قم بتمكين **تصنيفات المنتجات** لمتاجر البيع بالتجزئة.</span><span class="sxs-lookup"><span data-stu-id="b232c-125">Enable **Product ratings** for Retail Stores.</span></span> 
20. <span data-ttu-id="b232c-126">في الحقل **القيمة**، أدخل **صحيح**.</span><span class="sxs-lookup"><span data-stu-id="b232c-126">In the **Value** field, enter **true**.</span></span> 
21. <span data-ttu-id="b232c-127">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="b232c-127">Select **Save**.</span></span> 
22. <span data-ttu-id="b232c-128">انتقل إلى **Retail وCommerce> تكنولوجيا المعلومات في Commerce > جدول التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="b232c-128">Go to **Retail and Commerce> Commerce IT > Distribution schedule**.</span></span> 
23. <span data-ttu-id="b232c-129">استخدم **عامل التصفية السريع** للتصفية على حقل **الاسم** بقيمة **1110**.</span><span class="sxs-lookup"><span data-stu-id="b232c-129">Use the **Quick Filter** to filter on the **Name** field with a value of **1110**.</span></span> 
24. <span data-ttu-id="b232c-130">حدد **تشغيل الآن**.</span><span class="sxs-lookup"><span data-stu-id="b232c-130">Select **Run now**.</span></span>
25. <span data-ttu-id="b232c-131">حدد **نعم**.</span><span class="sxs-lookup"><span data-stu-id="b232c-131">Select **Yes**.</span></span> 

