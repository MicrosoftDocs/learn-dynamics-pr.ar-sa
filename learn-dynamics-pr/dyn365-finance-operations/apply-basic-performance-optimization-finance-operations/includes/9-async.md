---
ms.openlocfilehash: d22b6bdff75a5d2b2d0054c2558f0b8ba291d519
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071443"
---
<span data-ttu-id="279b5-101">يمكن أن تنتهي مهلة العمليات المستمرة لفترة طويلة في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="279b5-101">Long-running processes can time out in Finance and Operations apps.</span></span> <span data-ttu-id="279b5-102">للتغلب على ذلك، تتيح المعالجة غير المتزامنة للمستخدمين متابعة العمل أثناء تشغيل العملية في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="279b5-102">To overcome this, asynchronous processing lets users continue working while the process runs in the background.</span></span>

<span data-ttu-id="279b5-103">لتشغيل عملية بشكل غير متزامن، ستحتاج إلى استخدام أساليب `runAsync` من فئتي `FormRun` و`Global` لاستدعاء الطريقة الثابتة التي تريد تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="279b5-103">To run a process asynchronously, you will need to use the `runAsync` methods from the `FormRun` and `Global` classes to call the static method that you want to run.</span></span>
<span data-ttu-id="279b5-104">إذا تم تشغيل العملية من جانب العميل، فإننا نوصي باستخدام الأسلوب `runAsync` لفئة `FormRun`.</span><span class="sxs-lookup"><span data-stu-id="279b5-104">If the process is run on the client side, we recommend that you use the `FormRun` class's `runAsync` method.</span></span> <span data-ttu-id="279b5-105">تحتوي الفئة "Global" على الأسلوب `runAsync` التي نوصي بها لتشغيل التعليمات البرمجية خارج العميل.</span><span class="sxs-lookup"><span data-stu-id="279b5-105">The Global class has a `runAsync` method that we recommend for running code outside of the client.</span></span>

<span data-ttu-id="279b5-106">يمكنك استخدام أسلوب الاستدعاء لعرض رسالة عند اكتمال العملية.</span><span class="sxs-lookup"><span data-stu-id="279b5-106">You can use a callback method to display a message when the process is completed.</span></span> <span data-ttu-id="279b5-107">سيعرض الأسلوب `runAsync` فئة `FormRun` الرسالة على الفور.</span><span class="sxs-lookup"><span data-stu-id="279b5-107">Only the `FormRun` class `runAsync` method will display the message immediately.</span></span> <span data-ttu-id="279b5-108">إذا كنت تستخدم الأسلوب `runAsync` فئة `Global`، فستحتاج الصفحة إلى التحديث.</span><span class="sxs-lookup"><span data-stu-id="279b5-108">If you use the `Global` class `runAsync` method, the page will need to be refreshed.</span></span> 
