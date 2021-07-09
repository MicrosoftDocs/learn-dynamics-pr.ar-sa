---
ms.openlocfilehash: 296c1965b76adf91e143b2900896c0d8bd92617c
ms.sourcegitcommit: 0484f01637a384540476f9c6e45ba64bd86526a8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/19/2021
ms.locfileid: "6070415"
---
<span data-ttu-id="7ce10-101">تُستخدم أكواد المعلومات للحصول على معلومات إضافية وراء الإجراءات التي تحدث في قنوات Commerce في نقطة البيع ومركز الاتصال.</span><span class="sxs-lookup"><span data-stu-id="7ce10-101">Info codes are used to capture additional information behind actions that occur in the POS and call center Commerce channels.</span></span> <span data-ttu-id="7ce10-102">يمكن إعداد أكواد المعلومات في **البيع بالتجزئة والتجارة> إعداد القناة> أكواد المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="7ce10-102">Info codes can be set up in **Retail and Commerce > Channel Setup > Info codes**.</span></span>

<span data-ttu-id="7ce10-103">يمكن أن تكون البيانات الملتقطة أحد أنواع الإدخالات التالية:</span><span class="sxs-lookup"><span data-stu-id="7ce10-103">The captured data can be one of the following input types:</span></span>

-   <span data-ttu-id="7ce10-104">**بلا**</span><span class="sxs-lookup"><span data-stu-id="7ce10-104">**None**</span></span>
-   <span data-ttu-id="7ce10-105">**قائمة الرموز الفرعية** (قائمة نصية محددة مسبقاً)</span><span class="sxs-lookup"><span data-stu-id="7ce10-105">**Subcode list** (a predefined text list)</span></span>
-   <span data-ttu-id="7ce10-106">**تاريخ‬**</span><span class="sxs-lookup"><span data-stu-id="7ce10-106">**Date**</span></span>
-   <span data-ttu-id="7ce10-107">**رقمي**</span><span class="sxs-lookup"><span data-stu-id="7ce10-107">**Numeric**</span></span>
-   <span data-ttu-id="7ce10-108">**منتج** (من قائمة المنتجات)</span><span class="sxs-lookup"><span data-stu-id="7ce10-108">**Product** (from products list)</span></span>
-   <span data-ttu-id="7ce10-109">**عميل** (من قائمة العملاء)</span><span class="sxs-lookup"><span data-stu-id="7ce10-109">**Customer** (from customers list)</span></span>
-   <span data-ttu-id="7ce10-110">**معرف العامل** (من معرف العامل)</span><span class="sxs-lookup"><span data-stu-id="7ce10-110">**Operator ID** (from worker ID)</span></span>
-   <span data-ttu-id="7ce10-111">**نص**</span><span class="sxs-lookup"><span data-stu-id="7ce10-111">**Text**</span></span> 
-   <span data-ttu-id="7ce10-112">**أزرار الرموز الفرعية**</span><span class="sxs-lookup"><span data-stu-id="7ce10-112">**Subcode buttons**</span></span>
-   <span data-ttu-id="7ce10-113">**الحد العمري**</span><span class="sxs-lookup"><span data-stu-id="7ce10-113">**Age limit**</span></span>

<span data-ttu-id="7ce10-114">اعتماداً على نوع الإدخال، يمكن للمستخدمين تعيين العديد من الحدود والقيود لأنواع معينة من أكواد المعلومات.</span><span class="sxs-lookup"><span data-stu-id="7ce10-114">Depending on the input type, users can assign various limitations and restrictions for certain info code types.</span></span> <span data-ttu-id="7ce10-115">يمكن أن تتطلب بعض أكواد المعلومات إدخالاً، والتشغيل مرة واحدة فقط لكل حركة (بغض النظر عن المنتجات)، وربط أكواد معلومات متعددة معاً، وغير ذلك الكثير.</span><span class="sxs-lookup"><span data-stu-id="7ce10-115">Some info codes can require input, only trigger once for each transaction (regardless of products), link multiple info codes together, and more.</span></span> 
 

