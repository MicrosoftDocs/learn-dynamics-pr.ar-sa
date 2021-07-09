---
ms.openlocfilehash: 5f6e2cb5b637f30136cdeb0a72482b991b6c7de0
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073331"
---
<span data-ttu-id="aad0a-101">يمكن استخدام العمليات المتزامنة في شبكات الطرق البسيطة والمعقدة.</span><span class="sxs-lookup"><span data-stu-id="aad0a-101">Simultaneous operations can be used in simple and complex route networks.</span></span> <span data-ttu-id="aad0a-102">العملية المتزامنة هي عملية يتم فيها استخدام عدة موارد في نفس الوقت وحيث يجب جدولة الموارد بقدرة محدودة.</span><span class="sxs-lookup"><span data-stu-id="aad0a-102">A simultaneous operation is a process where several resources are used at the same time and where the resources must be scheduled with limited capacity.</span></span>

<span data-ttu-id="aad0a-103">يجب تعيين نفس الرقم للعمليات المتزامنة.</span><span class="sxs-lookup"><span data-stu-id="aad0a-103">You must assign the same number to simultaneous operations.</span></span> <span data-ttu-id="aad0a-104">تستخدم العمليات المتزامنة قدرة العديد من الموارد في نفس الوقت، على سبيل المثال، قد تستخدم آلة وعامل التشغيل الخاص بها وربما أداة معينة.</span><span class="sxs-lookup"><span data-stu-id="aad0a-104">Simultaneous operations use the capacity of several resources at the same time, for example, they might use a machine, its operator, and possibly a specific tool.</span></span>

<span data-ttu-id="aad0a-105">بالإضافة إلى ذلك، يجب إعطاء الأولوية للعمليات المتزامنة.</span><span class="sxs-lookup"><span data-stu-id="aad0a-105">In addition, the simultaneous operations must be prioritized.</span></span> <span data-ttu-id="aad0a-106">لتحديد أولويات العمليات المتزامنة، يتم تطبيق نفس رقم العملية أولاً على جميع العمليات المتزامنة، ثم يتم تحديد العملية الأساسية.</span><span class="sxs-lookup"><span data-stu-id="aad0a-106">To prioritize simultaneous operations, the same operation number is first applied to all simultaneous operations, and then the primary operation is specified.</span></span>

<span data-ttu-id="aad0a-107">خصائص العمل مع العمليات الأولية هي:</span><span class="sxs-lookup"><span data-stu-id="aad0a-107">Characteristics of working with primary operations are:</span></span>

-   <span data-ttu-id="aad0a-108">العملية الأساسية هي العملية التي تستخدم مورداً يمثل عنق الزجاجة أو يحد من العمليات المتزامنة.</span><span class="sxs-lookup"><span data-stu-id="aad0a-108">The primary operation is the one using a resource that represents a bottleneck or limits the simultaneous operations.</span></span>

-   <span data-ttu-id="aad0a-109">يُسمح بإجراء عملية أساسية واحدة فقط لكل رقم عملية في المسار.</span><span class="sxs-lookup"><span data-stu-id="aad0a-109">Only one primary operation is allowed for each operation number in a route.</span></span>

-   <span data-ttu-id="aad0a-110">جميع العمليات المتزامنة الأخرى ثانوية؛ لذلك، لا تؤخذ قدرتهم في الاعتبار.</span><span class="sxs-lookup"><span data-stu-id="aad0a-110">All the other simultaneous operations are secondary; therefore, their capacity is not taken into consideration.</span></span>

-   <span data-ttu-id="aad0a-111">يمكن إعداد إجمالي 20 عملية ثانوية لكل رقم عملية.</span><span class="sxs-lookup"><span data-stu-id="aad0a-111">A total of 20 secondary operations for each operation number can be set up.</span></span>

