---
ms.openlocfilehash: 816565023f3d3b43a3e240331bb35bb1916221a8
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072274"
---

<span data-ttu-id="ca940-101">عند إضافة عناصر أو تغييرها، عليك مزامنة قاعدة البيانات بحيث تعرف في أي الحقول (الأعمدة) عليها تخزين هذه العناصر.</span><span class="sxs-lookup"><span data-stu-id="ca940-101">When you add or change elements, you must synchronize the database so that it knows in which fields (columns) that it needs to store these elements.</span></span> <span data-ttu-id="ca940-102">وللقيام بذلك، حدد **تزامن قاعدة البيانات** من قائمة **Dynamics 365** ثم استخدم الزر **مزامنة** في مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="ca940-102">To do that, select **Synchronize Database** from the **Dynamics 365** menu and then use the **Synchronize** button in the dialog box.</span></span> 

<span data-ttu-id="ca940-103">يمكنك أيضا تحديد **تزامن قاعدة البيانات عند الإنشاء** من علامة التبويب **خيارات** في مربع الحوار **نماذج الإنشاء** لمزامنة قاعدة البيانات تلقائياً بعد إنشاء ناجح.</span><span class="sxs-lookup"><span data-stu-id="ca940-103">You can also select **Synchronize Database on Build** on the **Options** tab of the **Build Models** dialog box to automatically synchronize the database after a successful build.</span></span> <span data-ttu-id="ca940-104">ويعد هذا الخيار ملائماً لأنك ستحتاج للمزامنة فور الإنشاء.</span><span class="sxs-lookup"><span data-stu-id="ca940-104">This option is handy  because you will need to synchronize immediately after building.</span></span>

<span data-ttu-id="ca940-105">وفي بعض الأحيان، تتسبب قاعدة البيانات غير المتزامنة في قيام تطبيقات Finance and Operations بطرح أخطاء SQL.</span><span class="sxs-lookup"><span data-stu-id="ca940-105">Sometimes, an out-of-sync database will cause Finance and Operations apps to throw SQL errors.</span></span> <span data-ttu-id="ca940-106">ويمكن حل هذه المشكلة غالباً باستخدام مزامنة قاعدة بيانات ناجحة. حيث تعد مزامنة قاعدة البيانات مع الكود المبني محلياً ضرورية عند جلب البيانات إلى جهاز جديد.</span><span class="sxs-lookup"><span data-stu-id="ca940-106">This problem can often be resolved with a successful database sync. Synchronizing the database with locally built code is necessary when you are bringing data onto a new machine.</span></span>

<span data-ttu-id="ca940-107">يوضح الرسم المتحرك التالي عملية مزامنة قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="ca940-107">The following animation shows the process to sync the database.</span></span>


![رسم متحرك لعملية مزامنة قاعدة البيانات.](../media/database-sync.gif)
