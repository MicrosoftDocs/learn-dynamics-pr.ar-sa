---
ms.openlocfilehash: 2af545f958eab6fda8f812ba5db4d03e069329ae
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073416"
---
<span data-ttu-id="cc2de-101">يمكنك استخدام تكوين المنتج في Dynamics 365 Supply Chain Management لإنشاء العديد من متغيرات المنتجات التي تلبي متطلبات العملاء الفردية.</span><span class="sxs-lookup"><span data-stu-id="cc2de-101">You can use product configuration in Dynamics 365 Supply Chain Management to create many product variants that meet individual customer requirements.</span></span> <span data-ttu-id="cc2de-102">يمكنك تحقيق ذلك بإعادة استخدام مجموعة صغيرة من المكونات التي يمكنك تحديدها واستخدامها في العديد من التركيبات.</span><span class="sxs-lookup"><span data-stu-id="cc2de-102">You can achieve this by reusing a small set of components that you can define and use in many combinations.</span></span> 

<span data-ttu-id="cc2de-103">يمكنك إنشاء نموذج تكوين منتج لتمثيل هيكل منتج عام.</span><span class="sxs-lookup"><span data-stu-id="cc2de-103">You can create a product configuration model to represent a generic product structure.</span></span> <span data-ttu-id="cc2de-104">بعد أن يكون لديك نموذج تكوين منتج كامل، يمكنك إنشاء متغيرات منتج مميزة لها قوائم مكونات أصناف ومسارات فريدة خاصة بها.</span><span class="sxs-lookup"><span data-stu-id="cc2de-104">After you have a complete product configuration model, you can create distinct product variants that have their own unique BOMs and routes.</span></span>

<span data-ttu-id="cc2de-105">تتضمن بعض المجالات الرئيسية التي تمت مناقشتها في هذه الوحدة ما يلي:</span><span class="sxs-lookup"><span data-stu-id="cc2de-105">Some key areas that were discussed in this module include:</span></span>

-   <span data-ttu-id="cc2de-106">**معلمات تكوين المنتج** - ستحدث أخطاء إذا لم يتم تحديد المعلمات عند محاولة اختبار تكوين أو تكوين بند.</span><span class="sxs-lookup"><span data-stu-id="cc2de-106">**Product configuration parameters** - Errors will occur if the parameters are not defined when you try to test a configuration or configure a line.</span></span>

-   <span data-ttu-id="cc2de-107">**المكونات** - يجب إنشاء أو استخدام المكونات الحالية لإضافة مكونات فرعية إلى نموذج تكوين المنتج.</span><span class="sxs-lookup"><span data-stu-id="cc2de-107">**Components** - Must be created or existing components must be used to add subcomponents to a product configuration model.</span></span>

-   <span data-ttu-id="cc2de-108">**أنواع السمات** - حدد القيم المحتملة التي يمكن تعيينها للسمة.</span><span class="sxs-lookup"><span data-stu-id="cc2de-108">**Attribute types** - Define the possible values that can be assigned to an attribute.</span></span> <span data-ttu-id="cc2de-109">يمكن استخدامها لأي سمة في جميع نماذج تكوين المنتج.</span><span class="sxs-lookup"><span data-stu-id="cc2de-109">They can be used for any attribute in all product configuration models.</span></span>

-   <span data-ttu-id="cc2de-110">**المكونات الفرعية** - تمثل الهيكل الشجري لنموذج تكوين المنتج.</span><span class="sxs-lookup"><span data-stu-id="cc2de-110">**Subcomponents** - Represent the tree structure of a product configuration model.</span></span>

-   <span data-ttu-id="cc2de-111">**السمات** - وصف ميزات المنتج.</span><span class="sxs-lookup"><span data-stu-id="cc2de-111">**Attributes** - Describe the features of the product.</span></span>

-   <span data-ttu-id="cc2de-112">**القيود** - تمثيل الشروط التي يجب أن يستوفيها تكوين المنتج.</span><span class="sxs-lookup"><span data-stu-id="cc2de-112">**Constraints** - Represent conditions that a product configuration must satisfy.</span></span>

-   <span data-ttu-id="cc2de-113">**متطلبات المستخدمين** - تشبه المكونات الفرعية، باستثناء أنها لا تحتوي على تعيين رئيسي للعنصر وتتصرف مثل قائمة مكونات الصنف الوهمية.</span><span class="sxs-lookup"><span data-stu-id="cc2de-113">**User requirements** - Resemble subcomponents, except that they do not have the item master mapping and behave like a phantom BOM.</span></span>

-   <span data-ttu-id="cc2de-114">**بنود قائمة مكونات الصنف** - حدد قائمة مكونات الصنف للتصنيع لكل مكون ويمكن أن تشير إلى صنف أو خدمة.</span><span class="sxs-lookup"><span data-stu-id="cc2de-114">**BOM lines** - Identify a manufacturing BOM for each component and can reference an item or a service.</span></span>

-   <span data-ttu-id="cc2de-115">**عمليات المسار** - قم بتضمين عمليات المسار لتحديد طرق التصنيع للمكونات الفرعية.</span><span class="sxs-lookup"><span data-stu-id="cc2de-115">**Route operations** - Include route operations to identify the manufacturing routes for the subcomponents.</span></span> 
