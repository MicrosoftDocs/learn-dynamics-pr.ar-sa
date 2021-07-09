---
ms.openlocfilehash: 3eeb4d7a3a783988fd4783c15a1ded34f4c21396
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071073"
---
<span data-ttu-id="66230-101">قبل أن تتمكن من استيراد أسعار الصرف، يجب عليك إعداد المعلومات التي يطلبها مقدمو الخدمة الذين يقدمون أسعار الصرف.</span><span class="sxs-lookup"><span data-stu-id="66230-101">Before you can import exchange rates, you must set up the information that is required by the providers who offer the exchange rates.</span></span>

<span data-ttu-id="66230-102">تساعد معرفة كيفية تكوين موفري أسعار الصرف في تقليل الوقت اللازم لإدارة التغييرات المستمرة في السوق فيما يتعلق بأسعار الصرف.</span><span class="sxs-lookup"><span data-stu-id="66230-102">Knowing how to configure exchange rate providers helps reduce the time to manage ongoing changes in market regarding exchange rates.</span></span> <span data-ttu-id="66230-103">على الرغم من أن الشركات يمكنها إما تطوير خدمات موفر أسعار الصرف أو شراؤها أو الاشتراك فيها، إلا أنك ستجد موفرين مدمجين في Finance.</span><span class="sxs-lookup"><span data-stu-id="66230-103">Even though companies can either develop, purchase, or subscribe to the exchange rate provider services, you will find built-in providers in Finance.</span></span>

## <a name="exchange-rate-types"></a><span data-ttu-id="66230-104">أنواع أسعار الصرف</span><span class="sxs-lookup"><span data-stu-id="66230-104">Exchange rate types</span></span> 

<span data-ttu-id="66230-105">أنواع أسعار الصرف هي بيانات مشتركة عبر Finance ويجب إعدادها مرة واحدة فقط.</span><span class="sxs-lookup"><span data-stu-id="66230-105">Exchange rate types are shared data across Finance and only need to be set up once.</span></span> <span data-ttu-id="66230-106">أنواع أسعار الصرف عبارة عن مجموعة تسمح بأسعار صرف مختلفة لعملتين.</span><span class="sxs-lookup"><span data-stu-id="66230-106">Exchange rate types are a grouping that allows different exchange rates for two currencies.</span></span> <span data-ttu-id="66230-107">تشمل الأمثلة الشراء والبيع والسوق والموازنة.</span><span class="sxs-lookup"><span data-stu-id="66230-107">Examples include Buy, Sell, Spot, and Budget.</span></span> <span data-ttu-id="66230-108">إذا كانت الشركة تتداول بعملات متعددة، فيجب عليها استخدام تحويلات متعددة لأسعار الصرف.</span><span class="sxs-lookup"><span data-stu-id="66230-108">If a company trades with multiple currencies, they must use multiple exchange rate conversions.</span></span> 

<span data-ttu-id="66230-109">لا يمكن أن يوجد زوج العملات إلا مرة واحدة ولا يتم دعم الدخول في زوج عملات متبادلة.</span><span class="sxs-lookup"><span data-stu-id="66230-109">A currency pair can only exist once and entering a reciprocal pair is not supported.</span></span> <span data-ttu-id="66230-110">لذلك، إذا كان لديك بالفعل إعداد من الدولار الأمريكي إلى اليورو، فلا يمكنك إنشاء زوج عملات من اليورو إلى الدولار الأمريكي لنفس نوع سعر الصرف.</span><span class="sxs-lookup"><span data-stu-id="66230-110">Therefore, if you already have USD to EUR set up, you cannot create a EUR to USD currency pair for the same exchange rate type.</span></span> 

<span data-ttu-id="66230-111">سيحسب Finance السعر المتبادل تلقائياً إذا لم يتمكن من العثور على زوج العملات بالضبط أثناء تحويل الترجمة.</span><span class="sxs-lookup"><span data-stu-id="66230-111">Finance will calculate the reciprocal rate automatically if it cannot find the exact currency pair during the translation conversion.</span></span> <span data-ttu-id="66230-112">إذا كان لديك فقط إعداد من الدولار الأمريكي إلى اليورو وكنت تقوم بإدخال مبلغ الحركة باليورو في كيان قانوني حيث الدولار الأمريكي هو عملة المحاسبة، فسيقوم Finance أولاً بالبحث عن زوج العملات المحدد في نوع السعر الذي يستخدمه دفتر الأستاذ: اليورو إلى الدولار الأمريكي.</span><span class="sxs-lookup"><span data-stu-id="66230-112">If you only have USD to EUR set up and you are entering a transaction amount in EUR in a legal entity where USD is the accounting currency, Finance will first search for the exact currency pair in the rate type used by the ledger: EUR to USD.</span></span> <span data-ttu-id="66230-113">إذا لم يتم العثور عليه، فسيتم بعد ذلك البحث عن الدولار الأمريكي مقابل اليورو وحساب السعر المتبادل.</span><span class="sxs-lookup"><span data-stu-id="66230-113">If not found, it will then search for USD to EUR and calculate the reciprocal rate.</span></span>

