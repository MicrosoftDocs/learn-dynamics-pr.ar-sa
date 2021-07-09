---
ms.openlocfilehash: 4818c8093b24bf2f950393ada3e15cd603efbda3
ms.sourcegitcommit: 39329122b3d8cf83af3522a38bd0fd4b383e1cc3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/13/2021
ms.locfileid: "6071011"
---
<span data-ttu-id="06dc1-101">تعد أنواع الحركات الثلاثة التي يمكنك استخدامها لترحيل الإهلاك هي **الإهلاك** و **تسوية** **الإهلاك** و **الإهلاك**
**الاستثنائي**.</span><span class="sxs-lookup"><span data-stu-id="06dc1-101">The three Transaction types that you can use to post depreciation are **Depreciation**, **Depreciation** **adjustment**, and **Extraordinary**
**depreciation**.</span></span>

<span data-ttu-id="06dc1-102">**الإهلاك** هو نوع حركة دوري يقلل قيمة أصل ثابت.</span><span class="sxs-lookup"><span data-stu-id="06dc1-102">**Depreciation** is a periodic Transaction type that reduces the value of a fixed asset.</span></span> <span data-ttu-id="06dc1-103">في بعض السلطات، يمكن للشركة الحصول على الخفض في القيمة كخصم ضريبي للفترة.</span><span class="sxs-lookup"><span data-stu-id="06dc1-103">In some jurisdictions, a company can take the reduction in value as a tax deduction for the period.</span></span>

<span data-ttu-id="06dc1-104">يمكنك استخدام نوع حركة **تسوية الإهلاك** للتصحيحات، أو تعديل الإهلاك الذي تم ترحيله بالفعل.</span><span class="sxs-lookup"><span data-stu-id="06dc1-104">You can use the **Depreciation adjustment** Transaction type for corrections to, or the adjustment of, depreciation that is already posted.</span></span>

<span data-ttu-id="06dc1-105">يمكنك استخدام نوع حركة **الإهلاك الاستثنائي** للإهلاك الخاص بالأصول المتزامنة.</span><span class="sxs-lookup"><span data-stu-id="06dc1-105">You can use the **Extraordinary depreciation** Transaction type for concurrent depreciation of assets.</span></span> <span data-ttu-id="06dc1-106">على الرغم من أن وظائف الإهلاك الاستثنائي هي نفس الإهلاك الأساسي، فإن الإهلاك الاستثنائي يعمل بشكل مستقل عن الإهلاك الأساسي.</span><span class="sxs-lookup"><span data-stu-id="06dc1-106">Although Extraordinary depreciation functions the same as basic depreciation, Extraordinary depreciation works independently from the basic depreciation.</span></span> <span data-ttu-id="06dc1-107">ونظراً لذلك، يمكنك ترحيل الإهلاك الاستثنائي والإبلاغ عنه بشكل منفصل عن الإهلاك الأساسي العادي.</span><span class="sxs-lookup"><span data-stu-id="06dc1-107">Because of this, you can post and report Extraordinary depreciation separately from the ordinary, basic depreciation.</span></span>

<span data-ttu-id="06dc1-108">عادة ما يكون **الإهلاك الاستثنائي** حدث يقع مرة واحدة ويتم إعداده في الدفتر.</span><span class="sxs-lookup"><span data-stu-id="06dc1-108">**Extraordinary depreciation** is usually a one-time event and is set up on the book.</span></span> <span data-ttu-id="06dc1-109">يحتوي دفتر يومية الأصول الثابتة على مقترح إهلاك خاص للإهلاك الاستثنائي.</span><span class="sxs-lookup"><span data-stu-id="06dc1-109">The Fixed assets journal contains a special depreciation proposal for Extraordinary depreciation.</span></span>

