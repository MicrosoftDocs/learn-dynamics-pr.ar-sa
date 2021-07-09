---
ms.openlocfilehash: 203ecd42dc7c441cb4d1a540c561ab07fe81bbad
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073500"
---

<span data-ttu-id="732ae-101">من الأهداف المهمة للشركة في عملية التحويل بدون فاقد هو تحسين القدرة على تسليم منتج تم تجميعه حسب الطلب أو بناؤه حسب الطلب في وقت إنتاج تنافسي.</span><span class="sxs-lookup"><span data-stu-id="732ae-101">An important company objective in the lean transformation process is improving the ability to deliver a product that is assembled-to-order or built-to-order with a competitive lead time.</span></span>

<span data-ttu-id="732ae-102">توفر وظيفة المتاح للتعهد (CTP) لمتلقي الأوامر معلومات دقيقة عند نقطة إدخال الأمر حول توفر المنتجات والمواد والموارد المطلوبة لاستيفاء طلب عميل خاص.</span><span class="sxs-lookup"><span data-stu-id="732ae-102">The Capable-to-Promise (CTP) functionality provides the order takers with accurate information at the point of order entry about the availability of products, material, and resources that are needed to satisfy a specific customer demand.</span></span>

<span data-ttu-id="732ae-103">يمكن أن تحدث هذه الوظيفة تلقائياً وقت إدخال الأمر أو في وظيفة دفعية بعد إدخال أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="732ae-103">This functionality can occur automatically at order entry time or in a batch job after the sales order has been entered.</span></span> <span data-ttu-id="732ae-104">يمكن تحديد مدي توفر الموارد للتصنيع محدود الفاقد lean manufacturing عن طريق تحميل وظائف كانبان في جدول وظائف كانبان المرتبطة بخلية عمل.</span><span class="sxs-lookup"><span data-stu-id="732ae-104">The availability of resources for lean manufacturing can be determined by loading the kanban jobs on the Kanban job schedule that are related to a work cell.</span></span> <span data-ttu-id="732ae-105">يتم تحديد مدي توفر المواد بواسطة تحديد إجمالي المكونات المطلوبة وتثبيت السعر، بطريقة مماثلة للتصنيع باستخدام أوامر الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="732ae-105">The availability of material is determined by explosion and pegging, similar to manufacturing with production orders.</span></span>

### <a name="delivery-date-control-ctp"></a><span data-ttu-id="732ae-106">للتحكم في تاريخ التسليم للمتاح للتعهد (CTP)</span><span class="sxs-lookup"><span data-stu-id="732ae-106">Delivery date control CTP</span></span>

<span data-ttu-id="732ae-107">يساعد التحكم في تاريخ التسليم للمتاح للتعهد (CTP) الشركات في التحقق من تاريخ الشحن المطلوب والتحديث المحتمل لتاريخ الشحن المؤكد في بند المبيعات حين تظهر مشكلة في استيفاء تاريخ الشحن المطلوب من العميل.</span><span class="sxs-lookup"><span data-stu-id="732ae-107">The CTP delivery date control helps companies verify the requested ship date and potentially update the confirmed ship date on a sales line where there is a problem fulfilling the customer-requested ship date.</span></span>

<span data-ttu-id="732ae-108">يتم تمكين هذه الميزة من خلال توسيع عنصر تحكم التسليم باستخدام خيار المتاح للتعهد (CTP) الذي يقوم بتشغيل عملية تحديد إجمالي المكونات المطلوبة للجدولة الرئيسية واستخدام تاريخ العمليات الآجلة الذي تم إرجاعه كتاريخ الشحن المقترح.</span><span class="sxs-lookup"><span data-stu-id="732ae-108">This feature is enabled by extending the existing delivery control with a CTP option that triggers a Master Scheduling explosion and uses the returned futures date as the suggested ship date.</span></span>

<span data-ttu-id="732ae-109">فيما يلي المتطلبات الأساسية لتشغيل تاريخ التسليم للمتاح للتعهد (CTP):</span><span class="sxs-lookup"><span data-stu-id="732ae-109">The prerequisites for running delivery date CTP are:</span></span>

-   <span data-ttu-id="732ae-110">يتم تعيين مفتاح التكوين الخاص بالتخطيط الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="732ae-110">The configuration key for Master Planning is set.</span></span>

-   <span data-ttu-id="732ae-111">يتم إعداد خطة ديناميكية وتعيينها إلى معلمات التخطيط الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="732ae-111">A dynamic plan is set up and assigned to the Master Planning parameters.</span></span>

-   <span data-ttu-id="732ae-112">يتم تكوين خطة ديناميكية لرسائل العمليات الآجلة.</span><span class="sxs-lookup"><span data-stu-id="732ae-112">A dynamic plan is configured for futures messages.</span></span>

