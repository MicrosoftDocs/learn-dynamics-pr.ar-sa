---
ms.openlocfilehash: 921964846e4a5fd677bee390b961f1742305c954
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070063"
---
<span data-ttu-id="08129-101">يستند توزيع البيانات في Dynamics 365 Commerce على Commerce Data Exchange، والذي ينقل البيانات بين المركز الرئيسي (HQ) في Commerce والقنوات المختلفة.</span><span class="sxs-lookup"><span data-stu-id="08129-101">Data distribution in Dynamics 365 Commerce is based on Commerce Data Exchange, which transfers data between Commerce Headquarters (HQ) and the different channels.</span></span> 

<span data-ttu-id="08129-102">تستخدم خدمة المزامنة جدول Commerce لجدولة توزيع البيانات مع مهمات الرفع والتنزيل، وستوفر خدمة الوقت الحقيقي الاتصال الفوري بين المراكز الرئيسية والقنوات.</span><span class="sxs-lookup"><span data-stu-id="08129-102">The async service uses the Commerce scheduler to schedule data distribution with upload and download jobs and the Real-time service provides real-time communication between Headquarters and the channels.</span></span> <span data-ttu-id="08129-103">وتكون قاعدة البيانات التي تقوم بتخزين البيانات لإحدى القنوات، منفصلة عن قاعده بيانات Commerce.</span><span class="sxs-lookup"><span data-stu-id="08129-103">The database that stores data for a channel is separate from the Commerce database.</span></span> <span data-ttu-id="08129-104">تحتوي قاعدة بيانات القناة فقط على البيانات المطلوبة للحركات.</span><span class="sxs-lookup"><span data-stu-id="08129-104">The channel database holds only the data that is required for transactions.</span></span> 

<span data-ttu-id="08129-105">على سبيل المثال، يتم إعداد البيانات الرئيسية في المراكز الرئيسية ثم يتم توزيعها على القنوات، وعلى الجانب الآخر، يتم إنشاء بيانات الحركات في نقطه البيع (POS) أو المتجر على الإنترنت، ثم يتم رفعها إلى المراكز الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="08129-105">For example, master data is set up in Headquarters and then distributed to channels and, on the other side, transactional data is created in the point of sale (POS) or the online store and then uploaded to Headquarters.</span></span>

