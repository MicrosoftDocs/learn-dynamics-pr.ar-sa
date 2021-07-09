---
ms.openlocfilehash: bbf439ad5f7ebdcbdbc92dea41066ae69d3d589e
ms.sourcegitcommit: d190aa41f6104061e6ebe52ee5c86b6cb9febaf2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/12/2021
ms.locfileid: "6070533"
---
<span data-ttu-id="09cfe-101">إن القدرة على تنفيذ أمر ما بمرور الوقت باستخدام إذن دفع واحد ممكنة مع الالتقاط المتزايد.</span><span class="sxs-lookup"><span data-stu-id="09cfe-101">The ability to fulfill an order over time using a single payment authorization is possible with incremental capture.</span></span> <span data-ttu-id="09cfe-102">على سبيل المثال، قد يتم تنفيذ أمر العميل في ثلاث شحنات.</span><span class="sxs-lookup"><span data-stu-id="09cfe-102">For example, a customer's order, may be fulfilled in three shipments.</span></span> 

<span data-ttu-id="09cfe-103">دون الاستعانة بهذه الميزة، سيتم تسجيل الدفع للمبلغ الذي تم تحرير فاتورة به في كل مرة يتم فيها إصدار فاتورة بالشحنة، وسيتم إنشاء تفويض جديد للمبلغ المتبقي.</span><span class="sxs-lookup"><span data-stu-id="09cfe-103">Without this feature, payment for the amount invoiced will be captured each time a shipment is invoiced, and a new authorization will be created for the remaining amount.</span></span> <span data-ttu-id="09cfe-104">على مدار تنفيذ الأمر، توجد ثلاثة تفويضات مطلوبة في هذا السيناريو.</span><span class="sxs-lookup"><span data-stu-id="09cfe-104">Over the course of order fulfillment, three authorizations are required in this scenario.</span></span> <span data-ttu-id="09cfe-105">يمكن أن يؤدي هذا إلى تفويضات تتجاوز المبلغ الإجمالي للطلب أو قد يؤدي إلى الرفض، لأن التفويضات تتجاوز مبلغ الائتمان المفتوح المتاح لحاملي البطاقات.</span><span class="sxs-lookup"><span data-stu-id="09cfe-105">This can result in authorizations that exceed the total amount of the order or declines, because authorizations exceed the amount of open credit available to cardholders.</span></span>

<span data-ttu-id="09cfe-106">ستشير مدفوعات الأوامر التي تم إكمالها من مراكز التوزيع أو المتاجر إلى التفويض الأصلي إذا كان صالحاً عند السماح بهذه الوظيفة.</span><span class="sxs-lookup"><span data-stu-id="09cfe-106">Payments for orders that are completed from distribution centers or stores will reference the original authorization if it is valid when this function is allowed.</span></span> <span data-ttu-id="09cfe-107">وتتمثل بعض الفوائد في نسبة رفض أقل، وإحباط أقل للمستهلكين، وتسريع عملية الدفع وتسوية الفواتير.</span><span class="sxs-lookup"><span data-stu-id="09cfe-107">Some of the benefits are fewer declines, less consumer frustration, and faster payment and invoice reconciliation.</span></span> 

<span data-ttu-id="09cfe-108">يسلط الرسم البياني التالي الضوء على الاختلافات بين أطر عمل التقاط الدفع عندما يتم السماح بالتقاطات متعددة، مقابل عندما يتم تمكين تفويض واحد باستخدام دعم القناة متعددة الاتجاهات لالتقاط المدفوعات المتزايدة.</span><span class="sxs-lookup"><span data-stu-id="09cfe-108">The following graphic highlights the differences between the payment capture frameworks when multiple captures are authorized, versus when a single authorization is enabled by using omnichannel support for incremental payment capture.</span></span>

<span data-ttu-id="09cfe-109">[ ![رسم بياني يوضح طريقتين لأطر عمل تحصيل المدفوعات.](../media/payment-capture-c.png) ](../media/payment-capture-c.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="09cfe-109">[ ![Diagram showing the two methods of payment capture frameworks.](../media/payment-capture-c.png) ](../media/payment-capture-c.png#lightbox)</span></span>


> [!NOTE]
> <span data-ttu-id="09cfe-110">عند تنفيذ الطلبات من نقطة البيع والمركز الرئيسي لـ Commerce، يدعم Dynamics 365 Payment Connector for Adyen الالتقاط المتزايد بشكل جاهز.</span><span class="sxs-lookup"><span data-stu-id="09cfe-110">When orders are fulfilled from POS and Commerce headquarters, the Dynamics 365 Payment Connector for Adyen supports incremental capture out of the box.</span></span>

<span data-ttu-id="09cfe-111">يمكنك العثور على موارد إضافية حول الالتقاط المتزايد هنا:</span><span class="sxs-lookup"><span data-stu-id="09cfe-111">You can find additional resources about incremental capture here:</span></span>

- <span data-ttu-id="09cfe-112">[الالتقاط المتزايد لفواتير الأوامر](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/incremental-capture/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="09cfe-112">[Incremental capture for order invoicing](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/incremental-capture/?azure-portal=true).</span></span>
- <span data-ttu-id="09cfe-113">[Dynamics 365 Payment Connector for Adyen](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/adyen-connector?tabs=8-1-3/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="09cfe-113">[Dynamics 365 Payment Connector for Adyen](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/adyen-connector?tabs=8-1-3/?azure-portal=true).</span></span>
- <span data-ttu-id="09cfe-114">[مدفوعات أوامر القناة متعددة الاتجاهات لـ Commerce](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/commerce-payments/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="09cfe-114">[Omni-channel Commerce order payments](https://docs.microsoft.com/dynamics365/commerce/dev-itpro/commerce-payments/?azure-portal=true).</span></span>
