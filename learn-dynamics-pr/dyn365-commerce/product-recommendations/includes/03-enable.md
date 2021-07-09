---
ms.openlocfilehash: b65a7f992644fe825494383f38423fc6c8ee4bde
ms.sourcegitcommit: ca87deefdcd512d3b8e382cd49adf8a15d5995fc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/02/2021
ms.locfileid: "6070444"
---
<span data-ttu-id="32d1a-101">يمكن لتجار التجزئة تشغيل التوصيات بنقرة زر واحدة.</span><span class="sxs-lookup"><span data-stu-id="32d1a-101">Retailers can turn on recommendations at the click of a button.</span></span> <span data-ttu-id="32d1a-102">يشرح هذا الموضوع كيف يمكنك تمكين توصيات المنتج والقوائم المخصصة لعملاء Commerce.</span><span class="sxs-lookup"><span data-stu-id="32d1a-102">This topic explains how you can enable product recommendations and tailor lists for Commerce customers.</span></span> 

> [!NOTE]
> <span data-ttu-id="32d1a-103">سيؤدي تمكين التوصيات أيضاً إلى تمكين التوصيات الشخصية.</span><span class="sxs-lookup"><span data-stu-id="32d1a-103">Enabling recommendations will also enable personalized recommendations.</span></span> <span data-ttu-id="32d1a-104">لا يمكن لتجار التجزئة تمكين التخصيص دون تمكين خدمة التوصيات الأساسية أولاً.</span><span class="sxs-lookup"><span data-stu-id="32d1a-104">Retailers can’t enable personalization without first enabling the base recommendations service.</span></span> 

## <a name="recommendations-pre-check"></a><span data-ttu-id="32d1a-105">الفحص المسبق للتوصيات</span><span class="sxs-lookup"><span data-stu-id="32d1a-105">Recommendations pre-check</span></span>

<span data-ttu-id="32d1a-106">قبل تمكين التوصيات، لاحظ أن توصيات المنتج مدعومة فقط لعملاء Commerce الذين قاموا بترحيل وحدات التخزين الخاصة بهم لاستخدام Azure Data Lake storage، وأن الوظيفة غير متاحة للعملاء المحليين.</span><span class="sxs-lookup"><span data-stu-id="32d1a-106">Before enabling recommendations, note that product recommendations are only supported for Commerce customers who have migrated their storage to using Azure Data Lake storage, and the functionality is not available for on-premises customers.</span></span>

<span data-ttu-id="32d1a-107">قبل تمكين التوصيات، تأكد من إجراء التكوينات التالية على الشبكة:</span><span class="sxs-lookup"><span data-stu-id="32d1a-107">Before enabling recommendations, make sure that you perform the following configurations on the network:</span></span>

1.  <span data-ttu-id="32d1a-108">تأكد من شراء Azure Data Lake storage والتحقق منه بنجاح في البيئة.</span><span class="sxs-lookup"><span data-stu-id="32d1a-108">Ensure that Azure Data Lake storage has been purchased and successfully verified in the environment.</span></span> 
2.  <span data-ttu-id="32d1a-109">تأكد من تمكين قياس **RetailSales** لمتجر الكيان وتعيينه على **التحديث التلقائي**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-109">Ensure that the entity store **RetailSales** measurement has been enabled and set to **auto-refresh**.</span></span> 
3.  <span data-ttu-id="32d1a-110">تأكد من أن تكوين هوية Azure Active Directory (Azure AD) يحتوي على إدخال لـ **التوصيات**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-110">Confirm that Azure Active Directory (Azure AD) identity configuration contains an entry for **Recommendations**.</span></span> 

## <a name="azure-ad-identity-configuration"></a><span data-ttu-id="32d1a-111">تكوين هوية Azure AD</span><span class="sxs-lookup"><span data-stu-id="32d1a-111">Azure AD identity configuration</span></span>
<span data-ttu-id="32d1a-112">يُعد التأكد من تكوين هوية Azure AD لاحتواء إدخال للتوصيات خطوة مطلوبة لجميع العملاء الذين يقومون بتشغيل خدمة تأجير البنية التحتية (IaaS) والذين قاموا بإعداد بيئتهم الخاصة على النظام الأساسي Azure.</span><span class="sxs-lookup"><span data-stu-id="32d1a-112">Ensuring that Azure AD identity is configured to contain an entry for recommendations is a required step for all customers who are running an infrastructure as a service (IaaS) configuration and who have set up their own environment on the Azure platform.</span></span> <span data-ttu-id="32d1a-113">بالنسبة للعملاء الذين يعملون على أجهزة Windows تم تكوينها مسبقاً أو أجهزة Windows الظاهرية مع Azure Service Fabric، يجب أن تكون هذه الخطوة تلقائية، ونوصي بالتحقق من تكوين الإعداد كما هو متوقع.</span><span class="sxs-lookup"><span data-stu-id="32d1a-113">For customers who are running on preconfigured Windows machines or Windows virtual machines with Azure Service Fabric, this step should be automatic, and we recommend verifying that the setting is configured as expected.</span></span>

