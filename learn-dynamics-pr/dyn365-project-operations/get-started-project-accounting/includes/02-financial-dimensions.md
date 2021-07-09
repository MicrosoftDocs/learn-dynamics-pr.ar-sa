---
ms.openlocfilehash: df5639e65f8feb1d68d29dfd86376d543bdcadc0
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6072947"
---
<span data-ttu-id="32304-101">يستخدم Project Operations إطار عمل [الأبعاد المالية](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions/?azure-portal=true) في Dynamics 365 Finance لتوفير رؤى إضافية بشأن معاملات دفتر الأستاذ العام ودفتر الأستاذ الفرعي للمشروع.</span><span class="sxs-lookup"><span data-stu-id="32304-101">Project Operations uses the [Financial dimensions](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions/?azure-portal=true) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="32304-102">يمكن إعداد الأبعاد المالية الافتراضية في العميل أو مصدر تمويل المشروع أو الحدث الرئيسي أو بند عقد المشروع أو المشروع.</span><span class="sxs-lookup"><span data-stu-id="32304-102">Default financial dimensions can be set up on a customer, project funding source, milestone, project contract line, or project.</span></span>

![لقطه لعلامة التبويب "مصادر التمويل"، توضح الأبعاد المالية.](../media/funding-sources-ss.png)

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="32304-104">تحديد الأبعاد المالية الافتراضية لعميل</span><span class="sxs-lookup"><span data-stu-id="32304-104">Define default financial dimensions for a customer</span></span>
<span data-ttu-id="32304-105">يتم تحديد القيم الافتراضية لأبعاد العميل في التمويل.</span><span class="sxs-lookup"><span data-stu-id="32304-105">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="32304-106">أكمل الخطوات التالية لتعيين افتراضيات الأبعاد:</span><span class="sxs-lookup"><span data-stu-id="32304-106">Complete the following steps to set dimension defaults:</span></span>

1.  <span data-ttu-id="32304-107">انتقل إلى **الحسابات المدينة > العملاء > كافة العملاء**.</span><span class="sxs-lookup"><span data-stu-id="32304-107">Go to **Accounts receivable > Customers > All customers**.</span></span>
2.  <span data-ttu-id="32304-108">في صفحة **العملاء**، ضمن علامة التبويب **الأبعاد المالية**، قم بتعيين قيم الأبعاد المالية لعميل محدد.</span><span class="sxs-lookup"><span data-stu-id="32304-108">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for a specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="32304-109">تحديد الأبعاد المالية الافتراضية لعقود المشروع</span><span class="sxs-lookup"><span data-stu-id="32304-109">Define default financial dimensions for project contracts</span></span>
<span data-ttu-id="32304-110">يتم إنشاء عقود المشروع والمحافظة عليها في Microsoft Dataverse.</span><span class="sxs-lookup"><span data-stu-id="32304-110">Project contracts are created and maintained in Microsoft Dataverse.</span></span> <span data-ttu-id="32304-111">يتم تعيين سمات المحاسبة لعقود المشروع في الوحدة النمطية لإدارة المشاريع والمحاسبة في الشؤون المالية.</span><span class="sxs-lookup"><span data-stu-id="32304-111">Accounting attributes for project contracts are set in the Project management and accounting module in Finance.</span></span>

## <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="32304-112">تعيين الأبعاد المالية لمصدر تمويل مشروع</span><span class="sxs-lookup"><span data-stu-id="32304-112">Set financial dimensions for a project funding source</span></span>
<span data-ttu-id="32304-113">لتعيين الأبعاد المالية لمصدر تمويل مشروع، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="32304-113">To set financial dimensions for a project funding source, follow these steps:</span></span>

1.  <span data-ttu-id="32304-114">انتقل إلى **إدارة المشاريع والمحاسبة > المشاريع > عقود المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="32304-114">Go to **Project management and accounting > Projects > Project contracts**.</span></span>
2.  <span data-ttu-id="32304-115">حدد السجل الذي ترغب في تحديثه، وفي علامة التبويب **عقد المشروع**، حدد **إظهار المحاسبة الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="32304-115">Select the record that you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3.  <span data-ttu-id="32304-116">قم بتوسيع **المعلومات ذات الصلة** وحدد علامة التبويب **مصادر التمويل**.</span><span class="sxs-lookup"><span data-stu-id="32304-116">Expand **Related information** and select the **Funding sources** tab.</span></span>
4.  <span data-ttu-id="32304-117">قم بتعيين افتراضيات الأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="32304-117">Set the financial dimension defaults.</span></span> <span data-ttu-id="32304-118">لاحظ أنّ الأبعاد المالية تتخلف عن حساب العميل.</span><span class="sxs-lookup"><span data-stu-id="32304-118">Notice that the financial dimensions default from the customer account.</span></span>

