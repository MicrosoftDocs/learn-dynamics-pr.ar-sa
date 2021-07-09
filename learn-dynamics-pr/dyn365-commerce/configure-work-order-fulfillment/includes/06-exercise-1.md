---
ms.openlocfilehash: bf6ffd1e3d16585144c33e56dcdefcb47dc8a81e
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070118"
---
<span data-ttu-id="710f3-101">بالنسبة لهذا التمرين، والتمرينات الأخرى في هذه الوحدة، نوصي باستخدام بيانات العرض التوضيحي في الكيان القانوني **USRT**.</span><span class="sxs-lookup"><span data-stu-id="710f3-101">For this exercise, and the other exercises in this module, we recommend that you use the demo data of the company **USRT**.</span></span>

## <a name="scenario"></a><span data-ttu-id="710f3-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="710f3-102">Scenario</span></span>
<span data-ttu-id="710f3-103">أنت مسؤول عن تنفيذ عملية إدارة الأوامر الموزعة (DOM) الفعالة من حيث التكلفة في شركتك.</span><span class="sxs-lookup"><span data-stu-id="710f3-103">You are responsible for the implementation of a cost-effective distributed order management (DOM) process in your company.</span></span> <span data-ttu-id="710f3-104">‏‫ولهذا الغرض، يتعين عليك تحديد تكلفة شحن يجب أخذها في الاعتبار عندما يحسب نموذج كائن المستند (DOM) توصيات التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="710f3-104">For this purpose, you must define shipping cost to be considered when DOM calculates fulfillment recommendations.</span></span> 

<span data-ttu-id="710f3-105">اختارت شركتك أساساً بسيطاً لحساب المستوى، حيث تكون تكلفة الشحن ثابتة على 10.00 دولارات أمريكية لوضع التسليم 99 وتُحسب بـ 0.50 دولاراً أمريكياً لكل وحدة مسافة لوضع التسليم 60.</span><span class="sxs-lookup"><span data-stu-id="710f3-105">Your company has chosen a simple level calculation basis, where the shipping cost is fixed at USD 10.00 for mode of delivery 99 and is calculated at USD 0.50 for each distance unit for mode of delivery 60.</span></span>

1.  <span data-ttu-id="710f3-106">في الكيان القانوني **USRT** للشركة، انتقل إلى **Retail وCommerce > ‏‫إدارة الأوامر الموزعة‬ > الإعداد > تكوين التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="710f3-106">In the company **USRT**, go to **Retail and Commerce > Distributed order management > Setup > Cost configuration**.</span></span>
2.  <span data-ttu-id="710f3-107">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="710f3-107">Select **New**.</span></span>
3.  <span data-ttu-id="710f3-108">في الحقل **عامل التكلفة**، أدخل **شحن**.</span><span class="sxs-lookup"><span data-stu-id="710f3-108">In the **Cost factor** field, enter **Shipping**.</span></span>
4.  <span data-ttu-id="710f3-109">في حقل **الوصف**، أدخل **تكلفة الشحن**.</span><span class="sxs-lookup"><span data-stu-id="710f3-109">In the **Description** field, enter **Shipping cost**.</span></span>
5.  <span data-ttu-id="710f3-110">في الحقل **نوع التكلفة**، حدد **شحن**.</span><span class="sxs-lookup"><span data-stu-id="710f3-110">In the **Cost type** field, select **Shipping**.</span></span>  
6.  <span data-ttu-id="710f3-111">في الحقل **أساس الحساب**، حدد **بسيط**.</span><span class="sxs-lookup"><span data-stu-id="710f3-111">In the **Calculation basis** field, select **Simple**.</span></span> 
7.  <span data-ttu-id="710f3-112">في علامة التبويب **معايير الحساب**، حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="710f3-112">In the **Calculation criteria** tab, select **Add**.</span></span>
8.  <span data-ttu-id="710f3-113">في حقل **الشركة**، أدخل **USRT**.</span><span class="sxs-lookup"><span data-stu-id="710f3-113">In the **Company** field, enter **USRT**.</span></span>
9.  <span data-ttu-id="710f3-114">في الحقل **وضع التسليم**، أدخل **99**.</span><span class="sxs-lookup"><span data-stu-id="710f3-114">In the **Mode of delivery** field, enter **99**.</span></span>
10. <span data-ttu-id="710f3-115">في الحقل **نوع الحساب**، حدد **ثابت**.</span><span class="sxs-lookup"><span data-stu-id="710f3-115">In the **Calculation type** field, select **Fixed**.</span></span>
11. <span data-ttu-id="710f3-116">في الحقل **التكلفة**، أدخل **10**.</span><span class="sxs-lookup"><span data-stu-id="710f3-116">In the **Cost** field, enter **10**.</span></span> 
12. <span data-ttu-id="710f3-117">في حقل **الشركة**، أدخل **USRT**.</span><span class="sxs-lookup"><span data-stu-id="710f3-117">In the **Company** field, enter **USRT**.</span></span>
13. <span data-ttu-id="710f3-118">في الحقل **وضع التسليم**، أدخل **60**.</span><span class="sxs-lookup"><span data-stu-id="710f3-118">In the **Mode of delivery** field, enter **60**.</span></span>
14. <span data-ttu-id="710f3-119">في الحقل **نوع الحساب**، حدد **‬‏‫لكل وحدة مسافة**.</span><span class="sxs-lookup"><span data-stu-id="710f3-119">In the **Calculation type** field, select **Per distance unit**.</span></span>
15. <span data-ttu-id="710f3-120">في الحقل **التكلفة**، أدخل **0.50**.</span><span class="sxs-lookup"><span data-stu-id="710f3-120">In the **Cost** field, enter **0.50**.</span></span> 
16. <span data-ttu-id="710f3-121">عيّن الحقل **نشط** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="710f3-121">Set the **Active** field to **Yes**.</span></span> 


