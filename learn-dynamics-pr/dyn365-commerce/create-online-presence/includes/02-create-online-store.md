---
ms.openlocfilehash: 4f62cd3848f8776518c61306ca482489dda7d269
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070047"
---
<span data-ttu-id="97177-101">قبل إنشاء موقع التجارة الإلكترونية، يتعين عليك إعداد قناة واحدة على الأقل في Commerce لإنشاء المنتجات وتحديد الأسعار وطرق الدفع وأنماط التسليم ومراكز التنفيذ والجوانب الأخرى من التجارب على الإنترنت التي تريد توفيرها لعملاء بائعي التجزئة.</span><span class="sxs-lookup"><span data-stu-id="97177-101">Before creating the e-Commerce site, you must set up at least one online channel in Commerce to establish the products, pricing, payment methods, delivery modes, fulfillment centers, and other aspects of the online experience that you want to provide to the retailer’s customers.</span></span> 

<span data-ttu-id="97177-102">يمكنك إنشاء قناة على الإنترنت في Commerce Headquarters (HQ).</span><span class="sxs-lookup"><span data-stu-id="97177-102">You can create an online channel in Commerce Headquarters (HQ).</span></span> 

<span data-ttu-id="97177-103">الخصائص التي تم تحديدها للمتجر على الإنترنت، والتي تتحكم في أداء المتجر.</span><span class="sxs-lookup"><span data-stu-id="97177-103">The properties that are defined for the online store control the behavior of the store.</span></span> 

<span data-ttu-id="97177-104">على سبيل المثال، أنت قمت بتحديد تدرج هرمي لفئة التنقل، ثم قمت بربطه بالمتجر على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="97177-104">For example, you have defined a navigation category hierarchy and then linked it to the online store.</span></span> <span data-ttu-id="97177-105">عندما يكون المتجر على الإنترنت نشطاً، يكون التدرج الهرمي لفئة التنقل ذاته مرئياً في واجهة المتجر، ويمكن للعملاء استخدامه لاستعراض المتجر واكتشاف المنتجات.</span><span class="sxs-lookup"><span data-stu-id="97177-105">When the online store is active, the same navigation category hierarchy is visible in the storefront and customers can use it to browse the store and discover products.</span></span> 

<span data-ttu-id="97177-106">لتكوين متجر يعمل على الإنترنت، ستحتاج إلى إعداد عدة مكونات بحيث يمكن معالجة الحركات بنجاح للمتجر على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="97177-106">To configure a functioning online store, you need to set up multiple components so that transactions can be successfully processed for that online store.</span></span> <span data-ttu-id="97177-107">عند قيامك بتكوين المتجر على الإنترنت ومكوناته، يمكنك ربط القناة بموقع Commerce واحد أو أكثر أو أي حل آخر لواجهة المتجر يكون متوافقاً مع Commerce.</span><span class="sxs-lookup"><span data-stu-id="97177-107">When you have configured the online store and its components, you can link the channel to one or multiple Commerce sites or any other solution for a storefront that is compatible with Commerce.</span></span>

<span data-ttu-id="97177-108">شاهد الفيديو التالي للحصول على توضيح حول كيفية إنشاء قناة على الإنترنت وتكوينها.</span><span class="sxs-lookup"><span data-stu-id="97177-108">Watch the following video for a demonstration of how to create and configure an online channel.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4AMfx]

<span data-ttu-id="97177-109">لبدء تكوين متجر يعمل على الإنترنت، استخدم الإجراء التالي لإعداد الدفع بحساب Adyen، والذي يكون ضرورياً لقبول عمليات الدفع في موقع التجارة الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="97177-109">To begin configuring a functioning online store, use the following procedure for setting up the Adyen payment account, which is needed to accept payments in the e-Commerce site.</span></span> <span data-ttu-id="97177-110">تم تصميم القنوات على الإنترنت ليتم استخدامها بشكل غير مسبوق من خلال Dynamics 365 Payment Connector لحساب Adyen.</span><span class="sxs-lookup"><span data-stu-id="97177-110">Online channels are designed to be used out-of-the-box with the Dynamics 365 Payment Connector for Adyen.</span></span> 