![لقطة شاشة لصفحة أكواد معلومات Dynamics 365 Commerce.](../media/info-codes-17-ss.jpg) 

<span data-ttu-id="7ce10-117">مجموعات أكواد المعلومات هي تجميعات منطقية لأكواد المعلومات المكونة.</span><span class="sxs-lookup"><span data-stu-id="7ce10-117">Info code groups are logical groupings of the configured info codes.</span></span> <span data-ttu-id="7ce10-118">تتيح مجموعات أكواد المعلومات إعادة الاستخدام المتسق لأكواد المعلومات المتعددة لمنتجات متعددة.</span><span class="sxs-lookup"><span data-stu-id="7ce10-118">Info code groups enable consistent reuse of multiple info codes for multiple products.</span></span> <span data-ttu-id="7ce10-119">يمكن العثور على الصفحة التالية ضمن **البيع بالتجزئة والتجارة> إعداد القناة> مجموعات أكواد المعلومات**</span><span class="sxs-lookup"><span data-stu-id="7ce10-119">The following page can be found under **Retail and Commerce > Channel Setup > Info code groups**</span></span>
 

![لقطة شاشة لصفحة مجموعات أكواد المعلومات في Dynamics 365 Commerce.](../media/code-groups-18-ss.jpg)

<span data-ttu-id="7ce10-121">يتم بعد ذلك تكوين أكواد المعلومات التي تم إنشاؤها في ملفات تعريف الوظائف ضمن القسم **ملفات تعريف وظائف نقطة البيع > أكواد المعلومات** في **البيع بالتجزئة والتجارة> إعداد القناة> إعداد نقطة البيع> ملفات تعريف نقطة البيع> ملفات تعريف الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="7ce10-121">Created info codes are then configured on the functionality profiles under the **POS functionality profiles > Info codes** section in **Retail and Commerce > Channel Setup > POS setup > POS profiles > Functionality profiles**.</span></span> <span data-ttu-id="7ce10-122">يمكن أن يكون للعديد من الإجراءات المحددة مسبقاً أكواد معلومات مختلفة مخصصة لها.</span><span class="sxs-lookup"><span data-stu-id="7ce10-122">Several pre-defined actions can have different information codes assigned to them.</span></span> <span data-ttu-id="7ce10-123">يتم تعيين ملفات تعريف الوظائف للقنوات مباشرةً، بحيث يمكنك الحصول على تكوينات أكواد المعلومات المعينة لجميع القنوات كمجموعة أو لمجموعات قنوات قليلة أو لكل قناة على حدة لجعلها فريدة.</span><span class="sxs-lookup"><span data-stu-id="7ce10-123">Functionality profiles are assigned to channels directly, so you can have info code configurations assigned to all channels as a group, to a few channel groups, or to each channel individually to make them unique.</span></span>  


![لقطة شاشة لصفحة ملفات تعريف وظائف نقطة البيع.](../media/functionality-profiles-19-ssm.jpg)

<span data-ttu-id="7ce10-125">يمكن الوصول إلى أكواد المعلومات التي تم إدخالها من خلال الكشوف مباشرةً من خلال صفحة **حركات أكواد المعلومات** في **البيع بالتجزئة والتجارة> الاستعلامات والتقارير> حركات المتجر**.</span><span class="sxs-lookup"><span data-stu-id="7ce10-125">Info codes that are entered can be accessed through the statements directly through the **Info codes transactions** page in **Retail and Commerce > Inquiries and reports > Store transactions**.</span></span>
 

<span data-ttu-id="7ce10-126">[ ![لقطة شاشة لصفحة حركات المتجر في Dynamics 365 Commerce.](../media/store-transactions-20-ssm.jpg) ](../media/store-transactions-20-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ce10-126">[ ![Screenshot of the Dynamics 365 Commerce store transactions page.](../media/store-transactions-20-ssm.jpg) ](../media/store-transactions-20-ssm.jpg#lightbox)</span></span>
