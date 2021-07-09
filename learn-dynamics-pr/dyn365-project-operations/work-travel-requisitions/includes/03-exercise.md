---
ms.openlocfilehash: c943b67b6fce9fdbe9a065d08fde208f363fcf0b
ms.sourcegitcommit: 0a6b3a31165f421c2f7d3afb98b75c9100325f57
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2021
ms.locfileid: "6083627"
---
<span data-ttu-id="6d14d-101">لإجراء هذا التمرين، سيكون عليك الوصول إلى بيئة باستخدام Microsoft Dynamics 365 Project Operations أو Microsoft Dynamics 365 Finance مع بيانات العرض التوضيحي القياسية.</span><span class="sxs-lookup"><span data-stu-id="6d14d-101">To perform this exercise, you will need access to an environment with Microsoft Dynamics 365 Project Operations, or Microsoft Dynamics 365 Finance, with standard demo data.</span></span> <span data-ttu-id="6d14d-102">يمكنك الوصول إلى البيئة التجريبية لتطبيق Project Operations من خلال تحديد **الشروع في العمل** في أعلى الزاوية اليُمنى [من صفحة Dynamics 365 Project Operations على microsoft.com](https://dynamics.microsoft.com/project-operations/overview//?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="6d14d-102">You can access a trial environment of Project Operations by selecting **Get started** in the top-right corner of [the Dynamics 365 Project Operations page on microsoft.com](https://dynamics.microsoft.com/project-operations/overview//?azure-portal=true).</span></span>

<span data-ttu-id="6d14d-103">في هذا التمرين، ستنشئ طلب سفر مع بنود فئة مصروفات مفصلة ثم إرسال الطلب إلى سير عمل.</span><span class="sxs-lookup"><span data-stu-id="6d14d-103">In this exercise, you will create a travel requisition with detailed expense category lines and then submit the requisition to a workflow.</span></span> 

## <a name="scenario"></a><span data-ttu-id="6d14d-104">السيناريو</span><span class="sxs-lookup"><span data-stu-id="6d14d-104">Scenario</span></span>
<span data-ttu-id="6d14d-105">لديك زيارة مكتبية ربع سنوية مقبلة مجدولة في الشهر المقبل.</span><span class="sxs-lookup"><span data-stu-id="6d14d-105">You have an upcoming quarterly office visit scheduled for next month.</span></span> <span data-ttu-id="6d14d-106">نظراً لاقتراب نهاية العام، تتطلب جميع رحلات العمل طلب سفر معتمداً قبل السفر لضمان عدم تجاوز الموازنة.</span><span class="sxs-lookup"><span data-stu-id="6d14d-106">Because it is nearing year-end, all business trips require an approved travel requisition prior to traveling to ensure that the budget is not exceeded.</span></span> 

1.  <span data-ttu-id="6d14d-107">انتقل إلى **إدارة المصروفات > مصروفاتي > طلب السفر**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-107">Go to **Expense management > My expenses > Travel requisition**.</span></span>
2.  <span data-ttu-id="6d14d-108">حدد **طلب السفر الجديد**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-108">Select **New travel requisition**.</span></span>
3.  <span data-ttu-id="6d14d-109">في حقل **غرض الأعمال**، أدخل **زيارة مكتبية ربع سنوية**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-109">In the **Business purpose** field, enter **Quarterly office visit**.</span></span>
4.  <span data-ttu-id="6d14d-110">في حقل **الوجهة**، أدخل **ميامي، فلوريدا**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-110">In the **Destination** field, enter **Miami, Florida**.</span></span>
5.  <span data-ttu-id="6d14d-111">في حقل **وصف السفر**، أدخل **اجتماع ربع سنوي وزيارة مكتبية مع قسم التصنيع في مركز التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-111">In the **Travel description** field, enter **Quarterly meeting and office visit with the manufacturing department of the distribution center**.</span></span>
6.  <span data-ttu-id="6d14d-112">في علامة التبويب السريعة **بنود مصروفات طلب السفر**، حدد **مصروفات طلب جديدة**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-112">In the **Travel requisition expense lines** FastTab, select **New requisition expense**.</span></span>
7.  <span data-ttu-id="6d14d-113">في قائمة **فئة المصروفات**، حدد **فندق**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-113">In the **Expense category** list, select **Hotel**.</span></span>
8.  <span data-ttu-id="6d14d-114">في **التاريخ المقدر**، حدد **12 ديسمبر** للسنة الحالية.</span><span class="sxs-lookup"><span data-stu-id="6d14d-114">In the **Estimated date**, select **December 12** for the current year.</span></span>
9.  <span data-ttu-id="6d14d-115">في حقل **المبلغ المقدر**، أدخل **560**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-115">In the **Estimated amount** field, enter **560**.</span></span>
10. <span data-ttu-id="6d14d-116">في علامة التبويب السريعة **بنود مصروفات طلب السفر**، حدد **مصروفات طلب جديدة**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-116">In the **Travel requisition expense lines** FastTab, select **New requisition expense**.</span></span>
11. <span data-ttu-id="6d14d-117">في قائمة **فئة المصروفات**، حدد **الرحلات الجوية**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-117">In the **Expense category** list, select **Flights**.</span></span>
12. <span data-ttu-id="6d14d-118">في حقل **التاريخ المقدر**، حدد **12 ديسمبر** للسنة الحالية.</span><span class="sxs-lookup"><span data-stu-id="6d14d-118">In the **Estimated date** field, select **December 12** for the current year.</span></span>
13. <span data-ttu-id="6d14d-119">في حقل **المبلغ المقدر**، أدخل **350**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-119">In the **Estimated amount** field, enter **350**.</span></span>
14. <span data-ttu-id="6d14d-120">في علامة التبويب السريعة **بنود مصروفات طلب السفر**، حدد **مصروفات طلب جديدة**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-120">In the **Travel requisition expense lines** FastTab, select **New requisition expense**.</span></span>
15. <span data-ttu-id="6d14d-121">في قائمة **فئة المصروفات**، حدد **الوجبات**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-121">In the **Expense category** list, select **Meals**.</span></span>
16. <span data-ttu-id="6d14d-122">في حقل **التاريخ المقدر**، حدد **12 ديسمبر** للسنة الحالية.</span><span class="sxs-lookup"><span data-stu-id="6d14d-122">In the **Estimated date** field, select **December 12** for the current year.</span></span>
17. <span data-ttu-id="6d14d-123">في حقل **المبلغ المقدر**، أدخل **245**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-123">In the **Estimated amount** field, enter **245**.</span></span>
18. <span data-ttu-id="6d14d-124">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-124">Select **Save**.</span></span>
19. <span data-ttu-id="6d14d-125">حدد **سير العمل > ‏‏إرسال**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-125">Select **Workflow > Submit**.</span></span>
20. <span data-ttu-id="6d14d-126">في حقل **التعليق**، أدخل **يُرجى الموافقة على هذا الطلب**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-126">In the **Comment** field, enter **Approve this requisition please**.</span></span>
21. <span data-ttu-id="6d14d-127">حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="6d14d-127">Select **Submit**.</span></span>

