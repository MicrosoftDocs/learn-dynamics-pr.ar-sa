---
ms.openlocfilehash: 6f14a40ac602fb0a5c7b9c4786b2cd115f9adebd
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073057"
---

<span data-ttu-id="bd061-101">يمكن تكوين أنشطة النقل كأنشطة تعاقد من الباطن.</span><span class="sxs-lookup"><span data-stu-id="bd061-101">Transfer activities can be configured as subcontracting activities.</span></span> <span data-ttu-id="bd061-102">يتم تحديد دفعة التعاقد من الباطن بواسطة مزيج من الحقلين **المستودع** **‏‫شحن بواسطة‬** في إعداد النشاط.</span><span class="sxs-lookup"><span data-stu-id="bd061-102">The subcontracting payment is determined by a combination of the **Warehouse** and **Freighted by** fields in the activity setup.</span></span> <span data-ttu-id="bd061-103">يتم تكوين نشاط النقل كنشاط متعاقد عليه من الباطن بناءً على الحقل **شحن بواسطة** لنشاط النقل وإعداد المستودع.</span><span class="sxs-lookup"><span data-stu-id="bd061-103">A transfer activity is configured as a subcontracted activity depending on the **Freighted by** field of the transfer activity and the warehouse setup.</span></span>

<span data-ttu-id="bd061-104">يتم التعاقد من الباطن على النشاط إذا تم تعيين الحقل **شحن بواسطة** على **الشاحن‬** وكانت تتم إدارة مستودع التزويد بواسطة المورد، أو إذا تم تعيين الحقل **شحن بواسطة** على **المستلم** وكانت تتم إدارة مستودع التزويد بواسطة المورد.</span><span class="sxs-lookup"><span data-stu-id="bd061-104">The activity is subcontracted if the **Freighted by** field is set to **Shipper** and the Replenishing warehouse is managed by the vendor, or if the **Freighted by** field is set to **Recipient** and the Replenished warehouse is managed by the vendor.</span></span> <span data-ttu-id="bd061-105">إذا كانت تتم إدارة المستودع بواسطة المورد، سيتم تعيين حساب المورد المعين كمقاول من الباطن.</span><span class="sxs-lookup"><span data-stu-id="bd061-105">If the warehouse is managed by the vendor, it will have the vendor account designated as the subcontractor.</span></span>
