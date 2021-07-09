---
ms.openlocfilehash: 74e4aad91fee9bd5e8e9a4a5c8f242a3acff9603
ms.sourcegitcommit: 4ce9caef7d38158f172e82412bc70ae36883e42f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "6070424"
---
<span data-ttu-id="9aafe-101">يجب تطبيق بعض المتطلبات الأساسية لتتمكن من الشراء عبر الإنترنت والاستلام في المتجر (BOPIS):</span><span class="sxs-lookup"><span data-stu-id="9aafe-101">Some prerequisites must be in place for you to buy online and pick up in store (BOPIS):</span></span>

- <span data-ttu-id="9aafe-102">تتطلب سيناريوهات BOPIS التي تتضمن الدفع بالبطاقة المدينة محطة أجهزة.</span><span class="sxs-lookup"><span data-stu-id="9aafe-102">BOPIS scenarios that involve a credit card payment require a hardware station.</span></span> <span data-ttu-id="9aafe-103">يتم دمج محطة الأجهزة في نقطة البيع الحديثة لعملاء Windows وAndroid.</span><span class="sxs-lookup"><span data-stu-id="9aafe-103">The hardware station is built into Modern POS for Windows and Android clients.</span></span> <span data-ttu-id="9aafe-104">إذا كنت تستخدم نقطة بيع خاصة بالمجموعة أو نقطة بيع حديثة لنظام iOS، يجب إقران عميل نقطة البيع بمحطة أجهزة مشتركة.</span><span class="sxs-lookup"><span data-stu-id="9aafe-104">If you're using Cloud POS or Modern POS for iOS, the point of sale (POS) client must be paired with a shared hardware station.</span></span> 
- <span data-ttu-id="9aafe-105">قم بتمكين الخيار **استخدام محطة الأجهزة** في نقطة البيع الحديثة.</span><span class="sxs-lookup"><span data-stu-id="9aafe-105">Enable the **Use hardware station** option in the Modern POS.</span></span>
- <span data-ttu-id="9aafe-106">قبل تسجيل الدخول إلى نقطة البيع، تأكد من أن حساب Microsoft Azure Active Directory (Azure AD) الذي تستخدمه مرتبط بالعامل الذي قام بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="9aafe-106">Before signing in to POS, ensure that the Microsoft Azure Active Directory (Azure AD) account that you are using is associated with the worker who is signing in.</span></span>

<span data-ttu-id="9aafe-107">لقد تعلمت سابقاً كيفية إنشاء أمر الاستلام ومزامنته مع المركز الرئيسي لـ Commerce.</span><span class="sxs-lookup"><span data-stu-id="9aafe-107">Previously, you learned how to create an order for pickup and synchronize it to Commerce Headquarters.</span></span>

<span data-ttu-id="9aafe-108">للتعامل مع هذا الأمر الذي سيتم استلامه في المتجر، اتبع هذا الإجراء:</span><span class="sxs-lookup"><span data-stu-id="9aafe-108">To handle that order to be picked up in the store, follow this procedure:</span></span>
 
1. <span data-ttu-id="9aafe-109">قم بتسجيل الدخول إلى نقطة البيع (نقطة البيع الحديثة أو نقطة البيع الخاصة بالمجموعة)، وحدد **الأوامر المطلوب استلامها**.</span><span class="sxs-lookup"><span data-stu-id="9aafe-109">Sign in to POS (Modern POS or Cloud POS) and select **Orders to pick up**.</span></span>

    <span data-ttu-id="9aafe-110">[ ![لقطة شاشة للإجراء "الأوامر المطلوب استلامها" في Dynamics 365 Commerce.](../media/orders-pick-up-ss.jpg) ](../media/orders-pick-up-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9aafe-110">[ ![Screenshot of the Orders to pick up action Dynamics 365 Commerce.](../media/orders-pick-up-ss.jpg) ](../media/orders-pick-up-ss.jpg#lightbox)</span></span>
    
2. <span data-ttu-id="9aafe-111">حدد الأمر المطلوب استلامه (1)، ثم حدد **استلام** (2)، كما هو موضح في لقطة الشاشة التالية.</span><span class="sxs-lookup"><span data-stu-id="9aafe-111">Select the order to pick up (1), and then select **Pick up** (2), as shown in the following screenshot.</span></span>

    <span data-ttu-id="9aafe-112">[ ![لقطة شاشة لإجراء الاستلام في Dynamics 365 Commerce.](../media/pick-up-ss.jpg) ](../media/pick-up-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9aafe-112">[ ![Screenshot of the Pick up action in Dynamics 365 Commerce.](../media/pick-up-ss.jpg) ](../media/pick-up-ss.jpg#lightbox)</span></span>
    
3. <span data-ttu-id="9aafe-113">حدد الصنف المراد استلامه، ثم حدد **طرق الدفع** لإكمال الحركة.</span><span class="sxs-lookup"><span data-stu-id="9aafe-113">Select the item to be picked up and then select **Payment methods** to complete the transaction.</span></span>

    <span data-ttu-id="9aafe-114">[ ![لقطة شاشة للإجراء "طرق الدفع" في Dynamics 365 Commerce.](../media/payment-methods-ss.jpg) ](../media/payment-methods-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9aafe-114">[ ![Screenshot of the Payment methods action in Dynamics 365 Commerce.](../media/payment-methods-ss.jpg) ](../media/payment-methods-ss.jpg#lightbox)</span></span> 

