---
ms.openlocfilehash: 844e1ab2eef69245d3fdeec9bf18effad2d22d1c
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070344"
---
<span data-ttu-id="fa6c3-101">يحتوي Dynamics 365 Commerce على العديد من صفحات المعلمات:</span><span class="sxs-lookup"><span data-stu-id="fa6c3-101">Dynamics 365 Commerce contains several parameter pages:</span></span> 

-   <span data-ttu-id="fa6c3-102">**معلمات Commerce**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-102">**Commerce parameters**</span></span>
-   <span data-ttu-id="fa6c3-103">**معلمات Commerce المشتركة**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-103">**Commerce shared parameters**</span></span>
-   <span data-ttu-id="fa6c3-104">**معلمات مجدول Commerce**.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-104">**Commerce scheduler parameters**.</span></span> 

<span data-ttu-id="fa6c3-105">سيتم ملء العديد من المعلمات تلقائياً بالبيانات من عملية تهيئة البيانات الأولية، بينما سيحتاج البعض الآخر إلى التكوين يدوياً.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-105">Many parameters will automatically become populated with data from the initialize seed data process, while others will need to be manually configured.</span></span> <span data-ttu-id="fa6c3-106">لا يلزم تكوين جميع المعلمات لتنفيذ ما، ولا يلزم تكوينها كلها للحصول على توزيع عملي لحل Commerce.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-106">Not all parameters need to be configured for an implementation, and not all of them are required to be configured to get a working deployment of the Commerce solution.</span></span> 

<span data-ttu-id="fa6c3-107">بينما يمكن تغيير بعض المعلمات وتحديثها خلال التنفيذ حسب الحاجة، يمكن للبعض الآخر (مثل التسلسل الرقمي ومعلمات الترحيل) تغيير شكل البيانات النهائية بشكل جذري في المركز الرئيسي (HQ) لـ Commerce، لذا يجب التعامل مع تكوينها في البداية باستخدام اهتمام كبير.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-107">While some parameters can be changed and updated throughout the implementation as needed, others (such as the number sequences and posting parameters) can radically change how the final data looks in Commerce Headquarters (HQ), so configuring them at the beginning should be approached with great attention.</span></span>  

## <a name="commerce-parameters"></a><span data-ttu-id="fa6c3-108">معلمات Commerce</span><span class="sxs-lookup"><span data-stu-id="fa6c3-108">Commerce parameters</span></span>

<span data-ttu-id="fa6c3-109">يمكن العثور على صفحة **معلمات Commerce** ضمن **البيع بالتجزئة والتجارة > إعداد المركز الرئيسي > المعلمات> معلمات Commerce**.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-109">The **Commerce parameters** page can be found under **Retail and Commerce > Headquarters setup > Parameters > Commerce parameters**.</span></span> <span data-ttu-id="fa6c3-110">وهي تحتوي على المعلمات الخاصة بكل كيان قانوني:</span><span class="sxs-lookup"><span data-stu-id="fa6c3-110">It contains parameters that are specific for each legal entity:</span></span>

-   <span data-ttu-id="fa6c3-111">**عام** (التهيئة الأولية للبيانات الاولية)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-111">**General** (initial seed data initialization)</span></span>
-   <span data-ttu-id="fa6c3-112">**ترحيل** (مثل حسابات دفتر الأستاذ الخاص بالفاتورة وإعدادات ترحيل كشف الحساب)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-112">**Posting** (such as invoice ledger accounts and statement posting settings)</span></span> 
-   <span data-ttu-id="fa6c3-113">**التزويد**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-113">**Replenishment**</span></span>
-   <span data-ttu-id="fa6c3-114">**الأسعار والخصومات** (مثل كيفية معالجة الخصومات المتداخلة والمتراكبة)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-114">**Prices and discounts** (such as how to handle overlapping and compounding discounts)</span></span>
-   <span data-ttu-id="fa6c3-115">**مصادقة نقطة البيع**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-115">**POS authentication**</span></span>
-   <span data-ttu-id="fa6c3-116">**أوامر العميل**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-116">**Customer orders**</span></span>
-   <span data-ttu-id="fa6c3-117">**توزيع القناة**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-117">**Channel deployment**</span></span>
-   <span data-ttu-id="fa6c3-118">**التحقق من صحة الحركة**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-118">**Transaction validation**</span></span>
-   <span data-ttu-id="fa6c3-119">**إدارة القوى العاملة**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-119">**Workforce management**</span></span>
-   <span data-ttu-id="fa6c3-120">**التسلسلات الرقمية**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-120">**Number sequences**</span></span>
-   <span data-ttu-id="fa6c3-121">**معايير البحث عن نقطة البيع**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-121">**POS search criteria**</span></span>
-   <span data-ttu-id="fa6c3-122">**إقامة العلاقات مع العملاء** وتفاصيل الاتصال في **Dynamics 365 Customer Insights**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-122">**Clienteling** and **Dynamics 365 Customer Insights connection details**</span></span>  
-   <span data-ttu-id="fa6c3-123">**Dynamics Fraud Protection**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-123">**Dynamics Fraud Protection**</span></span>  


