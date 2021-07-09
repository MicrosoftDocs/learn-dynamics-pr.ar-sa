---
ms.openlocfilehash: 0991cfe72e774dc7df4ad2c294823758d6254780
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071072"
---
## <a name="scenario"></a><span data-ttu-id="24e33-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="24e33-101">Scenario</span></span>
<span data-ttu-id="24e33-102">ستقوم بإعداد محددات الأصول الثابتة ثم إنشاء فاتورة مورد جديدة.</span><span class="sxs-lookup"><span data-stu-id="24e33-102">You will set up fixed assets parameters and then create a new vendor invoice.</span></span>

## <a name="set-up-fixed-assets-parameters"></a><span data-ttu-id="24e33-103">إعداد معلمات الأصول الثابتة</span><span class="sxs-lookup"><span data-stu-id="24e33-103">Set up fixed assets parameters</span></span>

1.  <span data-ttu-id="24e33-104">في USMF، انتقل إلى **الأصول الثابتة > إعداد > معلمات الأصول الثابتة**</span><span class="sxs-lookup"><span data-stu-id="24e33-104">In USMF, go to **Fixed assets > Setup > Fixed assets parameters**.</span></span>
2.  <span data-ttu-id="24e33-105">قم بتوسيع القسم **أوامر الشراء**.</span><span class="sxs-lookup"><span data-stu-id="24e33-105">Expand the **Purchase orders** section.</span></span>
3.  <span data-ttu-id="24e33-106">تأكد من تمكين خيار **السماح بالحصول على الأصل من الشراء**.</span><span class="sxs-lookup"><span data-stu-id="24e33-106">Ensure the **Allow asset acquisition from Purchasing** option is enabled.</span></span>
4.  <span data-ttu-id="24e33-107">تأكد من تمكين خيار **إنشاء أصل أثناء ترحيل إيصال المنتج أو الفاتورة**.</span><span class="sxs-lookup"><span data-stu-id="24e33-107">Ensure the **Create asset during product receipt or invoice posting** option is enabled.</span></span>
5.  <span data-ttu-id="24e33-108">انقر على **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="24e33-108">Click **Save**.</span></span>

## <a name="create-a-new-vendor-invoice"></a><span data-ttu-id="24e33-109">إنشاء فاتورة مورد جديدة</span><span class="sxs-lookup"><span data-stu-id="24e33-109">Create a new vendor invoice</span></span>

1.  <span data-ttu-id="24e33-110">انتقل إلى **الحسابات الدائنة > مساحات عمل > إدخال فاتورة مورد**.</span><span class="sxs-lookup"><span data-stu-id="24e33-110">Go to **Accounts payable > Workspaces > Vendor invoice entry**.</span></span>
2.  <span data-ttu-id="24e33-111">حدد **فاتورة المورّد الجديدة**.</span><span class="sxs-lookup"><span data-stu-id="24e33-111">Select **New vendor invoice**.</span></span>
3.  <span data-ttu-id="24e33-112">في حقل **حساب الفاتورة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="24e33-112">In the **Invoice account** field, select the drop-down button to open the lookup.</span></span>
4.  <span data-ttu-id="24e33-113">في القائمة، حدد حساباً مثل **1001**.</span><span class="sxs-lookup"><span data-stu-id="24e33-113">In the list, select an account such as **1001**.</span></span>
5.  <span data-ttu-id="24e33-114">في حقل **الرقم**، اكتب قيمة، مثل 1000.00.</span><span class="sxs-lookup"><span data-stu-id="24e33-114">In the **Number** field, type a value, such as 1000.00.</span></span>
6.  <span data-ttu-id="24e33-115">في الحقل **تاريخ الترحيل**، يتم تعيين التاريخ افتراضياً على التاريخ الحالي.</span><span class="sxs-lookup"><span data-stu-id="24e33-115">In the **Posting date** field, the date defaults to current date.</span></span>
7.  <span data-ttu-id="24e33-116">حدد **إضافة سطر**.</span><span class="sxs-lookup"><span data-stu-id="24e33-116">Select **Add line**.</span></span>
8.  <span data-ttu-id="24e33-117">في الحقل **رقم الصنف**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="24e33-117">In the **Item number** field, select the drop-down button to open  the lookup.</span></span> 

    <span data-ttu-id="24e33-118">يمكن استخدام إما الأصناف غير المخزنة أو فئات التدبير لامتلاك الأصل الثابت.</span><span class="sxs-lookup"><span data-stu-id="24e33-118">Either non-stocked items or procurement categories can be used for fixed asset acquisition.</span></span>

