---
ms.openlocfilehash: 7f54ca352562573fdfd5b730ae5b35e99f250887
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071492"
---
<span data-ttu-id="25ae5-101">عند قيامك بتنفيذ كيانات البيانات، يكون الأداء عاملاً رئيسياً.</span><span class="sxs-lookup"><span data-stu-id="25ae5-101">When you are implementing data entities, performance is a major factor.</span></span> <span data-ttu-id="25ae5-102">تكون بنية الكيانات الخاصة بك أمراً أساسياً عندما يتعلق الأمر بالأداء.</span><span class="sxs-lookup"><span data-stu-id="25ae5-102">The architecture of your entities is key when it comes to performance.</span></span>

<span data-ttu-id="25ae5-103">يجب عليك إنشاء كيان يوفر كائناً شاملاً يقوم بتغليف منطق الأعمال في عقد واحد قابل للاستخدام.</span><span class="sxs-lookup"><span data-stu-id="25ae5-103">You should create an entity that provides a holistic object that encapsulates the business logic in one single consumable contract.</span></span> <span data-ttu-id="25ae5-104">وكما ذُكر سابقاً، يتم استخدام كيان البيانات بعد ذلك للكشف عن البيانات من خلال واجهات برمجة التطبيقات (API) مثل OData وإطار عمل الاستيراد/التصدير والتكامل ونموذج البرمجة.</span><span class="sxs-lookup"><span data-stu-id="25ae5-104">As previously mentioned, the data entity is then used to expose data through APIs like OData, import/export framework, integration, and the programming model.</span></span> <span data-ttu-id="25ae5-105">بصفتك مطوراً، يجب عليك التفكير في عدة عوامل للتأكد من أن كيان البيانات الخاص بك مصمم بطريقة تُعزز الأداء وسهولة الصيانة.</span><span class="sxs-lookup"><span data-stu-id="25ae5-105">As a developer, you should consider several factors to ensure that your data entity is designed in a way that promotes performance and easy maintenance.</span></span>  

## <a name="entity-encapsulation"></a><span data-ttu-id="25ae5-106">تغليف الكيان</span><span class="sxs-lookup"><span data-stu-id="25ae5-106">Entity encapsulation</span></span>

-   <span data-ttu-id="25ae5-107">يجب أن تقدّم كياناتك فكرة مجردة بين نموذج البيانات الفعلي ومستهلك الكيان.</span><span class="sxs-lookup"><span data-stu-id="25ae5-107">Your entities should provide an abstraction between the actual data model and the consumer of the entity.</span></span> <span data-ttu-id="25ae5-108">على سبيل المثال، يجب أن يغلف كيان البيانات الجداول الأساسية التي تحدد جميعها معاً الكيان.</span><span class="sxs-lookup"><span data-stu-id="25ae5-108">For example, the data entity should encapsulate the underlying tables that all together define the entity.</span></span>

-   <span data-ttu-id="25ae5-109">ويجب أن تغلف كياناتك عدة جداول ذات صلة لتمثيل الكائن.</span><span class="sxs-lookup"><span data-stu-id="25ae5-109">Your entities should encapsulate multiple related tables to represent the object.</span></span> <span data-ttu-id="25ae5-110">قد تكون هناك حالات يُستخدم فيها جدول واحد.</span><span class="sxs-lookup"><span data-stu-id="25ae5-110">There might be cases where a single table is used.</span></span>

## <a name="have-one-single-public-contract"></a><span data-ttu-id="25ae5-111">وجود عقد عام واحد</span><span class="sxs-lookup"><span data-stu-id="25ae5-111">Have one single public contract</span></span>

-   <span data-ttu-id="25ae5-112">يجب أن يكون العقد العام لكيان البيانات هو نفسه عبر جميع نقاط نهاية التكامل.</span><span class="sxs-lookup"><span data-stu-id="25ae5-112">The public contract for your data entity should be the same across all integration endpoints.</span></span> <span data-ttu-id="25ae5-113">وهذا يسمح بالتناسق للمخطط المنشور، بغض النظر عن آلية تفاعل المستهلك.</span><span class="sxs-lookup"><span data-stu-id="25ae5-113">This allows for consistency for the published schema, regardless of the mechanism for consumer interaction.</span></span>

-   <span data-ttu-id="25ae5-114">عند استهلاك كيان ما، يجب ألا يختلف منطق الأعمال الذي يتم تنفيذه داخل الكيان أثناء عمليات CRUD بناءً على نوع المستهلك.</span><span class="sxs-lookup"><span data-stu-id="25ae5-114">When an entity is consumed, the business logic that's performed within the entity during CRUD operations should not vary based on the type of consumer.</span></span>

## <a name="keep-your-entity-simple"></a><span data-ttu-id="25ae5-115">اجعل كيانك بسيطاً</span><span class="sxs-lookup"><span data-stu-id="25ae5-115">Keep your entity simple</span></span>

-   <span data-ttu-id="25ae5-116">يجب أن يتمكن مستهلك الكيان من التفاعل مع أحد الكيانات بناءً على تعريفات الصناعة أو المجال المقبولة.</span><span class="sxs-lookup"><span data-stu-id="25ae5-116">The entity consumer should be able to interact with an entity based on the accepted industry or domain definitions.</span></span> <span data-ttu-id="25ae5-117">ويجب إخفاء تفاصيل سلوك الكيان ويجب منعها من تشويه التفاعل.</span><span class="sxs-lookup"><span data-stu-id="25ae5-117">The behavior details of the entity should be kept hidden and should be prevented from distorting the interaction.</span></span>

-   <span data-ttu-id="25ae5-118">يجب أن يكون مستهلك الكيان قادراً على التفاعل مع الكيان باستخدام المفتاح الطبيعي للكيان.</span><span class="sxs-lookup"><span data-stu-id="25ae5-118">The consumer of the entity should be able to interact with the entity by using the natural key of the entity.</span></span>
