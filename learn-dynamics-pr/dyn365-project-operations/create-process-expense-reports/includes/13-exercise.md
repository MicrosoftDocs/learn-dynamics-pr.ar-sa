---
ms.openlocfilehash: c6170344780faf41106a36d5e2e7ad5e669b9842
ms.sourcegitcommit: 0a6b3a31165f421c2f7d3afb98b75c9100325f57
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2021
ms.locfileid: "6083610"
---
> [!NOTE]
> <span data-ttu-id="0e378-101">وتكون عملية إنشاء تقرير مصروفات في Finance and Operations بنفس الطريقة الموجودة في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0e378-101">The process for creating an expense report is the same in Finance and Operations as it is in Project Operations.</span></span> <span data-ttu-id="0e378-102">بالتالي، ستقوم بتنفيذ هذا المعمل في Finance and Operations، لأننا لا نمتلك حالياً بيئة Project Operations متوفرة في Microsoft Learn.</span><span class="sxs-lookup"><span data-stu-id="0e378-102">Therefore, you will perform this lab in Finance and Operations, as we do not currently have a Project Operations environment available on Microsoft Learn.</span></span>
> <span data-ttu-id="0e378-103">ومع ذلك، يمكنك الوصول إلى بيئة تجريبية لـ Project Operations عن طريق تحديد **بدء التشغيل** في الركن الأيمن العلوي من [صفحة Dynamics 365 Project Operations على microsoft.com](https://dynamics.microsoft.com/project-operations/overview//?azure-portal=true) إذا كنت تفضل تجربة المعمل هناك.</span><span class="sxs-lookup"><span data-stu-id="0e378-103">However, you can access a trial environment of Project Operations by selecting **Get started** in the top-right corner of [the Dynamics 365 Project Operations page on microsoft.com](https://dynamics.microsoft.com/project-operations/overview//?azure-portal=true) if you prefer to try the lab there.</span></span>

<span data-ttu-id="0e378-104">في هذا المعمل، ستقوم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="0e378-104">In this lab, you will:</span></span>

1. <span data-ttu-id="0e378-105">إنشاء تقرير مصروفات.</span><span class="sxs-lookup"><span data-stu-id="0e378-105">Create an expense report.</span></span>
1. <span data-ttu-id="0e378-106">إرفاق الإيصالات إلى تقرير المصروفات.</span><span class="sxs-lookup"><span data-stu-id="0e378-106">Attach receipts to an expense report.</span></span>
1. <span data-ttu-id="0e378-107">إرسال تقرير مصروفات إلى سير عمل.</span><span class="sxs-lookup"><span data-stu-id="0e378-107">Submit an expense report to a workflow.</span></span>

## <a name="scenario"></a><span data-ttu-id="0e378-108">السيناريو</span><span class="sxs-lookup"><span data-stu-id="0e378-108">Scenario</span></span>

<span data-ttu-id="0e378-109">لقد قمت للتو بالرجوع من مؤتمر أعمال في ناشفيل، تينيسي، وستقوم بإنشاء تقرير مصروفات.</span><span class="sxs-lookup"><span data-stu-id="0e378-109">You have just returned from a business conference in Nashville, Tennessee, and you will create an expense report.</span></span> <span data-ttu-id="0e378-110">عند إنشاء تقرير المصروفات، سيتم إرفاق إيصال الوجبات بتقرير المصروفات، ثم إرسال تقرير المصروفات إلى سير العمل.</span><span class="sxs-lookup"><span data-stu-id="0e378-110">When you’ve created the expense report, you will attach the meal receipt to the expense report and then submit the expense report to a workflow.</span></span>

## <a name="create-an-expense-report"></a><span data-ttu-id="0e378-111">إنشاء تقرير مصروفات</span><span class="sxs-lookup"><span data-stu-id="0e378-111">Create an expense report</span></span> 
<span data-ttu-id="0e378-112">لإنشاء تقرير مصروفات، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="0e378-112">To create an expense report, follow these steps:</span></span>

1.  <span data-ttu-id="0e378-113">انتقل إلى **إدارة المصروفات > مساحات العمل > إدارة المصروفات**.</span><span class="sxs-lookup"><span data-stu-id="0e378-113">Go to **Expense management > Workspaces > Expense management**.</span></span>
2.  <span data-ttu-id="0e378-114">حدد **تقرير مصروفات جديد**.</span><span class="sxs-lookup"><span data-stu-id="0e378-114">Select **New expense report**.</span></span>
3.  <span data-ttu-id="0e378-115">في الحقل **العنوان/الغرض**، أدخل **المؤتمر التجاري في أكتوبر**.</span><span class="sxs-lookup"><span data-stu-id="0e378-115">In the **Title/Purpose** field, enter **October trade conference**.</span></span>
5.  <span data-ttu-id="0e378-116">في حقل **الموقع**، أدخل **ناشفيل، تنيسي**.</span><span class="sxs-lookup"><span data-stu-id="0e378-116">In the **Location** field, enter **Nashville, TN**.</span></span> 
6.  <span data-ttu-id="0e378-117">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="0e378-117">Select **Create**.</span></span>
7.  <span data-ttu-id="0e378-118">في علامة التبويب **مصروفات**، حدد **مصروفات جديدة**.</span><span class="sxs-lookup"><span data-stu-id="0e378-118">In the **Expenses** tab, select **New expense**.</span></span>
8.  <span data-ttu-id="0e378-119">في القائمة **الفئة**، حدد **وجبة**.</span><span class="sxs-lookup"><span data-stu-id="0e378-119">In the **Category** menu, select **Meal**.</span></span>
9.  <span data-ttu-id="0e378-120">في حقل **المبلغ**، أدخِل **27.05**.</span><span class="sxs-lookup"><span data-stu-id="0e378-120">In the **Amount** field, enter **27.05**.</span></span>
10. <span data-ttu-id="0e378-121">في حقل **العملة**، حدد **دولار أمريكي**.</span><span class="sxs-lookup"><span data-stu-id="0e378-121">In the **Currency** field, select **USD**.</span></span>
11. <span data-ttu-id="0e378-122">في الحقل **التاريخ**، حدد **3 أكتوبر 2020**.</span><span class="sxs-lookup"><span data-stu-id="0e378-122">In the **Date** field, select **October 3, 2020**.</span></span>
12. <span data-ttu-id="0e378-123">في حقل **التاجر**، أدخل **Fourth Coffee**.</span><span class="sxs-lookup"><span data-stu-id="0e378-123">In the **Merchant** field, enter **Fourth Coffee**.</span></span> 
13. <span data-ttu-id="0e378-124">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0e378-124">Select **Save**.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="0e378-125">إرفاق الإيصالات إلى تقرير المصروفات</span><span class="sxs-lookup"><span data-stu-id="0e378-125">Attach receipts to an expense report</span></span>
<span data-ttu-id="0e378-126">لإرفاق إيصال إلى تقرير مصروفات، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="0e378-126">To attach a receipt to an expense report, follow these steps:</span></span>

1.  <span data-ttu-id="0e378-127">في تقرير المصروفات، حدد علامة التبويب **الإيصالات**.</span><span class="sxs-lookup"><span data-stu-id="0e378-127">On your expense report, select the **Receipts** tab.</span></span>
2.  <span data-ttu-id="0e378-128">حدد **إضافة إيصالات**.</span><span class="sxs-lookup"><span data-stu-id="0e378-128">Select **Add receipts**.</span></span>
3.  <span data-ttu-id="0e378-129">حدد الخيار **استعراض** ثم حدد **ملف الإيصال.pdf** من الكمبيوتر المكتبي.</span><span class="sxs-lookup"><span data-stu-id="0e378-129">Select **Browse** and then select the **receipt.pdf** file from the desktop.</span></span> <span data-ttu-id="0e378-130">وعادة ما يكون هذا الإيصال هو الإيصال الذي قمت بحفظه إلى الكمبيوتر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="0e378-130">Normally, this receipt would be one that you saved to your computer.</span></span>
4.  <span data-ttu-id="0e378-131">حدد **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="0e378-131">Select **Upload**.</span></span>
5.  <span data-ttu-id="0e378-132">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="0e378-132">Select **Close**.</span></span>

## <a name="submit-an-expense-report-to-a-workflow"></a><span data-ttu-id="0e378-133">إرسال تقرير مصروفات إلى سير عمل</span><span class="sxs-lookup"><span data-stu-id="0e378-133">Submit an expense report to a workflow</span></span> 
<span data-ttu-id="0e378-134">لإرسال تقرير مصروفات إلى سير عمل، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="0e378-134">To submit the expense report to a workflow, follow these steps:</span></span>

1.  <span data-ttu-id="0e378-135">في جزء الإجراءات الخاص بتقرير المصروفات، حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="0e378-135">On the Action Pane of the expense report, select **Submit**.</span></span>
2.  <span data-ttu-id="0e378-136">أدخل **الرجاء الموافقة** في مربع نص **التعليق**.</span><span class="sxs-lookup"><span data-stu-id="0e378-136">Enter **Please approve** in the **Comment** text box.</span></span>
3.  <span data-ttu-id="0e378-137">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="0e378-137">Select **Submit**.</span></span>

