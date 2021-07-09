---
ms.openlocfilehash: b1c547798e96cc6b7a74efe9e9c3dd54d012b334
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073501"
---
<span data-ttu-id="7a6ca-101">يتم استخدام وظائف كانبان للأحداث حيث يجب إنشاء وظائف كانبان، فقط عند حدوث أحداث معينة.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-101">Event kanbans are used where kanbans should be generated, only when certain events occur.</span></span> <span data-ttu-id="7a6ca-102">الأحداث التي تؤدي إلى تشغيل وظائف كانبان هذه هي أحداث سطر المبيعات وأحداث سطر قائمة مكونات الصنف للإنتاج وأحداث تجديد المخزون وأحداث سطر كانبان.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-102">The events that trigger these kanbans are sales line events, production BOM line events, stock replenishment events, and kanban line events.</span></span>

<span data-ttu-id="7a6ca-103">تحدد قواعد كانبان الخاصة بوحدات كانبان الحدث نوع الحدث الذي يؤدي إلى إنشاء كانبان.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-103">Kanban rules for event kanbans define the type of event that triggers the kanban to be created.</span></span> <span data-ttu-id="7a6ca-104">يمكن أن تحدث هذه المشغلات تلقائياً، عند تشغيل وظيفة دفعة، أو يدوياً حسب نوع الحدث وسياسة إنشاء كانبان للحدث.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-104">These triggers can occur automatically, upon running of a batch job, or manually depending on the type of event and the kanban creation policy of the event.</span></span>

- <span data-ttu-id="7a6ca-105">**أحداث بنود المبيعات** - يتم تشغيلها استناداً إلى خط المبيعات ويمكن أن تتضمن استخدام برنامج التحويلات النقدية لتوفير تواريخ تسليم أكثر دقة للعميل.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-105">**Sales line events** - Are triggered based off of a sales line and can include the use of CTP to provide more accurate delivery dates to the customer.</span></span>

- <span data-ttu-id="7a6ca-106">**أحداث بنود كانبان** - يتم تشغيلها استناداً إلى وظائف كانبان ذات المستوى الأعلى ويمكن تشغيلها تلقائياً أو يدوياً باستخدام معالجة الدُفعات.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-106">**Kanban line events** - Are triggered based off of upper level kanbans and can be automatically or manually triggered by using batch processing.</span></span>

- <span data-ttu-id="7a6ca-107">**أحداث بنود قائمة مكونات الصنف** - يتم تشغيلها بناءً على طلب أمر الإنتاج من المستوى الأعلى ويتم استخدامها في بيئات الوضع المختلط حيث يتم استخدام أوامر الإنتاج التقليدية للعملية النهائية.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-107">**BOM line events** - Are triggered based off of upper level production order demand and are used in mixed mode environments where traditional production orders are used for the downstream process.</span></span>

- <span data-ttu-id="7a6ca-108">**أحداث تزويد المخزون** - يتم تشغيلها بناءً على وصول عنصر ما إلى الحد الأدنى من إعدادات المخزون.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-108">**Stock replenishment events** - Are triggered based off of an item reaching the minimum stock settings.</span></span> <span data-ttu-id="7a6ca-109">تُعد هذه الأحداث مفيدة في بيئة التحول السريع، حيث يجب أن تنشئ مخالفات المخزون الاحتياطي كانبان على الفور ولا يمكنها الانتظار حتى يتم تشغيل التخطيط الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-109">These events are useful in a quick turning environment, where safety stock violations must instantly create a kanban and cannot wait for master planning to run.</span></span> 
