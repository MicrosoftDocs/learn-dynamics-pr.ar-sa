---
ms.openlocfilehash: f904c1ffca3ef04698ac92a526d1c99ec337c4f0
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071296"
---

<span data-ttu-id="a8d22-101">عند ترقية إصدارات تطبيقات Finance and Operations، قد لا يعمل الكود الحالي دائماً بالشكل المقصود في التطبيق الجديد.</span><span class="sxs-lookup"><span data-stu-id="a8d22-101">When upgrading application versions of Finance and Operations apps, your existing code might not always work as intended in the new application.</span></span>

<span data-ttu-id="a8d22-102">ستساعدك أفضل الممارسات الآتية على التنقل في عملية ترقية الكود:</span><span class="sxs-lookup"><span data-stu-id="a8d22-102">The following best practices will help you navigate the code upgrade process:</span></span>

-    <span data-ttu-id="a8d22-103">احصل على فرع كود لإجراء أي تغييرات لازمة للمساعدة على بقاء التطبيق القديم متوافقاً مع إصدار التطبيق الجديد.</span><span class="sxs-lookup"><span data-stu-id="a8d22-103">Have a code branch for developing any changes that are needed to help keep the old application compatible with the new application version.</span></span> <span data-ttu-id="a8d22-104">قم بالترقية من هذا الفرع إلى فرع اختبار للتأكد من عمل التغييرات قبل الترقية إلى فرع التطوير الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="a8d22-104">Promote from this branch into a test branch to confirm that the changes work before you promote into your main development branch.</span></span>
-   <span data-ttu-id="a8d22-105">أعِد توزيع بيئات مستضافة على الشبكة السحابية على الإصدار الجديد بدلاً من التحديث.</span><span class="sxs-lookup"><span data-stu-id="a8d22-105">Redeploy cloud-hosted environments on the new version rather than updating.</span></span>
-   <span data-ttu-id="a8d22-106">راجع مستندات Microsoft لمعرفة معلومات التوافق لتحديد ما إذا كان يجب تطبيق الكود أو تحديث التطبيق أولاً إلى بيئة الطبقة 2.</span><span class="sxs-lookup"><span data-stu-id="a8d22-106">Refer to Microsoft documentation for compatibility information to determine whether to apply the code or the application update first to a Tier 2 environment.</span></span> 

<span data-ttu-id="a8d22-107">تذكر، عند إجراء تغييرات في الكود، لا تستخدم ملحق ملف `.Extension` حتى يمكنك تجنب مشاكل التوافق المستقبلية.</span><span class="sxs-lookup"><span data-stu-id="a8d22-107">Remember, when making code changes, do not use the `.Extension` file extension so that you can avoid future compatibility issues.</span></span>
