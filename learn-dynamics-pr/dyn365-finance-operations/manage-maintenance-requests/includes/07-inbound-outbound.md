---
ms.openlocfilehash: 305d6289a37bb636aeaeb81892de438204245300
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072431"
---
<span data-ttu-id="7afae-101">تعقب الأصول عند نقلها بين المواقع أمر ضروري.</span><span class="sxs-lookup"><span data-stu-id="7afae-101">Tracking your assets when moving them between locations is essential.</span></span> <span data-ttu-id="7afae-102">على سبيل المثال، قد تضطر إلى نقل جزء من المعدات من موقع إلى موقع آخر لإجراء صيانة.</span><span class="sxs-lookup"><span data-stu-id="7afae-102">For example, you might have to move a piece of equipment from one location to another to perform maintenance.</span></span> <span data-ttu-id="7afae-103">ومن الضروري أن تعلم المؤسسة موقع جميع أصولها.</span><span class="sxs-lookup"><span data-stu-id="7afae-103">It is essential that an organization knows the location of all its assets.</span></span> <span data-ttu-id="7afae-104">يمكن لإدارة الأصول تعقب الأصول الواردة والصادرة بحيث يمكنك التحكم في موقع الأصول في جميع الأوقات.</span><span class="sxs-lookup"><span data-stu-id="7afae-104">Asset Management can track inbound and outbound assets so that you can stay on top of where your assets are at all times.</span></span> <span data-ttu-id="7afae-105">ويوضح القسم الآتي العملية.</span><span class="sxs-lookup"><span data-stu-id="7afae-105">The following section explains the process.</span></span>

## <a name="register-assets-as-inbound"></a><span data-ttu-id="7afae-106">تسجيل الأصول كواردة</span><span class="sxs-lookup"><span data-stu-id="7afae-106">Register assets as inbound</span></span>
<span data-ttu-id="7afae-107">فكِّر في السيناريو الذي تقوم خلاله بتسجيل الأصول الجاري استلامها في مؤسستك من موقع آخر.</span><span class="sxs-lookup"><span data-stu-id="7afae-107">Consider the scenario where you are registering assets that are being received into your organization from another location.</span></span> <span data-ttu-id="7afae-108">على سبيل المثال، قد يكون لديك ضاغط هواء يحتاج إلى الصيانة.</span><span class="sxs-lookup"><span data-stu-id="7afae-108">For example, you might have an air compressor that needs maintenance.</span></span> <span data-ttu-id="7afae-109">عند إجرائك الصيانة، تقوم بنقل المعدات من موقع إلى آخر، مثل ورشة.</span><span class="sxs-lookup"><span data-stu-id="7afae-109">When you perform maintenance, you take the equipment from one location to another, such as a workshop.</span></span> <span data-ttu-id="7afae-110">أنت بحاجة إلى نقل ضاغط الهواء من موقع إلى آخر.</span><span class="sxs-lookup"><span data-stu-id="7afae-110">You need to move the air compressor from one location to another.</span></span> 

<span data-ttu-id="7afae-111">عند إجراء هذه العملية، يجب تذكر التفاصيل الآتية:</span><span class="sxs-lookup"><span data-stu-id="7afae-111">When performing this operation, you should keep the following details in mind:</span></span>

- <span data-ttu-id="7afae-112">يجب أن تكون قد قمت فعلياً بإنشاء **واردة** أو **صادرة** أو شيئاً مشابهاً في **حالات دورة حياة طلب الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-112">You must have **Inbound** or **Outbound**, or something similar, already established in your **Maintenance request lifecycle states**.</span></span> 
- <span data-ttu-id="7afae-113">تأكد من أن **نموذج دورة الحياة** يتضمن حالات دورة الحياة التي تم نقلها إلى قسم **حالات دورة الحياة المحددة** وأن **تحديثات حالات دورة الحياة** تتضمن القدرة على الانتقال إلى الواردة والصادرة.</span><span class="sxs-lookup"><span data-stu-id="7afae-113">Ensure that the **Lifecycle model** has the lifecycle states moved into the **Lifecycle states selected** section and that the **Lifecycle state updates** includes the ability to move to inbound and outbound.</span></span>

<span data-ttu-id="7afae-114">لتسجيل أصل كوارد، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="7afae-114">To register an asset as inbound, follow these steps:</span></span>

1.  <span data-ttu-id="7afae-115">انتقل إلى **إدارة الأصول > عام > طلبات الصيانة > طلبات الصيانة النشطة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-115">Go to **Asset management > Common > Maintenance requests > Active maintenance requests**.</span></span>
2.  <span data-ttu-id="7afae-116">حدد طلب الصيانة من أجل فتحه.</span><span class="sxs-lookup"><span data-stu-id="7afae-116">Select the maintenance request to open it.</span></span>
3.  <span data-ttu-id="7afae-117">ضمن جزء الإجراءات ثم ضمن القائمة **حالة دورة الحياة**، حدد **تحديث حالة طلب الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-117">Under the Action Pane and then under the submenu titled **Lifecycle state**, select **Update maintenance request state**.</span></span>
4.  <span data-ttu-id="7afae-118">حدد **واردة** (أو حالة دورة حياة أخرى قمت بإنشائها للأصول الواردة)، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7afae-118">Select **Inbound** (or another lifecycle state that you've created for inbound assets), and then select **OK**.</span></span> 

    <span data-ttu-id="7afae-119">النتيجة: تم تعيين **حالة دورة الحياة الحالية** في علامة التبويب السريعة **عام** إلى **واردة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-119">Result: The **Current lifecycle state** on the **General** FastTab is set to **Inbound**.</span></span>

    <span data-ttu-id="7afae-120">**إدارة الأصول > عام > طلبات الصيانة > طلبات الصيانة النشطة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-120">**Asset management > Common > Maintenance requests > Active maintenance requests**</span></span>

    ![لقطة شاشة لصفحة "تحديث حالة طلب الصيانة"](../media/inbound-ss.png)
 


