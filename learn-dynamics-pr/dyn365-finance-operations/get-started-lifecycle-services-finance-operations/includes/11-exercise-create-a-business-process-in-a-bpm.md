---
ms.openlocfilehash: 64f8b155af052be351293e3fcdc9555fd74e75ce
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071906"
---

<span data-ttu-id="e666a-101">أنت ترغب في استيراد مكتبة العملية التجارية العمومية إلى مشروع Lifecycle Services (LCS) وتعديل المكتبة لتقديم عمليات جديدة لطلب النقدية والاقتناء للدفع والماليات الأساسية.</span><span class="sxs-lookup"><span data-stu-id="e666a-101">You want to import a global business process library to your Lifecycle Services (LCS) project and modify the library to introduce new processes for order to cash, procure to pay, and core financials.</span></span> <span data-ttu-id="e666a-102">للقيام بذلك، يجب عليك:</span><span class="sxs-lookup"><span data-stu-id="e666a-102">To do this, you must:</span></span>

- <span data-ttu-id="e666a-103">انسخ مكتبة عمليات تجارية.</span><span class="sxs-lookup"><span data-stu-id="e666a-103">Copy a business process library.</span></span> 
- <span data-ttu-id="e666a-104">قم بإنشاء مكتبة العمليات التجارية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="e666a-104">Create your own business process library.</span></span>

### <a name="copy-a-business-process-library"></a><span data-ttu-id="e666a-105">نسخ مكتبة عمليات تجارية</span><span class="sxs-lookup"><span data-stu-id="e666a-105">Copy a business process library</span></span> 

