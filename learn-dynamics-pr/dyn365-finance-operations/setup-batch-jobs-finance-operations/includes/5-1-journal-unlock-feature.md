---
ms.openlocfilehash: c770e48f61b1a7c3268041f0e822c4269060f4a1
ms.sourcegitcommit: 9134765f329ce8893f21b7a57a08277d75913363
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/16/2021
ms.locfileid: "6072528"
---
<span data-ttu-id="63ada-101">يتوفر زر في صفحة **دفتر اليومية** لإلغاء تأمين دفتر يومية عندما تكون قيمة حالة **مؤمن عن طريق النظام** هي **نعم**.</span><span class="sxs-lookup"><span data-stu-id="63ada-101">A button is available on the **Journal** page to unlock a journal when the status of the **Locked by system** value is **Yes**.</span></span> <span data-ttu-id="63ada-102">يمكن لمسؤول النظام الذي قام بتحليل وظائف الدُفعات المشغلة، والذي أكَّد أنه لم يعد تتم معالجة دفتر اليومية هذا بشكل نشط بواسطة وظيفة دفعية، إلغاء تأمينه.</span><span class="sxs-lookup"><span data-stu-id="63ada-102">A system admin who has analyzed the batch jobs that are running and has confirmed that this journal is no longer actively being processed by a batch job can unlock it.</span></span> 

<span data-ttu-id="63ada-103">يتم تمكين زر **إلغاء تأمين دفتر اليومية** بواسطة الميزة المسماة **زر إلغاء تأمين دفتر اليومية** في صفحة **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="63ada-103">The **Journal unlock** button is enabled by the feature named **Journal unlock button** on the **Feature management** page.</span></span>

<span data-ttu-id="63ada-104">[![لقطة شاشة لزر إلغاء تأمين دفتر اليومية في صفحة "إدارة الميزات".](../media/journal-unlock.png)](../media/journal-unlock.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="63ada-104">[![Screenshot of Journal unlock button on the Feature management page.](../media/journal-unlock.png)](../media/journal-unlock.png#lightbox)</span></span>

<span data-ttu-id="63ada-105">يمكن تأمين دفتر اليومية لضمان معالجة الحركات بدقة، وباستخدام مستوى عال من التزامن.</span><span class="sxs-lookup"><span data-stu-id="63ada-105">A journal can be locked to ensure transactions are processed accurately, and with a high level of concurrency.</span></span> <span data-ttu-id="63ada-106">بالنسبة لدفتر اليومية، يتم السماح لمستخدم واحد فقط في المرة بإدخال السطور، للحفاظ على التكامل والأمان.</span><span class="sxs-lookup"><span data-stu-id="63ada-106">For a journal, only one user at a time is allowed to enter lines, to maintain integrity and security.</span></span> <span data-ttu-id="63ada-107">وأحياناً بسبب الإنهاء غير الطبيعي أو أخطاء أخرى غير متوقعة، يصبح دفتر اليومية مؤمناً.</span><span class="sxs-lookup"><span data-stu-id="63ada-107">Sometimes because of an abnormal exit or other unexpected errors, the journal becomes locked.</span></span>

<span data-ttu-id="63ada-108">في لقطة الشاشة التالية، يمكنك ملاحظه أنه تم تأمين دفتر يومية وتمكين الزر **إلغاء تأمين**.</span><span class="sxs-lookup"><span data-stu-id="63ada-108">In the following screenshot, you can see that a journal is locked and the **Unlock** button is enabled.</span></span> <span data-ttu-id="63ada-109">لمعرفة أنه غير مؤمَّن، سيكون عليك تخصيص الصفحة لإضافة العمود المسمى **مؤمن عن طريق النظام**.</span><span class="sxs-lookup"><span data-stu-id="63ada-109">To see that it is unlocked, you would need to personalize the page to add the column named **Locked by system**.</span></span>

![لقطة شاشة لصفحة دفاتر اليومية العامة مع تمييز الزر "إلغاء تأمين" وعمود "مؤمَّن عن طريق النظام".](../media/unlock-button.png)

<span data-ttu-id="63ada-111">عند تحديد الزر **إلغاء تأمين**، يتم تعطيل **مؤمن عن طريق النظام**، ولا يظل دفتر اليومية مؤمَّناً.</span><span class="sxs-lookup"><span data-stu-id="63ada-111">When the **Unlock** button is selected, the **Locked by system** is disabled, and the journal is no longer locked.</span></span> 

![لقطة شاشة لصفحة دفاتر اليومية العامة، حيث لم يعد دفتر اليومية مؤمَّناً.](../media/unlocked.png)