## <a name="register-inbound-assets-as-received"></a><span data-ttu-id="7afae-122">تسجيل الأصول الواردة كمستلمة</span><span class="sxs-lookup"><span data-stu-id="7afae-122">Register inbound assets as received</span></span>
<span data-ttu-id="7afae-123">بعد استلام الأصل في مؤسستك، وضح أن الأصل قد تم استلامه:</span><span class="sxs-lookup"><span data-stu-id="7afae-123">After the asset has been received into your organization, indicate that the asset is received:</span></span>

1.   <span data-ttu-id="7afae-124">انتقل إلى **إدارة الأصول > عام > واردة/صادرة > الأصول الواردة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-124">Go to **Asset management > Common > Inbound/outbound > Inbound assets**.</span></span>
2.  <span data-ttu-id="7afae-125">حدد الأصل أو طلب الصيانة</span><span class="sxs-lookup"><span data-stu-id="7afae-125">Select the asset or maintenance request.</span></span>
3.  <span data-ttu-id="7afae-126">حدد **استلام الأصول**.</span><span class="sxs-lookup"><span data-stu-id="7afae-126">Select **Receive assets**.</span></span>
4.  <span data-ttu-id="7afae-127">في حقل **تم الاستلام**، أدخل التاريخ والوقت ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7afae-127">In the **Received** field, enter the date and time and then select **OK**.</span></span> <span data-ttu-id="7afae-128">تتم إزالة السجل من صفحة قائمة **الأصول الواردة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-128">The record is removed from the **Inbound assets** list page.</span></span>

## <a name="register-assets-as-outbound"></a><span data-ttu-id="7afae-129">تسجيل الأصول كصادرة</span><span class="sxs-lookup"><span data-stu-id="7afae-129">Register assets as outbound</span></span>
<span data-ttu-id="7afae-130">عند الانتهاء من مهمة الصيانة أو الإصلاح واستعدادك لإرجاع الأصل إلى موقعه الأصلي، يمكنك تسجيل الأصل بأنه تم إرجاعه.</span><span class="sxs-lookup"><span data-stu-id="7afae-130">When you've completed the maintenance or repair job and you are ready to return the asset to its home location, you can register the asset as returned.</span></span>

1.  <span data-ttu-id="7afae-131">حدد **إدارة الأصول > عام > طلبات الصيانة > طلبات الصيانة النشطة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-131">Select **Asset management > Common > Maintenance requests > Active maintenance requests**.</span></span>
2.  <span data-ttu-id="7afae-132">حدد طلب الصيانة</span><span class="sxs-lookup"><span data-stu-id="7afae-132">Select the maintenance request.</span></span>
3.  <span data-ttu-id="7afae-133">حدد **تحديث حالة طلب الصيانة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-133">Select **Update maintenance request state**.</span></span>
4.  <span data-ttu-id="7afae-134">حدد **واردة** (أو حالة دورة حياة أخرى قمت بإنشائها للأصول الصادرة)، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7afae-134">Select **Outbound** (or another lifecycle state that you've created for outbound assets) and then select **OK**.</span></span>


## <a name="register-outbound-assets-as-delivered"></a><span data-ttu-id="7afae-135">تسجيل الأصول كمُسلَّمة</span><span class="sxs-lookup"><span data-stu-id="7afae-135">Register outbound assets as delivered</span></span>
<span data-ttu-id="7afae-136">لتسجيل الأصول الصادرة كمُسلَّمة، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="7afae-136">To register outbound assets as delivered, follow these steps:</span></span>

1.  <span data-ttu-id="7afae-137">انتقل إلى **إدارة الأصول > عام > واردة/صادرة > الأصول الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-137">Select **Asset management > Common > Inbound/outbound > Outbound assets**.</span></span>
2.  <span data-ttu-id="7afae-138">حدد الأصل أو طلب الصيانة</span><span class="sxs-lookup"><span data-stu-id="7afae-138">Select the asset or maintenance request.</span></span>
3.  <span data-ttu-id="7afae-139">حدد **تسليم الأصول**.</span><span class="sxs-lookup"><span data-stu-id="7afae-139">Select **Deliver assets**.</span></span>
4.  <span data-ttu-id="7afae-140">في حقل **مُسلَّمة**، أدخل التاريخ والوقت ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="7afae-140">In the **Delivered** field, enter the date and time and then select **OK**.</span></span> <span data-ttu-id="7afae-141">تتم إزالة السجل من صفحة قائمة **الأصول الصادرة**.</span><span class="sxs-lookup"><span data-stu-id="7afae-141">The record is removed from the **Outbound assets** list page.</span></span>

