---
ms.openlocfilehash: d733fa173ee3934fb038ce603aff104f5cd0589e
ms.sourcegitcommit: 0af0a6f1739b0e2a5ec60989ffbf8aa131de41c3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/08/2021
ms.locfileid: "6072239"
---
<span data-ttu-id="bfb9f-101">+يُستخدم التزامن للتحكم في وقت توفر البيانات لتنفيذ عمليات أخرى.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-101">Concurrency is used to control when data is available for other processes.</span></span> <span data-ttu-id="bfb9f-102">تستخدم تطبيقات Finance and Operations نموذجين للتزامن:</span><span class="sxs-lookup"><span data-stu-id="bfb9f-102">Finance and Operations apps uses two concurrency models:</span></span>

-   <span data-ttu-id="bfb9f-103">**عنصر التحكم في التزامن غير المعزز بحماية التغييرات (PCC)** - يقوم بقفل السجلات بمجرد استرجاعها من قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-103">**Pessimistic Concurrency Control (PCC)** - Locks records as soon as    they are retrieved from the database.</span></span>
-   <span data-ttu-id="bfb9f-104">**عنصر التحكم في التزامن المعزز بحماية التغييرات (OCC)** - يقوم بتأمين السجلات أثناء تحديثها.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-104">**Optimistic Concurrency Control (OCC)** - Locks records when they    are being updated.</span></span>

<span data-ttu-id="bfb9f-105">يجب استخدام نموذج PCC عندما يكون هناك منطق تسلسل يتطلب أقفالاً على السجل أو عندما يُحتمل وجود تعارض أثناء التحديث.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-105">The PCC model should be used when there is serialization logic that requires locks on the record, or when update conflicts are likely.</span></span>

<span data-ttu-id="bfb9f-106">يجب استخدام OCC في الجداول لأنها تعمل على تحسين الإنتاجية على عكس PCC.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-106">OCC should be used on tables where it improves throughput in contrast to PCC.</span></span> <span data-ttu-id="bfb9f-107">ويُفضل أيضاً استخدام عنصر التحكم OCC إذا تم تحديث الجدول أو حذفه من نموذج وليس من كود.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-107">Also, OCC is preferred if the table is updated or deleted from a form and not from code.</span></span>
 
<span data-ttu-id="bfb9f-108">يتميز عنصر التحكم OCC بمزايا تساعد على زيادة أداء قاعدة البيانات:</span><span class="sxs-lookup"><span data-stu-id="bfb9f-108">OCC has advantages that help increase database performance:</span></span>

-   <span data-ttu-id="bfb9f-109">يتم استخدام موارد أقل لقفل السجلات أثناء التحديثات.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-109">Fewer resources are used to lock records during updates.</span></span>
-   <span data-ttu-id="bfb9f-110">يتم قفل السجلات لفترة زمنية أقصر عند استخدام OCC بدلاً من PCC.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-110">Records are locked for a shorter length of time by using OCC instead of PCC.</span></span>
-   <span data-ttu-id="bfb9f-111">تظل السجلات متاحة للعمليات الأخرى أثناء اختيارها من قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-111">Records remain available for other processes while they are selected    from the database.</span></span>

<span data-ttu-id="bfb9f-112">يحدث عيب استخدام عنصر التحكم OCC عندما تحاول عمليتان تحديث نفس السجل في نفس الوقت.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-112">The disadvantage of using OCC happens when two processes try to update the same record at the same time.</span></span> <span data-ttu-id="bfb9f-113">عند وقوع ذلك، سيفشل التحديث، ما قد يؤدي إلى خفض مستوي أداء قاعده البيانات إذا كانت هناك محاولات متعددة لإجراء التحديثات.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-113">When this occurs, the update will fail, which can lead to reduced database performance if there are multiple retries to updates.</span></span>

<span data-ttu-id="bfb9f-114">يتم تحديد نموذج التزامن لجميع الجداول القياسية في تطبيقات Finance and Operations وتستخدم معظم الجداول OCC.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-114">All standard tables in Finance and Operations apps have a concurrency model selected, and most of the tables use OCC.</span></span> <span data-ttu-id="bfb9f-115">يمكنك تعيين نموذج التزامن في خاصية الجدول `OccEnabled`.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-115">You can set the concurrency model on the `OccEnabled` table property.</span></span> <span data-ttu-id="bfb9f-116">بالإضافة إلى ذلك، يمكنك تجاوز نموذج تزامن الجدول في عبارة **Select**.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-116">Additionally, you can override the table concurrency model in a **Select** statement.</span></span> <span data-ttu-id="bfb9f-117">بعد الكلمة الرئيسية *Select* يمكنك استخدام الكلمة الرئيسية *optimisticLock* أو *pessimisticLock* لاستبدال الكلمة الرئيسية `forUpdate`.</span><span class="sxs-lookup"><span data-stu-id="bfb9f-117">After the keyword *Select*, you can use the keyword *optimisticLock* or *pessimisticLock* to replace the keyword `forUpdate`.</span></span>

![لقطة شاشة لصفحة الخصائص، مع إبراز القائمة المنسدلة لنموذج التزامن.](../media/concurrency-1.png)

