---
ms.openlocfilehash: 699a15858121628437461d5a06c49395f0da5c23
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073049"
---
## <a name="before-you-begin"></a><span data-ttu-id="a1f3b-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="a1f3b-101">Before you begin</span></span>
<span data-ttu-id="a1f3b-102">للاستفادة إلى أقصى حد من هذه التدريبات وغيرها في هذه الوحدة النمطية، نوصي بأن يكون لديك بيانات العينة القياسية المتوفرة في Supply Chain Management والتي تم تثبيتها باستخدام Lifecycle Services‎‏ (LCS)‏‏‏‎.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-102">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data that is available in Supply Chain Management that is installed by using Lifecycle Services (LCS).</span></span> 

## <a name="scenario"></a><span data-ttu-id="a1f3b-103">السيناريو</span><span class="sxs-lookup"><span data-stu-id="a1f3b-103">Scenario</span></span>
<span data-ttu-id="a1f3b-104">ستقوم أولاً بإعداد مورد افتراضي لمستودع ثم إنشاء اتفاقية شراء مع هذا المورد.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-104">You will first set up a default vendor for a warehouse and then create a purchase agreement with that vendor.</span></span> 

## <a name="set-up-a-default-vendor-for-a-warehouse"></a><span data-ttu-id="a1f3b-105">إعداد مورد افتراضي لأحد المستودعات</span><span class="sxs-lookup"><span data-stu-id="a1f3b-105">Set up a default vendor for a warehouse</span></span>

1.  <span data-ttu-id="a1f3b-106">في شركة **USMF**، انتقل إلى **إدارة المخزون> إعداد> تصنيف المخزون> مستودعات**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-106">In the **USMF** company, go to **Inventory management > Setup > Inventory breakdown > Warehouses**.</span></span>
2.  <span data-ttu-id="a1f3b-107">في القائمة، ابحث عن المستودع **12-801** وحدده.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-107">In the list, find and select Warehouse **12-801**.</span></span>
3.  <span data-ttu-id="a1f3b-108">ضمن علامة التبويب السريعة **عام**، تحقق من تعيين حقل **حساب المورد** على **US-801**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-108">Under the **General** FastTab, verify that the **Vendor account** field is set to **US-801**.</span></span>
4.  <span data-ttu-id="a1f3b-109">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-109">Close the page.</span></span>

## <a name="create-a-purchase-agreement"></a><span data-ttu-id="a1f3b-110">إنشاء اتفاقية شراء</span><span class="sxs-lookup"><span data-stu-id="a1f3b-110">Create a purchase agreement</span></span>

1.  <span data-ttu-id="a1f3b-111">انتقل إلى **التدبير والتوريد > اتفاقيات الشراء > اتفاقيات الشراء**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-111">Go to **Procurement and sourcing > Purchase agreements > Purchase agreements**.</span></span>
2.  <span data-ttu-id="a1f3b-112">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-112">Select **New**.</span></span>
3.  <span data-ttu-id="a1f3b-113">في الحقل **حساب المورد**، أدخل أو حدد **US-801**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-113">In the **Vendor account** field, enter or select **US-801**.</span></span>
4.  <span data-ttu-id="a1f3b-114">في الحقل **تصنيف اتفاقيه الشراء**، أدخل **المشتريات العامة** أو حددها.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-114">In the **Purchase agreement classification** field, enter or select **General purchases**.</span></span>
5.  <span data-ttu-id="a1f3b-115">قم بتوسيع القسم **عام**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-115">Expand the **General** section.</span></span>
6.  <span data-ttu-id="a1f3b-116">في الحقل **تاريخ انتهاء الصلاحية**، أدخل تاريخاً في المستقبل يجب أن تنتهي صلاحية الاتفاقيات بحلوله.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-116">In the **Expiration date** field, enter a date in the future when agreements should be expired by.</span></span> <span data-ttu-id="a1f3b-117">على سبيل المثال، تاريخ اليوم + 30 يوماً.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-117">For example, today's date + 30 days.</span></span>
7.  <span data-ttu-id="a1f3b-118">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-118">Select **OK**.</span></span>
8.  <span data-ttu-id="a1f3b-119">قم بتوسيع القسم **رأس اتفاقيه الشراء**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-119">Expand the **Purchase agreement header** section.</span></span>
9.  <span data-ttu-id="a1f3b-120">في الحقل **الالتزام الافتراضي**، حدد **التزام قيمة المنتج**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-120">In the **Default commitment** field, select **Product value commitment**.</span></span>
10. <span data-ttu-id="a1f3b-121">في علامة التبويب السريعة **سطور اتفاقية الشراء**، حدد **إضافة سطر**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-121">In the **Purchase agreement lines** FastTab, select **Add line**.</span></span>
11. <span data-ttu-id="a1f3b-122">في الحقل **رقم الصنف**، أدخل أو حدد **S0001**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-122">In the **Item number** field, enter or select **S0001**.</span></span>
12. <span data-ttu-id="a1f3b-123">في الحقل **مستودع**، أدخل أو حدد **12-801**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-123">In the **Warehouse** field, enter or select **12-801**.</span></span>
13. <span data-ttu-id="a1f3b-124">عيّن **المبلغ الصافي** على **73570.00**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-124">Set **Net amount** to **73570.00**.</span></span>
14. <span data-ttu-id="a1f3b-125">في الحقل **الحالة**، في **رأس اتفاقية الشراء**، حدد **فعال**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-125">In the **Status** field, in the **Purchase agreement header**, select **Effective**.</span></span>
15. <span data-ttu-id="a1f3b-126">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-126">Select **Save**.</span></span>
16. <span data-ttu-id="a1f3b-127">أغلق كافة الصفحات.</span><span class="sxs-lookup"><span data-stu-id="a1f3b-127">Close all pages.</span></span>
