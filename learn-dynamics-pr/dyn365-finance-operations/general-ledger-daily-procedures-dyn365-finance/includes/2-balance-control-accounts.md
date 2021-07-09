---
ms.openlocfilehash: 9c0cdcb02fe512f975850e5f2319a3ec0b357cea
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6071104"
---
<span data-ttu-id="dc3d1-101">ستستخدم حسابات التحكم في الرصيد لالتحكم في الرصيد الحالي والمتوقع على الحساب أثناء إدخال الحركات في دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-101">You'll use balance control accounts to monitor the current and expected balance on an account as transactions are entered in a journal.</span></span> 
 
<span data-ttu-id="dc3d1-102">إنه ليس إعداداً مطلوباً، ولكنه مفيد إذا كنت ترغب في العرض والتأكد من أن الأموال الموجودة في الحساب كافية لنشر الحركة.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-102">It is not a required setup, but it is helpful if you want to view and make sure that the funds within an account are enough to post the transaction.</span></span> <span data-ttu-id="dc3d1-103">سيتم استخدام هذا فقط لتلك المجموعة الفرعية من الحسابات حيث يكون من المنطقي القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-103">This will only be used for that subset of accounts where it makes sense to do so.</span></span>  <span data-ttu-id="dc3d1-104">الأكثر شيوعاً، للحسابات البنكية المستخدمة للمدفوعات.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-104">Most commonly, for bank accounts used for disbursements.</span></span>
  
<span data-ttu-id="dc3d1-105">ضع في الاعتبار السيناريو التالي.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-105">Consider the following scenario.</span></span>

<span data-ttu-id="dc3d1-106">يريد مدير محاسبة Adventure Works Cycles، جوناثان تتبع الرصيد الحالي والمتوقع لحسابات السيولة.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-106">The Adventure Works Cycles Accounting manager, Johnathan wants to track the current and expected balance of liquidity accounts.</span></span>  <span data-ttu-id="dc3d1-107">وهي تتضمن الحسابات البنكية والحسابات النقدية النثرية.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-107">These include bank accounts and petty cash accounts.</span></span>  <span data-ttu-id="dc3d1-108">بعد أن قام جوناثان بإعداد حسابات التحكم في الرصيد، يقوم منسق الحسابات الدائنة بالتحقق من الرصيد المتوقع للحساب البنكي للتأكد من أن الرصيد كافٍ لدفع الفواتير.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-108">After Johnathan has set up the balance control accounts, then the accounts payable coordinator verifies the expected balance of the bank account to make sure that the balance is enough to pay invoices.</span></span> <span data-ttu-id="dc3d1-109">سيتضمن الرصيد المتوقع كلاً من دفاتر اليومية المُرحلة وغير المنشورة.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-109">The expected balance is going to include both posted and unposted journals.</span></span>  

<span data-ttu-id="dc3d1-110">لإنشاء حسابات التحكم في الرصيد، انتقل إلى **دفتر الأستاذ العام > مخطط الحسابات > الحسابات > حسابات التحكم في الرصيد**.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-110">To create balance control accounts, go to **General ledger > Chart of accounts > Accounts > Balance control accounts**.</span></span>

<span data-ttu-id="dc3d1-111">من المهم معرفة أن حساب التحكم في الرصيد يرتبط بحساب دفتر الأستاذ، مثل حساب المصروفات النثرية.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-111">It's important to know that a balance control account relates to a ledger account, such as a petty cash account.</span></span> <span data-ttu-id="dc3d1-112">تعتبر الحسابات البنكية التي تم إعدادها نقداً وإدارة البنك بالفعل حسابات التحكم في الرصيد، وضمنياً، تعتبر الحسابات الرئيسية المرتبطة بها بالفعل حسابات التحكم في الرصيد.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-112">The bank accounts that are set up in cash and bank management are already considered balance control accounts, and by implication, the main accounts associated with them are already considered balance control accounts.</span></span>
 
![لقطة شاشة لصفحة حسابات التحكم في الرصيد.](../media/balance-control.png)

<span data-ttu-id="dc3d1-114">شاهد الفيديو لتتعلم كيف تستعمل:</span><span class="sxs-lookup"><span data-stu-id="dc3d1-114">Watch the video to learn how to use:</span></span>

- <span data-ttu-id="dc3d1-115">أوصاف دفتر اليومية أو نص بند دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-115">Journal descriptions or journal line text.</span></span>
- <span data-ttu-id="dc3d1-116">حقلا اقتراح الخصم والائتمان (**الخصم/الائتمان الافتراضي**) ومتطلبات الخصم والائتمان (**متطلبات الخصم/الائتمان**) في الحساب الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-116">The debit and credit proposal (**DB/CR default**) and the debit and credit requirement (**DB/CR requirement**) fields on the main account.</span></span> 
- <span data-ttu-id="dc3d1-117">إعداد حساب التحكم في الرصيد والاستعلام.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-117">Balance control account setup and inquiry.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE489XA]


<span data-ttu-id="dc3d1-118">يمكنك عرض التحكم في الرصيد في دفاتر اليومية العامة قبل الترحيل باستخدام **الاستعلامات > التحكم في الرصيد** كما ترى أدناه:</span><span class="sxs-lookup"><span data-stu-id="dc3d1-118">You can view the balance control in the general journals prior to posting by using the **Inquiries > Balance control** as you see below:</span></span>
 
<span data-ttu-id="dc3d1-119">[ ![لقطة شاشة لمثال على التحكم في الرصيد في دفتر يومية.](../media/journal-1.png) ](../media/journal-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="dc3d1-119">[ ![Screenshot of an example of Balance control in a journal.](../media/journal-1.png) ](../media/journal-1.png#lightbox)</span></span>

<span data-ttu-id="dc3d1-120">تظهر نتيجة هذا الاستعلام رصيد الحسابات التي تحاول بنود دفتر اليومية ترحيل المبالغ إليها ومقارنتها بالقيم قبل وبعد ترحيل دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-120">The result of this inquiry shows the balance of the accounts that the journal lines trying to post amounts to and compare it with the values before and after posting the journal.</span></span> <span data-ttu-id="dc3d1-121">سيعطي هذا لمحة عما سيحدث إذا رحلت دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="dc3d1-121">This will give a glance of what will happen if you post the journal.</span></span> 


