---
ms.openlocfilehash: 3b5a412f0c58117fe3b9031c34791fe830ea1e94
ms.sourcegitcommit: 3b7930e46f1a732939d8d75f99df7bf1f7ccc2ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "6072369"
---
<span data-ttu-id="d4d05-101">يجب إعداد تكوينات عديدة لضمان عمل وظيفة تأجير الأصول بالشكل المطلوب.</span><span class="sxs-lookup"><span data-stu-id="d4d05-101">Several configurations must be set up to ensure that the Asset leasing functionality operates as intended.</span></span>
## <a name="asset-leasing-parameters"></a><span data-ttu-id="d4d05-102">معلمات تأجير الأصول‬</span><span class="sxs-lookup"><span data-stu-id="d4d05-102">Asset leasing parameters</span></span>
1.  <span data-ttu-id="d4d05-103">انتقل إلى **تأجير الأصول > الإعداد > معلمات تأجير الأصول**.</span><span class="sxs-lookup"><span data-stu-id="d4d05-103">Go to **Asset leasing > Setup > Asset leasing parameters**.</span></span>
2.  <span data-ttu-id="d4d05-104">ضمن علامة التبويب **عقود الإيجار**، حدد علامة التبويب السريعة **عام**.</span><span class="sxs-lookup"><span data-stu-id="d4d05-104">On the **Leases** tab, select the **General** FastTab.</span></span>

    - <span data-ttu-id="d4d05-105">تحدد المعلمة **السماح بتجاوز التصنيف اليدوي** ما إذا كان من الممكن تجاوز تصنيف عقد الإيجار قبل تأكيد جدول الدفع.</span><span class="sxs-lookup"><span data-stu-id="d4d05-105">The **Allow manual classification override** parameter determines whether the lease classification can be overridden before the payment schedule is confirmed.</span></span>

    - <span data-ttu-id="d4d05-106">وتقرر معلمة **الدفعة عبر الكيان** ما إذا كان يمكنك الترحيل إلى كيانات قانونية أخرى من الكيان القانوني الحالي.</span><span class="sxs-lookup"><span data-stu-id="d4d05-106">The **Cross-entity batch** parameter determines whether you can post to other legal entities from the current legal entity.</span></span> <span data-ttu-id="d4d05-107">إذا تم تشغيل هذه المعلمة، يمكنك إنشاء إدخالات دفتر اليومية للكيانات القانونية التي يتوفر لديك حق الوصول إليها.</span><span class="sxs-lookup"><span data-stu-id="d4d05-107">If this parameter is turned on, you can create journal entries for the legal entities that you have access to.</span></span>

    - <span data-ttu-id="d4d05-108">عيّن خيار **السماح بعمليات عكس الإهلاك على إصدار دفتر مغلق** إلى **نعم** للسماح بعكس حركات مصروفات الإهلاك.</span><span class="sxs-lookup"><span data-stu-id="d4d05-108">Set the **Allow depreciation reversals on closed book version** option to **Yes** to allow depreciation expense transactions to be reversed.</span></span> <span data-ttu-id="d4d05-109">يمكن عكس حركات المصروفات، حتى عندما يكون إصدار الدفتر مغلقاً.</span><span class="sxs-lookup"><span data-stu-id="d4d05-109">Expense transactions can be reversed, even when the book version is closed.</span></span>

    - <span data-ttu-id="d4d05-110">عيّن خيار **السماح بحذف عقود الإيجار المؤكدة** إلى **نعم** للسماح بحذف عقود الإيجار التي أكدت جداول الدفع.</span><span class="sxs-lookup"><span data-stu-id="d4d05-110">Set the **Allow deletion of confirmed leases** option to **Yes** to allow leases that have confirmed payment schedules to be deleted.</span></span> <span data-ttu-id="d4d05-111">لا يمكن حذف عقود الإيجار عند اقتران الحركات المُرحلة أو غير المرحلة بها، بغض النظر عن إعداد هذا الخيار.</span><span class="sxs-lookup"><span data-stu-id="d4d05-111">Leases can't be deleted if posted or unposted transactions are associated with them, regardless of this option’s setting.</span></span> <span data-ttu-id="d4d05-112">لا يمكنك استعادة سجل عقد إيجار بعد حذفه.</span><span class="sxs-lookup"><span data-stu-id="d4d05-112">You can't restore a lease record after it has been deleted.</span></span> <span data-ttu-id="d4d05-113">إذا قمت بتحميل سجلات لعقد إيجار محذوف، إما يدوياً أو من خلال كيانات البيانات، فسيتم التعامل مع المعلومات التي تم تحميلها على أنها جديدة، وليس كتحديث لعقد إيجار موجود.</span><span class="sxs-lookup"><span data-stu-id="d4d05-113">If you upload records for a deleted lease, either manually or through data entities, the uploaded information is treated as new, not as an update to an existing lease.</span></span> 

        > [!NOTE]
        > <span data-ttu-id="d4d05-114">ونوصي بأن تحتفظ بتعيين الخيار **السماح بحذف عقود الإيجار المؤكدة** إلى القيمة **لا**.</span><span class="sxs-lookup"><span data-stu-id="d4d05-114">We recommend that you keep the **Allow deletion of confirmed leases** option set as **No**.</span></span> <span data-ttu-id="d4d05-115">يتم استخدام تعيين هذا الخيار كوسيلة للتحقق من الصحة والتحكم في منع حدوث إهلاك عرضي لإصدار دفتر مغلق.</span><span class="sxs-lookup"><span data-stu-id="d4d05-115">The setting of this option is used as a validation and control to prevent a closed book version from being accidently depreciated.</span></span>

![لقطة شاشة لصفحة معلمات "تأجير الأصول".](../media/asset-leasing-parameters.png)
