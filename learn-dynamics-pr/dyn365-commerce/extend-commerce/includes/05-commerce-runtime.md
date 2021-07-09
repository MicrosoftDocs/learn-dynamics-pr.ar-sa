---
ms.openlocfilehash: d55af91ea29eab579082cd7c08ca75e2746ae56d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070084"
---
<span data-ttu-id="bb4b1-101">يُعد Commerce runtime (CRT) بمثابة مجموعة من مكتبات ‎.NET المحمولة التي تحتوي على منطق الأعمال الأساسي لقناة التجارة ووظيفة التسعير.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-101">Commerce runtime (CRT) is a collection of portable .NET libraries that contain the core business logic for the commerce channel and pricing functionality.</span></span> <span data-ttu-id="bb4b1-102">لإضافة منطق الأعمال أو تعديله، يمكنك تخصيص CRT.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-102">To add or modify business logic, you can customize CRT.</span></span>  

<span data-ttu-id="bb4b1-103">تتكون خدمة CRT من مجموعة من واحد أو أكثر من الطلبات والاستجابات.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-103">CRT service consists of a group of one or more requests and responses.</span></span> <span data-ttu-id="bb4b1-104">ترسل نقطة البيع طلباً إلى خادم البيع بالتجزئة (RS)، والذي يستدعي بدوره CRT لتشغيل منطق الأعمال.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-104">POS sends a request to the Retail server (RS), which calls CRT to run the business logic.</span></span> <span data-ttu-id="bb4b1-105">تقوم خدمة CRT بمعالجة الطلب وإرسال الرد مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-105">CRT processes the request and sends back the response.</span></span>

## <a name="crt-extension-patterns"></a><span data-ttu-id="bb4b1-106">أنماط ملحق CRT</span><span class="sxs-lookup"><span data-stu-id="bb4b1-106">CRT extension patterns</span></span>

<span data-ttu-id="bb4b1-107">يمكنك تمديد CRT لتناسب سيناريوهات مختلفة من خلال اتباع أنماط تمديد CRT المدعومة.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-107">You can extend CRT for various scenarios by following the supported CRT extension patterns.</span></span> <span data-ttu-id="bb4b1-108">ملحقات CRT التالية مدعومة:</span><span class="sxs-lookup"><span data-stu-id="bb4b1-108">The following CRT extensions are supported:</span></span>

-  <span data-ttu-id="bb4b1-109">**إنشاء خدمة CRT جديدة** - إنشاء وظيفة أو ميزة جديدة.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-109">**Create a new CRT service** - Create a new functionality or feature.</span></span>

-  <span data-ttu-id="bb4b1-110">**تجاوز الخدمة الحالية** - يمكنك تجاوز وظيفة حالية أو تخصيصها وفقاً لسير العمل الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-110">**Override existing service** - You can override an existing functionality or customize it according to your business flow.</span></span> <span data-ttu-id="bb4b1-111">تجنب تجاوز المعالج.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-111">Avoid overriding the handler.</span></span> <span data-ttu-id="bb4b1-112">يمكنك تنفيذ معظم سيناريوهات تمديد خدمة CRT باستخدام المشغلات المسبقة أو اللاحقة.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-112">You can implement most of the CRT extension scenarios by using pre or post triggers.</span></span> <span data-ttu-id="bb4b1-113">التجاوز مطلوب فقط عندما تريد استبدال الوظيفة الحالية بالكامل.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-113">Overriding is required only when you want to completely replace the existing functionality.</span></span>

-  <span data-ttu-id="bb4b1-114">**المشغلات** - تشغيل منطق إضافي قبل أو بعد أي طلب.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-114">**Triggers** - Run additional logic before or after any request.</span></span>

## <a name="triggers"></a><span data-ttu-id="bb4b1-115">المشغلات</span><span class="sxs-lookup"><span data-stu-id="bb4b1-115">Triggers</span></span>
<span data-ttu-id="bb4b1-116">في ملحق التشغيل المسبق، يمكنك تنفيذ بعض إجراءات التحقق من الصحة والمنطق المخصص وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-116">In the pre-trigger extension, you can do some validation, custom logic, and so on.</span></span>
<span data-ttu-id="bb4b1-117">في ملحق التشغيل اللاحق، يمكنك إضافة بعض المعلومات المخصصة إلى الطلب ثم إرسالها إلى نقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-117">In the post-trigger extension, you can add some custom information to the request and then send it to POS.</span></span> <span data-ttu-id="bb4b1-118">وبدلاً من ذلك، يمكنك تعديل النتيجة التي تم إرجاعها من الوظيفة القياسية أو إنشاء منطق عمل إضافي.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-118">Alternatively, you can modify the result that is returned from the standard functionality or create some additional business logic.</span></span>

<span data-ttu-id="bb4b1-119">على سبيل المثال، تمنحك مشغلات CRT طريقة لتوسيع سير عمل CRT كما تتيح لك إمكانية إضافة منطق عمل قبل وبعد كل طلب CRT يتم تنفيذه.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-119">For example, CRT triggers give you a way to extend the CRT workflow and let you add business logic before and after every CRT request is implemented.</span></span> 

<span data-ttu-id="bb4b1-120">يتم تنفيذ الطريقتين التاليتين في ملحق التشغيل:</span><span class="sxs-lookup"><span data-stu-id="bb4b1-120">The following two methods are implemented in the trigger extension:</span></span>

- <span data-ttu-id="bb4b1-121">**OnExecuting** - تتم الاستعانة بهذه الطريقة قبل معالجة الطلب بواسطة **‎IRequestHandler** مطابق.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-121">**OnExecuting** - This method is invoked before a request has been processed by a corresponding **IRequestHandler** implementation.</span></span>

- <span data-ttu-id="bb4b1-122">**OnExecuted** - تتم الاستعانة بهذه الطريقة بعد معالجة الطلب بواسطة **‎IRequestHandler** مطابق.</span><span class="sxs-lookup"><span data-stu-id="bb4b1-122">**OnExecuted** - This method is invoked after the request has been processed by a corresponding **IRequestHandler** implementation.</span></span>

<span data-ttu-id="bb4b1-123">لمزيد من المعلومات، راجع [Commerce runtime (CRT) ‏‫وقابلية توسعة Retail Server‬](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/commerce-runtime-extensibility?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="bb4b1-123">For more information, see [Commerce runtime (CRT) and Retail Server extensibility](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/commerce-runtime-extensibility?azure-portal=true).</span></span>

