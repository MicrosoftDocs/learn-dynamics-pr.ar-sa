---
ms.openlocfilehash: 6f09cd1cebd3a2f7789ec847b5f219439ddf1011
ms.sourcegitcommit: ad358034a3371aed45c7d4883e01645b232fa589
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2021
ms.locfileid: "6070432"
---
<span data-ttu-id="2dd6c-101">تتوفر العديد من نماذج التوزيع المتعددة للعملاء، وذلك وفقاً لاحتياجاتهم وبيئات التشغيل لديهم.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-101">Multiple deployment patterns are available to customers, depending on their needs and operating environments.</span></span> <span data-ttu-id="2dd6c-102">يمكن استخدام النماذج بسيناريوهات متعددة، وتشمل السناريوهات المختلطة في حالة وجود خليط من النماذج لديك، وسيناريو يمكنك من خلاله استخدام نماذج متعددة على نحو متزامن، والمزيد.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-102">The patterns can be used in multiple scenarios, including hybrid scenarios where you have a mix of patterns, a scenario where you can use multiple patterns in parallel, and more.</span></span>

## <a name="cloud-1st"></a><span data-ttu-id="2dd6c-103">الشبكة السحابية الأولى</span><span class="sxs-lookup"><span data-stu-id="2dd6c-103">Cloud 1st</span></span>
 
<span data-ttu-id="2dd6c-104">المخطط الأول والأكثر شمولاً هو **نقاط البيع (POS) السحابية الأولى**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-104">The first and most generic topology is the **Cloud 1st point of sale (POS)**.</span></span> <span data-ttu-id="2dd6c-105">وعلى الرغم من أنه لا يدخل بشكل كبير ضمن الأمور المتعلقة بالتوزيع، إلا أنه يغطي أجزاءً من التوزيع مثل تثبيت نقطة بيع حديثة (MPOS) باستخدام نظام إدارة يعمل على الإشراف على ما تقوم به سجلاتك، كما يقرر الشكل الذي ستظهر عليه قاعدة البيانات لديك.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-105">Though it is not highly involved in terms of deployment, it covers parts of the deployment such as installing Modern point of sale (MPOS), using a management system that oversees what your registers are doing, and determining what your databases look like.</span></span> <span data-ttu-id="2dd6c-106">تتضمن **نقاط البيع السحابية الأولى** مجموعة متنوعة من الأجهزة الطرفية المتصلة بشكل مباشر.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-106">**Cloud 1st POS** includes a variety of peripherals that are connected directly.</span></span> <span data-ttu-id="2dd6c-107">هذا النموذج هو المستخدم بشكل شائع عبر قاعدة العملاء، وخصوصاً للعملاء غير المتأكدين من مدى الجودة التي سيكون عليها اتصال WAN لديهم داخل المتجر.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-107">This pattern is one that is commonly used across the customer base, especially for customers who aren't certain about how good their WAN connection is going to be in-store.</span></span> 

<span data-ttu-id="2dd6c-108">تعرض الصورة التالية **نموذج الشبكة السحابية الأولى**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-108">The following image shows the **Cloud 1st** pattern.</span></span>

![الرسم التخطيطي لنموذج الشبكة السحابية الأولى في Dynamics 365 Commerce.](../media/cloud-first.png)
 
## <a name="cloud-pos-only"></a><span data-ttu-id="2dd6c-110">نقاط البيع السحابية فقط</span><span class="sxs-lookup"><span data-stu-id="2dd6c-110">Cloud POS only</span></span>

<span data-ttu-id="2dd6c-111">تعرض الصورة التالية نموذج **نقاط البيع السحابية فقط**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-111">The following image shows the **Cloud POS only** pattern.</span></span> <span data-ttu-id="2dd6c-112">يكون هذا النموذج مفيداً للعملاء الذين يخططون لنسخ الشبكة احتياطياً ويكون اتصال WAN متاحاً بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-112">This pattern is beneficial for customers who tend to have network back up and the WAN connection is always available.</span></span> <span data-ttu-id="2dd6c-113">لتمكين العمل المناسب لهذا النموذج واستخدام نقاط البيع السحابية، سيكون لديك وحدة محطة أجهزة منفصلة داخل المتجر، والتي تتصل بالأجهزة الطرفية، ثم تقوم بتوصيلها جميعاً إلى الشبكة السحابية، الأمر الذي يسمح لواجهة Retail Server ونقاط البيع السحابية في الشبكة السحابية من التصرف كبيئة أساسية.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-113">To enable the proper functioning of this pattern and use Cloud POS, you would have a separate hardware station unit in-store that connects to the peripherals and connects them all to the cloud, allowing Retail Server and Cloud POS in the cloud acting as the base environment.</span></span> 