<span data-ttu-id="97177-111">هناك متطلب أساسي قبل أن تقوم بإضافة تكوين الدفع للمتجر على الإنترنت وهو أن يكون لديك اشتراك حساب نشط في Adyen.</span><span class="sxs-lookup"><span data-stu-id="97177-111">A prerequisite before you can add the payment configuration for the online store is that you have an active account set up with Adyen.</span></span> 

1.  <span data-ttu-id="97177-112">انتقل إلى **البيع بالتجزئة وCommerce > القنوات > المتاجر على الإنترنت**.</span><span class="sxs-lookup"><span data-stu-id="97177-112">Go to **Retail and Commerce > Channels > Online stores**.</span></span>
2.  <span data-ttu-id="97177-113">حدد وافتح شاشة التفاصيل للمتجر على الإنترنت الذي تريد إضافة حساب الدفع إليه.</span><span class="sxs-lookup"><span data-stu-id="97177-113">Select and open the details view of the online store that you want to add the payment account to.</span></span> 
3.  <span data-ttu-id="97177-114">حدد **تحرير** لبدء نمط التحرير وبعد ذلك إضافة معلومات حساب الدفع.</span><span class="sxs-lookup"><span data-stu-id="97177-114">Select **Edit** to start the edit mode and then add the payment account information.</span></span>
4.  <span data-ttu-id="97177-115">حدد علامة التبويب **حسابات الدفع**، ثم حدد **إضافة** لإضافة موصل دفع.</span><span class="sxs-lookup"><span data-stu-id="97177-115">Select the **Payment accounts** tab, and then select **Add** to add a payment connector.</span></span> 
5.  <span data-ttu-id="97177-116">بشكل افتراضي، يتم تعيين الحقل **بيئة البوابة** على **مباشر**.</span><span class="sxs-lookup"><span data-stu-id="97177-116">By default, the **Gateway Environment** field is set to **Live**.</span></span> <span data-ttu-id="97177-117">في حالة قيامك بإنشاء تكوين تجريبي، قم بتغيير الحقل **بيئة البوابة** إلى **تجريبي**.</span><span class="sxs-lookup"><span data-stu-id="97177-117">If you are creating a test configuration, change the **Gateway Environment** field to **Test**.</span></span>
6.  <span data-ttu-id="97177-118">أدخل **معرف حساب التاجر** و **مفتاح Cloud API** من حسابك على Adyen.</span><span class="sxs-lookup"><span data-stu-id="97177-118">Enter the **Merchant account ID** and **Cloud API Key** from your Adyen account.</span></span>
7.  <span data-ttu-id="97177-119">في حقل **البنية الطرفية**، أدخل **شبكة سحابية**.</span><span class="sxs-lookup"><span data-stu-id="97177-119">In the **Terminal architecture** field, enter **Cloud**.</span></span>
8.  <span data-ttu-id="97177-120">قم بتعيين الخيار **إتاحة معلومات توفير الدفع في التجارة الإلكترونية** على **صحيح**.</span><span class="sxs-lookup"><span data-stu-id="97177-120">Set the **Allow saving payment information in e-Commerce** option to **True**.</span></span>
9.  <span data-ttu-id="97177-121">أما باقي القيم فيمكن تركها بالقيم الافتراضية، أو يمكنك تغييرها لتعكس سيناريوهات الأعمال المخصصة لديك.</span><span class="sxs-lookup"><span data-stu-id="97177-121">All other values can be left with the defaults, or you can change them to reflect your specific business scenarios.</span></span>
10. <span data-ttu-id="97177-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="97177-122">Select **Save**.</span></span>

<span data-ttu-id="97177-123">لإنهاء تكوين القناة على الإنترنت وضمان أن تكون المنتجات قابلة للاكتشاف في متجر التجارة الإلكترونية، يتعين عليك أيضاً إنشاء تدرج هرمي تنقل للقناة ومزامنة البيانات لقاعدة بيانات المتجر على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="97177-123">To finalize the online channel configuration and ensure that the products are discoverable in the e-Commerce store, you should also create a channel navigation hierarchy and sync the data to the online store database.</span></span> 

<span data-ttu-id="97177-124">يمكن لكل قناة أن يكون لها تدرج هرمي فريد للقناة.</span><span class="sxs-lookup"><span data-stu-id="97177-124">Each channel can have a unique channel hierarchy.</span></span>


