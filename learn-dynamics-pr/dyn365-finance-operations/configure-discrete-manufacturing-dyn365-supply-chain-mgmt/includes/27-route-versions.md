---
ms.openlocfilehash: ea533d426a21d6c55a341e4a716222e242354aa8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073512"
---
<span data-ttu-id="9440d-101">تُستخدم إصدارات المسارات لاستيعاب الاختلافات في إنتاج المنتجات، أو لتزويدك بتحكم أكبر في عملية الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="9440d-101">Route versions are used to accommodate variations in the production of products, or to provide you greater control over the production process.</span></span>
<span data-ttu-id="9440d-102">إنها إصدارات بديلة من المسار الرئيسي الذي يستوعب الاختلافات في إنتاج نفس الصنف.</span><span class="sxs-lookup"><span data-stu-id="9440d-102">They are alternative versions of the main route that accommodate variations in the production of the same item.</span></span>

<span data-ttu-id="9440d-103">على سبيل المثال، إذا كنت تحتاج فقط إلى تغيير بعض الأصناف على مسار لتلبية متطلبات أمر إنتاج معين، فيمكنك توفير التكاليف عن طريق إنشاء إصدار مسار جديد وتغييره بحيث يتم استخدام أجهزة مختلفة تتطلب قدرة أقل بدلاً من الآلات المستخدمة في المسار الأصلي.</span><span class="sxs-lookup"><span data-stu-id="9440d-103">For example, if you only need to change a few items on a route to meet the requirements of a specific production order, you can save costs by creating a new route version and changing it so that different machines that require less capacity are used instead of the machines that are used on the original route.</span></span>

<span data-ttu-id="9440d-104">عند تحديد مسار أو إصدار مسار من أعلى صفحة **المسار**، يمكنك عرض تفاصيل الأصناف التي يحتوي عليها في قسم الإصدار في الجزء السفلي.</span><span class="sxs-lookup"><span data-stu-id="9440d-104">When you select a route or a route version from the top of the **Route** page, you can view a breakdown of the items it contains in the Version section at the bottom.</span></span>

<span data-ttu-id="9440d-105">يتم سرد كل صنف في المسار ويحتوي على تفاصيل حول المواد والعمليات المرتبطة بأمر الإنتاج الذي تم إنشاء الصنف منه.</span><span class="sxs-lookup"><span data-stu-id="9440d-105">Each item in the route is listed and it contains details about the material and operations that are associated with the production order from which the item originates.</span></span>

<span data-ttu-id="9440d-106">**مثال**</span><span class="sxs-lookup"><span data-stu-id="9440d-106">**Example**</span></span>

<span data-ttu-id="9440d-107">يوضح هذا المثال تعريف أرقام العمليات بمزيد من التفصيل.</span><span class="sxs-lookup"><span data-stu-id="9440d-107">This example explains the definition of operation numbers in more detail.</span></span> <span data-ttu-id="9440d-108">تظهر العملية الأولى على أنها العملية رقم 10 (اللحام)، والتالية كرقم العملية 20 (التجميع)، والأخيرة كرقم العملية 30 (الحزمة).</span><span class="sxs-lookup"><span data-stu-id="9440d-108">The first operation is shown as operation number 10 (Weld), the next as operation number 20 (Assemble), and the last as operation number 30 (Pack).</span></span>

<span data-ttu-id="9440d-109">كما هو مذكور، تحتوي كل عملية في مسار الإنتاج على رقم تعريف يحدد المهام المتضمنة في تصنيع الصنف.</span><span class="sxs-lookup"><span data-stu-id="9440d-109">As stated, each operation in the production route has an identifying number that identifies the tasks that are involved in manufacturing the item.</span></span> <span data-ttu-id="9440d-110">يتم دائماً تمثيل العملية الأولى بأقل رقم عملية في التسلسل.</span><span class="sxs-lookup"><span data-stu-id="9440d-110">The first operation is always represented by the lowest operation number in the sequence.</span></span> <span data-ttu-id="9440d-111">يتم دائماً تمثيل العملية الأخيرة بالقيمة 0 (صفر) في الحقل **التالي**.</span><span class="sxs-lookup"><span data-stu-id="9440d-111">The last operation is always represented by the value 0 (zero) in the **Next** field.</span></span>

-   <span data-ttu-id="9440d-112">10 اللحام 20</span><span class="sxs-lookup"><span data-stu-id="9440d-112">10 Weld 20</span></span>

-   <span data-ttu-id="9440d-113">20 تجميع 30</span><span class="sxs-lookup"><span data-stu-id="9440d-113">20 Assemble 30</span></span>

-   <span data-ttu-id="9440d-114">30 حزمة 0</span><span class="sxs-lookup"><span data-stu-id="9440d-114">30 Pack 0</span></span>

<span data-ttu-id="9440d-115">إذا كان الصنف لا يحتوي على مسار في البيانات الأساسية، فسيكون مسار الإنتاج فارغاً.</span><span class="sxs-lookup"><span data-stu-id="9440d-115">If an item does not have a route in base data, the production route is blank.</span></span> <span data-ttu-id="9440d-116">يمكنك إجراء تغييرات على مسارات الإنتاج فقط على الطلبات حتى تلك التي تم تعيينها لحالة البدء وتضمينها.</span><span class="sxs-lookup"><span data-stu-id="9440d-116">You can make changes to production routes only on orders up to and including those assigned the Start status.</span></span> <span data-ttu-id="9440d-117">إذا كانت تغييراتك تؤثر على تقدير التكلفة أو جدولة الوظائف، فقم بإجراء التقدير و/أو إجراءات جدولة العمليات/الوظيفة مرة أخرى قبل المتابعة.</span><span class="sxs-lookup"><span data-stu-id="9440d-117">If your changes affect cost estimation or job scheduling, run the estimation and/or operations/job scheduling procedures again before proceeding.</span></span>