## <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="32304-119">قم بتعيين الأبعاد المالية لبند عقد مشروع</span><span class="sxs-lookup"><span data-stu-id="32304-119">Set financial dimensions for a project contract line</span></span>
<span data-ttu-id="32304-120">لتعيين الأبعاد المالية لبند عقد مشروع، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="32304-120">To set financial dimensions for a project contract line, follow these steps:</span></span>

1.  <span data-ttu-id="32304-121">انتقل إلى **إدارة المشاريع والمحاسبة > المشاريع > عقود المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="32304-121">Go to **Project management and accounting > Projects > Project contracts**.</span></span>
2.  <span data-ttu-id="32304-122">حدد السجل الذي ترغب في تحديثه، وفي علامة التبويب **عقد المشروع**، حدد **إظهار المحاسبة الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="32304-122">Select the record that you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3.  <span data-ttu-id="32304-123">قم بتوسيع **المعلومات ذات الصلة** وحدد علامة التبويب **بنود العقد**.</span><span class="sxs-lookup"><span data-stu-id="32304-123">Expand **Related information** and select the **Contract lines** tab.</span></span>
4.  <span data-ttu-id="32304-124">قم بتعيين افتراضيات الأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="32304-124">Set the financial dimension defaults.</span></span> <span data-ttu-id="32304-125">تكون افتراضيات الأبعاد المالية قابلة للتطبيق ويمكن استخدامها فقط مع بنود العقود الخاصة **بالسعر الثابت (الحدث الرئيسي)**.</span><span class="sxs-lookup"><span data-stu-id="32304-125">The financial dimension defaults are applicable and can be used only with **Fixed price (milestone)** contract lines.</span></span>

<span data-ttu-id="32304-126">يتم استخدام هذه الإعدادات الافتراضية في بنود الفواتير والمعاملات على الحساب الخاصة بالمشروع ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="32304-126">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="32304-127">تحديد الأبعاد المالية الافتراضية للمشاريع</span><span class="sxs-lookup"><span data-stu-id="32304-127">Define default financial dimensions for projects</span></span>
<span data-ttu-id="32304-128">يتم إنشاء المشاريع والمحافظة عليها في Microsoft Dataverse.</span><span class="sxs-lookup"><span data-stu-id="32304-128">Projects are created and maintained in Microsoft Dataverse.</span></span> <span data-ttu-id="32304-129">يتم تعيين سمات المحاسبة للمشاريع في الوحدة النمطية لإدارة المشاريع والمحاسبة في الشؤون المالية.</span><span class="sxs-lookup"><span data-stu-id="32304-129">Accounting attributes for projects are set in the Project management and accounting module in Finance.</span></span>

1.  <span data-ttu-id="32304-130">انتقل إلى **إدارة المشاريع والمحاسبة > المشاريع > كل المشاريع**.</span><span class="sxs-lookup"><span data-stu-id="32304-130">Go to **Project management and accounting > Projects > All projects**.</span></span>
2.  <span data-ttu-id="32304-131">حدد السجل الذي ترغب في تحديثه، وفي علامة التبويب **المشروع**، حدد **إظهار المحاسبة الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="32304-131">Select the record that you want to update, and on the **Project** tab, select **Show default accounting**.</span></span>
3.  <span data-ttu-id="32304-132">قم بتوسيع **المعلومات ذات الصلة** وحدد علامة التبويب **الإعداد**.</span><span class="sxs-lookup"><span data-stu-id="32304-132">Expand **Related information** and select the **Setup** tab.</span></span>
4.  <span data-ttu-id="32304-133">قم بتعيين افتراضيات الأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="32304-133">Set the financial dimension defaults.</span></span> <span data-ttu-id="32304-134">لاحظ أن الأبعاد المالية تتخلف عن حساب العميل.</span><span class="sxs-lookup"><span data-stu-id="32304-134">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="32304-135">إذا كان المشروع مرتبطاً ببند عقد يحتوي على عملاء عقود مشاريع متعددين، فسيتم استخدام العميل الأساسي للتخلف عن الأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="32304-135">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="32304-136">يتم استخدام الأبعاد المالية الافتراضية للمشروع لتعيين افتراضيات سطر دفتر اليومية لمعاملات الوقت والمصروفات والرسوم في **دفتر يومية تكامل Project Operations** وفي بنود فواتير المشاريع ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="32304-136">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration journal** and on related project invoice lines.</span></span>

