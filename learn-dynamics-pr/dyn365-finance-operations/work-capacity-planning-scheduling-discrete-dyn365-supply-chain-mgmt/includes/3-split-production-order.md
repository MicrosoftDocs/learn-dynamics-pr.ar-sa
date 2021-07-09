---
ms.openlocfilehash: 0b41c78b8eeabd948a8369505fd92c0760cf9690
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073550"
---
<span data-ttu-id="8965e-101">وحتى يتم بدء إجمالي الكمية المجدولة للإنتاج، يمكن تقسيم الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8965e-101">Until the total scheduled quantity of a production is started, the production can be split.</span></span> <span data-ttu-id="8965e-102">ويعني تقسيم الإنتاج انخفاض الكمية المجدولة للإنتاج الحالي، وإنشاء إنتاج جديد للكمية التي يتم تقسيمها من عملية الإنتاج الأصلية.</span><span class="sxs-lookup"><span data-stu-id="8965e-102">Splitting the production means that the current production's scheduled quantity is decreased, and a new production is created for the quantity that is split from the original production.</span></span>
<span data-ttu-id="8965e-103">على سبيل المثال، يمكنك تقسيم الإنتاج للعملاء الذين طلبوا بالفعل كمية كبيرة ولكن مع تسليم جزء من الكمية المطلوبة في أسرع وقت ممكن.</span><span class="sxs-lookup"><span data-stu-id="8965e-103">For example, you can split production for customers who have already placed a large order but then decided to have part of the ordered quantity delivered as soon as possible.</span></span>

<span data-ttu-id="8965e-104">خذ بعين الاعتبار الخيارات التالية عند استخدام وظيفة التقسيم:</span><span class="sxs-lookup"><span data-stu-id="8965e-104">Consider the following options when using the split functionality:</span></span>

-   <span data-ttu-id="8965e-105">يمكنك فقط تقسيم كميات الإنتاج التي تكون حالتها **تم الإنشاء** أو **مقدرة** أو **مجدولة** أو **تم إصدارها**.</span><span class="sxs-lookup"><span data-stu-id="8965e-105">You can only split production quantities that have a status of **Created**, **Estimated**, **Scheduled**, or **Released**.</span></span>
    
-   <span data-ttu-id="8965e-106">عند تقسيم أمر إنتاج، تتم إعادة جدولة أمر الإنتاج الأصلي وأوامر الإنتاج المشتقة من المرجع وأوامر الشراء باستخدام جدولة إعادة التوجيه.</span><span class="sxs-lookup"><span data-stu-id="8965e-106">When you split a production order, the original production order and reference-derived production orders and purchase orders are rescheduled by using forward scheduling.</span></span> <span data-ttu-id="8965e-107">سيبدأ التقسيم في وقت البدء المجدول الفعلي.</span><span class="sxs-lookup"><span data-stu-id="8965e-107">The split will start at the actual scheduled start time.</span></span> <span data-ttu-id="8965e-108">يمكنك جدولة عمليات الإنتاج المقسمة الجديدة باستخدام جدولة رجعية، ثم بدء تشغيلها في التاريخ المحسوب بالعد الرجعي من وقت التسليم المعين.</span><span class="sxs-lookup"><span data-stu-id="8965e-108">You can schedule the new split productions by using backward scheduling, and then start them on the calculated date by counting backward from the assigned delivery time.</span></span>
    
-   <span data-ttu-id="8965e-109">الحد الأقصى للكمية التي يمكن تقسيمها هو الكمية التي لم تبدأ بعد في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="8965e-109">The maximum quantity that you can split is the quantity that has not yet started in production.</span></span>
    
-   <span data-ttu-id="8965e-110">تفحص Supply Chain Management الحالة والكمية المتاحة في عمليات الإنتاج وعمليات الشراء المشتقة قبل إجراء التقسيم.</span><span class="sxs-lookup"><span data-stu-id="8965e-110">Supply Chain Management checks the status and quantity that is available on derived productions and purchases before performing the split.</span></span> <span data-ttu-id="8965e-111">لا يمكنك تقسيم إنتاج إذا كانت الكمية الكاملة للإنتاج المشتق قد بدأت بالفعل أو إذا كان الشراء المشتق مسجلاً بالفعل في الإجمالي.</span><span class="sxs-lookup"><span data-stu-id="8965e-111">You cannot split a production if the whole quantity of a derived production has already been started or if a derived purchase has already been registered in total.</span></span>


### <a name="example"></a><span data-ttu-id="8965e-112">مثال</span><span class="sxs-lookup"><span data-stu-id="8965e-112">Example</span></span>

<span data-ttu-id="8965e-113">بدأت شركة ما أمر إنتاج كبير لأحد العملاء.</span><span class="sxs-lookup"><span data-stu-id="8965e-113">A company started a large production order for a customer.</span></span>
<span data-ttu-id="8965e-114">يرغب العميل في استلام الطلب في أسرع ما يمكن.</span><span class="sxs-lookup"><span data-stu-id="8965e-114">The customer wants to receive the order as quickly as possible.</span></span> <span data-ttu-id="8965e-115">وعلى الرغم من أن الشركة لا يمكنها زيادة الإنتاج للأمر، فإنه يمكن شحن المنتجات في دفعات أصغر بدلاً من الانتظار لإكمال الأمر بأكمله.</span><span class="sxs-lookup"><span data-stu-id="8965e-115">Though the company cannot increase production for the order, it can ship products in smaller batches instead of waiting for the whole order to be completed.</span></span> <span data-ttu-id="8965e-116">ويمكن أن تقوم الشركة بتقسيم أمر الإنتاج الكبير إلى العديد من الأوامر الصغيرة بحيث يتم شحن الأمر بدون الانتظار حتى إكمال الأمر بأكمله.</span><span class="sxs-lookup"><span data-stu-id="8965e-116">The company can split the large production order into several small orders so that, as each order is finished, it can be shipped without waiting for the whole order to be completed.</span></span>

