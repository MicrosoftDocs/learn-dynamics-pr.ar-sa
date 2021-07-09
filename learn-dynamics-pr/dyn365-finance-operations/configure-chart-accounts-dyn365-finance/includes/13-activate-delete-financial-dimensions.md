---
ms.openlocfilehash: d001781eb70407f4155561d5b806ac1337f69f89
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071079"
---
## <a name="activate-a-financial-dimension"></a><span data-ttu-id="58f32-101">تنشيط بُعد مالي</span><span class="sxs-lookup"><span data-stu-id="58f32-101">Activate a financial dimension</span></span> 

<span data-ttu-id="58f32-102">عند تنشيط بعد مالي، يتم تحديث الجدول بحيث يتضمن اسم البعد المالي.</span><span class="sxs-lookup"><span data-stu-id="58f32-102">When you activate a financial dimension, the table is updated so that it includes the name of the financial dimension.</span></span> <span data-ttu-id="58f32-103">تتم إزالة الأبعاد المحذوفة.</span><span class="sxs-lookup"><span data-stu-id="58f32-103">Deleted dimensions are removed.</span></span> <span data-ttu-id="58f32-104">يمكنك إدخال قيم الأبعاد قبل تنشيط البُعد المالي.</span><span class="sxs-lookup"><span data-stu-id="58f32-104">You can enter dimension values before you activate a financial dimension.</span></span> 

<span data-ttu-id="58f32-105">لا يمكن استخدام بُعد مالي في Finance حتى يتم تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="58f32-105">A financial dimension cannot be used in Finance until it's activated.</span></span> 

<span data-ttu-id="58f32-106">على سبيل المثال، لا يمكن إضافة بعد مالي إلى بنية حساب حتى يتم تنشيط البُعد المالي.</span><span class="sxs-lookup"><span data-stu-id="58f32-106">For example, you can't add a financial dimension to an account structure until the financial dimension has been activated.</span></span> <span data-ttu-id="58f32-107">عند تحديد **تنشيط**، يتم تحديث كافة الأبعاد وسيتم تحديث حقل **الحالة** إلى **نشط**.</span><span class="sxs-lookup"><span data-stu-id="58f32-107">When you select **Activate**, all dimensions are updated and the **Status** field will be updated to **Active**.</span></span>

<span data-ttu-id="58f32-108">**دفتر الأستاذ العام > دليل الحسابات > الحسابات > الأبعاد المالية**</span><span class="sxs-lookup"><span data-stu-id="58f32-108">**General ledger > Chart of accounts > Accounts > Financial dimensions**</span></span>
 
![لقطة شاشة لصفحة الأبعاد المالية مع تمييز تنشيط.](../media/activate-dim.png)

## <a name="translations"></a><span data-ttu-id="58f32-110">الترجمات</span><span class="sxs-lookup"><span data-stu-id="58f32-110">Translations</span></span> 

<span data-ttu-id="58f32-111">في الصفحة **ترجمات النص**، يمكنك إدخال نص للبُعد المالي المحدد بلغات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="58f32-111">On the **Text translations** page, you can enter text for the selected financial dimension in various languages.</span></span> <span data-ttu-id="58f32-112">في أية صفحة في Finance تحتوي على الزر **ترجمات**، مثل الصفحة **ترجمة الحساب الرئيسي**، يمكنك إدخال هذا النص.</span><span class="sxs-lookup"><span data-stu-id="58f32-112">In any page in Finance that has a **Translations** button, such as on the **Main account translation** page, you can enter this text.</span></span>
 