1.  <span data-ttu-id="e666a-106">انتقل إلى مدخل LCS ([https://lcs.dynamics.com/v2](https://lcs.dynamics.com/v2/?azure-portal=true)) وقم بتسجيل الدخول إلى مشروع LCS الخاص بك باستخدام الاسم المستعار الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="e666a-106">Go to the LCS portal ([https://lcs.dynamics.com/v2](https://lcs.dynamics.com/v2/?azure-portal=true)) and sign in to your LCS project by using your alias.</span></span> 
2.  <span data-ttu-id="e666a-107">حدد المشروع الذي قمت بإنشائه في بيئة السحابة التي تم نشرها في اشتراك Azure Pass الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="e666a-107">Select on your project that you created in the cloud environment that has been deployed on your Azure Pass subscription.</span></span> 
3.  <span data-ttu-id="e666a-108">من الصفحة **تفاصيل المشروع**، انتقل إلى القسم **أدوات إضافية**، وحدد تجانب **عملية الأعمال**، أو استخدم رمز القائمة وحدد "أداة تكوين عمليات الأعمال".</span><span class="sxs-lookup"><span data-stu-id="e666a-108">On the **Project details** page, go to the **More tools** section, and Select the **Business Process** tile, or use the menu icon and select “Business process modeler”.</span></span>
    > [!NOTE]
    >  <span data-ttu-id="e666a-109">ووفقا لنوع مشروع LCS، يمكن الوصول إلى قائمة **أداة تكوين عمليات الأعمال** إما من قسم الأدوات (الشريك الموجه) أو من رمز القائمة.</span><span class="sxs-lookup"><span data-stu-id="e666a-109">Depending on the type of LCS project, the **Business process modeler** menu can be accessed either from the Tools section (partner oriented) or from the menu icon.</span></span> 
4.  <span data-ttu-id="e666a-110">حدد **عرض هذه الصفحة في تجربة BPM المحدثة**.</span><span class="sxs-lookup"><span data-stu-id="e666a-110">Select **View this page in the updated BPM experience**.</span></span>
5.  <span data-ttu-id="e666a-111">حدد علامة القطع (...) لمكتبة **تطبيقات APQC Unified Library for Microsoft Finance and Operations (الخاصة بشهر مارس 2018) (لكل الصناعات)** وتحديد نسخ.</span><span class="sxs-lookup"><span data-stu-id="e666a-111">Select the ellipsis (…) for the **(March 2018 - All languages) APQC Unified Library for Microsoft Finance and Operations apps (Cross industry)** library and Select Copy.</span></span> 
6.  <span data-ttu-id="e666a-112">قم بإعادة تسمية المكتبة، ثم اختر **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="e666a-112">Rename the library and **Create**.</span></span> 
7.  <span data-ttu-id="e666a-113">ستتوفر مكتبة BPM الخاصة بك في القسم **مكتبات المشروعات** الجاهزة للاستخدام في مشروع LCS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="e666a-113">Your BPM library will be available in the **Project libraries** section, ready to be used in your LCS project.</span></span> 
8.  <span data-ttu-id="e666a-114">حدد المكتبة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="e666a-114">Select your new library.</span></span> 
9.  <span data-ttu-id="e666a-115">قم بمراجعة العمليات المتوفرة.</span><span class="sxs-lookup"><span data-stu-id="e666a-115">Review available processes.</span></span>

### <a name="create-your-own-business-process-library"></a><span data-ttu-id="e666a-116">إنشاء مكتبة العمليات التجارية الخاصة بك</span><span class="sxs-lookup"><span data-stu-id="e666a-116">Create your own business process library</span></span>
1.  <span data-ttu-id="e666a-117">حدد **مكتبة جديدة**.</span><span class="sxs-lookup"><span data-stu-id="e666a-117">Select **New Library**.</span></span>
2.  <span data-ttu-id="e666a-118">تعيين اسم وتحديد **إنشاء**</span><span class="sxs-lookup"><span data-stu-id="e666a-118">Assign a name and Select **Create**</span></span>
3.  <span data-ttu-id="e666a-119">حدد لوحة مكتبة جديدة.</span><span class="sxs-lookup"><span data-stu-id="e666a-119">Select your new library tile.</span></span>
4.  <span data-ttu-id="e666a-120">حدد **نموذج العملية الأساسية للأعمال**، ثم حدد **وضع التحرير** لإجراء تغيير على المكتبة.</span><span class="sxs-lookup"><span data-stu-id="e666a-120">Select **Sample Core Business process**, and then Select **Edit Mode** to make a change to the library.</span></span> 
5.  <span data-ttu-id="e666a-121">في اللوحة اليسرى، قم بتغيير اسم العملية **طلب نقدية**، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e666a-121">In the right panel, change the name of the process to **Order to Cash**, Select **Save**.</span></span> 
6.  <span data-ttu-id="e666a-122">حدد **إضافة عملية** وحدد **كتابع**.</span><span class="sxs-lookup"><span data-stu-id="e666a-122">Select **Add Process** and select **As Sibling**.</span></span> <span data-ttu-id="e666a-123">حدد **وضع التحرير** وقم بتغيير الاسم إلى "عملية التدبير إلى الدفع".</span><span class="sxs-lookup"><span data-stu-id="e666a-123">Select **Edit Mode** and change the name to ‘Procure to Pay’.</span></span> 
7.  <span data-ttu-id="e666a-124">كرر الخطوة السابقة على "الماليات الأساسية" و"عملية التدبير إلى الدفع".</span><span class="sxs-lookup"><span data-stu-id="e666a-124">Repeat the previous step for ‘Core Financials’ and ‘Procure to Pay’.</span></span>
8.  <span data-ttu-id="e666a-125">حدد **طلب النقدية** وأضف عملية ذات مستوى تابع.</span><span class="sxs-lookup"><span data-stu-id="e666a-125">Select **Order to Cash** and add a child-level process.</span></span> 
9.  <span data-ttu-id="e666a-126">حدد **إضافة عملية كفرعي** > **وضع التحرير** وقم بتغيير الاسم إلى "فاتورة نص حر"، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e666a-126">Select **Add Process As Child** > **Edit Mode** and change the name to “Free Text Invoice”, and then Select **Save**.</span></span> 
10. <span data-ttu-id="e666a-127">قم بإضافة العملية التالية ضمن **طلب النقدية** لـ "دفتر يومية الاستلام".</span><span class="sxs-lookup"><span data-stu-id="e666a-127">Add the next process under **Order to Cash** for ‘Receipt Journal’.</span></span>
11. <span data-ttu-id="e666a-128">يمكنك تغيير التسلسل بتحديد الخيار لنقل العملية.</span><span class="sxs-lookup"><span data-stu-id="e666a-128">You can change the sequence by selecting the option to move process.</span></span> 
12. <span data-ttu-id="e666a-129">كرر الخطوات السابقة لإضافة عمليات تابعة إلى العملية الأخرى كما يلي:</span><span class="sxs-lookup"><span data-stu-id="e666a-129">Repeat the previous steps to add child processes to the other process as follows:</span></span>

| <span data-ttu-id="e666a-130">العملية</span><span class="sxs-lookup"><span data-stu-id="e666a-130">Process</span></span> | <span data-ttu-id="e666a-131">عملية فرعية</span><span class="sxs-lookup"><span data-stu-id="e666a-131">Child process</span></span> |
 | ------------- | ------------- |
 | <span data-ttu-id="e666a-132">طلب نقدية</span><span class="sxs-lookup"><span data-stu-id="e666a-132">Order to Cash</span></span>  | <span data-ttu-id="e666a-133">دفتر يومية الاستلام، فاتورة ذات نص حر</span><span class="sxs-lookup"><span data-stu-id="e666a-133">Receipt journal,  Free Text invoice</span></span>  |
 | <span data-ttu-id="e666a-134">عملية التدبير إلى الدفع</span><span class="sxs-lookup"><span data-stu-id="e666a-134">Procure to Pay</span></span>  |    <span data-ttu-id="e666a-135">أمر الشراء، فاتورة المورد، دفع المورد</span><span class="sxs-lookup"><span data-stu-id="e666a-135">Purchase order, Vendor invoice, Vendor payment</span></span> |
| <span data-ttu-id="e666a-136">الماليات الأساسية</span><span class="sxs-lookup"><span data-stu-id="e666a-136">Core Financials</span></span> | <span data-ttu-id="e666a-137">دفتر اليومية العام، تشغيل التقارير المالية، نهاية الفترة</span><span class="sxs-lookup"><span data-stu-id="e666a-137">General journal, Run Financial reports, Period end</span></span>  |

    


