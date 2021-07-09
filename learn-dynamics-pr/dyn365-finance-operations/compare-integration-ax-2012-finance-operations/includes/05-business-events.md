---
ms.openlocfilehash: 122dc1615829be0eb936af0ea247710a679e18d9
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072409"
---
<span data-ttu-id="4eeb3-101">تعمل أحداث الأعمال على تمكين عمليات تكامل سير العمل بين تطبيقات Finance and Operations والأنظمة الخارجية بطريقة منفصلة.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-101">Business events enable business process integrations between Finance and Operations apps and external systems in a decoupled fashion.</span></span> 

- <span data-ttu-id="4eeb3-102">**أحداث الأعمال الثابتة**- يجب ألا يتم إرسال أحداث أعمال خاطئة إلى المستلم.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-102">**Durable business events** - No false business events should be sent to the recipient.</span></span> <span data-ttu-id="4eeb3-103">إذا تم إرسال حدث أعمال خاص بتأكيد أمر الشراء، فيجب على المستلم الوثوق في أن أمر الشراء تم تأكيده بالفعل.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-103">If a purchase order confirmation business event was sent out, then the recipient must trust that the purchase order was indeed confirmed.</span></span> <span data-ttu-id="4eeb3-104">يجب أن يضمن اختيار التصميم طبيعة الحركات هذه.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-104">The design choice must ensure this transactional nature.</span></span> 

- <span data-ttu-id="4eeb3-105">**الموجهة** ينبغي أن تصمم أحداث الأعمال بهدف تحسين مسألة الاستهلاك للمستلم.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-105">**Targeted** - Business events must be designed to optimize the consumption story for the recipient.</span></span> <span data-ttu-id="4eeb3-106">بمعنى آخر، ينبغي أن تسهل على المستلم استهلاك أحداث الأعمال قدر المستطاع.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-106">In other words, you must make it as easy as possible for the recipient to consume business events.</span></span> <span data-ttu-id="4eeb3-107">ولذلك، يجب أن تكون أحداث الأعمال محدده وموجهة لمستهلك معين.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-107">Hence, business events must be specific and targeted to a specific consumer.</span></span> 

- <span data-ttu-id="4eeb3-108">**صامتة** - يجب أن ينتقل المجهود البسيط إلى التصميم المطلوب لتصفيه الضوضاء.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-108">**Noiseless** - Little effort should go into the design that is needed to filter out noise.</span></span> <span data-ttu-id="4eeb3-109">لإجراء أحداث أعمال محددة، تأكد من تجنب كتابه منطق عوامل التصفية لتصفيه الشروط التي لا تتطابق مع حدث الأعمال المتوقع.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-109">To make business events specific, make sure that you avoid writing filtering logic to filter out conditions that do not match the expected business event.</span></span> 


<span data-ttu-id="4eeb3-110">توجد أنواع مختلفة من الأحداث، ومنها **أحداث التطبيق وسير العمل** و **التنبيه**.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-110">Different types of events exist, including **Application, Workflow**, and **Alert** events.</span></span> <span data-ttu-id="4eeb3-111">ويمكن استهلاك هذه الأحداث من خلال نقاط نهاية الخدمات السحابية مثل Microsoft Power Automate أو Azure Logic Apps أو Azure Data Lake Storage للعديد من السيناريوهات المختلفة، مثل عمليات سير العمل أو الإخطارات أو عمليات التكامل.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-111">These events can be consumed by cloud endpoints like Microsoft Power Automate, Azure Logic Apps, or Azure Data Lake Storage for many different scenarios, such as for workflows, notifications, or integrations.</span></span> 


![الرسم التخطيطي للأنواع المختلفة من أحداث الأعمال.](../media/business-event.png)

<span data-ttu-id="4eeb3-113">للحصول على مزيد من المعلومات، راجع [استهلاك أحداث الأعمال في تطبيقات Finance and Operations.](https://docs.microsoft.com/learn/modules/business-events-finance-operations/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="4eeb3-113">For more information, see [Consume business events in Finance and Operations apps.](https://docs.microsoft.com/learn/modules/business-events-finance-operations/?azure-portal=true).</span></span>


