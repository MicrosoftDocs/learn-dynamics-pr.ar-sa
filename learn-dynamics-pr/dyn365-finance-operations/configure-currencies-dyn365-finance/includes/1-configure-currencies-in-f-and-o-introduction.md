---
ms.openlocfilehash: d7ab11cab758f576fe710edd947d47e76779938b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070757"
---
<span data-ttu-id="b74d7-101">أول وأهم خطوات تنفيذ Dynamics 365 Finance هي إعداد العملة.</span><span class="sxs-lookup"><span data-stu-id="b74d7-101">One of the first and most important steps of implementing Dynamics 365 Finance is currency setup.</span></span>  <span data-ttu-id="b74d7-102">يعد إعداد العملة إحدى الخطوات المطلوبة في تكوين النظام ويتم استخدامها لتسجيل الحركات المالية.</span><span class="sxs-lookup"><span data-stu-id="b74d7-102">Currency setup is a required step in the configuration of the system and is used to record financial transactions.</span></span> <span data-ttu-id="b74d7-103">وتشرح هذه الوحدة النمطية إدارة العملات في Finance.</span><span class="sxs-lookup"><span data-stu-id="b74d7-103">This module explains currency management in Finance.</span></span>

<span data-ttu-id="b74d7-104">سوف تتعرف في هذه الوحدة على:</span><span class="sxs-lookup"><span data-stu-id="b74d7-104">In this module, you will learn about:</span></span>

- <span data-ttu-id="b74d7-105">أنواع مختلفة من العملات في Finance.</span><span class="sxs-lookup"><span data-stu-id="b74d7-105">Different types of currencies in Finance.</span></span>
- <span data-ttu-id="b74d7-106">مفهوم عملة التحويل الثلاثي.</span><span class="sxs-lookup"><span data-stu-id="b74d7-106">The concept of triangulation currency.</span></span>
- <span data-ttu-id="b74d7-107">كيفية إعداد عمليات التحويل والعملات الخاصة بالكيان القانوني.</span><span class="sxs-lookup"><span data-stu-id="b74d7-107">How to set up legal entity currencies and conversions.</span></span>
- <span data-ttu-id="b74d7-108">تكوين موفري أسعار الصرف.</span><span class="sxs-lookup"><span data-stu-id="b74d7-108">Configuration of exchange rate providers.</span></span>
- <span data-ttu-id="b74d7-109">كيفية استيراد أسعار الصرف من الموفرين.</span><span class="sxs-lookup"><span data-stu-id="b74d7-109">How to import exchange rates from providers.</span></span>

<span data-ttu-id="b74d7-110">هناك نوعان من العملات في Finance.</span><span class="sxs-lookup"><span data-stu-id="b74d7-110">There are two types of currencies in Finance.</span></span> 

<span data-ttu-id="b74d7-111">ويطلق على العملة الأساسية التي تستخدمها الشركة اسم **عملة المحاسبة**.</span><span class="sxs-lookup"><span data-stu-id="b74d7-111">The main currency that a company uses is called the **accounting currency**.</span></span> <span data-ttu-id="b74d7-112">وعادة، يجب أن تقوم الشركة بتقديم تقرير عن الحركات المالية المسجلة بناء على عملة مختلفة، والتي تعرف باسم **عملة التقارير**.</span><span class="sxs-lookup"><span data-stu-id="b74d7-112">Often, a company must report recorded financial transactions based on a different currency, which is known as the **reporting currency**.</span></span> 

<span data-ttu-id="b74d7-113">سيكون لكافة الشركات عملة تقارير أساسية، وفي بعض الشركات التي ستكون هي العملة الوحيدة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="b74d7-113">All companies will have a base reporting currency, and in some companies that will be the only currency needed.</span></span>  

<span data-ttu-id="b74d7-114">يمكن استخدام وظيفة متعدد العملات إذا كانت شركتك تتعامل مع أكثر من عملة واحدة.</span><span class="sxs-lookup"><span data-stu-id="b74d7-114">Multicurrency functionality may be used if your company does business in more than one currency.</span></span>  <span data-ttu-id="b74d7-115">إذا كانت المؤسسة تحتوي على العديد من الكيانات القانونية وتتعامل بعملات متعددة، فإن الحفاظ على العملات وأسعار الصرف المقابلة لها أمر أساسي.</span><span class="sxs-lookup"><span data-stu-id="b74d7-115">If your organization has multiple legal entities and transacts in multiple currencies, then maintaining currencies and their corresponding exchange rates is essential.</span></span>  

<span data-ttu-id="b74d7-116">حدد أنواع سعر الصرف التي تسمح لك بإعداد أسعار صرف العملات.</span><span class="sxs-lookup"><span data-stu-id="b74d7-116">Specify exchange rate types that allow you to set up the currency exchange rates.</span></span>  <span data-ttu-id="b74d7-117">عند تحديد العمليات الحسابية وإعداد تقارير حول العملات، فإنه يتم تحديد أسعار صرف العملة بين عملتين أو زوج من العملات.</span><span class="sxs-lookup"><span data-stu-id="b74d7-117">When you have determined the accounting and reporting currencies, then you define currency exchange rates between two currencies or a currency pair.</span></span>  <span data-ttu-id="b74d7-118">وفي الوحدة التالية، ستتعلم كيفية إعداد العملات وتحويلات العملات لكيان قانوني تم إنشاؤه حديثاً.</span><span class="sxs-lookup"><span data-stu-id="b74d7-118">In the next unit you will learn how to set up currencies and currency conversions for a newly created legal entity.</span></span>