<span data-ttu-id="58f32-113">[![لقطة شاشة لصفحة ترجمات النص في Finance and Operations.](../media/translation-1.png)](../media/translation-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="58f32-113">[![Screenshot of the Finance and Operations Text translations page.](../media/translation-1.png)](../media/translation-1.png#lightbox)</span></span>

## <a name="legal-entity-overrides"></a><span data-ttu-id="58f32-114">تجاوزات الكيان القانوني</span><span class="sxs-lookup"><span data-stu-id="58f32-114">Legal entity overrides</span></span> 

<span data-ttu-id="58f32-115">لا تكون كافة الأبعاد صالحة لكافة الكيانات القانونية.</span><span class="sxs-lookup"><span data-stu-id="58f32-115">Not all dimensions are valid for all legal entities.</span></span> <span data-ttu-id="58f32-116">كذلك، قد تكون بعض الأبعاد مرتبطة فقط لفترة محددة.</span><span class="sxs-lookup"><span data-stu-id="58f32-116">Also, some dimensions might be relevant only for a specific period.</span></span> <span data-ttu-id="58f32-117">في هذه الحالات، يمكنك استخدام القسم **تجاوزات الكيان القانوني** لتحديد الشركات التي يجب أن يتم إيقاف البُعد بها بشكل مؤقت للمالك والفترة التي يكون البُعد نشطاً فيها.</span><span class="sxs-lookup"><span data-stu-id="58f32-117">In these cases, you can use the **Legal entity overrides** section to specify the companies that the dimension should be suspended for, the owner, and the period when the dimension is active.</span></span>

<span data-ttu-id="58f32-118">**دفتر الأستاذ العام > دليل الحسابات > الأبعاد > الأبعاد المالية** ثم حدد بعداً مالياً وحدد **قيم الأبعاد**.</span><span class="sxs-lookup"><span data-stu-id="58f32-118">**General ledger > Chart of accounts > Dimensions > Financial dimensions** and then select a Financial dimension and select **Dimension values**.</span></span>
 
<span data-ttu-id="58f32-119">[![جزء لقطة شاشة لصفحة قسم تجاوزات الكيان القانوني في الأبعاد المالية.](../media/legal-entity-overrides.png)](../media/legal-entity-overrides.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="58f32-119">[![Screenshot of the  Legal entity overrides section on the Financial dimensions page.](../media/legal-entity-overrides.png)](../media/legal-entity-overrides.png#lightbox)</span></span>


 
## <a name="delete-a-financial-dimension"></a><span data-ttu-id="58f32-120">حذف بُعد مالي</span><span class="sxs-lookup"><span data-stu-id="58f32-120">Delete a financial dimension</span></span> 

<span data-ttu-id="58f32-121">للمساعدة في الحفاظ على التكامل المرجعي للبيانات، يمكن أن يتم حذف الأبعاد المالية في حالات نادرة.</span><span class="sxs-lookup"><span data-stu-id="58f32-121">To help maintain referential integrity of the data, financial dimensions can rarely be deleted.</span></span> <span data-ttu-id="58f32-122">إذا حاولت حذف بعد مالي، يتم تقييم المعايير التالية:</span><span class="sxs-lookup"><span data-stu-id="58f32-122">If you try to delete a financial dimension, the following criteria are evaluated:</span></span>

- <span data-ttu-id="58f32-123">هل تم استخدام البُعد المالي في أية حركات مرحلة أو غير مرحلة، أو في أي نوع من مجموعة قيم الأبعاد؟</span><span class="sxs-lookup"><span data-stu-id="58f32-123">Has the financial dimension been used on any posted or unposted transactions, or in any type of dimension value combination?</span></span>
- <span data-ttu-id="58f32-124">هل البُعد المالي مستخدم في أيه بنية حساب نشط أو بنية قاعدة متقدمة أو مجموعة أبعاد مالية؟</span><span class="sxs-lookup"><span data-stu-id="58f32-124">Is the financial dimension used in any active account structure, advanced rule structure, or financial dimension set?</span></span>
- <span data-ttu-id="58f32-125">هل البُعد المالي هو جزء من تنسيق تكامل البُعد المالي الافتراضي؟</span><span class="sxs-lookup"><span data-stu-id="58f32-125">Is the financial dimension part of a default financial dimension integration format?</span></span>
- <span data-ttu-id="58f32-126">هل تم إعداد البُعد المالي كبعد افتراضي؟</span><span class="sxs-lookup"><span data-stu-id="58f32-126">Has the financial dimension been set up as a default dimension?</span></span>

<span data-ttu-id="58f32-127">في حالة استيفاء أي من هذه المعايير، لن يمكنك حذف البُعد المالي.</span><span class="sxs-lookup"><span data-stu-id="58f32-127">If any of these criteria are met, you cannot delete the financial dimension.</span></span>

