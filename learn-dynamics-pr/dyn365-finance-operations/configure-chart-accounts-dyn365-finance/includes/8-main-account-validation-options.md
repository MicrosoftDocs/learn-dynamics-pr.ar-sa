---
ms.openlocfilehash: abffc8274ae5c4182e6e1971c4a56d32892a6a3e
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071077"
---
<span data-ttu-id="8026a-101">توجد أربعة إعدادات للتحقق من صحة الترحيل يمكن تحديدها لكل حساب.</span><span class="sxs-lookup"><span data-stu-id="8026a-101">There are four posting validation settings that can be defined for each account.</span></span> <span data-ttu-id="8026a-102">يمكن تعيين التحقق من صحة الترحيل للخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="8026a-102">Posting validation can be set for the following options:</span></span> 

- <span data-ttu-id="8026a-103">‏رمز العملة</span><span class="sxs-lookup"><span data-stu-id="8026a-103">Currency code</span></span>
- <span data-ttu-id="8026a-104">معرِف المستخدم</span><span class="sxs-lookup"><span data-stu-id="8026a-104">User ID</span></span>  
- <span data-ttu-id="8026a-105">أنواع الترحيل</span><span class="sxs-lookup"><span data-stu-id="8026a-105">Posting types</span></span>
- <span data-ttu-id="8026a-106">نوع ترحيل ضريبة المبيعات لمجموعة ترحيل دفتر الأستاذ</span><span class="sxs-lookup"><span data-stu-id="8026a-106">Sales tax posting type for ledger posting group</span></span>

<span data-ttu-id="8026a-107">يمكن أن تستند إعدادات التحقق من الصحة إلى المعايير التالية:</span><span class="sxs-lookup"><span data-stu-id="8026a-107">Validation settings can be based on the following criteria:</span></span> 

- <span data-ttu-id="8026a-108">**اختياري** - لا يتم التحقق من صحة الحقل وقت الترحيل.</span><span class="sxs-lookup"><span data-stu-id="8026a-108">**Optional** - The field is not validated at the time of posting.</span></span> <span data-ttu-id="8026a-109">ويكون ذلك هو الإعداد الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="8026a-109">This is the default setting.</span></span>  
- <span data-ttu-id="8026a-110">**مطلوب** - يتحقق النظام من اكتمال الحقل للترحيل.</span><span class="sxs-lookup"><span data-stu-id="8026a-110">**Required** - The system verifies that the field is completed for posting.</span></span> <span data-ttu-id="8026a-111">لم يتم التحقق من القيمة.</span><span class="sxs-lookup"><span data-stu-id="8026a-111">The value is not checked.</span></span>  
- <span data-ttu-id="8026a-112">**تحديد خيار واحد صالح** - يتحقق النظام من اكتمال الحقل للترحيل وأن القيمة تتوافق مع القيمة المحددة في الحساب.</span><span class="sxs-lookup"><span data-stu-id="8026a-112">**Specify single valid option** - The system verifies that the field is completed for posting and that the value corresponds with the value specified in the account.</span></span>  
- <span data-ttu-id="8026a-113">**تحديد عدة خيارات صالحة** - يتحقق النظام من اكتمال الحقل بإحدى القيم المحددة في الزر **قائمة التحقق من الصحة**.</span><span class="sxs-lookup"><span data-stu-id="8026a-113">**Specify multiple valid options** - The system verifies that the field is completed with one of the values that are defined on the **Validation list** button.</span></span> <span data-ttu-id="8026a-114">إنه يمكّن أزرار التحقق من الصحة مثل **التحقق من صحة المستخدم** و **التحقق من صحة الترحيل**.</span><span class="sxs-lookup"><span data-stu-id="8026a-114">It enables the validation buttons such as **User validation** and **Posting validation**.</span></span> 

### <a name="scenario"></a><span data-ttu-id="8026a-115">السيناريو</span><span class="sxs-lookup"><span data-stu-id="8026a-115">Scenario</span></span>

<span data-ttu-id="8026a-116">يطلب قسم الشؤون المالية للشركة أن يقوم أشخاص معينون فقط بترحيل الحركات التي تقع تحت نوع ترحيل ضريبة المبيعات.</span><span class="sxs-lookup"><span data-stu-id="8026a-116">A company's finance department requires that only specific persons can post transactions that have the Sales tax posting type.</span></span>

<span data-ttu-id="8026a-117">والحل لهذا هو تعيين إعداد التحقق من صحة إلى **التحقق من المستخدم** ليكون **تحديد عدة خيارات صالحة** وأنواع الترحيل إلى **تحديد خيار واحد صالح**.</span><span class="sxs-lookup"><span data-stu-id="8026a-117">The solution for this is to set up the validation setting for **Validate user** to be **Specify multiple valid options** and Posting types to be **Specify single valid option**.</span></span>

<span data-ttu-id="8026a-118">**دفتر الأستاذ العام > دليل الحسابات > الحسابات > الحسابات الرئيسية**</span><span class="sxs-lookup"><span data-stu-id="8026a-118">**General ledger > Chart of accounts > Accounts > Main accounts**</span></span>

<span data-ttu-id="8026a-119">[![لقطة شاشة من القائمة المنسدلة للتحقق من صحة المستخدم في علامة التبويب السريعة التحقق من صحة الترحيل.](../media/posting-validation.png)](../media/posting-validation.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="8026a-119">[![Screenshot of the Validate user dropdown list in the Posting validation FastTab.](../media/posting-validation.png)](../media/posting-validation.png#lightbox)</span></span>