![الرسم التخطيطي لنموذج نقاط البيع السحابية فقط في Dynamics 365 Commerce.](../media/cloud-pos-only.png)
 
## <a name="cloud-pos-whardware-station"></a><span data-ttu-id="2dd6c-115">نقاط البيع السحابية المزودة بمحطة أجهزة</span><span class="sxs-lookup"><span data-stu-id="2dd6c-115">Cloud POS w/hardware station</span></span>

<span data-ttu-id="2dd6c-116">يعد الإصدار الأكثر تنظيماً من نموذج **نقاط البيع السحابية فقط** هو **نقاط البيع السحابية المزودة بمحطة أجهزة**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-116">A more structured version of the **Cloud POS only** pattern is the **Cloud POS w/hardware station**.</span></span> <span data-ttu-id="2dd6c-117">يسمح هذا النموذج بالاتصال المباشر بالأجهزة الطرفية غير المتصلة بالشبكة.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-117">This pattern allows for connecting non-networked peripherals directly.</span></span> <span data-ttu-id="2dd6c-118">وقد يكون هو السيناريو الأكثر معيارية عندما تقوم بإعداد نقطة بيع سحابية، ولكنه يكون النموذج الأمثل مثل النموذج السابق بشكل فعال.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-118">It tends to be the more standard scenario when you are setting up Cloud POS, but it's effectively the exact pattern as the previous one.</span></span> 

<span data-ttu-id="2dd6c-119">تعرض الصورة التالية نموذج **نقطة البيع السحابية المزودة بمحطة أجهزة**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-119">The following image shows the **Cloud POS w/hardware station** pattern.</span></span>

![الرسم التخطيطي لنموذج نقطة البيع السحابية المزودة بمحطة أجهزة في Dynamics 365 Commerce.](../media/cloud-pos-hardware-station.png)

## <a name="cloud-wpos-offline"></a><span data-ttu-id="2dd6c-121">الشبكة السحابية المزودة بنقطة بيع غير متصلة</span><span class="sxs-lookup"><span data-stu-id="2dd6c-121">Cloud w/POS offline</span></span>

<span data-ttu-id="2dd6c-122">يقدم النموذج **الشبكة السحابية المزودة بقطة بيع غير متصلة** نموذجاً مختلطاً يغطي كلا من نقطة البيع الحديثة (MPOS) ونقطة البيع السحابية كجزء من الإعداد.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-122">The **Cloud w/POS offline** pattern presents a hybrid pattern that covers both Modern point of sale (MPOS) and Cloud POS as part of the setup.</span></span> <span data-ttu-id="2dd6c-123">الحالة النموذجية لهذا السيناريو هي المكان الذي تستخدم فيه نقطة البيع السحابية بشكل أساسي ثم تستخدم MPOS كوحدات نسخ احتياطي أو كوحدات قياسية تعمل دائماً عن طريق الصرّافين.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-123">The typical case for this scenario is where you use Cloud POS primarily and then have MPOS as backup units or standard units that are always operated by cashiers.</span></span>

<span data-ttu-id="2dd6c-124">تعرض الصورة التالية نموذج **الشبكة السحابية المزودة بنقطة بيع غير متصلة**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-124">The following image shows the **Cloud w/POS offline** pattern.</span></span>

![الرسم التخطيطي لنموذج الشبكة السحابية المزودة بنقطة بيع غير متصلة في Dynamics 365 Commerce.](../media/cloud-pos-offline.png) 
 
## <a name="csu-deployed-in-store"></a><span data-ttu-id="2dd6c-126">وحدات CSU الموزعة داخل المتجر</span><span class="sxs-lookup"><span data-stu-id="2dd6c-126">CSU deployed in-store</span></span>

