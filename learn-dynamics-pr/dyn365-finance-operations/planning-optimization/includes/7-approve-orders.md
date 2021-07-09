---
ms.openlocfilehash: dd10995d15d553cc0244e65c0bfa261e9969a638
ms.sourcegitcommit: 01f8d224bf1e548ba0cbe53b3e2150c43302c125
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "6072090"
---
<span data-ttu-id="230f6-101">تعتبر الموافقة على الأوامر المخططة أمراً اختيارياً وهي خطوة لإنشاء أمر مؤكد.</span><span class="sxs-lookup"><span data-stu-id="230f6-101">The approval of planned orders is optional and is a step on the way to creating a firmed order.</span></span> <span data-ttu-id="230f6-102">باستخدام حالة الموافقة، إذا تم تشغيل خطة رئيسية أخرى، فلن يتم حذف أمر تمت الموافقة عليه.</span><span class="sxs-lookup"><span data-stu-id="230f6-102">By using the approval status, if another master plan is run, it will not delete an approved order.</span></span> <span data-ttu-id="230f6-103">ستقوم بالكتابة فوق أي أوامر متبقية في الحالة **غير معالج** استناداً إلى البيانات الحالية.</span><span class="sxs-lookup"><span data-stu-id="230f6-103">It will overwrite any orders that remain in an **Unprocessed** status based on current data.</span></span> 

<span data-ttu-id="230f6-104">يشتمل الأمر المخطط على إحدى الحالات الثلاثة التالية:</span><span class="sxs-lookup"><span data-stu-id="230f6-104">A planned order has one of three statuses:</span></span>

- <span data-ttu-id="230f6-105">**غير معالج** - الحالة الافتراضية عند قيام التخطيط الرئيسي بإنشاء أمر.</span><span class="sxs-lookup"><span data-stu-id="230f6-105">**Unprocessed** - The default status when master planning generates an order.</span></span> <span data-ttu-id="230f6-106">في هذه الحالة، سيتم حذف الأمر في المرة التالية.</span><span class="sxs-lookup"><span data-stu-id="230f6-106">In this status, an order will be deleted the next time.</span></span> 
- <span data-ttu-id="230f6-107">**مكتمل** -تعني هذه الحالة أنك قمت بتقييم الأمر وقررت عدم تأكيد الأمر.</span><span class="sxs-lookup"><span data-stu-id="230f6-107">**Completed** - This status means that you have evaluated the order and decided not to firm the order.</span></span> <span data-ttu-id="230f6-108">يعتبر النظام أن **غير معالج** و **مكتمل** متماثلين.</span><span class="sxs-lookup"><span data-stu-id="230f6-108">The system considers **Unprocessed** and **Completed** to be the same.</span></span> 
- <span data-ttu-id="230f6-109">**تمت الموافقة عليه** - يتم اعتبار الأوامر المخططة بالحالة **تمت الموافقة عليه** ثابتة ويتم التخطيط لها من خلال التخطيط الرئيسي، لذلك لا يتم تغييرها أو حذفها عند تشغيل خطة أخرى.</span><span class="sxs-lookup"><span data-stu-id="230f6-109">**Approved** - Planned orders with a status of **Approved** are considered as fixed and being planned by master planning, so they are not changed or deleted when another plan is run.</span></span> <span data-ttu-id="230f6-110">سيتم نسخ الأمر من إصدار الخطة القديمة إلى الخطة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="230f6-110">It will copy the order from the old plan version to the new plan.</span></span>


    ![ <span data-ttu-id="230f6-111">تعرض لقطة الشاشة حالات الأوامر المخططة الثلاثة.</span><span class="sxs-lookup"><span data-stu-id="230f6-111">Screenshot showing the three planned order statuses.</span></span>](../media/approve-ssm.png)