<span data-ttu-id="32d1a-114">للتحقق من إعداد هوية Azure AD، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="32d1a-114">To check the Azure AD identity setup, follow these steps:</span></span>

1.  <span data-ttu-id="32d1a-115">في Commerce، ابحث عن صفحة **تطبيقات Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-115">In Commerce, search for the **Azure Active Directory applications** page.</span></span>
2.  <span data-ttu-id="32d1a-116">تحقق من وجود إدخال لـ **RecommendationSystemApplication-1**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-116">Verify if an entry exists for **RecommendationSystemApplication-1**.</span></span>

    <span data-ttu-id="32d1a-117">إذا لم يكن الإدخال موجودا، فقم بإضافة إدخال جديد بالمعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="32d1a-117">If the entry does not exist, add a new entry with the following information:</span></span>

    - <span data-ttu-id="32d1a-118">**معرف العميل** - d37b07e8-dd1c-4514-835d-8b918e6f9727</span><span class="sxs-lookup"><span data-stu-id="32d1a-118">**Client ID** - d37b07e8-dd1c-4514-835d-8b918e6f9727</span></span>
    - <span data-ttu-id="32d1a-119">**الاسم** - RecommendationSystemApplication-1</span><span class="sxs-lookup"><span data-stu-id="32d1a-119">**Name** - RecommendationSystemApplication-1</span></span>
    - <span data-ttu-id="32d1a-120">**معرف المستخدم** - RetailServiceAccount</span><span class="sxs-lookup"><span data-stu-id="32d1a-120">**User ID** - RetailServiceAccount</span></span>

3.  <span data-ttu-id="32d1a-121">حدد **حفظ** وأغلق الصفحة.</span><span class="sxs-lookup"><span data-stu-id="32d1a-121">**Save** and close the page.</span></span>

<span data-ttu-id="32d1a-122">لتشغيل توصيات المنتج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="32d1a-122">To turn on product recommendations, follow these steps:</span></span>

1.  <span data-ttu-id="32d1a-123">انتقل إلى **البيع بالتجزئة وCommerce > توصيات المنتج > معلمات التوصيات**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-123">Go to **Retail and Commerce > Product recommendations > Recommendation parameters**.</span></span>
2.  <span data-ttu-id="32d1a-124">في الصفحة **المعلمات العامة المشتركة**، حدد **توصيات المنتج**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-124">In the **Common shared parameters** page, select **Product recommendations**.</span></span>
3.  <span data-ttu-id="32d1a-125">قم بتعيين الخيار **تمكين التوصيات** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-125">Set the **Enable recommendations** option to **Yes**.</span></span>

<span data-ttu-id="32d1a-126">توضح لقطة الشاشة التالية كيفية تمكين التوصيات في Commerce.</span><span class="sxs-lookup"><span data-stu-id="32d1a-126">The following screenshot shows how to enable recommendations in Commerce.</span></span>
 
