---
ms.openlocfilehash: 47f17aaaef6cae837e88a925182365a3004db1ca
ms.sourcegitcommit: e3f27696e7d66a3d06c8371b64691e113b3e91f4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "6071053"
---
<span data-ttu-id="97f7d-101">تعد ملفات تعريف الترحيل شائعة في جميع الوحدات النمطية في Finance.</span><span class="sxs-lookup"><span data-stu-id="97f7d-101">Posting profiles are common throughout all modules in Finance.</span></span>

<span data-ttu-id="97f7d-102">في ملفات تعريف ترحيل الحسابات الدائنة، يتم تحديد الحسابات الملخصة للموردين.</span><span class="sxs-lookup"><span data-stu-id="97f7d-102">In Accounts payable posting profiles, the summary accounts are defined for vendors.</span></span> <span data-ttu-id="97f7d-103">تُعد الحسابات الموجزة حسابات مؤقتة حيث يتم ترحيل جميع الفواتير إليها وتسويتها عند الدفع للمورد.</span><span class="sxs-lookup"><span data-stu-id="97f7d-103">Summary accounts are temporary accounts where all invoices are posted to and offset when the vendor is paid.</span></span> <span data-ttu-id="97f7d-104">يمكنك تعيين ملفات تعريف الترحيل إلى ما يلي:</span><span class="sxs-lookup"><span data-stu-id="97f7d-104">You can assign posting profiles to the following:</span></span>

- <span data-ttu-id="97f7d-105">مورد واحد</span><span class="sxs-lookup"><span data-stu-id="97f7d-105">A single vendor</span></span>
- <span data-ttu-id="97f7d-106">مجموعات موردين</span><span class="sxs-lookup"><span data-stu-id="97f7d-106">Groups of vendors</span></span>
- <span data-ttu-id="97f7d-107">كافة الموردين</span><span class="sxs-lookup"><span data-stu-id="97f7d-107">All vendors</span></span>

<span data-ttu-id="97f7d-108">عندما تقوم بترحيل حركة مورد تلقائياً، يبحث Finance عن حسابات دفتر الأستاذ المعروضة في الأمر السابق.</span><span class="sxs-lookup"><span data-stu-id="97f7d-108">When you post a vendor transaction automatically, Finance searches for the ledger accounts shown in the previous order.</span></span> 

<span data-ttu-id="97f7d-109">تأمل الأمثلة التالية:</span><span class="sxs-lookup"><span data-stu-id="97f7d-109">Consider the following examples:</span></span>

- <span data-ttu-id="97f7d-110">يوجد بند ملف تعريف الترحيل للمورد؛ وهو يستخدم هذا البند.</span><span class="sxs-lookup"><span data-stu-id="97f7d-110">A posting profile line exists for the vendor; this line is used.</span></span>
- <span data-ttu-id="97f7d-111">لا يوجد بند ملف تعريف الترحيل للمورد، ومع ذلك، يتم استخدام البند المحدد لمجموعة الموردين المرفق بها المورد.</span><span class="sxs-lookup"><span data-stu-id="97f7d-111">No posting profile line exists for the vendor, however, the line specified for the vendor group that the vendor is attached to is used.</span></span>
- <span data-ttu-id="97f7d-112">لا يوجد أي منهما، يتم استخدام بند ملف تعريف الترحيل لجميع الموردين.</span><span class="sxs-lookup"><span data-stu-id="97f7d-112">Neither of these exist, the posting profile line for all vendors are used.</span></span>

<span data-ttu-id="97f7d-113">في صفحة **ملفات تعريف ترحيل المورد**، يمكن إعداد العديد من ملفات تعريف ترحيل المورد.</span><span class="sxs-lookup"><span data-stu-id="97f7d-113">In the **Vendor posting profiles** page, you can set up many vendor posting profiles.</span></span> <span data-ttu-id="97f7d-114">إذا تمت معالجة جميع حركات المورد معاً، فأنت تقوم بإعداد ملف تعريف ترحيل واحد فقط لجميع الموردين.</span><span class="sxs-lookup"><span data-stu-id="97f7d-114">If all vendor transactions are processed together, you set up only one posting profile for all vendors.</span></span>

<span data-ttu-id="97f7d-115">**الحسابات الدائنة > إعداد > ملفات تعريف ترحيل المورد**</span><span class="sxs-lookup"><span data-stu-id="97f7d-115">**Accounts payable > Setup > Vendor posting profiles**</span></span>
 
<span data-ttu-id="97f7d-116">[![لقطة شاشة لصفحة ملفات تعريف ترحيل المورد.](../media/vendor-posting-profile.png)](../media/vendor-posting-profile.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="97f7d-116">[![Screenshot of the Vendor posting profiles page.](../media/vendor-posting-profile.png)](../media/vendor-posting-profile.png#lightbox)</span></span>

<span data-ttu-id="97f7d-117">إذا كنت تستخدم سجل فواتير ودفتر يومية الموافقة على الفواتير، فسيتم تسجيل جميع فواتير المورّد باعتبارها قد وصلت ولكن لم تتم الموافقة عليها بعد ويتم ترحيلها في حساب **حركات الوصول** وحساب **مقابل حركات الوصول**.</span><span class="sxs-lookup"><span data-stu-id="97f7d-117">If you use an invoice register and invoice approval journal, all vendor invoices are recorded as having arrived but not yet approved and are posted in the **Arrivals** account and the **Arrivals offset** account.</span></span> <span data-ttu-id="97f7d-118">عند الموافقة على هذه الفواتير، يتم تحويل الدين إلى حساب **ملخص المورد**.</span><span class="sxs-lookup"><span data-stu-id="97f7d-118">When these invoices are approved, the debt is transferred to the **Vendor summary** account.</span></span> <span data-ttu-id="97f7d-119">إذا كانت شركتك لا تستخدم سجل فواتير ودفتر يومية موافقة على الفواتير، فسيتم تحديث كافة فواتير المورّد مباشرةً في حساب **ملخص المورد**.</span><span class="sxs-lookup"><span data-stu-id="97f7d-119">If your company does not use an invoice register and invoice approval journal, all vendor invoices are updated directly in the **Vendor summary** account.</span></span> 

<span data-ttu-id="97f7d-120">لمزيد من المعلومات، راجع [تنفيذ الإجراءات اليومية للحسابات الدائنة في Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/accounts-payable-daily-procedures-dyn365-finance/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="97f7d-120">For more information, see  [Perform Accounts payable daily procedures in Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/accounts-payable-daily-procedures-dyn365-finance/?azure-portal=true).</span></span>

<span data-ttu-id="97f7d-121">بعد إنشاء ملفات تعريف الترحيل، تحتاج إلى تعيين ملف تعريف ترحيل افتراضي في **الحسابات الدائنة > إعداد > معلمات الحسابات الدائنة**.</span><span class="sxs-lookup"><span data-stu-id="97f7d-121">After you create posting profiles, you need to set a default posting profile in **Accounts payable > Setup > Accounts payable parameters**.</span></span> <span data-ttu-id="97f7d-122">حدد علامة التبويب **دفتر الأستاذ وضريبة المبيعات** ثم حدد قيمة من أجل **ملف تعريف الترحيل**.</span><span class="sxs-lookup"><span data-stu-id="97f7d-122">Select the **Ledger and sales tax** tab, and then select a value for **Posting profile**.</span></span> <span data-ttu-id="97f7d-123">يجب تحديد ملف تعريف الترحيل لكل تحديث لحركة المورد.</span><span class="sxs-lookup"><span data-stu-id="97f7d-123">A posting profile must be specified for every update of a vendor transaction.</span></span>

