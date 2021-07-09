---
ms.openlocfilehash: 231d0daef7d922832660defc534245b28223085c
ms.sourcegitcommit: ad358034a3371aed45c7d4883e01645b232fa589
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2021
ms.locfileid: "6070426"
---
<span data-ttu-id="350e9-101">يمكن توسيع واجهة مستخدم نقطة البيع (POS) ومنطق الأعمال لإضافة وظائف مخصصة.</span><span class="sxs-lookup"><span data-stu-id="350e9-101">The point of sale (POS) user interface and business logic can be extended to add custom functionality.</span></span> 

<span data-ttu-id="350e9-102">تدعم واجهة مستخدم نقطة البيع (POS) أنماط الامتداد التالية:</span><span class="sxs-lookup"><span data-stu-id="350e9-102">The POS user interface supports the following extension patterns:</span></span>

-   <span data-ttu-id="350e9-103">**أزرار شريط التطبيق** - أضف أزراراً مخصصة إلى شريط التطبيقات في الصفحات المحددة.</span><span class="sxs-lookup"><span data-stu-id="350e9-103">**App bar buttons** - Add custom buttons to the app bar on selected pages.</span></span>
-   <span data-ttu-id="350e9-104">**مجموعات الأعمدة المخصصة** - استبدل أعمدة الشبكة بأعمدة مخصصة في الصفحات المحددة.</span><span class="sxs-lookup"><span data-stu-id="350e9-104">**Custom column sets** - Replace the grid columns with custom columns on selected pages.</span></span>
-   <span data-ttu-id="350e9-105">**عناصر تحكم مخصصة** - إضافة عناصر تحكم جديدة إلى الصفحات المحددة.</span><span class="sxs-lookup"><span data-stu-id="350e9-105">**Custom controls** - Add new controls to selected pages.</span></span>

<span data-ttu-id="350e9-106">لتوضيح هذه الوظيفة بشكل أفضل، ضع في اعتبارك الموقف الذي تحتاج فيه إلى إضافة عمود مخصص وأزرار شريط التطبيق في صفحة البحث **المنتجات** التي تعرض معلومات إضافية حول المنتج.</span><span class="sxs-lookup"><span data-stu-id="350e9-106">To illustrate this functionality better, consider a situation where you need to add a custom column and app bar buttons in the **Products** search page that display additional information about the product.</span></span> <span data-ttu-id="350e9-107">في صفحة **تفاصيل المنتج**، يجب إضافة عناصر تحكم مخصصة تعرض مدى توفر المنتج.</span><span class="sxs-lookup"><span data-stu-id="350e9-107">In the **Product details** page, you should add custom controls that will display the availability of the product.</span></span> 

<span data-ttu-id="350e9-108">تُظهر لقطة الشاشة التالية مثالاً على عمود مخصص وأزرار شريط التطبيق التي تمت إضافتها في نقاط البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-108">The following screenshot shows an example of a custom column and app bar buttons that have been added in POS.</span></span>