<span data-ttu-id="06dc1-110">وعادة ما يتم ترحيل الإهلاك باستخدام ملفات تعريف الإهلاك، والتي يمكن إعدادها لإنشاء مقترحات في دفاتر يومية للإهلاك.</span><span class="sxs-lookup"><span data-stu-id="06dc1-110">Typically, depreciation is posted by using depreciation profiles, which can be set up to create proposals in journals for depreciation.</span></span>
<span data-ttu-id="06dc1-111">يمكن أيضا ترحيل الإهلاك يدوياً.</span><span class="sxs-lookup"><span data-stu-id="06dc1-111">Depreciation can also be posted manually.</span></span>

## <a name="depreciation-run-date"></a><span data-ttu-id="06dc1-112">تاريخ تشغيل الإهلاك</span><span class="sxs-lookup"><span data-stu-id="06dc1-112">Depreciation run date</span></span>

<span data-ttu-id="06dc1-113">في الحقل **تاريخ تشغيل الإهلاك**، يعرض الحقل تاريخ البدء المتوقع لحساب الإهلاك الأول.</span><span class="sxs-lookup"><span data-stu-id="06dc1-113">In the **Depreciation run date** field, the field displays the expected starting date for the first depreciation calculation.</span></span> <span data-ttu-id="06dc1-114">هذا هو تاريخ إنشاء الدفتر.</span><span class="sxs-lookup"><span data-stu-id="06dc1-114">This is the date when the book is created.</span></span>

<span data-ttu-id="06dc1-115">لا يمكن حساب أي إهلاك وترحيله قبل **الوضع في تاريخ الخدمة.**</span><span class="sxs-lookup"><span data-stu-id="06dc1-115">No depreciation can be calculated and posted before the **Placed in the service date.**</span></span>

<span data-ttu-id="06dc1-116">ولذلك، إذا تم اعداد الإهلاك للبدء قبل التاريخ التي تم إدخاله في الحقل **الوضع في تاريخ الخدمة**، فان الإهلاك الأول الذي يتم حسابه بعد هذا التاريخ سيتضمن أيضا الإهلاك قبل التاريخ الذي تم إدخاله في الحقل **الوضع في تاريخ الخدمة**.</span><span class="sxs-lookup"><span data-stu-id="06dc1-116">Therefore, if the depreciation is set up to start before the date entered in the **Placed in the service date** field, the first depreciation calculated after that date will also include the depreciation before the date entered in the **Placed in the service date** field.</span></span>

## <a name="example"></a><span data-ttu-id="06dc1-117">مثال</span><span class="sxs-lookup"><span data-stu-id="06dc1-117">Example</span></span>

<span data-ttu-id="06dc1-118">يتم إعداد أحد الأصول بتاريخ 1 يوليو 2019 ويتم إنشاء دفاتر الأصل.</span><span class="sxs-lookup"><span data-stu-id="06dc1-118">An asset is set up on July 1, 2019, and the asset's books are created.</span></span>

<span data-ttu-id="06dc1-119">يتم وضع الأصل الثابت في الخدمة في 31 ديسمبر 2019، ويكون ملف تعريف الإهلاك بالبند الثابت ربع سنوي.</span><span class="sxs-lookup"><span data-stu-id="06dc1-119">The fixed asset is placed in service on December 31, 2019, and the depreciation profile is straight line quarterly.</span></span>

<span data-ttu-id="06dc1-120">يبدأ الإهلاك في 1 يوليو، 2019 (بناء علي القيمة الموجودة في حقل **تاريخ بدء الإهلاك**)، وسعر الاستحواذ هو 10،000.00 دولار أمريكي (USD)، وتكون مدة الخدمة أربعة (أرباع السنة).</span><span class="sxs-lookup"><span data-stu-id="06dc1-120">Depreciation starts on July 1, 2019 (based on the value in the **Depreciation run date** field), the acquisition price is 10,000.00 United States dollars (USD), and the service life is four (quarters).</span></span>

<span data-ttu-id="06dc1-121">عند حساب الإهلاك لأول مره في 31 ديسمبر 2019، فإنه يتم حسابه مقابل USD 5،000.00 (لربعين من الأرباع).</span><span class="sxs-lookup"><span data-stu-id="06dc1-121">When the depreciation is first calculated on December 31, 2019, it is calculated for USD 5,000.00 (for two quarters).</span></span>
