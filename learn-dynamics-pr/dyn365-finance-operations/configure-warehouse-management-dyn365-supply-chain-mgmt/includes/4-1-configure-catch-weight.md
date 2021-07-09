---
ms.openlocfilehash: ba574c3df81ffe8567553f93ff45363457af02e2
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073787"
---

<span data-ttu-id="0abc1-101">إن معالجة منتج وزن التعبئة عبارة عن مفهوم يسمح بتتبع المخزون في وحدتين من وحدات القياس: وحدة المخزون (رطل أو كيلوجرام) ووحدة وزن التعبئة لعكس وحدة المبيعات الخاصة بالمنتج، مثل "كل" أو كيس.</span><span class="sxs-lookup"><span data-stu-id="0abc1-101">Catch weight product processing is a concept that allows tracking of inventory in two units of measure: an inventory unit (pounds or kilograms) and a catch weight unit to reflect the sales unit of the product, such as an "each" or a bag.</span></span> <span data-ttu-id="0abc1-102">قد يكون أحد الأمثلة عن وحدة وزن التعبئة بيع كيس من البطاطس يبلغ وزنه 15 رطلاً ككيس واحد، ولكن مع تقليل المخزون بمقدار 15.2 رطلاً.</span><span class="sxs-lookup"><span data-stu-id="0abc1-102">An example of a catch weight unit might be selling a 15-pound bag of potatoes as one bag, but reducing inventory by 15.2 pounds.</span></span> 

<span data-ttu-id="0abc1-103">لمزيد من المعلومات حول استخدام منتجات وزن التعبئة، انتقل إلى [وزن التعبئة](https://docs.microsoft.com/learn/modules/configure-use-process-manufacturing-dyn365-supply-chain-mgmt/11-catch-weight "Microsoft Learn - تكوين التصنيع التحويلي واستخدامه في Dynamics 365 Supply Chain Management").</span><span class="sxs-lookup"><span data-stu-id="0abc1-103">For more information on using catch weight products, go to [Catch weight](https://docs.microsoft.com/learn/modules/configure-use-process-manufacturing-dyn365-supply-chain-mgmt/11-catch-weight "Microsoft Learn - Configure and use process manufacturing in Dynamics 365 Supply Chain Management").</span></span>

<span data-ttu-id="0abc1-104">في إدارة المستودعات، يجب إكمال الإعداد الأساسي التالي:</span><span class="sxs-lookup"><span data-stu-id="0abc1-104">In warehouse management, you must complete the following basic setup:</span></span>

1. <span data-ttu-id="0abc1-105">حدد تحويل الوزن بين وحدة المخزون بالأرطال (على سبيل المثال) ووحدة وزن التعبئة، مثل "كل" أو أكياس في صفحة **المنتجات الصادرة** ضمن علامة التبويب السريعة **إدارة المخزون**.</span><span class="sxs-lookup"><span data-stu-id="0abc1-105">Define the weight conversion between the inventory unit of pounds (for example) and the catch weight unit, such as "eaches" or bags, on the **Released products** page under the **Manage inventory** FastTab.</span></span>

2. <span data-ttu-id="0abc1-106">حدد الحد الأدنى والحد الأقصى لتفاوتات الوزن كجزء من إعداد وزن التعبئة في صفحة **المنتجات الصادرة** على علامة التبويب السريعة **إدارة المخزون**.</span><span class="sxs-lookup"><span data-stu-id="0abc1-106">Define the minimum and maximum weight tolerances as part of the catch weight setup on the **Released product** page on the **Manage inventory** FastTab.</span></span>

    <span data-ttu-id="0abc1-107">[ ![لقطة شاشة لصفحة إدارة المخزون.](../media/manage-inventory-setup-ssm.png) ](../media/manage-inventory-setup-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0abc1-107">[ ![Screenshot of the manage inventory page.](../media/manage-inventory-setup-ssm.png) ](../media/manage-inventory-setup-ssm.png#lightbox)</span></span> 

    <span data-ttu-id="0abc1-108">في لقطة الشاشة السابقة، تم تعيين صنف وزن التعبئة إلى **ea** (كل) والكمية الاسمية هي **10**، مما يعني تعيين الوزن الهدف للمنتج إلى 10 أرطال.</span><span class="sxs-lookup"><span data-stu-id="0abc1-108">In the preceding screenshot, the catch weight item is set to **ea** (each) and the nominal quantity is **10**, meaning that the goal weight of the product is set to 10 pounds.</span></span> <span data-ttu-id="0abc1-109">الحدان الأدنى والأقصى للكمية هما 9 أرطال و11 رطلاً، مما يعني أن وزن "كل" كمية قد يكون بين 9 أرطال و11 رطلاً.</span><span class="sxs-lookup"><span data-stu-id="0abc1-109">The minimum and maximum quantity are 9 and 11 pounds, meaning that the weight of "each" can be between 9 and 11 pounds.</span></span> 

3. <span data-ttu-id="0abc1-110">أنشئ **مجموعة تسلسلات الوحدات**، حيث وحدة وزن التعبئة معينة إلى وحدة حفظ المخزون الأدنى.</span><span class="sxs-lookup"><span data-stu-id="0abc1-110">Create a **unit sequence group**, where the catch weight unit is set as the lowest stock keeping unit.</span></span>
 
4. <span data-ttu-id="0abc1-111">قم بإعداد سياسة معالجة وزن التعبئة.</span><span class="sxs-lookup"><span data-stu-id="0abc1-111">Set up a catch weight handling policy.</span></span>


    > <span data-ttu-id="0abc1-112">[ ![لقطة شاشة لصفحة سياسات معالجة وزن التعبئة](../media/catch-weight-handling-policy-ss.png) ](../media/catch-weight-handling-policy-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0abc1-112">[ ![Screenshot of catch weight handling policies page](../media/catch-weight-handling-policy-ss.png) ](../media/catch-weight-handling-policy-ss.png#lightbox)</span></span>