<span data-ttu-id="2dd6c-127">تمثل **وحدات Commerce Scale Units (‏CSU)** المفهوم المحلي، بمعنى أنه سيتم توزيعه داخل المتجر.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-127">The **Commerce Scale Units (CSU) deployed in-store** pattern is the on-premises concept, meaning that it would be deployed in-store.</span></span> <span data-ttu-id="2dd6c-128">على سبيل المثال، يمكن استخدام هذا النموذج في مركز بيانات أو في عدة أماكن أخرى.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-128">For example, this pattern could be used in a data center or in several other places.</span></span> <span data-ttu-id="2dd6c-129">ومع ذلك، فإن السيناريو غالبا قد يتضمن MPOS أو نقطة بيع سحابية تتصل بوحدة Commerce Scale Unit في الطبقة المحلية ثم الانتقال إلى الشبكة السحابية لإجراء مكالمات الوقت الحقيقي والسيناريوهات التي تتطلب وصول WAN.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-129">However, the scenario would most often involve MPOS or Cloud POS communicating with that Commerce Scale Unit directly at the local layer and then going out to the cloud for real-time calls and scenarios that require WAN access.</span></span> 

<span data-ttu-id="2dd6c-130">تعرض الصورة التالية نموذج **وحدة CSU الموزعة داخل المتجر**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-130">The following image shows the **CSU deployed in-store** pattern.</span></span>
 
![الرسم التخطيطي لنموذج وحدات المقياس الموزعة داخل المتجر في Dynamics 365 Commerce.](../media/cloud-scale-unit-deployed-in-store.png) 

## <a name="csu-deployed-in-private-cloud"></a><span data-ttu-id="2dd6c-132">وحدات CSU الموزعة في المجموعة الخاصة</span><span class="sxs-lookup"><span data-stu-id="2dd6c-132">CSU deployed in private cloud</span></span>
 
<span data-ttu-id="2dd6c-133">يغطي نموذج **وحدات CSU الموزعة في المجموعة الخاصة** مفهوم المتاجر المتعددة.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-133">The **CSU deployed in private cloud** pattern covers the concept of multi-store.</span></span> <span data-ttu-id="2dd6c-134">يمكنك استخدام هذا النموذج إذا كانت لديك قاعدة بيانات أحادية القناة، ثم أصبح لديك متاجر متعددة متصلة بوحدة CSU فردية.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-134">You can use this pattern when you have a single channel database and then have multiple stores that are connecting to a single CSU.</span></span> <span data-ttu-id="2dd6c-135">ولا تكون بالضرورة علاقة واحد لواحد.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-135">It’s not necessarily a one-to-one relation.</span></span> 

<span data-ttu-id="2dd6c-136">حالة الاستخدام هذه هي الأكثر شيوعاً لأن معظم المتاجر تتصل بوحدة CSU واحدة، وتقوم عادةً بمشاركه نفس مجموعة البيانات.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-136">This use case is the most common because most stores connect to one CSU and usually share the same dataset.</span></span> <span data-ttu-id="2dd6c-137">وغالباً ما يُستخدم هذا السيناريو بواسطة عملاء المؤسسات الكبيرة الذين لديهم مراكز بيانات خاصة بهم ويرغبون في استخدامها.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-137">Often, this scenario is used by large enterprise customers who have their own data centers and want to use them.</span></span> <span data-ttu-id="2dd6c-138">كما يفضلون الاعتماد على وحدات CSU في مراكز البيانات الخاصة بهم، ثم يكون لديهم متجراً وحداً أو أكثر تنتشر في مناطق مختلفة متصلة بمراكز البيانات لديهم.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-138">They tend to take CSUs on premises into their data centers and then have one or many stores that are based in different regions connected to those data centers.</span></span> 

<span data-ttu-id="2dd6c-139">تعرض الصورة التالية نموذج **وحدة CSU الموزعة في مجموعة خاصة**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-139">The following image shows the **CSU deployed in private cloud** pattern.</span></span>

![الرسم التخطيطي لنموذج وحدات المقياس الموزعة داخل مجموعة خاصة في Dynamics 365 Commerce.](../media/cloud-scale-unit-deployed-private-cloud.png) 

## <a name="n-1-with-ax-2012-r3"></a><span data-ttu-id="2dd6c-141">"N-1" مع AX2012 R3</span><span class="sxs-lookup"><span data-stu-id="2dd6c-141">“N-1” with AX 2012 R3</span></span>
 
<span data-ttu-id="2dd6c-142">سيتم استخدام النموذج **"‏N-1" مع AX 2012 R3** عندما تكون جميع المتاجر لديك من متاجر الإصدار القديم Dynamics AX 2012 R3، وترغب في استخدام Dynamics 365 Commerce.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-142">The **“N-1” with AX 2012 R3** pattern would be used when all your stores are legacy Dynamics AX 2012 R3 version stores and you want to use Dynamics 365 Commerce.</span></span> <span data-ttu-id="2dd6c-143">وتعد هذه الإصدارات إصدارات المتجر القديمة التي ستتصل بخادم البيع بالتجزئة، لكنك ستستخدم Microsoft Cloud لعمليات Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-143">These versions are the old store versions that will communicate with the Retail server, but you'll use Microsoft Cloud for Dynamics 365 operations.</span></span> 

