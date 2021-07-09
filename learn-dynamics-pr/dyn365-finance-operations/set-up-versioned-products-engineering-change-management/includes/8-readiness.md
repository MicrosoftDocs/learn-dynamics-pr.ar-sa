---
ms.openlocfilehash: 2582c6efd64b65058eea5a35af859977be429fdb
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074935"
---
<span data-ttu-id="63a84-101">توفر سياسات جاهزية المنتج فحصاً للتأكد من تحديد جميع البيانات الرئيسية المطلوبة لمنتج قبل استخدامه في الحركات.</span><span class="sxs-lookup"><span data-stu-id="63a84-101">Product readiness policies provide a check to ensure that all required master data has been specified for a product before it can be used in transactions.</span></span> <span data-ttu-id="63a84-102">يمكن إصدار منتج أو استخدامه في الحركات في حالة التحقق من صحة فحص الجاهزية فقط.</span><span class="sxs-lookup"><span data-stu-id="63a84-102">Only when a readiness check has been validated can a product be released or used in transactions.</span></span> <span data-ttu-id="63a84-103">لا يُشترط فحص الجاهزية لإضافتها إلى فئة أو منتج.</span><span class="sxs-lookup"><span data-stu-id="63a84-103">The readiness check isn't required to be added to a category or a product.</span></span>

<span data-ttu-id="63a84-104">يصف الجدول التالي الأنواع الثلاثة من فحوصات الجاهزية المضمنة في كل سياسة.</span><span class="sxs-lookup"><span data-stu-id="63a84-104">The following table describes the three types of readiness checks that are included in each policy.</span></span>

|<span data-ttu-id="63a84-105">النوع</span><span class="sxs-lookup"><span data-stu-id="63a84-105">Type</span></span> | <span data-ttu-id="63a84-106">فحص</span><span class="sxs-lookup"><span data-stu-id="63a84-106">Check</span></span> |
|-----|-------|
|<span data-ttu-id="63a84-107">فحص النظام</span><span class="sxs-lookup"><span data-stu-id="63a84-107">System check</span></span> | <span data-ttu-id="63a84-108">سيتحقق النظام من وجود تسجيل صالح، وفقاً لإعداد السياسة.</span><span class="sxs-lookup"><span data-stu-id="63a84-108">The system will check if a valid recording exists, according to the policy setup.</span></span> |
|<span data-ttu-id="63a84-109">فحص يدوي</span><span class="sxs-lookup"><span data-stu-id="63a84-109">Manual check</span></span> | <span data-ttu-id="63a84-110">سيتحقق المستخدم من صحة السجل، ويمكن للمستخدم تحديد ما إذا كان قد تم استيفاء شرط الجاهزية.</span><span class="sxs-lookup"><span data-stu-id="63a84-110">The user will verify if the record is valid; the user can determine if the readiness requirement has been met.</span></span> |
|<span data-ttu-id="63a84-111">قائمة الاختيار</span><span class="sxs-lookup"><span data-stu-id="63a84-111">Checklist</span></span> | <span data-ttu-id="63a84-112">سيتطلب هذا الفحص أن يجيب المستخدم على سلسلة من الأسئلة من قائمة التحقق، وسيحدد النظام بعد ذلك ما إذا كانت المعايير قد استوفيت أم لا.</span><span class="sxs-lookup"><span data-stu-id="63a84-112">This check will require that the user answers a series of questions from a checklist, and the system will then determine if the criteria have been met.</span></span> |

<span data-ttu-id="63a84-113">لإنشاء الفحوصات، استخدم علامة التبويب السريعة **التحكم في الجاهزية**، حيث يمكنك إضافة الفحوصات من خلال إدراج **منطقة العملية** و **نوع** الفحص.</span><span class="sxs-lookup"><span data-stu-id="63a84-113">To create the checks, use the **Readiness control** FastTab, where you can add checks by listing the **Process area** and the **Type** of check.</span></span> <span data-ttu-id="63a84-114">توجد الصفحة في **إدارة التغيير الهندسي > إعداد > سياسات جاهزية المنتج**.</span><span class="sxs-lookup"><span data-stu-id="63a84-114">The page is located in **Engineering change management > Setup > Product readiness policies**.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="63a84-115">[![لقطة شاشة لسياسات جاهزية المنتج لمجموعات السماعات، مع تعيين نوع المنتج إلى العنصر ونشط إلى نعم. تعرض قائمة الفحوصات المضافة.](../media/product-readiness-policies.png)](../media/product-readiness-policies.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63a84-115">[![Screenshot of the Product readiness policies for Speaker sets, with Product type set to Item and Active set to Yes. It shows a list of added checks.](../media/product-readiness-policies.png)](../media/product-readiness-policies.png#lightbox)</span></span>

<span data-ttu-id="63a84-116">يأتي النظام مزوداً بـ 13 نظاماً أو فحصاً يدوياً، والتي يمكنك الاختيار من بينها عن طريق تحديد **إضافة فحص**.</span><span class="sxs-lookup"><span data-stu-id="63a84-116">The system comes with 13 system or manual checks, which you can choose from by selecting **Add check**.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="63a84-117">[![لقطة شاشة لصفحة إضافة فحص التي تسرد عمليات التحقق المتنوعة المتاحة للاختيار من بينها.](../media/add-check.png)](../media/add-check.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63a84-117">[![Screenshot of the Add check page that lists the various checks that are available to choose from.](../media/add-check.png)](../media/add-check.png#lightbox)</span></span>

<span data-ttu-id="63a84-118">لإضافة قائمة تحقق، حدد **إضافة استبيان موجود**، والذي سينشئ بند متضمناً **قائمة الاختيار** كنوع.</span><span class="sxs-lookup"><span data-stu-id="63a84-118">To add a checklist, select **Add existing questionnaire**, which will create a line with **Checklist** as the type.</span></span> <span data-ttu-id="63a84-119">يمكنك بعد ذلك الاستمرار في تغيير **منطقة العملية** وإضافة الاستبيان.</span><span class="sxs-lookup"><span data-stu-id="63a84-119">Then, you can continue to change the **Process area** and add the questionnaire.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="63a84-120">[![عند تحديد فحصاً من لقطة الشاشة السابقة، تعرض لقطة الشاشة هذه كيف سيظهر التحديد على الصفحة.](../media/check-process-area.png)](../media/check-process-area.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63a84-120">[![When you select a check from the previous screenshot, this screenshot displays how the selection will appear on the page.](../media/check-process-area.png)](../media/check-process-area.png#lightbox)</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="63a84-121">[![توفر لقطة الشاشة هذه مثالاً على وقت تطبيق الفحص.](../media/apply-check-on.png)](../media/apply-check-on.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63a84-121">[![This screenshot provides an example of when the check will be applied.](../media/apply-check-on.png)](../media/apply-check-on.png#lightbox)</span></span>