<span data-ttu-id="66230-114">نظراً لإمكانية وجود أسعار متعددة للعملة نفسها، فإن تاريخ الترحيل يحدد السعر المطبق.</span><span class="sxs-lookup"><span data-stu-id="66230-114">Because the same currency can have several rates, the posting date determines the rate applied.</span></span>

<span data-ttu-id="66230-115">على سبيل المثال، تم إدخال سعر الصرف في 1 يناير، وإدخال سعر صرف آخر في 1 فبراير.</span><span class="sxs-lookup"><span data-stu-id="66230-115">For example, an exchange rate is entered on January 1, and another exchange rate is entered on February 1.</span></span> <span data-ttu-id="66230-116">إذا تم إصدار فاتورة بأمر مبيعات في 15 يناير، فسيتم استخدام سعر الصرف اعتباراً من 1 يناير لحساب مبلغ الفاتورة.</span><span class="sxs-lookup"><span data-stu-id="66230-116">If a sales order is invoiced on January 15, the exchange rate from January 1 is used to calculate the invoice amount.</span></span> <span data-ttu-id="66230-117">إذا تم تنفيذ تسوية الصرف في 2 فبراير، فسيتم استخدام السعر من 1 فبراير كتسوية.</span><span class="sxs-lookup"><span data-stu-id="66230-117">If an exchange adjustment is run on February 2, the rate from February 1 is used as an adjustment.</span></span>

<span data-ttu-id="66230-118">استخدم صفحة **تكوين موفري أسعار الصرف** في **دفتر الأستاذ العام > العملات** لتحديد موفري أسعار الصرف.</span><span class="sxs-lookup"><span data-stu-id="66230-118">Use the **Configure exchange rate providers** page in **General ledger > Currencies** to select the exchange rate providers.</span></span> 
 
![لقطة شاشة توضح كيفية الانتقال إلى صفحة تكوين موفري أسعار الصرف.](../media/currencies-menu.png)


<span data-ttu-id="66230-120">يتم تضمين بعض موفري أسعار الصرف في بيانات العرض التوضيحي في Finance.</span><span class="sxs-lookup"><span data-stu-id="66230-120">Some exchange rate providers are included with the demo data in Finance.</span></span> 

## <a name="import-currency-exchange-rates"></a><span data-ttu-id="66230-121">استيراد أسعار صرف العملات</span><span class="sxs-lookup"><span data-stu-id="66230-121">Import currency exchange rates</span></span>

<span data-ttu-id="66230-122">إذا تلقى كيان قانوني فواتير بعملات أجنبية، فمن الضروري تحويل العملة الأجنبية إلى العملة المحلية.</span><span class="sxs-lookup"><span data-stu-id="66230-122">If a legal entity has received invoices in foreign currencies, it’s necessary to convert the foreign currency into the local currency.</span></span> <span data-ttu-id="66230-123">يعني هذا أن أسعار الصرف المحدثة للعملات المختلفة مطلوبة.</span><span class="sxs-lookup"><span data-stu-id="66230-123">This means that up-to-date exchange rates for different currencies are required.</span></span> 

<span data-ttu-id="66230-124">تقدم هذه الوحدة نظرة عامة على الإعدادات والمعالجة المطلوبة لاستيراد أسعار الصرف المرجعية المنشورة عبر الإنترنت من قِبل موفري أسعار الصرف، مثل البنك المركزي الأوروبي والبنك المركزي لروسيا الاتحادية.</span><span class="sxs-lookup"><span data-stu-id="66230-124">This unit provides an overview of the required settings and processing for importing foreign exchange reference rates published over the internet by the exchange rate providers, such as the Central Bank of Europe and the Central Bank of the Russian Federation.</span></span>

<span data-ttu-id="66230-125">يمكنك استيراد أسعار الصرف من موفري أسعار الصرف وإعدادها في صفحة **أسعار صرف العملات**.</span><span class="sxs-lookup"><span data-stu-id="66230-125">You can import exchange rates from the exchange rate providers and set them up on the **Currency exchange rates** page.</span></span> <span data-ttu-id="66230-126">استخدم صفحة **استيراد أسعار الصرف** لاستيراد أسعار الصرف.</span><span class="sxs-lookup"><span data-stu-id="66230-126">Use the **Import currency exchange rates** page to import the exchange rates.</span></span> 

<span data-ttu-id="66230-127">شاهد هذا الفيديو للتعرف على كيفية استيراد أسعار صرف العملات.</span><span class="sxs-lookup"><span data-stu-id="66230-127">Watch this video to learn how to import currency exchange rates.</span></span>


 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3URoR] 