<span data-ttu-id="32d1a-127">[ ![لقطة شاشة لصفحة معلمات Commerce المشتركة](../media/commerce-shared-parameters-ssm.jpg) ](../media/commerce-shared-parameters-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="32d1a-127">[ ![Screenshot of the Commerce shared parameters page.](../media/commerce-shared-parameters-ssm.jpg) ](../media/commerce-shared-parameters-ssm.jpg#lightbox)</span></span>

<span data-ttu-id="32d1a-128">بالنسبة للتحديث 10.0.12، يمكن للتجار تمكين التوصيات من صفحة **إدارة الميزات** وتنفيذ المهام المتعلقة بالتوصيات من صفحة **تكوين التوصيات**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-128">For the 10.0.12 update, merchandisers can enable recommendations from the **Feature management** page and perform recommendations-related tasks from the **Configure recommendations** page.</span></span> 

 
<span data-ttu-id="32d1a-129">[ ![لقطة شاشة لصفحة تكوين التوصيات.](../media/configure-recommendations-ss.jpg) ](../media/configure-recommendations-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="32d1a-129">[ ![Screenshot of the Configure recommendations page.](../media/configure-recommendations-ss.jpg) ](../media/configure-recommendations-ss.jpg#lightbox)</span></span>
 
<span data-ttu-id="32d1a-130">يبدأ إجراء تمكين التوصيات بعملية إنشاء قوائم توصيات المنتج.</span><span class="sxs-lookup"><span data-stu-id="32d1a-130">The procedure of enabling recommendations starts with the process of generating product recommendation lists.</span></span> <span data-ttu-id="32d1a-131">قد يستغرق الأمر عدة ساعات قبل أن تصبح القوائم متاحة ويمكن عرضها في نقطة البيع أو في Commerce.</span><span class="sxs-lookup"><span data-stu-id="32d1a-131">It might take several hours before the lists are available and can be viewed at the point of sale (POS) or in Commerce.</span></span>

<span data-ttu-id="32d1a-132">بعد تمكين توصيات المنتج، ستصبح الإعدادات الافتراضية سارية المفعول مع القيم التي يتم ملؤها تلقائياً، يمكن تكوين معلمات السوق هذه لتجار التجزئة لتعكس تدفق الأعمال بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="32d1a-132">After you have enabled product recommendations, the default settings will take effect with auto-filled values; these market parameters are configurable for retailers to best reflect the flow of business.</span></span> <span data-ttu-id="32d1a-133">نوصي بقضاء بعض الوقت في تقييم ما إذا كانت النتائج تتناسب مع حركة بيع المنتجات.</span><span class="sxs-lookup"><span data-stu-id="32d1a-133">We recommend that you spend time evaluating whether the results fit the selling motion of products.</span></span>

<span data-ttu-id="32d1a-134">في الوقت الحالي، يمكن تكوين نوعين من معلمات السوق بواسطة تجار التجزئة:</span><span class="sxs-lookup"><span data-stu-id="32d1a-134">Currently, two types of market parameters are configurable by retailers:</span></span>

- <span data-ttu-id="32d1a-135">**عمر المنتج (بالأيام)** - يمكن استخدام المنتجات التي تمت إضافتها خلال العدد المحدد من الأيام قبل التاريخ الحالي لتحديد المنتجات المرشحة.</span><span class="sxs-lookup"><span data-stu-id="32d1a-135">**Age of product (in days)** - Products that have been added within the specified number of days before the current date can be used to select product candidates.</span></span> <span data-ttu-id="32d1a-136">تشير القيمة الافتراضية في الصورة إلى أنه يمكن استخدام المنتجات القديمة التي يصل عمرها إلى 180 يوماً في قائمة **المنتجات المتداولة**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-136">The default value in the picture suggests that products as old as 180 days can be used in the **Trending product** list.</span></span>
- <span data-ttu-id="32d1a-137">**مراعاة محفوظات المبيعات (بالأيام)** - يمكن استخدام حركات المبيعات التي حدثت خلال العدد المحدد من الأيام قبل التاريخ الحالي لطلب المنتجات.</span><span class="sxs-lookup"><span data-stu-id="32d1a-137">**Consider sales history (in days)** - Sales transactions that have occurred within the specified number of days before the current date can be used to order the products.</span></span> <span data-ttu-id="32d1a-138">تشير القيمة الافتراضية التي تظهر أعلى هذه المعلمة إلى أنه سيتم استخدام جميع مشتريات المنتج في آخر 36 يوماً لتحديد موضع المنتج في قائمة **المنتجات المتداولة**.</span><span class="sxs-lookup"><span data-stu-id="32d1a-138">The default value that is shown above this parameter suggests that all purchases of a product in the last 36 days would be used to determine the placement of the product in the **Trending product** list.</span></span>

![لقطة شاشة لمعلمات السوق القابلة للتكوين من خلال تجار التجزئة في Dynamics 365 Commerce.](../media/market-parameters-ss.jpg)
 
<span data-ttu-id="32d1a-140">بعد تمكين التوصيات في Commerce، تحتاج إلى إضافة لوحة التوصيات إلى شاشة التحكم في نقطة البيع باستخدام أداة التخطيط قبل أن تبدأ التوصيات في الظهور على السداد وتسجيل الخروج.</span><span class="sxs-lookup"><span data-stu-id="32d1a-140">After enabling recommendations in Commerce, you need to add the recommendations panel to the control POS screen by using the layout tool before recommendations can start appearing on the checkout screen.</span></span>

## <a name="enable-omnichannel-personalized-product-recommendations"></a><span data-ttu-id="32d1a-141">تمكين توصيات منتجات القناة متعددة الاتجاهات المخصصة</span><span class="sxs-lookup"><span data-stu-id="32d1a-141">Enable omnichannel personalized product recommendations</span></span>
<span data-ttu-id="32d1a-142">شاهد مقطع الفيديو التالي لمعرفة كيفية تمكين التوصيات الشخصية للقناة متعددة الاتجاهات.</span><span class="sxs-lookup"><span data-stu-id="32d1a-142">Watch the following video to learn how to enable omnichannel personalized recommendations.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4xo0b]
