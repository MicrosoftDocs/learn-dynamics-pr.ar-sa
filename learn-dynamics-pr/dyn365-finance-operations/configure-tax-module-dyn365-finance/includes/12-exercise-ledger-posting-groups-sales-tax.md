---
ms.openlocfilehash: c06b098b18c45bd2c24221df11cddbd9352d8457
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070914"
---
<span data-ttu-id="6b6a4-101">في هذا التمرين، سوف تقوم بإعداد مجموعات ترحيل دفتر الأستاذ لضريبة المبيعات.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-101">In this exercise, you will set up ledger posting groups for sales tax.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="6b6a4-102">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="6b6a4-102">Before you begin</span></span> 

<span data-ttu-id="6b6a4-103">للحصول على أقصى استفادة من هذا التدريب وغيره من التدريبات الأخرى في هذه الوحدة، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في Finance والتي يتم تثبيتها باستخدام Lifecycle Services.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-103">To get the most benefit from this and other exercises in this module, we recommend that you have the standard sample data available in Finance that is installed via Lifecycle Services.</span></span> 

<span data-ttu-id="6b6a4-104">استخدم الشركة DEMF لكافة التمرينات في هذه الوحدة النمطية.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-104">Use the company DEMF for all exercises in this module.</span></span> 

1.  <span data-ttu-id="6b6a4-105">انتقل إلى **الضريبة > الإعداد > ضريبة المبيعات > مجموعات ترحيل دفتر أستاذ**.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-105">Go to **Tax > Setup > Sales tax > Ledger posting groups**.</span></span>
2.  <span data-ttu-id="6b6a4-106">حدد **جديد** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-106">Select **New** in the Action Pane.</span></span>
3.  <span data-ttu-id="6b6a4-107">في الحقل **مجموعة ترحيل دفتر الأستاذ**، اكتب قيمة.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-107">In the **Ledger posting group** field, type a value.</span></span>
4.  <span data-ttu-id="6b6a4-108">في حقل **الوصف** أدخل قيمة.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-108">In the **Description** field, type a value.</span></span>
5.  <span data-ttu-id="6b6a4-109">في الحقل **ضريبة المبيعات** مستحقة الدفع، حدد الحساب الرئيسي لضرائب المبيعات الصادرة المستحقة لهيئة الضرائب.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-109">In the **Sales tax payable** field, select the main account for outgoing sales taxes that are payable to the tax authority.</span></span>
6.  <span data-ttu-id="6b6a4-110">في الحقل **ضريبة المبيعات مستحقة القبض**، حدد الحساب الرئيسي لضرائب المبيعات الصادرة المستحقة لهيئة الضرائب.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-110">In the **Sales tax receivable** field, select the main account for incoming taxes that are received from the tax authority.</span></span>
7.  <span data-ttu-id="6b6a4-111">في الحقل **استخدام مصروفات الضريبة**، حدد الحساب الرئيسي لترحيل ضرائب الاستخدام الخاضعة للخصم التي لم يتم طلبها أو الإبلاغ عن هيئة الضرائب بواسطة الموردين كجزء من ضريبة القيمة المضافة للتكاليف العكسية في الاتحاد الأوروبي.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-111">In the **Use tax expense** field, select the main account for posting deductible use taxes that are not claimed or reported to the tax authority by vendors as part of EU reverse charge VAT.</span></span> 
8.  <span data-ttu-id="6b6a4-112">في الحقل **استخدام الضريبة مستحقة الدفع**، حدد الحساب الرئيسي لترحيل ضرائب الاستخدام الصادرة المستحقة لهيئة الضرائب.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-112">In the **Use tax payable** field, select the main account for posting incoming use taxes that are payable to tax authorities.</span></span>
9.  <span data-ttu-id="6b6a4-113">في الحقل **حساب التسوية**، حدد الحساب الرئيسي الذي سيتم ترحيل صافي الرصيد الخاص بحسابات دفتر الأستاذ المحدد في حقلي **ضريبة المبيعات مستحقة القبض** و **ضريبة الاستخدام مستحقة القبض**.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-113">In the **Settlement account** field, select the main account that the net balance of the ledger accounts specified in the **Use tax payable** and **Sales tax receivable** fields will be posted.</span></span>
10. <span data-ttu-id="6b6a4-114">في حقل **الخصم النقدي للمورد**، حدد الحساب الرئيسي لترحيل الخصومات النقدية لأكواد ضريبة المبيعات المرتبطة بمجموعة ترحيل دفتر الأستاذ الحالية.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-114">In the **Vendor cash discount** field, select the main account to post cash discounts for sales tax codes associated with this ledger posting group.</span></span>
11. <span data-ttu-id="6b6a4-115">في حقل **الخصم النقدي للعميل**، حدد الحساب الرئيسي لترحيل الخصومات النقدية لأكواد ضريبة المبيعات المرتبطة بمجموعة ترحيل دفتر الأستاذ الحالية.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-115">In the **Customer cash discount** field, select the main account to post cash discounts for sales tax codes associated with this ledger posting group.</span></span>
12. <span data-ttu-id="6b6a4-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="6b6a4-116">Select **Save**.</span></span>

