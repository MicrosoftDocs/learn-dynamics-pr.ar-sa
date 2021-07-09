---
ms.openlocfilehash: f241189a9507b90ca9186000fe0219585eabb62e
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6071136"
---
<span data-ttu-id="c2136-101">بعد تكوين المحاسبة بين الشركات الشقيقة، يمكنك بعد ذلك إنشاء الحركات بين الشركات الشقيقة وترحيلها.</span><span class="sxs-lookup"><span data-stu-id="c2136-101">After the intercompany accounting is configured, you can then create and post intercompany transactions.</span></span> <span data-ttu-id="c2136-102">سيقوم Finance بإنشاء إدخالات بين الشركات الشقيقة تلقائياً باستخدام حسابات دفتر الأستاذ ودفاتر اليومية التي تم إعدادها بالفعل.</span><span class="sxs-lookup"><span data-stu-id="c2136-102">Finance will create intercompany entries automatically by using the ledger accounts and journals that are already set up.</span></span> 
 
<span data-ttu-id="c2136-103">عند إجراء الإدخال الأولي، لن تحتاج إلى استخدام دفتر يومية **يومي بين الشركات الشقيقة** الذي تم إعداده.</span><span class="sxs-lookup"><span data-stu-id="c2136-103">When making the initial entry, you do not need to use the **Intercompany daily** journal that was set up.</span></span> <span data-ttu-id="c2136-104">يُستخدم دفتر اليومية هذا في الشركة ذات الصلة لتسجيل الإدخالات التلقائية بين الشركات الشقيقة.</span><span class="sxs-lookup"><span data-stu-id="c2136-104">That journal is used in the related company to record the automatic intercompany entries.</span></span> <span data-ttu-id="c2136-105">يمكنك بدء إدخال بين الشركات الشقيقة من أي نوع من دفاتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="c2136-105">You can initiate an intercompany entry from any kind of journal.</span></span>

<span data-ttu-id="c2136-106">عندما تقوم بتحديد شركة في حقل حسابات **الشركة**، يتوفر حقل حسابات **الشركة المقابلة** أو كلاهما، وتتوفر كل الشركات.</span><span class="sxs-lookup"><span data-stu-id="c2136-106">When you select a company in the **Company** accounts field, **Offset company** accounts field, or both, all companies are available.</span></span> <span data-ttu-id="c2136-107">ومع ذلك، لن تعمل عملية الترحيل إلا بين الشركات التي تم إعداد حسابات ترحيل الشركات الشقيقة فيها.</span><span class="sxs-lookup"><span data-stu-id="c2136-107">However, posting will only work between companies that have intercompany posting accounts set up.</span></span>

<span data-ttu-id="c2136-108">قم بترحيل الحركات بين الشركات الشقيقة إلى حسابات **دفتر الأستاذ**، وحسابات **العملاء**، وحسابات **الموردين** وحسابات **البنوك** باستخدام حقل **نوع الحساب المقابل** لإجراء التحديد.</span><span class="sxs-lookup"><span data-stu-id="c2136-108">Post Intercompany transactions to **Ledger** accounts, **Customer** accounts, **Vendor** accounts, and **Bank** accounts by using the **Offset account type** field to make the selection.</span></span>

<span data-ttu-id="c2136-109">ستكون الأبعاد المالية للحسابات الرئيسية **مستحق إلى** و **مستحق من** افتراضية مع الأبعاد الثابتة المحددة في الحسابات الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="c2136-109">The financial dimensions for the **Due to** and **Due from** main accounts will default with the fixed dimensions defined on the main accounts.</span></span> <span data-ttu-id="c2136-110">يمكن أيضاً أن تكون الأبعاد المالية افتراضية من الحساب والحساب المقابل في دفتر اليومية، ولكن فقط إذا تم إدخال الحركة بين الشركات الشقيقة كإيصال من بند واحد.</span><span class="sxs-lookup"><span data-stu-id="c2136-110">The financial dimensions can also default from the Account and Offset account on the journal, but only if the intercompany transaction is entered as a single-line voucher.</span></span> <span data-ttu-id="c2136-111">لن تقوم الإيصالات متعددة البنود بافتراض الأبعاد المالية لكل من حسابات دفتر الأستاذ المنشأ والوجهة **مستحق إلى** و **مستحق من**.</span><span class="sxs-lookup"><span data-stu-id="c2136-111">Multi-line vouchers will not default the financial dimensions to both the originating and destination **Due to** and **Due from** ledger accounts.</span></span> <span data-ttu-id="c2136-112">لا يمكن تحديد الأبعاد المالية بشكل متكرر بإيصال متعدد البنود.</span><span class="sxs-lookup"><span data-stu-id="c2136-112">The financial dimensions often cannot be determined with a multi-line voucher.</span></span> 
 
<span data-ttu-id="c2136-113">عند ترحيل الإدخال، سيتم ترحيل الإيصالات على الفور في شركات المنشأ والوجهة.</span><span class="sxs-lookup"><span data-stu-id="c2136-113">When the entry posts, the vouchers will immediately post in the originating and destination companies.</span></span> <span data-ttu-id="c2136-114">يوضح نموذج المعلومات الذي يظهر أنه تم ترحيل إيصالين، واحد لكل شركة.</span><span class="sxs-lookup"><span data-stu-id="c2136-114">The Infolog form that displays shows that two vouchers are posted, one for each company.</span></span> <span data-ttu-id="c2136-115">يساعد ذلك على التحقق من ترحيل الإدخال التلقائي في الشركة الأخرى.</span><span class="sxs-lookup"><span data-stu-id="c2136-115">This helps verify that the automatic entry posted in the other company.</span></span> 

<span data-ttu-id="c2136-116">تعرض الصورة التالية صفحة **حركات الإيصالات** في **دفتر الأستاذ العام > الاستعلامات والتقارير > سجل التدقيق**
![لقطة شاشة لصفحة حركات الإيصالات.](../media/voucher-transactions.png)</span><span class="sxs-lookup"><span data-stu-id="c2136-116">The following image shows the **Voucher transactions** page in **General ledger > Inquiries and reports > Audit trail**
![Screenshot of the Voucher transactions page.](../media/voucher-transactions.png)</span></span>

<span data-ttu-id="c2136-117">شاهد هذا الفيديو للتعرف على كيفية إنشاء إدخالات دفتر اليومية العام بين الشركات الشقيقة وترحيلها:</span><span class="sxs-lookup"><span data-stu-id="c2136-117">Watch this video to learn how you can create and post intercompany general journal entries:</span></span>

&nbsp;

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3TQTT]


