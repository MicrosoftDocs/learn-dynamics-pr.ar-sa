---
ms.openlocfilehash: cdd1745f30c4ab5acc105526d059ffea178f602b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071674"
---

<span data-ttu-id="a977b-101">يمكنك تطوير خدمات مخصصة للتطبيقات Finance and Operations من أجل عرض وظائف ‎‎X‎ + +‎ للعملاء الخارجيين.</span><span class="sxs-lookup"><span data-stu-id="a977b-101">You can develop custom services for Finance and Operations apps to expose X++ functionality to external clients.</span></span> <span data-ttu-id="a977b-102">يمكن عرض الكود الموجود كخدمة مخصصة من خلال إضافة سمة إلى الكود.</span><span class="sxs-lookup"><span data-stu-id="a977b-102">Existing code can be exposed as a custom service by adding an attribute to the code.</span></span> <span data-ttu-id="a977b-103">يتم تعيين السمة في فئة عقد البيانات وأعضائها من أجل إجراء التسلسل وإلغاء التسلسل تلقائياً للبيانات التي يتم إرسالها واستلامها عبر اتصال الشبكة.</span><span class="sxs-lookup"><span data-stu-id="a977b-103">The attribute is set on the data contract class and its members to automatically serialize and deserialize data that is sent and received across a network connection.</span></span>

<span data-ttu-id="a977b-104">يمكنك استخدام خدمة مخصصة عندما يكون مخطط الكيان يمكن كتابته كفئة عقد بيانات بسيط مع تعيين سمات عضو البيانات ذي الصلة.</span><span class="sxs-lookup"><span data-stu-id="a977b-104">You can use custom service when the schema for the entity can be written as a simple data contract class with relevant data member attributes set.</span></span> <span data-ttu-id="a977b-105">يتم تحديد تسلسل عقد بيانات X++ وإلغاء التسلسل باستخدام السمتين `DataContractAttribute` و`DataMemberAttribute`.</span><span class="sxs-lookup"><span data-stu-id="a977b-105">X++ data contract serialization and deserialization are specified by using the attributes `DataContractAttribute` and `DataMemberAttribute`.</span></span>

<span data-ttu-id="a977b-106">عند كتابة خدمة مخصصة ضمن مجموعة خدمة، يتم دائماً توزيع مجموعة الخدمة على نقطتي نهاية:</span><span class="sxs-lookup"><span data-stu-id="a977b-106">When you write a custom service under a service group, the service group is always deployed on two endpoints:</span></span>

-   <span data-ttu-id="a977b-107">نقطة نهاية SOAP</span><span class="sxs-lookup"><span data-stu-id="a977b-107">SOAP endpoint</span></span>
-   <span data-ttu-id="a977b-108">نقطة نهاية JavaScript Object Notation ‏(JSON)</span><span class="sxs-lookup"><span data-stu-id="a977b-108">JavaScript Object Notation (JSON) endpoint</span></span>

<span data-ttu-id="a977b-109">باستخدام خدمة مخصصة مستندة إلى SOAP، يتم توزيع جميع مجموعات الخدمة الموجودة ضمن العقدة **مجموعة خدمة AOT** تلقائياً، ويجب أن تكون الخدمات التي يتم توزيعها جزءاً من مجموعة خدمة.</span><span class="sxs-lookup"><span data-stu-id="a977b-109">With a SOAP-based custom service, all service groups under the **AOTService group** node are automatically deployed, and services that are deployed must be part of a service group.</span></span> <span data-ttu-id="a977b-110">تُستهلك فئات X++ كخدمات JSON، لذا فإن مجموعة بيانات الإرجاع تكون بتنسيق JSON.</span><span class="sxs-lookup"><span data-stu-id="a977b-110">X++ classes are consumed as JSON services, so the return data set is in JSON format.</span></span> <span data-ttu-id="a977b-111">يتم استخدام JSON لتوصيل البيانات بين العميل والخادم.</span><span class="sxs-lookup"><span data-stu-id="a977b-111">JSON is used to communicate data between the client and the server.</span></span> 
