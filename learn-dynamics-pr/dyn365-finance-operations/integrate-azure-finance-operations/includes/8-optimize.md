---
ms.openlocfilehash: f457987d7880b8018c1a1fa487bda14e77c2972f
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071960"
---
<span data-ttu-id="c68f3-101">تتمثل إحدى طرق تحسين أداء عمليات التكاملات في تغيير سلوك كيانات البيانات.</span><span class="sxs-lookup"><span data-stu-id="c68f3-101">One method of improving the performance of integrations is to change the behavior of data entities.</span></span> <span data-ttu-id="c68f3-102">عند إحضار الكيانات غير المركبة والتي لا تتطلب منطقاً على مستوى الصف، يمكن أن يساعد تشغيل المعالجة القائمة على المجموعة للكيان.</span><span class="sxs-lookup"><span data-stu-id="c68f3-102">When bringing in entities that are not composite and don't require row-level logic, turning on set-based processing for the entity can help.</span></span> <span data-ttu-id="c68f3-103">وتسمح المعالجة المستندة إلى المجموعة بجمع الصفوف ونقلها في مجموعات، مما يقلل من تأثير الاتصال الكامن مع قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="c68f3-103">Set-based processing allows for rows to be collected and moved in groups, reducing the effect of latent communication with the database.</span></span>

<span data-ttu-id="c68f3-104">والطريقة الأخرى التي تعمل مع الكيانات غير المركبة هي تقسيم ملفات الإدخال إلى أجزاء متعددة.</span><span class="sxs-lookup"><span data-stu-id="c68f3-104">Another method that works for entities that are not composite is to split input files into multiple parts.</span></span> <span data-ttu-id="c68f3-105">يتيح القيام بذلك لتطبيقات Finance and Operations الاستفادة من تعدد مؤشرات الترابط إلى الحد الذي تكون فيه البيئة قادرة على القيام بعملياتها.</span><span class="sxs-lookup"><span data-stu-id="c68f3-105">Doing so allows Finance and Operations apps to take advantage of multithreading to the extent that the environment is capable.</span></span> 
