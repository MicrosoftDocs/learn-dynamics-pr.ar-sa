---
ms.openlocfilehash: 930ed54297b0adab8901bc70ca704cd200922310
ms.sourcegitcommit: 4ecdf5debbb9e9098084bff71834755f0976db57
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2021
ms.locfileid: "6072556"
---
<span data-ttu-id="acbc9-101">بتعيين مستخدم لدور الأمان **مدير الوظائف الدفعية**، تتوفر للمستخدم أذونات نسخ الوظائف الدفعية، وتغيير الشخص الذي سيقوم بتنفيذ الوظائف، وتحديد النطاقات الزمنية التي يمكن تنفيذ الوظائف خلالها.</span><span class="sxs-lookup"><span data-stu-id="acbc9-101">By assigning a user to the **Batch job manager** security role, the user has permissions to copy batch jobs, change who will execute jobs, and specify the time ranges during which jobs can execute.</span></span> <span data-ttu-id="acbc9-102">يعد امتياز الأمان الخاص بالوظائف الدفعية للوظيفة الدفعية "صيانة" جزءاً من دور الأمان الخاص بمدير الوظائف الدفعية، ويسمح للمستخدم بإنشاء وظيفة دفعية غير مخططة ومنح امتيازات لمستخدمين آخرين.</span><span class="sxs-lookup"><span data-stu-id="acbc9-102">The batch Maintain batch jobs security privilege is part of the Batch job manager security role and it allows a user to create an unplanned batch job and grant privileges to other users.</span></span>

<span data-ttu-id="acbc9-103">فقط ليتمكن المستخدم من إدارة الوظائف الدفعية، يجب تعيينه إلى دور **مدير الوظيفة الدفعية**، وليس إلى مسؤول النظام أو أمان مسؤول تكنولوجيا المعلومات.</span><span class="sxs-lookup"><span data-stu-id="acbc9-103">To just be able to manage batch jobs, a user should be assigned to the **Batch job manager** role, and not to the System admin or IT admin security.</span></span>

## <a name="run-by-feature"></a><span data-ttu-id="acbc9-104">ميزة تشغيل بواسطة</span><span class="sxs-lookup"><span data-stu-id="acbc9-104">Run by feature</span></span>

<span data-ttu-id="acbc9-105">تتيح ميزة **تشغيل بواسطة** لمديري الوظائف المجمعة تحديد مستخدم لتشغيل وظيفة دفعية.</span><span class="sxs-lookup"><span data-stu-id="acbc9-105">The **Run by** feature allows Batch job managers to specify a user to run the batch job.</span></span> <span data-ttu-id="acbc9-106">فعلى سبيل المثال، عندما تريد تغيير المستخدم الذي تم تعيينه حالياً لتشغيل الوظيفة، أو إذا كنت ترغب في تعيين مستخدم سريعاً أثناء نسخ الوظائف الدفعية من شركة إلى أخرى.</span><span class="sxs-lookup"><span data-stu-id="acbc9-106">For example, when you want to change the user who is currently assigned to run the job, or if you want to quickly set a user while copying the batch jobs from one company to another.</span></span> <span data-ttu-id="acbc9-107">يمكنك أيضاً استخدام هذه الوظيفة لنسخ وظائف دفعية.</span><span class="sxs-lookup"><span data-stu-id="acbc9-107">You can also use this functionality to copy batch jobs.</span></span>

<span data-ttu-id="acbc9-108">يمكنك أدناه رؤية خيار **تشغيل بواسطة** الموجود على **إدارة النظام > الاستعلامات > الوظائف الدفعية > علامة التبويب تبديل إلى النموذج المحسن**.</span><span class="sxs-lookup"><span data-stu-id="acbc9-108">Below you can see the **Run by** option found on **System administration > Inquires > Batch jobs > Switch to enhanced form** tab.</span></span>

![لقطة شاشة لصفحة الوظائف الدفعية مع تمييز حقل تشغيل بواسطة.](../media/run-by-user.png)
