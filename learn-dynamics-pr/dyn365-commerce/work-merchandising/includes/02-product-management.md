---
ms.openlocfilehash: 3275edb333425bdc211f8bb37597062a0790f588
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070197"
---
<span data-ttu-id="8f9ec-101">يحتوي Commerce على إطار عمل لإنشاء المنتجات وإدارتها يسهل العمليات المبسطة من خلال السماح بإنشاء البيانات مرة واحدة ثم توسيع تلك البيانات لتشمل كيانات قانونية متعددة.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-101">Commerce contains a product creation and management framework that facilitates streamlined processes by allowing for the creation of data once and then extending that data to multiple legal entities.</span></span> <span data-ttu-id="8f9ec-102">باستخدام اطار العمل هذا، فإن الإدخالات المكررة غير ضرورية.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-102">With this framework, duplicate entry is unnecessary.</span></span> 

<span data-ttu-id="8f9ec-103">وفيما يلي نوعان من المنتجات:</span><span class="sxs-lookup"><span data-stu-id="8f9ec-103">The two types of products are:</span></span> 

- <span data-ttu-id="8f9ec-104">المنتجات</span><span class="sxs-lookup"><span data-stu-id="8f9ec-104">Products</span></span>
- <span data-ttu-id="8f9ec-105">أصول المنتجات</span><span class="sxs-lookup"><span data-stu-id="8f9ec-105">Product masters</span></span>

<span data-ttu-id="8f9ec-106">عندما يتم تكوين كلا المنتجين بشكل كامل، يتم تكوينهما على المستوى العمومي ويكونان غير متاحين للاستخدام بعد في أي مكان في النظام.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-106">When both products are fully configured, they are configured at the global level and are not yet available to be used anywhere in the system.</span></span> <span data-ttu-id="8f9ec-107">ويجب إصدارهما إلى الكيانات القانونية التي سيتم استخدامها فيها.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-107">They must be released to the legal entities in which they will be used.</span></span> <span data-ttu-id="8f9ec-108">يسمح هذا الأسلوب بوجود إعداد واحد متسق لصنف يمكن بعد ذلك استخدامه وإدارته بشكل مختلف للمتطلبات الخاصة بالكيان القانوني.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-108">This approach allows for a single consistent setup of an item that can then be used and managed differently for legal entity-specific requirements.</span></span> 

## <a name="products"></a><span data-ttu-id="8f9ec-109">المنتجات</span><span class="sxs-lookup"><span data-stu-id="8f9ec-109">Products</span></span>
<span data-ttu-id="8f9ec-110">المنتجات هي الأصناف الفردية القابلة للجرد التي تتم إدارتها وتصنيفها على أنها وحدة SKU أو رمز شريطي واحد.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-110">Products are single inventoriable items that are managed and categorized as a single SKU or barcode.</span></span> <span data-ttu-id="8f9ec-111">أصول المنتجات هي منتجات فردية لها أشكال متعددة لنفس المنتج، وتسمى متغيرات المنتج.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-111">Product masters are single products that have multiple variations of the same product, called product variants.</span></span> 

<span data-ttu-id="8f9ec-112">ويعد كل متغير منتج منفصل مع الرمز الشريطي الخاص به.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-112">Each variant is a separate product with its own barcode.</span></span> 

## <a name="product-masters"></a><span data-ttu-id="8f9ec-113">أصول المنتجات</span><span class="sxs-lookup"><span data-stu-id="8f9ec-113">Product masters</span></span>
<span data-ttu-id="8f9ec-114">يمكن لأصول المنتجات إنشاء مجموعات متغيرات المنتج باستخدام مجموعة أبعاد منتجات تحدد أبعاد المنتج الصالحة للمنتج: **الحجم**، **واللون**، **والنمط**، **والتكوين**.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-114">Product masters can create product variant combinations by using a product dimension group that defines which product dimensions are valid for the product: **Size**, **Color**, **Style**, and **Configuration**.</span></span> 

<span data-ttu-id="8f9ec-115">على سبيل المثال، يمكن اعتبار القميص منتجاً معيناً لأغراض إعداد التقارير، ولكن يتم بيعه بمواصفات مختلفة مثل صغير أو متوسط أو كبير أو أزرق أو أحمر أو أخضر.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-115">For example, a t-shirt might be considered a specific product for reporting purposes, but it is sold in different specifications such as small, medium, or large, or blue, red, or green.</span></span> <span data-ttu-id="8f9ec-116">يمكن أن يؤدي الجمع بين هذه المواصفات إلى العديد من الأصناف المختلفة ذات وحدات مخزون ورموز شريطية الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-116">The combination of these specifications can result in many different items with their own inventories and barcodes.</span></span> <span data-ttu-id="8f9ec-117">قد لا تكون بعض المجموعات صالحة لجميع الأصناف.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-117">Some combinations might not be valid for all items.</span></span> 

## <a name="variant-suggestions"></a><span data-ttu-id="8f9ec-118">اقتراحات المتغيرات</span><span class="sxs-lookup"><span data-stu-id="8f9ec-118">Variant suggestions</span></span>
<span data-ttu-id="8f9ec-119">تُستخدم وظيفة **اقتراحات المنتج** الموجودة في **Retail وCommerce > المنتجات والفئات > متغيرات المنتج** لإنشاء مجموعات من الأصناف تلقائياً وفقاً للقيم الموجودة في أبعاد المنتج.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-119">The **Variant suggestions** functionality in **Retail and Commerce > Products and categories > Product variants** is used to automatically create combinations of items based on the values in the product dimensions.</span></span> <span data-ttu-id="8f9ec-120">إذا لم تكن هناك أبعاد جديدة متاحة للإنشاء، فسيشير النظام إلى تلك المعلومة.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-120">If no new dimensions are available to generate, the system will indicate that information.</span></span>
 
 
<span data-ttu-id="8f9ec-121">[ ![لقطة شاشة لعلامة تبويب ‏‫اقتراحات المتغيرات‬](../media/variant-suggestions-ssm.jpg) ](../media/variant-suggestions-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="8f9ec-121">[ ![Screenshot of the Variant suggestions tab](../media/variant-suggestions-ssm.jpg) ](../media/variant-suggestions-ssm.jpg#lightbox)</span></span>

<span data-ttu-id="8f9ec-122">شاهد مقطع الفيديو التالي لمعرفة كيفية إنشاء منتج في Commerce.</span><span class="sxs-lookup"><span data-stu-id="8f9ec-122">Watch the following video to learn how to create a Commerce product.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4Afyg]
