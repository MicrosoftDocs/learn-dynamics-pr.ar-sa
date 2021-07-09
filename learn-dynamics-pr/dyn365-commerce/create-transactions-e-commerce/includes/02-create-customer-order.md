---
ms.openlocfilehash: 1abc5acf409399c6ab7954e2862e22cb5dd87a49
ms.sourcegitcommit: 4ce9caef7d38158f172e82412bc70ae36883e42f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "6070425"
---
<span data-ttu-id="b5146-101">لإنشاء أوامر العميل الخاصة بالتجارة الإلكترونية (عملية الانتقاء والشحن)، اتبع الإجراء التالي:</span><span class="sxs-lookup"><span data-stu-id="b5146-101">To create an e-Commerce customer order (pick-up and ship), follow this procedure:</span></span>

1. <span data-ttu-id="b5146-102">انتقل إلى موقع التجارة الإلكترونية باتباع الارتباط في Microsoft Dynamics365 Lifecycle Services، في علامة التبويب **التجارة الإلكترونية**.</span><span class="sxs-lookup"><span data-stu-id="b5146-102">Go to the e-Commerce site by following the link in Microsoft Dynamics 365 Lifecycle Services, in the **e-Commerce** tab.</span></span>
2. <span data-ttu-id="b5146-103">انتقل إلى صفحة المنتج، وحدد متغير المنتج، ثم حدد الزر **إضافة إلى الحقيبة**.</span><span class="sxs-lookup"><span data-stu-id="b5146-103">Go to a product page, select a product variant, and then select the **Add to bag** button.</span></span> 
3. <span data-ttu-id="b5146-104">انتقل إلى صفحة منتج مختلف، وحدد متغير المنتج، ثم حدد الزر **إضافة إلى الحقيبة**.</span><span class="sxs-lookup"><span data-stu-id="b5146-104">Go to a different product page, select a product variant, and then select the **Add to bag** button.</span></span>

    <span data-ttu-id="b5146-105">[![لقطه شاشه للإجراء "إضافة إلى الحقيبة" في Dynamics 365 Commerce](../media/add-to-bag-ss.jpg)](../media/add-to-bag-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b5146-105">[ ![Screenshot of the Add to bag action in Dynamics 365 Commerce.](../media/add-to-bag-ss.jpg) ](../media/add-to-bag-ss.jpg#lightbox)</span></span>
    
4. <span data-ttu-id="b5146-106">حدد أحد المنتجات للاختيار.</span><span class="sxs-lookup"><span data-stu-id="b5146-106">Select one of the products for pickup.</span></span> <span data-ttu-id="b5146-107">في مربع الحوار **تحديد متجر**، أدخل المتجر الذي يمكن انتقاء البضائع فيه، ثم حدد زر **البحث**.</span><span class="sxs-lookup"><span data-stu-id="b5146-107">In the **Select a store** dialog box, enter the store where the goods can be picked up and then select the **Search** button.</span></span> <span data-ttu-id="b5146-108">في قائمة النتائج، ابحث عن المتجر الذي تريده للاختيار، ثم حدد **اختيار هنا**.</span><span class="sxs-lookup"><span data-stu-id="b5146-108">In the list of results, find the store that you want for the pickup and then select **Pick up here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b5146-109">تعتمد المتاجر التي يمكنك تحديدها لانتقاء الأمر في نقطة البيع على تكوين **تعيين مجموعة التنفيذ** على المتجر على الإنترنت المرتبط بموقع التجارة الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="b5146-109">The stores that you will be able to select for picking up the order at POS depend on the **Fulfillment group assignment** configuration on the online store that is related to the e-Commerce site.</span></span> 
 
<span data-ttu-id="b5146-110">يمكن شحن الصنف الآخر إلى أحد العناوين.</span><span class="sxs-lookup"><span data-stu-id="b5146-110">The other item can be shipped to an address.</span></span>

5. <span data-ttu-id="b5146-111">حدد **السداد**.</span><span class="sxs-lookup"><span data-stu-id="b5146-111">Select **Checkout**.</span></span>

    <span data-ttu-id="b5146-112">[![لقطة شاشة لإجراء السداد في Dynamics 365 Commerce](../media/checkout-ss.jpg)](../media/checkout-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b5146-112">[ ![Screenshot of the Checkout action in Dynamics 365 Commerce.](../media/checkout-ss.jpg) ](../media/checkout-ss.jpg#lightbox)</span></span>
    
6. <span data-ttu-id="b5146-113">قم بتسجيل الدخول إلى حساب العميل أو حدد **تسجيل** لإنشاء حساب عميل جديد، إذا لم يكن لديك حساب بالفعل.</span><span class="sxs-lookup"><span data-stu-id="b5146-113">Sign in to your customer account or select **Sign up** to create a new customer account, if you don’t already have one.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="b5146-114">يمكن إنشاء الأوامر ومعالجتها للاختيار والشحن كضيف وكعميل مسجل للدخول، سواء كعميل موجود، أو عند قيامك بإنشاء حساب عميل جديد اثناء إنشاء أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="b5146-114">You can create and process orders for pick-up and for shipping as a Guest and as a signed-in customer, either as an existing customer or when you are creating a new customer account during the creation of the order.</span></span>
    
    ![لقطة شاشة لصفحة تسجيل الدخول في Dynamics 365 Commerce.](../media/sign-in-ss.jpg) 
    
7. <span data-ttu-id="b5146-116">سيؤدي التسجيل إلى إرسال رمز تحقق إلى عنوان البريد الكتروني الذي قمت بتقديمه.</span><span class="sxs-lookup"><span data-stu-id="b5146-116">Signing up will send a verification code to the email address that you provide.</span></span> <span data-ttu-id="b5146-117">قم بتسجيل الدخول إلى حسابك الجديد على الموقع باستخدام رمز التحقق هذا.</span><span class="sxs-lookup"><span data-stu-id="b5146-117">Sign in to your new account on the site by using this verification code.</span></span> 
8. <span data-ttu-id="b5146-118">أثناء وجود الأمر الخاص بك قيد التقدم، قم بملء الجزء **عنوان الشحن**، ثم حدد **حفظ ومتابعة**.</span><span class="sxs-lookup"><span data-stu-id="b5146-118">On your order in process, fill out the **Shipping Address** section and then select **Save & continue**.</span></span>
9. <span data-ttu-id="b5146-119">حدد نمط التسليم، ثم حدد **حفظ ومتابعة**.</span><span class="sxs-lookup"><span data-stu-id="b5146-119">Select a delivery mode and then select **Save & continue**.</span></span>

    <span data-ttu-id="b5146-120">[ ![لقطة شاشة للإجراء حفظ ومتابعة في Dynamics 365 Commerce.](../media/save-continue-ss.jpg) ](../media/save-continue-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b5146-120">[ ![Screenshot of the Save & continue action in Dynamics 365 Commerce.](../media/save-continue-ss.jpg) ](../media/save-continue-ss.jpg#lightbox)</span></span>
    
10. <span data-ttu-id="b5146-121">املأ طريقة الدفع.</span><span class="sxs-lookup"><span data-stu-id="b5146-121">Fill out the payment method.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="b5146-122">بالنسبة لأغراض الاختبار، يمكنك استخدام أي اسم واستخدام رقم بطاقة الائتمان 4111 1111 1111 1111بتاريخ انتهاء صلاحية 10/20 CVC 737.</span><span class="sxs-lookup"><span data-stu-id="b5146-122">For testing purposes, you can use any name and use credit card number 4111 1111 1111 1111 expiry 10/20 CVC 737.</span></span>
    > <span data-ttu-id="b5146-123">لا تستخدم أبداً معلومات بطاقة الائتمان الفعلية في موقع الاختبار.</span><span class="sxs-lookup"><span data-stu-id="b5146-123">Never use actual credit card information on the test site.</span></span>
    
11. <span data-ttu-id="b5146-124">قم بتقديم عنوان بريد الكتروني في الحقل **معلومات جهة الاتصال** ثم حدد **وضع الأمر**.</span><span class="sxs-lookup"><span data-stu-id="b5146-124">Provide an email address in the **Contact information** field and then select **Place order**.</span></span> <span data-ttu-id="b5146-125">ستتلقى رسالة تأكيد بالبريد الكتروني بعد وضع الأمر.</span><span class="sxs-lookup"><span data-stu-id="b5146-125">You will receive a confirmation email after placing the order.</span></span>

    <span data-ttu-id="b5146-126">[ ![لقطة شاشة للإجراء وضع الأمر في Dynamics 365 Commerce.](../media/place-order-ss.jpg) ](../media/place-order-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b5146-126">[ ![Screenshot of the Place order action in Dynamics 365 Commerce.](../media/place-order-ss.jpg) ](../media/place-order-ss.jpg#lightbox)</span></span>
    
<span data-ttu-id="b5146-127">سيعرض هذا الموقع صفحة **تأكيد الأمر**.</span><span class="sxs-lookup"><span data-stu-id="b5146-127">The site will show an **Order Confirmation** page.</span></span>

 <span data-ttu-id="b5146-128">[ ![لقطة شاشة لصفحة تأكيد الأمر Dynamics 365 Commerce.](../media/order-confirmation-ss.jpg) ](../media/order-confirmation-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b5146-128">[ ![Screenshot of the Order confirmation page Dynamics 365 Commerce.](../media/order-confirmation-ss.jpg) ](../media/order-confirmation-ss.jpg#lightbox)</span></span> 

<span data-ttu-id="b5146-129">لعرض الحركة في المقر التجاري (‏HQ)، قم بتشغيل المهمة **P 0001** و **مزامنة الأوامر** لسحب الأوامر من Commerce scale units.</span><span class="sxs-lookup"><span data-stu-id="b5146-129">To view the transaction in Commerce Headquarters (HQ), run the **P-0001** job and **Synchronize Orders** to pull in the orders from the Commerce scale units.</span></span>

1. <span data-ttu-id="b5146-130">في المقر التجاري HQ، انتقل إلى **البيع بالتجزئة والتجارة >تكنولوجيا المعلومات(IT) بالتجزئة والتجارة > جدولة التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="b5146-130">In Commerce HQ, go to **Retail and Commerce > Retail and Commerce IT > Distribution schedule**.</span></span>
2. <span data-ttu-id="b5146-131">حدد المهمة **P-0001**، ثم حدد **تشغيل الآن**.</span><span class="sxs-lookup"><span data-stu-id="b5146-131">Select the **P-0001** job and then select **Run now**.</span></span>

 <span data-ttu-id="b5146-132">[![لقطة شاشة للوظيفة "التشغيل الآن" والمهمة "P-0001" Dynamics 365 Commerce. ](../media/run-now-job-ss.jpg)](../media/run-now-job-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b5146-132">[ ![Screenshot of the Run now and P-0001 job Dynamics 365 Commerce.](../media/run-now-job-ss.jpg) ](../media/run-now-job-ss.jpg#lightbox)</span></span>
 
3. <span data-ttu-id="b5146-133">في Commerce HQ، انتقل إلى **البيع بالتجزئة والتجارة >تكنولوجيا المعلومات (IT) بالتجزئة والتجارة > مزامنة الأوامر**.</span><span class="sxs-lookup"><span data-stu-id="b5146-133">In Commerce HQ, go to **Retail and Commerce > Retail and Commerce IT > Synchronize Orders**.</span></span>
4. <span data-ttu-id="b5146-134">حدد القناة التي تعمل بها على الإنترنت وقم بإضافتها إلى **عُقد المؤسسة المحددة**.</span><span class="sxs-lookup"><span data-stu-id="b5146-134">Select the online channel that you are working with and add it to the **SELECTED ORGANIZATION NODES**.</span></span>
5. <span data-ttu-id="b5146-135">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b5146-135">Select **OK**.</span></span>
6. <span data-ttu-id="b5146-136">ابحث عن **حركات المتجر على الإنترنت** للبحث عن الأمر في **قائمة الحركات**.</span><span class="sxs-lookup"><span data-stu-id="b5146-136">Search for **Online store transactions** to find the order in the **Transaction list**.</span></span> <span data-ttu-id="b5146-137">يجب أن تكون قادراً على مطابقه التاريخ والوقت ورسوم الأمر بالنسبة للأمر الذي قمت بإنشائه على الموقع.</span><span class="sxs-lookup"><span data-stu-id="b5146-137">You should be able to match the date, time, and order charge to the order that you created on the site.</span></span>

> [!NOTE]
> <span data-ttu-id="b5146-138">يتم تنفيذ تشغيل المهمة **P-0001** و **مزامنة الأوامر** عن طريق مهام الدفعات في سيناريوهات الحياة الحقيقية.</span><span class="sxs-lookup"><span data-stu-id="b5146-138">Running the **P-0001** job and **Synchronize orders** is performed by batch jobs in real-life scenarios.</span></span> <span data-ttu-id="b5146-139">يتم تضمين هذه الخطوات في هذا التدريب بغرض استيعاب العملية.</span><span class="sxs-lookup"><span data-stu-id="b5146-139">These steps are included in this exercise for the purpose of understanding the process.</span></span>

<span data-ttu-id="b5146-140">شاهد الفيديو التالي للتعرف على كيفيه إنشاء طلب عميل خاص بالتجارة الإلكترونية من خلال عملية السداد للضيف.</span><span class="sxs-lookup"><span data-stu-id="b5146-140">Watch the following video to learn how to create an e-Commerce customer order with a guest checkout.</span></span> 

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4AJHT] 


