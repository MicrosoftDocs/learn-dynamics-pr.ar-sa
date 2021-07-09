---
ms.openlocfilehash: a814db95afdbd0b10623a4530ac9beb6a73dc0e9
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070233"
---
<span data-ttu-id="e75dd-101">يتميز كل متجر ومحطة طرفية بخصائص ومتطلبات مميزة بناءً على ملفات تعريف الشبكة والاحتياجات الوظيفية داخل المتجر وعبر المتاجر ونفقات الصيانة العامة.</span><span class="sxs-lookup"><span data-stu-id="e75dd-101">Each store and terminal have distinct characteristics and requirements based on network profiles, in-store and cross-store functional needs, and maintenance overhead.</span></span> <span data-ttu-id="e75dd-102">يتمتع العملاء بالمرونة لمزج التكوينات ومطابقتها بسلاسة لكل متجر وكل محطة، بناءً على هذه الخصائص والمتطلبات، للحصول على أقصى قيمة بأقل تكلفة صيانة وتشغيل.</span><span class="sxs-lookup"><span data-stu-id="e75dd-102">Customers have the flexibility to seamlessly mix and match configurations for each store and each terminal, based on these characteristics and requirements, to get the most value at the lowest maintenance and operating cost.</span></span>
 
<span data-ttu-id="e75dd-103">عند التفكير في طوبولوجيا في المتجر، عليك مراعاة هذه النقاط الرئيسية:</span><span class="sxs-lookup"><span data-stu-id="e75dd-103">When considering an in-store topology, you need to consider these main points:</span></span>

- <span data-ttu-id="e75dd-104">**الاتصال** يتطلب توفر شبكة LAN وشبكة WAN دراسة متأنية.</span><span class="sxs-lookup"><span data-stu-id="e75dd-104">**Connectivity** – LAN and WAN network availability requires careful consideration.</span></span> 
- <span data-ttu-id="e75dd-105">**الأجهزة الفعلية/الأجهزة الطرفية** أحد الجوانب الهامة لنظام Retail POS هو قدرته على استخدام أجهزة نقاط البيع الطرفية، مثل الطابعات وأدراج النقدية ووحدات الدفع الطرفية.</span><span class="sxs-lookup"><span data-stu-id="e75dd-105">**Hardware devices/peripherals** – An important aspect of a Retail POS system is its ability to use POS peripherals such as printers, cash drawers, and payment terminals.</span></span> 
- <span data-ttu-id="e75dd-106">**التوزيع والصيانة** – يمكن أن يختلف تعقيد متطلبات التوزيع والصيانة، اعتماداً على خيارات التطبيق والتوزيع.</span><span class="sxs-lookup"><span data-stu-id="e75dd-106">**Deployment and servicing** – The complexity of deployment and servicing requirements can vary, depending on the application and deployment choices.</span></span> 
 
<span data-ttu-id="e75dd-107">استناداً إلى هذه الاعتبارات، لديك الخيارات التالية فيما يتعلق بطبولوجيا في المتجر:</span><span class="sxs-lookup"><span data-stu-id="e75dd-107">Based on these considerations, you have the following options regarding in-store topologies:</span></span>

- <span data-ttu-id="e75dd-108">**MPOS بوحدة Store Scale Unit دون اتصال بالإنترنت** – تعد هذه الطبولوجيا الأنسب للمتاجر ذات الاتصال الضعيف بالشبكة أو درجة تحمل منخفضة ضد فقدان الاتصال داخل شبكات LAN أو WAN.</span><span class="sxs-lookup"><span data-stu-id="e75dd-108">**MPOS with offline and Store Scale Unit** – This topology is most suitable for stores with poor network connectivity or low tolerance for connectivity loss within the LAN or WAN networks.</span></span>
- <span data-ttu-id="e75dd-109">**MPOS بوحدة Cloud Scale Unit دون اتصال بالإنترنت**– تعد هذه الطبولوجيا الأكثر ملاءمة للمتاجر التي لديها اتصال شبكة LAN ضعيف ولكن لديها اتصال WAN جيد.</span><span class="sxs-lookup"><span data-stu-id="e75dd-109">**MPOS with offline and Cloud Scale Unit** – This topology is most suitable for stores that have poor LAN network connectivity but have a good WAN connection.</span></span>
- <span data-ttu-id="e75dd-110">**MPOS أو CPOS ووحدة Store Scale Unit** – إذا كان المتجر يتمتع باتصال جيد بشبكة LAN أو درجة تحمل عالية ضد فقدان اتصال LAN وفي نفس الوقت اتصال WAN ضعيف أو درجة تحمل منخفضة ضد فقدان اتصال WAN.</span><span class="sxs-lookup"><span data-stu-id="e75dd-110">**MPOS or CPOS and Store Scale Unit** – If the store has a good LAN connectivity or high tolerance for LAN connectivity loss and at the same time poor WAN connectivity or low tolerance for WAN connectivity loss.</span></span> 
- <span data-ttu-id="e75dd-111">**MPOS أو CPOS ووحدة Cloud Scale Unit** – يوصى باستخدام هذا الهيكل للمتاجر التي تتمتع باتصال جيد أو درجة تحمل عالية ضد فقدان الاتصال لشبكات LAN وWAN.</span><span class="sxs-lookup"><span data-stu-id="e75dd-111">**MPOS or CPOS and Cloud Scale Unit** – This topology is recommended for stores that have good connectivity or high tolerance for connectivity loss, for LAN and WAN.</span></span>