-   <span data-ttu-id="732ae-113">تم حساب الخطط الثابتة والديناميكية.</span><span class="sxs-lookup"><span data-stu-id="732ae-113">The static and dynamic plans have been calculated.</span></span>

<span data-ttu-id="732ae-114">عند استخدام المتاح للتعهد (CTP) لمنتج محدد، يتم اقتراح المتطلبات الأساسية التالية:</span><span class="sxs-lookup"><span data-stu-id="732ae-114">Where CTP is used for a given product, the following prerequisites are suggested:</span></span>

-   <span data-ttu-id="732ae-115">إعداد مجموعة التغطية في حالة تمكين رسائل العمليات الآلية</span><span class="sxs-lookup"><span data-stu-id="732ae-115">Coverage group setting where Futures messages are enabled</span></span>

-   <span data-ttu-id="732ae-116">إعدادات الأمر الافتراضية مع وقت عميل هام للمبيعات يبلغ صفر من الأيام</span><span class="sxs-lookup"><span data-stu-id="732ae-116">Default order settings with a sales lead time of zero days</span></span>

-   <span data-ttu-id="732ae-117">إعدادات الأمر الافتراضية مع التحكم في تاريخ التسليم للمتاح للتعهد (CTP)</span><span class="sxs-lookup"><span data-stu-id="732ae-117">Default order settings with the delivery date control of CTP</span></span>

-   <span data-ttu-id="732ae-118">توجد قاعدة كانبان لحدث المبيعات المجدول أو التلقائي</span><span class="sxs-lookup"><span data-stu-id="732ae-118">A kanban rule exists for either scheduled or automatic sales event</span></span>

-   <span data-ttu-id="732ae-119">تعيين التخطيط التلقائي لقاعدة كانبان إلى **1**</span><span class="sxs-lookup"><span data-stu-id="732ae-119">Automatic planning on the kanban rule is set to **1**</span></span>

-   <span data-ttu-id="732ae-120">بالنسبة لوحدات كانبان المجدولة، سيكون من المطلوب وجود حد زمني للتأكيد</span><span class="sxs-lookup"><span data-stu-id="732ae-120">For scheduled kanbans, a firming fence is required</span></span>


### <a name="batch-calculation-by-using-ctp"></a><span data-ttu-id="732ae-121">حساب الدفعة باستخدام المتاح للتعهد (CTP)</span><span class="sxs-lookup"><span data-stu-id="732ae-121">Batch calculation by using CTP</span></span>

<span data-ttu-id="732ae-122">يمكن تشغيل عملية حسابية بعد إدخال بنود المبيعات من رأس أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="732ae-122">A calculation can be run after the sales lines have been entered from the header of the sales order.</span></span>

-   <span data-ttu-id="732ae-123">من رأس أمر المبيعات، حدد **البيع > إنشاء > تواريخ التسليم المؤكدة**.</span><span class="sxs-lookup"><span data-stu-id="732ae-123">From the sales order header, select **Sell > Generate > Calculate > Confirmed delivery dates**.</span></span>

-   <span data-ttu-id="732ae-124">قم بتشغيل التحقق من المتاح للتعهد (CTP) لأوامر المبيعات بدون تحديد خيار **تحديث التواريخ المؤكدة**.</span><span class="sxs-lookup"><span data-stu-id="732ae-124">Run the CTP check for the sales orders without the **Update confirmed dates** option selected.</span></span>

-   <span data-ttu-id="732ae-125">ستقوم الوظيفة الدفعية بتشغيل عملية تحديد إجمالي المكونات المطلوبة للمتاح للتعهد (CTP) لكافة بنود أوامر المبيعات وتوفير شريط معلومات يتضمن تواريخ الشحن المؤكدة الناتجة، ولكن بدون تحديث بند المبيعات.</span><span class="sxs-lookup"><span data-stu-id="732ae-125">The batch job will run the CTP explosion for all sales order lines and provide an InfoBar with the resulting confirmed ship dates, but without updating the sales line.</span></span>

-   <span data-ttu-id="732ae-126">إذا كانت تواريخ الشحن المقترحة مقبولة، يتم تشغيل العملية الحسابية مرة أخرى مع تحديد خيار **تحديث تواريخ التسليم في بنود المبيعات**.</span><span class="sxs-lookup"><span data-stu-id="732ae-126">If the proposed ship dates are acceptable, the calculation is run again with the **Update delivery dates on sales lines** option selected.</span></span>
    <span data-ttu-id="732ae-127">يعمل هذا الخيار على تشغيل عملية تحديد إجمالي المكونات المطلوبة للمتاح للتعهد (CTP) وتحديث تواريخ الشحن المؤكدة وتواريخ الاستلام المؤكدة في بنود المبيعات.</span><span class="sxs-lookup"><span data-stu-id="732ae-127">This option runs the CTP explosion and updates the confirmed ship dates and confirmed receipt dates on the sales lines.</span></span>