9.  <span data-ttu-id="24e33-119">في القائمة، حدد صنفاً مثل **C0003**.</span><span class="sxs-lookup"><span data-stu-id="24e33-119">In the list, select an item, such as **C0003**.</span></span>
10. <span data-ttu-id="24e33-120">في الحقل **كمية**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="24e33-120">In the **Quantity** field, enter a number.</span></span>

    <span data-ttu-id="24e33-121">سيقوم بند فاتورة واحد بإنشاء أصل ثابت واحد فقط، بغض النظر عن الكمية.</span><span class="sxs-lookup"><span data-stu-id="24e33-121">One invoice line will only create one fixed asset, regardless of quantity.</span></span> <span data-ttu-id="24e33-122">سيتم تحويل قيمة حقل كمية الفواتير إلى كمية الأصل الثابت.</span><span class="sxs-lookup"><span data-stu-id="24e33-122">The invoice quantity field value will be transferred to the fixed asset quantity.</span></span>

11.  <span data-ttu-id="24e33-123">في حقل **سعر الوحدة**، أدخل رقماً.</span><span class="sxs-lookup"><span data-stu-id="24e33-123">In the **Unit price** field, enter a number.</span></span>
12.  <span data-ttu-id="24e33-124">قم بتوسيع قسم **‎‏‫تفاصيل البند** أو طيه.</span><span class="sxs-lookup"><span data-stu-id="24e33-124">Expand or collapse the **Line details** section.</span></span>
13.  <span data-ttu-id="24e33-125">حدد علامة التبويب **الأصول الثابتة**.</span><span class="sxs-lookup"><span data-stu-id="24e33-125">Select the **Fixed assets** tab.</span></span>
14.  <span data-ttu-id="24e33-126">قم بتمكين الخيار **إنشاء أصل ثابت جديد**.</span><span class="sxs-lookup"><span data-stu-id="24e33-126">Enable the **Create a new fixed asset** option.</span></span>
15.  <span data-ttu-id="24e33-127">في الحقل **مجموعة الأصول الثابتة**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="24e33-127">In the **Fixed asset group** field, select the drop-down button to open the lookup.</span></span>
16.  <span data-ttu-id="24e33-128">في القائمة، حدد مجموعة الأصول الثابتة المطلوب استخدامها عند إنشاء الأصل الثابت الجديد.</span><span class="sxs-lookup"><span data-stu-id="24e33-128">In the list, select the fixed asset group to be used when you are creating the new fixed asset.</span></span>
17.  <span data-ttu-id="24e33-129">في القائمة، انقر على الارتباط في الصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="24e33-129">In the list, click the link in the selected row.</span></span>
18.  <span data-ttu-id="24e33-130">انقر على **نشر**.</span><span class="sxs-lookup"><span data-stu-id="24e33-130">Click **Post**.</span></span> <span data-ttu-id="24e33-131">سيتم إنشاء الأصل الثابت والحصول عليه عند ترحيل الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="24e33-131">The fixed asset will be created and acquired when the invoice is posted.</span></span>

<span data-ttu-id="24e33-132">[![لقطة شاشة لفاتورة المورد التي تم إنشاؤها.](../media/fa-create-vendor-invoice.png)](../media/fa-create-vendor-invoice.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="24e33-132">[![Screenshot of the vendor invoice that has been created.](../media/fa-create-vendor-invoice.png)](../media/fa-create-vendor-invoice.png#lightbox)</span></span>



