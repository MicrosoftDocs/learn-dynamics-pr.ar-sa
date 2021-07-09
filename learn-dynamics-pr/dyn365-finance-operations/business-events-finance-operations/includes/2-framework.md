---
ms.openlocfilehash: c7432b74650f3b11cb0d3489355825d743cc517e
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071726"
---
<span data-ttu-id="42ae4-101">يحدد إطار عمل حدث الأعمال ما إذا كان سيتم نشر حدث أعمال لمستخدم تطبيقات Finance and Operations أو لا.</span><span class="sxs-lookup"><span data-stu-id="42ae4-101">The business events framework determines whether a business event is published to a Finance and Operations apps user.</span></span> <span data-ttu-id="42ae4-102">من أفضل الممارسات أن يرسل التطبيق حدث أعمال، بغض النظر عما إذا كان حدث الأعمال ممكّناً أو لا.</span><span class="sxs-lookup"><span data-stu-id="42ae4-102">It is best practice to have the application send a business event, regardless of whether the business event is enabled or not.</span></span> <span data-ttu-id="42ae4-103">إذا كانت هناك حاجة إلى منطق إضافي مهم، أو إذا كان منطق إرسال حدث أعمال له تأثير على الأداء، يمكن للنظام التحقق مما إذا كان حدث أعمال معين ممكّناً قبل تشغيل منطق الأعمال المرتبط بإرسال أحداث الأعمال.</span><span class="sxs-lookup"><span data-stu-id="42ae4-103">If significant additional logic is needed, or if the logic for sending a business event has a performance impact, the system can check whether a specific business event is enabled before it runs business logic that is associated with sending business events.</span></span>