<span data-ttu-id="350e9-109">[ ![لقطة شاشة Dynamics 365 Commerce لصفحة "عملاء المنتجات".](../media/custom-column-and-bar-button-2-ssm.jpg) ](../media/custom-column-and-bar-button-2-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="350e9-109">[ ![Screenshot of the Dynamics 365 Commerce Products Customers page.](../media/custom-column-and-bar-button-2-ssm.jpg) ](../media/custom-column-and-bar-button-2-ssm.jpg#lightbox)</span></span>

 
<span data-ttu-id="350e9-110">تمت تسمية العمود المخصص بالتسمية **خصص**، وفي أسفل الصفحة مثال على أزرار شريط التطبيق المخصصة.</span><span class="sxs-lookup"><span data-stu-id="350e9-110">The custom column is named with the label **CUSTOM**, and at the bottom of the page is an example of custom app bar buttons.</span></span> <span data-ttu-id="350e9-111">في ملحق أزرار شريط التطبيق، يمكنك كتابة منطق مخصص للتنقل إلى طريقة عرض مختلفة ومنطق عمل وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="350e9-111">In the app bar buttons extension, you can write custom logic to navigate to a different view, business logic, and so on.</span></span> 

<span data-ttu-id="350e9-112">تُظهر لقطة الشاشة التالية مثالاً لعنصر تحكم مخصص في نقطة البيع POS يمكنك استخدامه لعرض معلومات مخصصة ذات صلة بالمنتج.</span><span class="sxs-lookup"><span data-stu-id="350e9-112">The following screenshot shows an example of a custom control in POS that you can use to display custom information that is related to the product.</span></span> 

<span data-ttu-id="350e9-113">[ ![لقطة شاشة Dynamics 365 Commerce لصفحة المنتجات.](../media/custom-control-3-ssm.jpg)](../media/custom-control-3-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="350e9-113">[ ![Screenshot of the Dynamics 365 Commerce Products page.](../media/custom-control-3-ssm.jpg)](../media/custom-control-3-ssm.jpg#lightbox)</span></span>

<span data-ttu-id="350e9-114">ليست كل طرق عرض نقاط البيع قابلة للتوسعة.</span><span class="sxs-lookup"><span data-stu-id="350e9-114">Not all POS views are extensible.</span></span> <span data-ttu-id="350e9-115">لمزيد من المعلومات، راجع [توسيع طرق عرض نقاط البيع لإضافة أعمدة مخصصة وأزرار شريط التطبيق](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-view-extension/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="350e9-115">For more information, see [Extend POS views to add custom columns and app bar buttons](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-view-extension/?azure-portal=true).</span></span> 

<span data-ttu-id="350e9-116">على سبيل المثال، إذا احتوت طريقة عرض نقطة البيع على شبكة، فيمكنك إضافة عمود مخصص فيها، ولكن لا يمكنك إضافة عنصر تحكم مخصص.</span><span class="sxs-lookup"><span data-stu-id="350e9-116">For example, if the POS view contains a grid, then you can add a custom column in it, but you can't add a custom control.</span></span> <span data-ttu-id="350e9-117">لا يمكن إضافة عناصر التحكم في طرق العرض التي تحتوي على شبكة.</span><span class="sxs-lookup"><span data-stu-id="350e9-117">Controls can't be added in views that contain a grid.</span></span> <span data-ttu-id="350e9-118">في طرق عرض POS UI الخاصة بإدارة خارج النطاق (OOB)، لا يمكنك إخفاء عناصر التحكم أو الأزرار، يمكنك فقط إضافة عناصر تحكم أو أزرار مخصصة جديدة.</span><span class="sxs-lookup"><span data-stu-id="350e9-118">In the Out-of-Band Management (OOB) POS UI views, you can't hide controls or buttons, you can only add new custom controls or buttons.</span></span>

## <a name="pos-business-logic-extension"></a><span data-ttu-id="350e9-119">ملحق منطق الأعمال نقطة البيع POS</span><span class="sxs-lookup"><span data-stu-id="350e9-119">POS business logic extension</span></span>

<span data-ttu-id="350e9-120">يمكن تمديد سير عمل نقطة البيع أو منطق الأعمال.</span><span class="sxs-lookup"><span data-stu-id="350e9-120">POS workflow or business logic can be extended.</span></span> <span data-ttu-id="350e9-121">تصف الأقسام التالية الأنماط المدعومة للامتدادات لتوسيع المنطق الحالي في نقاط البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-121">The following sections describe the supported patterns for extensions to extend the existing logic in POS.</span></span> <span data-ttu-id="350e9-122">على سبيل المثال، قد ترغب في تغيير كيفية التقاط الرقم التسلسلي في نقطة البيع، وتغيير المفتاح في تدفق الأسعار للعناصر، وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="350e9-122">For example, you might want to change how a serial number is captured in POS, change the key in price flow for items, and so on.</span></span> 

- <span data-ttu-id="350e9-123">**تمديد** - يوفر هذا النمط رموز الامتداد التالية التي يمكنك اختيارها وفقاً لاحتياجاتك:</span><span class="sxs-lookup"><span data-stu-id="350e9-123">**Extend** - This pattern provides the following extension codes that you can choose according to your needs:</span></span>

  - <span data-ttu-id="350e9-124">**المشغلات** - يمكن أن يضيف كود الامتداد منطقاً سابقاً أو منطقاً لاحقاً قبل عمليات نقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-124">**Triggers** - The extension code can add pre or post logic before POS operations.</span></span>
  - <span data-ttu-id="350e9-125">**تجاوز معالجات** - يمكن أن يتجاوز كود الامتداد معالجات نقاط البيع لإضافة منطق عمل مخصص.</span><span class="sxs-lookup"><span data-stu-id="350e9-125">**Override handlers** - The extension code can override POS handlers to add custom business logic.</span></span>

- <span data-ttu-id="350e9-126">**الاستهلاك** - إذا كان الملحق ينشئ وظائف جديدة في نقاط البيع، فيمكن للإضافة أن تستهلك بعض واجهات برمجة التطبيقات الحالية أو APIs في نقاط البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-126">**Consume** - If the extension is creating new functionality in POS, then the extension can consume some of the existing APIs or controls in POS.</span></span> <span data-ttu-id="350e9-127">على سبيل المثال، إذا كنت تريد إضافة العنصر إلى سلة التسوق، فيمكن للملحق استخدام **إضافة صنف إلى عربة التسوق** API بدلاً من الاضطرار إلى إنشاء منطق مخصص لإضافة الصنف.</span><span class="sxs-lookup"><span data-stu-id="350e9-127">For example, if you want to add the item to the cart, then the extension can use the **AddItemToCart** API instead of you having to create custom logic to add the item.</span></span>

- <span data-ttu-id="350e9-128">**واجهات برمجة التطبيقات (API) لنقاط البيع** - يمكن أن تستهلك الإضافة واجهات برمجة التطبيقات (API) لنقاط البيع في كود الامتداد.</span><span class="sxs-lookup"><span data-stu-id="350e9-128">**POS APIs** - Extension can consume POS APIs in the extension code.</span></span>

- <span data-ttu-id="350e9-129">**POS UI SDK** - يمكن للإضافة أن تستهلك عناصر التحكم في نقاط البيع ومربعات الحوار في عروض الامتداد.</span><span class="sxs-lookup"><span data-stu-id="350e9-129">**POS UI SDK** - Extension can consume POS controls and dialogs in the extension views.</span></span>

## <a name="pos-extension-samples"></a><span data-ttu-id="350e9-130">عينات تمديد نقاط البيع</span><span class="sxs-lookup"><span data-stu-id="350e9-130">POS extension samples</span></span>

<span data-ttu-id="350e9-131">راجع صفحات التوثيق التالية للاطلاع على سيناريوهات ونماذج مختلفة لتمديد نقاط البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-131">See the following documentation pages for various POS extension scenarios and samples.</span></span>

### <a name="user-interface"></a><span data-ttu-id="350e9-132">واجهة المستخدم</span><span class="sxs-lookup"><span data-stu-id="350e9-132">User interface</span></span>

<span data-ttu-id="350e9-133">بالنسبة لسيناريوهات تمديد نقاط البيع ونماذج لواجهة المستخدم، حدد الروابط التالية:</span><span class="sxs-lookup"><span data-stu-id="350e9-133">For POS extension scenarios and samples for the UI, select the following links:</span></span>

-  [<span data-ttu-id="350e9-134">إضافة أعمدة مخصصة إلى شبكة معاملات نقطة البيع (POS)</span><span class="sxs-lookup"><span data-stu-id="350e9-134">Add custom columns to a point of sale (POS) transaction grid</span></span>](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-custom-transaction-column/?azure-portal=true)

-  <span data-ttu-id="350e9-135">[توسيع طرق عرض نقاط البيع لإضافة أعمدة مخصصة وأزرار شريط التطبيق](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-view-extension/?azure-portal=true) - بالنسبة إلى طرق العرض القائمة على مصمم تخطيط غير الشاشة.</span><span class="sxs-lookup"><span data-stu-id="350e9-135">[Extend POS views to add custom columns and app bar buttons](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-view-extension/?azure-portal=true) - For non-screen layout designer- based views.</span></span> 

-  [<span data-ttu-id="350e9-136">إضافة عناصر تحكم مخصصة إلى عروض نقاط البيع</span><span class="sxs-lookup"><span data-stu-id="350e9-136">Add custom controls to POS views</span></span>]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-custom-control/?azure-portal=true)   


### <a name="workflow"></a><span data-ttu-id="350e9-137">سير العمل</span><span class="sxs-lookup"><span data-stu-id="350e9-137">Workflow</span></span>

<span data-ttu-id="350e9-138">بالنسبة لسيناريوهات تمديد نقاط البيع ونماذج لسير العمل، حدد الارتباطات التالية:</span><span class="sxs-lookup"><span data-stu-id="350e9-138">For POS extension scenarios and samples for the workflow, select the following links:</span></span>

-  <span data-ttu-id="350e9-139">[مشغلات نقاط البيع]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-trigger-printing/?azure-portal=true) - لإضافة المشغلات السابقة واللاحقة في عمليات نقاط البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-139">[POS Triggers]( https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-trigger-printing/?azure-portal=true) - To add pre and post-triggers in POS operations.</span></span> 

-  <span data-ttu-id="350e9-140">[واجهات برمجة تطبيقات نقاط البيع (POS)](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-apis/?azure-portal=true) - للتعرف على كيفية استهلاك واجهات برمجة تطبيقات نقاط البيع في سيناريوهات الإضافات.</span><span class="sxs-lookup"><span data-stu-id="350e9-140">[Point of sale (POS) APIs](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-apis/?azure-portal=true) - To learn how to consume POS APIs in extension scenarios.</span></span>

-  <span data-ttu-id="350e9-141">[تجاوز معالج طلب نقاط البيع](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-handler/?azure-portal=true) - لمعرفة كيفية تجاوز منطق عمل نقاط البيع.</span><span class="sxs-lookup"><span data-stu-id="350e9-141">[Override POS request handler](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/pos-handler/?azure-portal=true) - To learn how to override POS business logic.</span></span> 



