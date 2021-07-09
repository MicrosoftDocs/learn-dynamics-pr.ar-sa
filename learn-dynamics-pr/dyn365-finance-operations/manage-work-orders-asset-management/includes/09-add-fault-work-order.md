---
ms.openlocfilehash: e65b488d058840c2475c090119a2bf2fb4fc8562
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072383"
---
<span data-ttu-id="63878-101">في جميع أوامر العمل، يمكنك إضافة خطأ محدد تم إنشاؤه للأصل المعين.</span><span class="sxs-lookup"><span data-stu-id="63878-101">On all work orders, you can add a specific fault that has been created for the particular asset.</span></span> <span data-ttu-id="63878-102">ويتم إعداد هذه الأخطاء في مصمم الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="63878-102">These faults are set up in the fault designer.</span></span> <span data-ttu-id="63878-103">لمعرفة المزيد، انتقل إلى [إدارة الأخطاء](https://docs.microsoft.com/dynamics365/supply-chain/asset-management/setup-for-work-orders/fault-management/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="63878-103">To learn more, go to [Fault management](https://docs.microsoft.com/dynamics365/supply-chain/asset-management/setup-for-work-orders/fault-management/?azure-portal=true).</span></span> 

<span data-ttu-id="63878-104">يتم إعداد الأخطاء حسب أنواع الأصول.</span><span class="sxs-lookup"><span data-stu-id="63878-104">Faults are set up by asset types.</span></span> <span data-ttu-id="63878-105">ومن ثَمَّ، عند إنشاء أمر عمل لأحد الأصول، ستتوفر فقط لهذا التحديد الأخطاء التي تم تعيينها لأنواع الأصول.</span><span class="sxs-lookup"><span data-stu-id="63878-105">Thus, when you create a work order for an asset, only the faults that are assigned to those asset types will be available for selection.</span></span> <span data-ttu-id="63878-106">على سبيل المثال، في أمر العمل الموضح في لقطة الشاشة الآتية، يكون الأصل هو "أداة الإنشاء" باستخدام نوع الأصل الخاص بـ "أداة الإنشاء".</span><span class="sxs-lookup"><span data-stu-id="63878-106">For example, in the work order shown in the following screenshot, the asset is a Generator with the asset type of Generator.</span></span>  

<span data-ttu-id="63878-107">**إدارة الأصول > عام > أوامر العمل > جميع أوامر العمل**</span><span class="sxs-lookup"><span data-stu-id="63878-107">**Asset management > Common > Work orders > All work orders**</span></span>

<span data-ttu-id="63878-108">[![لقطة شاشة لأخطاء الأصول في صفحة جميع أوامر العمل.](../media/asset-fault-setup-ssm.png)](../media/asset-fault-setup-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63878-108">[![Screenshot of the Asset fault on the all work orders page.](../media/asset-fault-setup-ssm.png)](../media/asset-fault-setup-ssm.png#lightbox)</span></span>
 
<span data-ttu-id="63878-109">في الصفحة **أخطاء الأصول**، يمكنك تحديد **الأعراض** و **أسباب الأعراض المحددة** و **الحلول الخاصة بالأعراض المحددة** لأنه تم إعدادها في **مصمم الخطأ**.</span><span class="sxs-lookup"><span data-stu-id="63878-109">In the **Asset faults** page, you can select the **Symptoms**, **Causes for selected symptom**, and **Remedies for selected symptom** because they were set up in the **Fault designer**.</span></span>

## <a name="create-a-fault"></a><span data-ttu-id="63878-110">إنشاء خطأ</span><span class="sxs-lookup"><span data-stu-id="63878-110">Create a fault</span></span>
<span data-ttu-id="63878-111">قبل أن تتمكن من إضافة خطأ لأمر العمل، يجب إنشاء الخطأ.</span><span class="sxs-lookup"><span data-stu-id="63878-111">Before you can add a fault for a work order, you need to create the fault.</span></span>

1.  <span data-ttu-id="63878-112">انتقل إلى **إدارة الأصول > الإعداد > الخطأ > مصمم الخطأ**.</span><span class="sxs-lookup"><span data-stu-id="63878-112">Go to **Asset management > Setup > Fault > Fault designer**.</span></span>
2.  <span data-ttu-id="63878-113">ضع المؤشر على **الرافعة الشوكية**.</span><span class="sxs-lookup"><span data-stu-id="63878-113">Place your cursor on **Forklift**.</span></span>
3.  <span data-ttu-id="63878-114">في القائمة العليا، حدد **إنشاء مجموعات الأخطاء**.</span><span class="sxs-lookup"><span data-stu-id="63878-114">On the top menu, select **Create fault combinations**.</span></span>
4.  <span data-ttu-id="63878-115">في مربع الحوار، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="63878-115">In the dialog box, select **OK**.</span></span>
5.  <span data-ttu-id="63878-116">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="63878-116">Close the page.</span></span>

## <a name="add-a-fault-to-a-work-order"></a><span data-ttu-id="63878-117">إضافة خطأ إلى أمر العمل</span><span class="sxs-lookup"><span data-stu-id="63878-117">Add a fault to a work order</span></span>
<span data-ttu-id="63878-118">والآن بعد أن تعرفت على كيفية إنشاء خطأ، اتبع الخطوات الآتية لإضافة خطأ إلى أمر العمل.</span><span class="sxs-lookup"><span data-stu-id="63878-118">Now that you know how to create a fault, follow these steps to add a fault to a work order.</span></span>

1.  <span data-ttu-id="63878-119">انتقل إلى **إدارة الأصول > عام > أوامر العمل > جميع أوامر العمل**.</span><span class="sxs-lookup"><span data-stu-id="63878-119">Go to **Asset management > Common > Work orders > All work orders**.</span></span>
2.  <span data-ttu-id="63878-120">حد أمر عمل.</span><span class="sxs-lookup"><span data-stu-id="63878-120">Select a work order.</span></span>
3.  <span data-ttu-id="63878-121">في القسم **الأصل**، حدد **خطأ الأصل‬**.</span><span class="sxs-lookup"><span data-stu-id="63878-121">In the **Asset** section, select **Asset fault**.</span></span> <span data-ttu-id="63878-122">تظهر الصفحة **خطأ الأصل**‬.</span><span class="sxs-lookup"><span data-stu-id="63878-122">The **Asset fault** page appears.</span></span>
4.  <span data-ttu-id="63878-123">في علامة التبويب السريعة **الأعراض**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="63878-123">In the **Symptom** FastTab, select **Add line**.</span></span>
5.  <span data-ttu-id="63878-124">في الحقل **أعراض الأخطاء**، حدد **مصهر محترق**.</span><span class="sxs-lookup"><span data-stu-id="63878-124">In the **Fault symptom** field, select **Blown fuse**.</span></span>
6.  <span data-ttu-id="63878-125">في الحقل **منطقة الخطأ**، أدخل **كهربائي**.</span><span class="sxs-lookup"><span data-stu-id="63878-125">In the **Fault area** field, select **Electrical**.</span></span>
7.  <span data-ttu-id="63878-126">في الحقل **نوع الخطأ**، أدخل **ضار**.</span><span class="sxs-lookup"><span data-stu-id="63878-126">In the **Fault type** field, select **Harmful**.</span></span>
8.  <span data-ttu-id="63878-127">في علامة التبويب السريعة **أسباب الأعراض المحددة**، حدد **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="63878-127">On the **Causes for selected symptom** FastTab, select **Add line**.</span></span>
9.  <span data-ttu-id="63878-128">في الحقل **سبب الخطأ**، حدد **مصهر معيب**.</span><span class="sxs-lookup"><span data-stu-id="63878-128">In the **Fault cause** field, select **Faulty fuse**.</span></span>
10. <span data-ttu-id="63878-129">أغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="63878-129">Close the page.</span></span>

    <span data-ttu-id="63878-130">[![لقطة شاشة لـ "أخطاء الأصول" مع أسباب وحلول الأعراض المحددة.](../media/asset-faults-ssm.png)](../media/asset-faults-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63878-130">[![Screenshot of the Asset faults with causes and remedies for selected symptom.](../media/asset-faults-ssm.png)](../media/asset-faults-ssm.png#lightbox)</span></span>
 
<span data-ttu-id="63878-131">سيظهر كل خطأ يتم إنشاؤه على أحد أوامر العمل في صفحة الاستعلام، والتي يمكنك العثور عليها بالانتقال إلى **إدارة الأصول > الاستعلامات > خطأ الأصل > أخطاء الأصول**.</span><span class="sxs-lookup"><span data-stu-id="63878-131">Each fault that is created on a work order will appear on an inquiry page, which you can find by going to **Asset management > Inquiries > Asset fault > Asset faults**.</span></span>

<span data-ttu-id="63878-132">[![لقطة شاشة لطريقة عرض "استعلامات أخطاء الأصول".](../media/asset-faults-inquiries-ss.png)](../media/asset-faults-inquiries-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63878-132">[![Screenshot of the Asset faults inquiries view.](../media/asset-faults-inquiries-ss.png)](../media/asset-faults-inquiries-ss.png#lightbox)</span></span>
 
<span data-ttu-id="63878-133">بالإضافة إلى ذلك، في الصفحة **إدارة الأصول > عام > الأصول > تفاصيل كل الأصول** لأحد الأصول، في علامة التبويب **عام**، يمكنك إنشاء تقرير حول جميع الأخطاء التي تم تسجيلها لأحد الأصول.</span><span class="sxs-lookup"><span data-stu-id="63878-133">In addition, on the **Asset management > Common > Assets > All asset detail** page for an asset, on the **General** tab, you can generate a report on all faults that are recorded for an asset.</span></span> 

<span data-ttu-id="63878-134">[![لقطة شاشة لتفاصيل تقرير "خطأ الأصل".](../media/all-faults-ss.png)](../media/all-faults-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63878-134">[![Screenshot of the Asset fault report details.](../media/all-faults-ss.png)](../media/all-faults-ss.png#lightbox)</span></span>