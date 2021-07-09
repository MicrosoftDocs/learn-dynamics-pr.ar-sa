---
ms.openlocfilehash: ac50efe5dad2cb7778698ffeabc9a788276bf1a3
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6073697"
---
<span data-ttu-id="aec00-101">يمكن للشركات ربط البيانات المالية ذات الصلة بحركات المخزون التي يتم الحصول عليها في كل موقع في بيئة الإنتاج متعددة المواقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-101">Companies can link relevant financial data to the inventory transactions that are taking place at each site in a multisite production environment.</span></span> <span data-ttu-id="aec00-102">يؤدي هذا الارتباط إلى:</span><span class="sxs-lookup"><span data-stu-id="aec00-102">This link results in:</span></span>

-   <span data-ttu-id="aec00-103">بُعد مالي مقترن ببُعد مخزون الموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-103">A financial dimension that is associated with the site inventory dimension.</span></span>

-   <span data-ttu-id="aec00-104">قيمة بُعد مالي مقترنة بكل موقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-104">A financial dimension value that is associated with each site.</span></span>

<span data-ttu-id="aec00-105">تفترض روابط البُعد المالي أن الإيرادات المعنية تعزى مباشرةً إلى موقع التسليم.</span><span class="sxs-lookup"><span data-stu-id="aec00-105">Financial dimension links assume that the revenue in question is directly attributable to the delivering site.</span></span> <span data-ttu-id="aec00-106">عندما يكون هذا هو الحال، تسمح هذه الميزة للشركات بتتبع أرقام الأرباح والخسائر مباشرةً من موقع التشغيل.</span><span class="sxs-lookup"><span data-stu-id="aec00-106">When this is the case, this feature allows companies to trace profit and loss figures directly to the operational site.</span></span>

<span data-ttu-id="aec00-107">**إعداد > إدارة المخزون > ترحيل > ارتباط البُعد**</span><span class="sxs-lookup"><span data-stu-id="aec00-107">**Inventory management > Setup > Posting > Dimension link**</span></span>

![لقطة شاشة للقائمة المنسدلة على صفحة ارتباط البُعد.](../media/dimension-link.png) 


<span data-ttu-id="aec00-109">يجب تنشيط الارتباط بمجرد ربط الأبعاد المالية بحركات المخزون في أحد المواقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-109">After linking financial dimensions to inventory transactions at a site, you need to activate the link.</span></span>

<span data-ttu-id="aec00-110">إذا قمت بتحديد زر **تنشيط الارتباط**، سيتم تحديد قيمة البُعد المحدد على كافة الحركات استناداً إلى قيمة بُعد تخزين الموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-110">If you select the **Activate link** button, the value of the selected dimension on all transactions will be determined based on the value of the Site storage dimension.</span></span> <span data-ttu-id="aec00-111">ومع ذلك، قد يستمر ترحيل الحركات بغض النظر عن قيمة البُعد.</span><span class="sxs-lookup"><span data-stu-id="aec00-111">However, transactions might still be posted regardless of the dimension value.</span></span>

<span data-ttu-id="aec00-112">ينتج عن تنشيط ارتباط البُعد المالي حدوث الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="aec00-112">Activation of the financial dimension link results in the following conditions:</span></span>

-   <span data-ttu-id="aec00-113">عند إنشاء حركات جديدة تحمل كل من أبعاد المخزون والأبعاد المالية، يتم تعيين قيمة البُعد الخاصة بالبُعد المالي المرتبط بالموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-113">When new transactions are created that carry both inventory dimensions and financial dimensions, the linked financial dimension is assigned the dimension value that is specified for the site.</span></span>

-   <span data-ttu-id="aec00-114">يمكن ترحيل الحركات التي تحمل أبعاد المخزون والأبعاد المالية، على الرغم من أن قيمة البُعد المالي المرتبطة لا تتطابق مع القيمة المحددة للموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-114">Transactions that carry both inventory dimensions and financial dimensions can be posted, even though the linked financial dimension value does not match the value that is specified for the site.</span></span>

-   <span data-ttu-id="aec00-115">يمكن تغيير قيمة البُعد المالي المرتبط بالحركات المفتوحة التي تحمل أبعاد المخزون والأبعاد المالية.</span><span class="sxs-lookup"><span data-stu-id="aec00-115">The value of the linked financial dimension can be changed on open transactions that carry both inventory dimensions and financial dimensions.</span></span>

<span data-ttu-id="aec00-116">إذا قمت بتحديد زر **تأمين الارتباط**، يمكن ترحيل الحركات فقط إذا كانت قيمة البُعد المحدد تطابق القيمة المقترنة ببُعد تخزين الموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-116">If you select the **Lock link** button, transactions can only be posted if the value of the selected dimension matches the value associated with the Site storage dimension.</span></span>
<span data-ttu-id="aec00-117">وبالتالي، يجب تحديث كافة الحركات المفتوحة قبل تأمين ارتباط البُعد.</span><span class="sxs-lookup"><span data-stu-id="aec00-117">Hence, all open transactions must be updated before the dimension link can be locked.</span></span>

<span data-ttu-id="aec00-118">يؤدي تأمين ارتباط البُعد المالي إلى حدوث الحالات التالية:</span><span class="sxs-lookup"><span data-stu-id="aec00-118">Locking the financial dimension link results in the following conditions:</span></span>

-   <span data-ttu-id="aec00-119">يتم تعيين قيمة بُعد مالي لحركات المخزون الجديدة التي تحمل أبعاد المخزون والأبعاد المالية على حد سواء استناداً إلى القيمة المحددة للموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-119">New inventory transactions that carry both inventory dimensions and financial dimensions are assigned a financial dimension value based on the value that is specified for the site.</span></span>

-   <span data-ttu-id="aec00-120">لا يمكنك ترحيل المعاملات التي تحمل أبعاد المخزون والأبعاد المالية إلا عندما تكون قيمة البُعد المالي المرتبطة مطابقة للقيمة المحددة للموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-120">You can post transactions that carry both inventory dimensions and financial dimensions only when the linked financial dimension value matches the value that is specified for the site.</span></span>

-   <span data-ttu-id="aec00-121">ولا يمكنك تغيير قيمة البُعد المالي المتصل بالمعاملات التي تحمل أبعاد المخزون والأبعاد المالية على حد سواء.</span><span class="sxs-lookup"><span data-stu-id="aec00-121">You cannot change the value of the linked financial dimension on transactions that carry both inventory dimensions and financial dimensions.</span></span>

-   <span data-ttu-id="aec00-122">لا يمكنك تحرير قيمة البُعد المالي المقترنة بموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-122">You cannot edit the financial dimension value that is associated with a site.</span></span> <span data-ttu-id="aec00-123">تتمثل الشروط المسبقة لتأمين ارتباط‬ البُعد المالي في: وجوب إنشاء ارتباط البُعد المالي مع بُعد مخزون الموقع.</span><span class="sxs-lookup"><span data-stu-id="aec00-123">The prerequisites for locking the financial dimension link are: A financial dimension link with the site inventory dimension must be established.</span></span>
