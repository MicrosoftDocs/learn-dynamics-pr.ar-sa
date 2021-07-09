---
ms.openlocfilehash: f0b5584304f067b833820ca8c0b119775dd5dfba
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072290"
---
<span data-ttu-id="af68a-101">توفر العملية الحسابية **مكان استخدام الصنف** نظرة عامة على مكان استخدام الصنف في إدارة الأصول وتتضمن كيفية استخدام الصنف في أثناء مدة بقائه.</span><span class="sxs-lookup"><span data-stu-id="af68a-101">The **Item where used** calculation provides an overview of where the item is in use in Asset Management and includes how the item was used during its lifetime.</span></span> <span data-ttu-id="af68a-102">يمكن فتح صفحة **مكان استخدام الصنف** من قائمة إدارة الأصول الرئيسية، كما يمكن الوصول إليها من الصفحات الآتية:</span><span class="sxs-lookup"><span data-stu-id="af68a-102">The **Item where used** page can be opened from the main Asset Management menu, and it can also be accessed from the following pages:</span></span>

- <span data-ttu-id="af68a-103">**‏‫قوائم مكونات الأصناف (BOM)‬‬ الخاصة بالأصول**</span><span class="sxs-lookup"><span data-stu-id="af68a-103">**Asset BOMs**</span></span>
- <span data-ttu-id="af68a-104">**الأجزاء الاحتياطية** في الإعدادات الافتراضية لنوع الأصل‬</span><span class="sxs-lookup"><span data-stu-id="af68a-104">**Spare parts** on asset type defaults</span></span>
- <span data-ttu-id="af68a-105">**فئات أنواع مهام الصيانة** و **أنواع مهام الصيانة** و **متغيرات أنواع مهام الصيانة** و **‏‫العمليات التجارية المرتبطة بأنواع مهام الصيانة‬** و **قوائم فحص الصيانة**</span><span class="sxs-lookup"><span data-stu-id="af68a-105">**Maintenance job type categories** and **Maintenance job types**, **Maintenance job type variants**, **Maintenance job trades**, and **Maintenance checklists**</span></span>
- <span data-ttu-id="af68a-106">**التنبؤ بمتطلبات الصيانة**</span><span class="sxs-lookup"><span data-stu-id="af68a-106">**Maintenance forecast**</span></span>
- <span data-ttu-id="af68a-107">**المشتريات**</span><span class="sxs-lookup"><span data-stu-id="af68a-107">**Procurement**</span></span>
- <span data-ttu-id="af68a-108">**شراء أمر العمل**</span><span class="sxs-lookup"><span data-stu-id="af68a-108">**Work order purchase**</span></span>

<span data-ttu-id="af68a-109">لإنشاء العملية الحسابية "مكان استخدام الصنف"، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="af68a-109">To create an item-where-used calculation, follow these steps:</span></span>

1.  <span data-ttu-id="af68a-110">انتقل إلى **إدارة الأصول > الاستعلامات > مكان استخدام الصنف** أو حدد زر **مكان استخدام الصنف** في إحدى الصفحات المذكورة سابقاً.</span><span class="sxs-lookup"><span data-stu-id="af68a-110">Go to **Asset management > Inquiries > Item where used** or select the **Item where used** button on one of the pages mentioned previously.</span></span>
2.  <span data-ttu-id="af68a-111">في مربع حوار **مكان استخدام الصنف**، حدد الصنف الذي ترغب في إجراء عملية حسابية له في حقل رقم الصنف، مثل **A0001**.</span><span class="sxs-lookup"><span data-stu-id="af68a-111">In the **Item where used** dialog box, select the item for which you want to make the calculation in the Item number field, for example, **A0001**.</span></span>
3.  <span data-ttu-id="af68a-112">يعمل حقل **المستوى** على تعيين مدى تفاصيل سطور الصنف التي تريدها لأماكن العمل.</span><span class="sxs-lookup"><span data-stu-id="af68a-112">The **Level** field assigns how detailed you want the item lines to be for functional locations.</span></span>
    - <span data-ttu-id="af68a-113">**1** = ستتم إضافة جميع المواقع مع بعضها في موقع عمل متعدد المستويات ويتم عرضها في موقع عمل من المستوى الأعلى.</span><span class="sxs-lookup"><span data-stu-id="af68a-113">**1** = All locations in a multi-level functional location will be added together and shown in the top-level functional location.</span></span>
    - <span data-ttu-id="af68a-114">**0** = سيتم عرض جميع القيم التفصيلية لجميع البنود متعددة المستويات لموقع العمل.</span><span class="sxs-lookup"><span data-stu-id="af68a-114">**0** = All detailed values of all multi-level lines of the functional location will be shown.</span></span>
4.  <span data-ttu-id="af68a-115">في قسم **تضمين**، حدد **نعم** في أزرار التبديل التي تريد تضمينها في العملية الحسابية.</span><span class="sxs-lookup"><span data-stu-id="af68a-115">In the **Include** section, select **Yes** on the toggle buttons that you want to include in the calculation.</span></span>
5.  <span data-ttu-id="af68a-116">حدد **موافق** لبدء الحساب.</span><span class="sxs-lookup"><span data-stu-id="af68a-116">Select **OK** to start the calculation.</span></span>
6.  <span data-ttu-id="af68a-117">في علامة التبويب **مكان استخدام الصنف**، حدد زر **تصنيف حسب** لإظهار مستوى التفاصيل المطلوب للعملية الحسابية.</span><span class="sxs-lookup"><span data-stu-id="af68a-117">On the **Item where used** tab, select the **Group by** buttons to show the required detail level of the calculation.</span></span> <span data-ttu-id="af68a-118">يتم تمييز أزرار **تجميع حسب** المحددة.</span><span class="sxs-lookup"><span data-stu-id="af68a-118">The selected **Group by** buttons are highlighted.</span></span> <span data-ttu-id="af68a-119">حدد زراً لتنشيطه أو إلغاء تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="af68a-119">Select a button to activate or deactivate it.</span></span>
7.  <span data-ttu-id="af68a-120">إذا كنت ترغب في عرض الأبعاد المرتبطة بالصنف، فحدد **أبعاد العرض** ثم حدد الأبعاد التي سيتم عرضها.</span><span class="sxs-lookup"><span data-stu-id="af68a-120">If you want to show dimensions that are related to the item, select **Display dimensions** and then select the dimensions to be shown.</span></span>


<span data-ttu-id="af68a-121">**إدارة الأصول > الاستعلامات > مكان استخدام الصنف**</span><span class="sxs-lookup"><span data-stu-id="af68a-121">**Asset management > Inquiries > Item where used**</span></span>
 

![لقطة شاشة لصفحة "مكان استخدام الصنف".](../media/item-where-used-ss.png)
 