<span data-ttu-id="fa6c3-124">[ ![لقطة شاشة لصفحة إعداد معلمات البيع بالتجزئة للترحيل](../media/retail-parameters-for-posting-03-ss.jpg) ](../media/retail-parameters-for-posting-03-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-124">[ ![Screenshot of set up the retail parameters for posting page](../media/retail-parameters-for-posting-03-ss.jpg) ](../media/retail-parameters-for-posting-03-ss.jpg#lightbox)</span></span>

## <a name="commerce-shared-parameters"></a><span data-ttu-id="fa6c3-125">معلمات Commerce المشتركة</span><span class="sxs-lookup"><span data-stu-id="fa6c3-125">Commerce shared parameters</span></span>

<span data-ttu-id="fa6c3-126">يمكن العثور على صفحة **معلمات Commerce المشتركة** ضمن **البيع بالتجزئة والتجارة > إعداد المركز الرئيسي > المعلمات> معلمات Commerce المشتركة**.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-126">The **Commerce shared parameters** page can be found under **Retail and Commerce > Headquarters setup > Parameters > Commerce shared parameters**.</span></span> <span data-ttu-id="fa6c3-127">وهي تحتوي على المعلمات التي تمثل تكوينات عمومية عبر الكيانات القانونية:</span><span class="sxs-lookup"><span data-stu-id="fa6c3-127">It contains parameters that are cross-legal entity global configurations:</span></span>

-   <span data-ttu-id="fa6c3-128">**مدفوعات القناة متعددة الاتجاهات** (تمكين بطاقات الهدايا الخارجية ومدفوعات القناة متعددة الاتجاهات)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-128">**Omni-channel payments** (enables external gift cards and omnichannel payments)</span></span>
-   <span data-ttu-id="fa6c3-129">**خرائط Bing** (تمكين خرائط Bing في نقطة البيع، وحساب المسافات، وعمليات تكامل خرائط Bing للتجارة الإلكترونية للعملاء)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-129">**Bing Maps** (enables Bing maps in the POS, calculation of distances, and customer ecommerce Bing map integrations)</span></span>
-   <span data-ttu-id="fa6c3-130">**توصيات المنتج** (تمكين الإعدادات مثل "الأكثر مبيعاً" و"‬‏‫الأشخاص يفضلون أيضاً..." و"المنتجات المتداولة" و"المنتجات الجديدة"، وغيرها)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-130">**Product recommendations** (enables settings such as Bestselling, People also like..., Trending products, New products, and so on)</span></span>
-   <span data-ttu-id="fa6c3-131">**موفرو الهويات**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-131">**Identity Providers**</span></span>
-   <span data-ttu-id="fa6c3-132">**قالب التحقق من صحة الكيان**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-132">**Entity validation template**</span></span>
-   <span data-ttu-id="fa6c3-133">**الأمان**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-133">**Security**</span></span>
-   <span data-ttu-id="fa6c3-134">**التسميات**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-134">**Labels**</span></span>
-   <span data-ttu-id="fa6c3-135">**التكامل المالي**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-135">**Fiscal integration**</span></span>
 

<span data-ttu-id="fa6c3-136">[ ![لقطة شاشة لصفحة إعداد معلمات commerce المشتركة العامة](../media/shared-parameters-04-ss.jpg) ](../media/shared-parameters-04-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-136">[ ![Screenshot of set up the general commerce shared parameters  page](../media/shared-parameters-04-ss.jpg) ](../media/shared-parameters-04-ss.jpg#lightbox)</span></span>

## <a name="commerce-scheduler-parameters"></a><span data-ttu-id="fa6c3-137">معلمات مجدول Commerce</span><span class="sxs-lookup"><span data-stu-id="fa6c3-137">Commerce scheduler parameters</span></span>

<span data-ttu-id="fa6c3-138">يمكن العثور على صفحة **معلمات مجدول Commerce** ضمن **البيع بالتجزئة والتجارة > إعداد المركز الرئيسي > المعلمات> معلمات مجدول Commerce**.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-138">The **Commerce scheduler parameters** page can be found under **Retail and Commerce > Headquarters setup > Parameters > Commerce scheduler parameters**.</span></span> <span data-ttu-id="fa6c3-139">وهي تحتوي على المعلمات الخاصة بكل كيان قانوني، كما تقوم بإدارة الاتصال بين المركز الرئيسي (HQ) لـ Commerce وقنوات Commerce من خلال إطار عمل توزيع البيانات.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-139">It contains parameters that are specific to each legal entity, and it manages the communication between Commerce Headquarters (HQ) and the Commerce channels through the data distribution framework.</span></span> <span data-ttu-id="fa6c3-140">تحتوي الصفحة على تكوينات من أجل:</span><span class="sxs-lookup"><span data-stu-id="fa6c3-140">The page contains configurations for:</span></span>

-   <span data-ttu-id="fa6c3-141">**اسم الخادم**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-141">**Server name**</span></span>
-   <span data-ttu-id="fa6c3-142">**اسم قاعدة البيانات**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-142">**Database name**</span></span>
-   <span data-ttu-id="fa6c3-143">**عدد المحاولات**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-143">**Try count**</span></span>
-   <span data-ttu-id="fa6c3-144">**مهلة أوامر SQL**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-144">**SQL Command timeout**</span></span>
-   <span data-ttu-id="fa6c3-145">**فترة الاحتجاز بالأيام**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-145">**Retention period in days**</span></span>
-   <span data-ttu-id="fa6c3-146">**الوظيفة الدفعية الحالية**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-146">**Current batch job**</span></span>
-   <span data-ttu-id="fa6c3-147">**حالة الدُفعة الحالية**</span><span class="sxs-lookup"><span data-stu-id="fa6c3-147">**Current batch status**</span></span>
  
<span data-ttu-id="fa6c3-148">[ ![لقطة شاشة توضح معلمات مجدول Commerce](../media/scheduler-parameters-05-ss.jpg) ](../media/scheduler-parameters-05-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa6c3-148">[ ![Screenshot of Commerce scheduler parameters page](../media/scheduler-parameters-05-ss.jpg) ](../media/scheduler-parameters-05-ss.jpg#lightbox)</span></span>

<span data-ttu-id="fa6c3-149">يتم تكوين معلمات إضافية خاصة بالكيان القانوني في صفحات محددة غير تابعة لـ Commerce في النظام.</span><span class="sxs-lookup"><span data-stu-id="fa6c3-149">Additional legal entity-specific parameters are configured in non-commerce specific pages in the system.</span></span> <span data-ttu-id="fa6c3-150">على الرغم من أن القائمة التالية ليست شاملة، إلا أنها توفر نقطة بداية للعديد من هذه المعلمات التي ستحتاج إليها في أثناء إعداد الحل Commerce:</span><span class="sxs-lookup"><span data-stu-id="fa6c3-150">While not comprehensive, the following list provides a starting point for several of these parameters that you will need while setting up the Commerce solution:</span></span>

-   <span data-ttu-id="fa6c3-151">معلمات البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="fa6c3-151">Email parameters</span></span>
-   <span data-ttu-id="fa6c3-152">قوالب البريد الإلكتروني للمؤسسة</span><span class="sxs-lookup"><span data-stu-id="fa6c3-152">Organization email templates</span></span>
-   <span data-ttu-id="fa6c3-153">معلمات النظام</span><span class="sxs-lookup"><span data-stu-id="fa6c3-153">System parameters</span></span>
-   <span data-ttu-id="fa6c3-154">معلمات الحسابات المدينة</span><span class="sxs-lookup"><span data-stu-id="fa6c3-154">Accounts receivable parameters</span></span>
-   <span data-ttu-id="fa6c3-155">معلمات المخزن الرئيسي</span><span class="sxs-lookup"><span data-stu-id="fa6c3-155">Key vault parameters</span></span>
-   <span data-ttu-id="fa6c3-156">معلمات إدارة المستندات</span><span class="sxs-lookup"><span data-stu-id="fa6c3-156">Document management parameters</span></span>
-   <span data-ttu-id="fa6c3-157">أنواع المستندات</span><span class="sxs-lookup"><span data-stu-id="fa6c3-157">Document types</span></span> 