<span data-ttu-id="2dd6c-144">تعرض الصورة التالية النموذج **"‏N-1" مع AX2012 R3**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-144">The following image shows the **“N-1” with AX 2012 R3** pattern.</span></span> 

![الرسم التخطيطي للنموذج N - 1 مع A X 2012 R 3 في Dynamics 365 Commerce.](../media/n1-ax2012r3.png) 

## <a name="multi-geo-cloud-topology"></a><span data-ttu-id="2dd6c-146">مخطط المجموعة متعددة المناطق</span><span class="sxs-lookup"><span data-stu-id="2dd6c-146">Multi-geo cloud topology</span></span>
   
<span data-ttu-id="2dd6c-147">يعد أول السيناريوهات الأكثر تقدماً هو **مخطط المجموعة متعددة المناطق**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-147">The first of the more advanced scenarios is the **Multi-geo cloud topology**.</span></span> <span data-ttu-id="2dd6c-148">عندما تقوم أولاً بإنشاء إحدى البيئات، إذا كانت مؤسستك تنتشر عبر مواقع عدة حول العالم، فمن الضروري أن تمتلك القدرة على إنشاء وحدات Commerce Scale Units (‏CSU) التي تتسم بالطابع المحلي بشكل أكبر للأماكن التي تقع بها مجموعات المتاجر لديك.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-148">When you first generate an environment, if your enterprise is spread throughout multiple locations worldwide, it is crucial to be able to generate Commerce Scale Units (CSU) that are more localized to where your store clusters are located.</span></span> <span data-ttu-id="2dd6c-149">سيظل المقر الرئيسي في موقع واحد، لذلك من المحتمل أن يحدث بعض التأخير في مكالمات الوقت الحقيقي لديك، لكن ستلحظ تحسناً كبيراً في التشغيل في التعاملات الأكثر شيوعاً لديك وفي الأنشطة التجارية اليومية.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-149">Your headquarters will still be in one location, so your real-time calls will potentially have some latency, but you will notice significant operational improvement in your most common transactions and daily business activities.</span></span>

<span data-ttu-id="2dd6c-150">تعرض الصورة التالية مثالاً على **مخطط المجموعة متعددة المناطق**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-150">The following image shows an example of a **CSU multi-geo cloud topology**.</span></span>

![الرسم التخطيطي لمخطط المجموعة متعددة المناطق لوحدات Dynamics 365 Commerce Scale Unit.](../media/multi-geo-cloud-topology.png) 
 
## <a name="lbd--local-business-data"></a><span data-ttu-id="2dd6c-152">LBD – البيانات المحلية للشركة</span><span class="sxs-lookup"><span data-stu-id="2dd6c-152">LBD – Local business data</span></span>

<span data-ttu-id="2dd6c-153">يتم استخدام نموذج **LBD – البيانات المحلية للشركة** للحلول المحلية.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-153">The **LBD – Local business data** pattern is used for on-premises solutions.</span></span> <span data-ttu-id="2dd6c-154">يستخدم هذا النموذج نسيج الخدمة لمنحك بيئة متكاملة مزودة بكل الميزات للسيناريو المحلي، وذلك عندما يكون لديك مجموعة متنوعة من الأجهزة الظاهرية ولديك القدرة على التعامل مع المشكلات في الفرع الرئيسي، والوصول إلى مقراتك الرئيسية، ولديك القدرة على استخدام Retail Store Scale Unit أو وحدة Commerce Scale Unit (فيما سبق).</span><span class="sxs-lookup"><span data-stu-id="2dd6c-154">This pattern uses the service fabric to give you a full environment with all the features of an on-premises scenario, where you have a variety of virtual machines, the ability to handle issues at the head office, access to your headquarters, and the ability to use the (formerly) Retail Store Scale Unit or Commerce Scale Unit.</span></span>

<span data-ttu-id="2dd6c-155">تعرض الصورة التالية نموذج **البيانات المحلية للشركة**.</span><span class="sxs-lookup"><span data-stu-id="2dd6c-155">The following image shows the **Local business data** pattern.</span></span>


![الرسم التخطيطي لنموذج البيانات المحلية للشركة في Dynamics 365 Commerce.](../media/local-business-data-pattern.png)

