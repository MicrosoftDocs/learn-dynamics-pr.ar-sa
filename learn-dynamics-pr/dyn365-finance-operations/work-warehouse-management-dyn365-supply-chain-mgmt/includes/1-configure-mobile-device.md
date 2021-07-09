---
ms.openlocfilehash: 2ff4974670a2f019ed782596f827dcc265cdba94
ms.sourcegitcommit: f699c9a05571bd0157969b1a0e0f33c3a4790958
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "6073821"
---
<span data-ttu-id="3d153-101">قبل إجراء أي من عمليات Warehouse management باستخدام جهاز محمول، يجب تكوينه لـ Dynamics 365 Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="3d153-101">Before performing any of the Warehouse management processes with a mobile device, you must configure it for Dynamics 365 Supply Chain Management.</span></span>


<span data-ttu-id="3d153-102">المجالات الخمسة الأساسية في الإعداد هي:</span><span class="sxs-lookup"><span data-stu-id="3d153-102">The five basic areas in the setup are:</span></span>

-    <span data-ttu-id="3d153-103">**فئات العمل** - تستخدم لتعريف أنواع أوامر العمل التي يمكن لجهاز المحمول معالجتها.</span><span class="sxs-lookup"><span data-stu-id="3d153-103">**Work classes** - Use to define the types of work orders that a mobile device can process.</span></span>

-    <span data-ttu-id="3d153-104">**قوائم الأجهزة** - تستخدم لتحديد الخيارات المتوفرة والتنقل لتلك الخيارات على كل جهاز.</span><span class="sxs-lookup"><span data-stu-id="3d153-104">**Device menus** - Use to outline which options are available and the navigation for those options on each device.</span></span>

-    <span data-ttu-id="3d153-105">**تخطيط الجهاز** - يسمح لك بتحديد معلومات مثل الخط واللون، وخريطة اختصارات لوحة المفاتيح، وتحديد تنسيق التاريخ لعرضها على الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3d153-105">**Device layout** - Allows you to define information such as font and color, map keyboard shortcuts, and determine the date format to display on the device.</span></span>

-    <span data-ttu-id="3d153-106">**مستخدمو الأجهزة** - يحدد الأشخاص أو العاملين الذين يمكنهم الوصول إلى الأجهزة المحمولة ومستوي الوصول المطلوب.</span><span class="sxs-lookup"><span data-stu-id="3d153-106">**Device users** - Defines the people or workers that can access the mobile devices and what level of access is required.</span></span>

-    <span data-ttu-id="3d153-107">**إعدادات الطباعة** - تتيح لك التحكم في التخطيط، والطابعة، والقالب المراد استخدامه لطباعة التسميات.</span><span class="sxs-lookup"><span data-stu-id="3d153-107">**Print settings** - Allows you to control the layout, printer, and template to be used for printing labels.</span></span>


## <a name="work-classes"></a><span data-ttu-id="3d153-108">فئات العمل</span><span class="sxs-lookup"><span data-stu-id="3d153-108">Work classes</span></span>

<span data-ttu-id="3d153-109">يتم استخدام فئات العمل لتحديد أوامر العمل التي يمكن لجهاز المحمول معالجتها إذا كان صنف القائمة سيقوم بمعالجة العمل الموجود.</span><span class="sxs-lookup"><span data-stu-id="3d153-109">Work classes are used to specify the work orders that a mobile device can process if the menu item will process existing work.</span></span>

![لقطة شاشة لفئات عمل Finance and Operations.](../media/work-classes-ss.png)

<span data-ttu-id="3d153-111">على سبيل المثال، قد يتضمن أمر العمل أوامر شراء أو عمليات التحويل والإيصالات أو التزويد أو أوامر الإرجاع.</span><span class="sxs-lookup"><span data-stu-id="3d153-111">For example, a work order could include purchase orders, transfers and receipts, replenishment, or return orders.</span></span> <span data-ttu-id="3d153-112">سيقوم صنف القائمة فقط بمعالجة العمل الخاص بنوع أمر العمل المحدد.</span><span class="sxs-lookup"><span data-stu-id="3d153-112">The menu item will only process work for the specified type of work order.</span></span>

## <a name="device-menus"></a><span data-ttu-id="3d153-113">قوائم الأجهزة</span><span class="sxs-lookup"><span data-stu-id="3d153-113">Device menus</span></span>

<span data-ttu-id="3d153-114">تحتوي القائمة على أصناف القائمة التي سيستخدمها العاملون في المستودع لتنفيذ عملهم.</span><span class="sxs-lookup"><span data-stu-id="3d153-114">The menu contains the menu items that warehouse workers will use to perform their work.</span></span> <span data-ttu-id="3d153-115">يمكنك إنشاء بنية القائمة الخاصة بالجهاز المحمول عن طريق إضافة أصناف القائمة والقوائم.</span><span class="sxs-lookup"><span data-stu-id="3d153-115">You can create the structure of the mobile device menu by adding menu items and menus.</span></span> <span data-ttu-id="3d153-116">عندما تقوم بإضافة قائمة، يتم تعيين أصناف القائمة الخاصة بها أيضاً.</span><span class="sxs-lookup"><span data-stu-id="3d153-116">When you add a menu, its menu items are also assigned.</span></span>

![لقطة شاشة لقائمة جهاز محمول Finance and Operations.](../media/mobile-menu-ss.png)

<span data-ttu-id="3d153-118">يمكنك تكوين أصناف القائمة من أجل:</span><span class="sxs-lookup"><span data-stu-id="3d153-118">You can configure menu items to:</span></span>

-   <span data-ttu-id="3d153-119">معالجة استعلام أو تنفيذ نشاط، مثل طباعة تسمية أو إنشاء لوحات ترخيص المستخدم أو بدء أمر إنتاج أو البحث بسرعة بين المعلومات الخاصة بالأصناف الموجودة في الموقع.</span><span class="sxs-lookup"><span data-stu-id="3d153-119">Process an inquiry or perform an activity, such as print a label, generate license plate numbers, start a production order, or quickly look up information about items in a location.</span></span>

-   <span data-ttu-id="3d153-120">إنشاء العمل الذي سيتم تنفيذه من خلال عملية أخرى.</span><span class="sxs-lookup"><span data-stu-id="3d153-120">Create work that will be performed through another process.</span></span> <span data-ttu-id="3d153-121">على سبيل المثال، يمكن أن يؤدي استلام صنف لأمر شراء إلى إنشاء عمل استبعاد لعامل آخر.</span><span class="sxs-lookup"><span data-stu-id="3d153-121">For example, receiving an item for a purchase order can create put away work for another worker.</span></span>

-   <span data-ttu-id="3d153-122">تنفيذ العمل الذي تم إنشاؤه بواسطة عملية أخرى.</span><span class="sxs-lookup"><span data-stu-id="3d153-122">Perform work that was created by another process.</span></span> <span data-ttu-id="3d153-123">وهذا يُعرف بالعمل الموجود.</span><span class="sxs-lookup"><span data-stu-id="3d153-123">This is called existing work.</span></span> <span data-ttu-id="3d153-124">على سبيل المثال، تنفيذ عمل الاستبعاد الذي تم إنشاؤه عند استلام صنف لأمر شراء.</span><span class="sxs-lookup"><span data-stu-id="3d153-124">For example, performing put away work that was created when an item was received for a purchase order.</span></span>

<span data-ttu-id="3d153-125">يتم تكوين أصناف القائمة التي تظهر على قوائم الجهاز المحمول الخاصة بالمستودع في صفحة **أصناف قائمة الجهاز المحمول**.</span><span class="sxs-lookup"><span data-stu-id="3d153-125">The menu items that appear on a warehouse mobile device's menus are configured on the **Mobile device menu items** page.</span></span> <span data-ttu-id="3d153-126">نظراً لأنه يمكن وضع أصناف القائمة في قوائم مختلفة، فإنه من السهل تكوين بنية القائمة بحيث يتم عرض أنواع معينة فقط من العمل لمستخدمين بعينهم.</span><span class="sxs-lookup"><span data-stu-id="3d153-126">Because the menu items can be put onto different menus, it's simple to configure menu structures so that only specific types of work are exposed to specific users.</span></span> 

## <a name="device-users"></a><span data-ttu-id="3d153-127">مستخدمو الأجهزة</span><span class="sxs-lookup"><span data-stu-id="3d153-127">Device users</span></span> 

<span data-ttu-id="3d153-128">يتعين عليك إعداد حساب مستخدم لعامل مستودع للوصول إلى جهاز محمول.</span><span class="sxs-lookup"><span data-stu-id="3d153-128">You need to set up a user account for a warehouse worker to access a mobile device.</span></span> <span data-ttu-id="3d153-129">يتضمن هذا إعداد عامل كمستخدم عمل، وتحديد قوائم الأجهزة المحمولة التي يمكن للعامل الوصول إليها، وتحديد معلومات تسجيل الدخول الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="3d153-129">This involves setting up a worker as a work user, selecting the mobile device menus that the worker can access, and specifying their sign-on information.</span></span>

<span data-ttu-id="3d153-130">يمكنك إنشاء العديد من مستخدمي العمل لكل عامل إذا كانوا بحاجة إلى الاطلاع والحصول على أذونات مختلفة في مواقع مختلفة.</span><span class="sxs-lookup"><span data-stu-id="3d153-130">You can create multiple work users for each worker if they'll need to see and have different permissions in different locations.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE41Cjs]


## <a name="print-settings-for-labels"></a><span data-ttu-id="3d153-131">إعدادات الطباعة للتسميات</span><span class="sxs-lookup"><span data-stu-id="3d153-131">Print settings for labels</span></span>

<span data-ttu-id="3d153-132">يمكن إعداد أصناف قائمة الجهاز المحمول التي تمكن العاملين من استخدام الجهاز المحمول الخاص بهم لطباعة التسميات أو إعادة طباعتها.</span><span class="sxs-lookup"><span data-stu-id="3d153-132">You can set up the mobile device menu items that enable workers to use their mobile device to print or reprint labels.</span></span> <span data-ttu-id="3d153-133">الجزء المهم من عملية المستودع هو طباعة التسميات للأصناف التي يتم استلامها بحيث يمكن التعرف عليها باستخدام ماسح ضوئي للاستخدام في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="3d153-133">An important part of the warehouse process is the printing of labels for the items that are received so that they can be identified with a scanner for future use.</span></span>
<span data-ttu-id="3d153-134">يتم عادةً إجراء الطباعة عند إكمال العمل، مثل الانتقاء والاستلام.</span><span class="sxs-lookup"><span data-stu-id="3d153-134">Printing is typically done as you complete work, such as picking and receiving.</span></span>


## <a name="install-and-configure-supply-chain-management---warehousing"></a><span data-ttu-id="3d153-135">تثبيت Supply Chain Management وتكوينها - التخزين‬</span><span class="sxs-lookup"><span data-stu-id="3d153-135">Install and configure Supply Chain Management - Warehousing</span></span>

<span data-ttu-id="3d153-136">**Supply Chain Management - التخزين** هو أحد التطبيقات المتوفرة على متجر Google play ومتجر Windows.</span><span class="sxs-lookup"><span data-stu-id="3d153-136">**Supply Chain Management - Warehousing** is an application that is available on Google Play Store and Windows Store.</span></span> <span data-ttu-id="3d153-137">يتم توفير هذا التطبيق كمكون مستقل، وهو ما يعني التوزيع الذاتي على الأجهزة التي يتم استخدامها لمهام المستودع.</span><span class="sxs-lookup"><span data-stu-id="3d153-137">This app is provided as a standalone component, which means self-deployment on devices that are used for warehouse tasks.</span></span>

<span data-ttu-id="3d153-138">لاستخدام التطبيق في بيئة Supply Chain Management، يجب تنزيل التطبيق على كل جهاز وتكوينه للاتصال بالبيئة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="3d153-138">To use the app in your Supply Chain Management environment, you must download the app on each device and configure it to connect to your environment.</span></span> 

## <a name="create-a-web-service-application-in-azure-active-directory"></a><span data-ttu-id="3d153-139">قم بإنشاء تطبيق خدمة الويب في Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3d153-139">Create a web service application in Azure Active Directory</span></span>

<span data-ttu-id="3d153-140">لتمكين التطبيق من التفاعل مع خادم Supply Chain Management المحدد، يجب تسجيل تطبيق خدمة ويب في Azure Active Directory (Azure AD) من Microsoft للمستأجر.</span><span class="sxs-lookup"><span data-stu-id="3d153-140">To enable the app to interact with a specific Supply Chain Management server, you must register a web service application in a Microsoft Azure Active Directory (Azure AD) for the tenant.</span></span> <span data-ttu-id="3d153-141">لأسباب تتعلق بالأمان، نوصي بإنشاء تطبيق خدمة ويب لكل جهاز تستخدمه.</span><span class="sxs-lookup"><span data-stu-id="3d153-141">For security reasons, we recommend that you create a web service application for each device that you use.</span></span> <span data-ttu-id="3d153-142">لإنشاء تطبيق خدمة ويب في Azure AD، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="3d153-142">To create a web service application in Azure AD, complete the following steps:</span></span>

1.  <span data-ttu-id="3d153-143">في مستعرض الويب، انتقل إلى <https://portal.azure.com>.</span><span class="sxs-lookup"><span data-stu-id="3d153-143">In a web browser, go to <https://portal.azure.com>.</span></span>

2.  <span data-ttu-id="3d153-144">أدخل الاسم وكلمة المرور للمستخدم الذي لديه حق الوصول إلى اشتراك Azure.</span><span class="sxs-lookup"><span data-stu-id="3d153-144">Enter the name and password for the user who has access to the Azure subscription.</span></span>

3.  <span data-ttu-id="3d153-145">في مدخل Azure، في جزء التنقل الأيمن، حدد **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="3d153-145">In Azure portal, in the left navigation pane, select **Azure Active Directory**.</span></span>

4.  <span data-ttu-id="3d153-146">تأكد من أن مثيل خدمة Active Directory هو نفسه الذي تستخدمه Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="3d153-146">Ensure that the Active Directory instance is the one that is used by Supply Chain Management.</span></span>

5.  <span data-ttu-id="3d153-147">في القائمة، حدد **تسجيلات التطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="3d153-147">In the list, select **App registrations**.</span></span>

6.  <span data-ttu-id="3d153-148">في الجزء العلوي، حدد **تسجيل تطبيق جديد**.</span><span class="sxs-lookup"><span data-stu-id="3d153-148">In the top pane, select **New application registration**.</span></span> <span data-ttu-id="3d153-149">يبدأ تشغيل معالج إضافة التطبيق.</span><span class="sxs-lookup"><span data-stu-id="3d153-149">The Add application wizard starts.</span></span>

    ![لقطة شاشة لتسجيلات تطبيق Azure Active Directory من Microsoft.](../media/azure-1-ssm.png)


7.  <span data-ttu-id="3d153-151">أدخل اسماً للتطبيق وحدد **تطبيق ويب/API الويب**.</span><span class="sxs-lookup"><span data-stu-id="3d153-151">Enter a name for the application and select **Web application/web API**.</span></span> <span data-ttu-id="3d153-152">أدخل **عنوان URL لتسجيل الدخول**، وهو عنوان URL الخاص بتطبيق الويب الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="3d153-152">Enter the **sign-on URL**, which is your web app URL.</span></span> <span data-ttu-id="3d153-153">عنوان URL هذا هو نفس عنوان URL الخاص بالتوزيع، ولكن يتم إضافة "oauth" إلى النهاية.</span><span class="sxs-lookup"><span data-stu-id="3d153-153">This URL is the same as your deployment URL, but "oauth" is added to the end.</span></span>


8.  <span data-ttu-id="3d153-154">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="3d153-154">Select **Create**.</span></span>

9. <span data-ttu-id="3d153-155">حدد التطبيق الجديد في القائمة.</span><span class="sxs-lookup"><span data-stu-id="3d153-155">Select the new app in the list.</span></span> 

10. <span data-ttu-id="3d153-156">تذكر **معرف التطبيق**؛ ستحتاجه لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="3d153-156">Remember the **Application ID**; you will need it later.</span></span> <span data-ttu-id="3d153-157">ستتم الإشارة إلى **معرف التطبيق** لاحقاً على أنه **معرف العميل**.</span><span class="sxs-lookup"><span data-stu-id="3d153-157">The **Application ID** will later be referred to as the **Client ID**.</span></span>

11. <span data-ttu-id="3d153-158">حدد **مفاتيح** في جزء الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="3d153-158">Select **Keys** in the Settings pane.</span></span> <span data-ttu-id="3d153-159">قم بإنشاء مفتاح عن طريق إدخال وصف المفتاح والمدة في **كلمات المرور** .</span><span class="sxs-lookup"><span data-stu-id="3d153-159">Create a key by entering a key description and a duration in the **Passwords** section.</span></span>

12. <span data-ttu-id="3d153-160">حدد **حفظ** وانسخ المفتاح.</span><span class="sxs-lookup"><span data-stu-id="3d153-160">Select **Save** and copy the key.</span></span> <span data-ttu-id="3d153-161">ستتم الإشارة إلى هذا المفتاح لاحقاً باعتباره **سر العميل**.</span><span class="sxs-lookup"><span data-stu-id="3d153-161">This key will later be referred to as the **Client secret**.</span></span> 

## <a name="create-and-configure-a-user-account-in-supply-chain-management"></a><span data-ttu-id="3d153-162">إنشاء حساب مستخدم وتكوينه في Supply Chain Management</span><span class="sxs-lookup"><span data-stu-id="3d153-162">Create and configure a user account in Supply Chain Management</span></span>

<span data-ttu-id="3d153-163">يمكنك إنشاء حساب مستخدم لـ Supply Chain Management التي تتوافق مع بيانات اعتماد مستخدم التطبيق الذي يتم تخزينه.</span><span class="sxs-lookup"><span data-stu-id="3d153-163">You can create a Supply Chain Management user account that corresponds to the warehousing app user credentials.</span></span> <span data-ttu-id="3d153-164">بعد ذلك، يمكنك إقران تطبيق Azure AD الخاص بك مع مستخدم التطبيق الذي يتم تخزينه.</span><span class="sxs-lookup"><span data-stu-id="3d153-164">Then, you can associate your Azure AD application with the warehousing app user.</span></span>

<span data-ttu-id="3d153-165">لتمكين Supply Chain Management لاستخدام تطبيق Azure AD الخاص بك، أكمل خطوات التكوين التالية:</span><span class="sxs-lookup"><span data-stu-id="3d153-165">To enable Supply Chain Management to use your Azure AD application, complete the following configuration steps:</span></span>

1.  <span data-ttu-id="3d153-166">في Supply Chain Management، انتقل إلى **> إدارة النظام > شائع > المستخدمون**.</span><span class="sxs-lookup"><span data-stu-id="3d153-166">In Supply Chain Management, go to **System administration > Common > Users**.</span></span>

2.  <span data-ttu-id="3d153-167">إنشاء مستخدم جديد.</span><span class="sxs-lookup"><span data-stu-id="3d153-167">Create a new user.</span></span>

3.  <span data-ttu-id="3d153-168">قم بتعيين مستخدم **جهاز محمول المستودع**.</span><span class="sxs-lookup"><span data-stu-id="3d153-168">Assign the **Warehouse mobile device** user.</span></span> 

    ![تم توسيع لقطة الشاشة لأدوار المستخدم لإظهار دور مستخدم الجهاز المحمول الخاص بالمستودع.](../media/mobile-user-ss.png)

4.  <span data-ttu-id="3d153-170">في Supply Chain Management، انتقل إلى **إدارة النظام > إعداد > تطبيقات Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="3d153-170">In Supply Chain Management, go to **System administration > Setup > Azure Active Directory applications**.</span></span>

5.  <span data-ttu-id="3d153-171">إنشاء سطر جديد.</span><span class="sxs-lookup"><span data-stu-id="3d153-171">Create a new line.</span></span>

6.  <span data-ttu-id="3d153-172">أدخل **معرف العميل** (الذي تم الحصول عليه في القسم الأخير)، وأعطه اسماً وحدد المستخدم الذي تم إنشاؤه مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="3d153-172">Enter the **Client ID** (obtained in the last section), give it a name, and select the previously created user.</span></span> <span data-ttu-id="3d153-173">نوصي بوضع علامات على كافة الأجهزة بحيث يمكنك إزالة حق وصولهم بسهوله لـ Supply Chain Management من هذه الصفحة في حاله فقدهم.</span><span class="sxs-lookup"><span data-stu-id="3d153-173">We recommend that you tag all your devices so that you can easily remove their access to Supply Chain Management from this page in case they are lost.</span></span> 


## <a name="configure-the-application"></a><span data-ttu-id="3d153-174">تكوين التطبيق</span><span class="sxs-lookup"><span data-stu-id="3d153-174">Configure the application</span></span>

<span data-ttu-id="3d153-175">يجب تكوين التطبيق على الجهاز للاتصال بخادم Supply Chain Management من خلال تطبيق Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3d153-175">You must configure the app on the device to connect to the Supply Chain Management server through the Azure AD application.</span></span> <span data-ttu-id="3d153-176">للقيام بذلك، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="3d153-176">To do this, complete the following steps:</span></span>

1.  <span data-ttu-id="3d153-177">في التطبيق، انتقل إلى إعدادات **اتصال**.</span><span class="sxs-lookup"><span data-stu-id="3d153-177">In the app, go to **Connection** settings.</span></span>

2.  <span data-ttu-id="3d153-178">قم بمسح حقل **وضع العرض التوضيحي**.</span><span class="sxs-lookup"><span data-stu-id="3d153-178">Clear the **Demo mode** field.</span></span>

    ![لقطة شاشة لإعدادات اتصال تطبيق الأجهزة المحمولة.](../media/mobile-app-1-ss.png)

3.  <span data-ttu-id="3d153-180">أدخل المعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="3d153-180">Enter the following information:</span></span>

    -   <span data-ttu-id="3d153-181">**معرف عميل Azure Active directory** - يتم الحصول على معرف العميل في الخطوة 11 في قسم إنشاء تطبيق خدمة ويب في Active directory.</span><span class="sxs-lookup"><span data-stu-id="3d153-181">**Azure Active directory client ID** - The client ID is obtained in step 11 in the Create a web service application in Active Directory section.</span></span>

    -   <span data-ttu-id="3d153-182">**سر عميل Azure Active directory** - يتم الحصول على سر العميل في الخطوة 13 في قسم إنشاء تطبيق خدمة ويب في Active directory.</span><span class="sxs-lookup"><span data-stu-id="3d153-182">**Azure Active directory client secret** - The client secret is obtained in step 13 in the Create a web service application in Active Directory section.</span></span>

    -   <span data-ttu-id="3d153-183">**مورد Azure Active directory** - يصور مورد دليل Azure AD عنوان URL لجذر Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="3d153-183">**Azure Active directory resource** - The Azure AD directory resource depicts the Supply Chain Management root URL.</span></span> <span data-ttu-id="3d153-184">ملاحظة: لا تنهي هذا الحقل بحرف الخط المائل للأمام (/).</span><span class="sxs-lookup"><span data-stu-id="3d153-184">Note: Do not end this field with a forward slash character (/).</span></span>

    -   <span data-ttu-id="3d153-185">**مستأجر Azure Active directory** - مستأجر دليل Azure AD المستخدم مع خادم Supply Chain Management: https:\//login.windows.net/your-AD-tenant-ID.</span><span class="sxs-lookup"><span data-stu-id="3d153-185">**Azure Active directory tenant** - The Azure AD directory tenant that is used with the Supply Chain Management server: https:\//login.windows.net/your-AD-tenant-ID.</span></span> <span data-ttu-id="3d153-186">على سبيل المثال: https:\//login.windows.net/contosooperations.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="3d153-186">For example: https:\//login.windows.net/contosooperations.onmicrosoft.com.</span></span> <span data-ttu-id="3d153-187">لا تنهِ حقل **URL** بحرف الخط المائل للأمام (/).</span><span class="sxs-lookup"><span data-stu-id="3d153-187">Do not end the **URL** field with a forward slash character (/).</span></span>

    -   <span data-ttu-id="3d153-188">**الشركة** - إدخال الكيان القانوني في Supply Chain Management التي ترغب في إجراء اتصال التطبيق بها.</span><span class="sxs-lookup"><span data-stu-id="3d153-188">**Company** - Enter the legal entity in Supply Chain Management to which you want the application to connect.</span></span>


4.  <span data-ttu-id="3d153-189">حدد الزر **"رجوع"** الموجود في الركن العلوي الأيمن من التطبيق.</span><span class="sxs-lookup"><span data-stu-id="3d153-189">Select the **Back** button in the top-left corner of the application.</span></span> <span data-ttu-id="3d153-190">سيقوم التطبيق الآن بالاتصال بخادم Finance and Operations الخاص بك وسيتم عرض شاشه تسجيل الدخول للعامل في المستودع.</span><span class="sxs-lookup"><span data-stu-id="3d153-190">The application will now connect to your Finance and Operations server and the login screen for the warehouse worker will display.</span></span> 

## <a name="mass-deployment-for-warehouse-mobile-app"></a><span data-ttu-id="3d153-191">التوزيع الجماعي لـ Warehouse mobile app</span><span class="sxs-lookup"><span data-stu-id="3d153-191">Mass deployment for Warehouse mobile app</span></span>

<span data-ttu-id="3d153-192">غالباً ما تكون هذه عملية معقدة لتوزيع إعدادات الاتصال على هؤلاء المستخدمين الذين سيستخدمون تطبيق المستودع.</span><span class="sxs-lookup"><span data-stu-id="3d153-192">Often, it is a complex process to distribute connection settings to those users who will be using the Warehouse application.</span></span> <span data-ttu-id="3d153-193">لاستخدام هذه العملية، يمكن توزيع هذه الإعدادات بشكل شامل للأفراد المتأثرين باستخدام أداة التوزيع مثل Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3d153-193">To alleviate this process, those settings can be silently mass deployed to affected personnel using a deployment tool such as Microsoft Intune.</span></span> <span data-ttu-id="3d153-194">بالإضافة إلى التوزيع، يمكن لهذه الأداة أيضاً أن تحتوي على الأجهزة المحمولة الخاصة بمستودع الخدمة.</span><span class="sxs-lookup"><span data-stu-id="3d153-194">Along with deployment, this tool can also service warehouse mobile devices.</span></span> <span data-ttu-id="3d153-195">لمزيد من التفاصيل حول هذا، انتقل إلى [https://docs.microsoft.com/mem/intune/apps/apps-windows-10-app-deploy](https://docs.microsoft.com/mem/intune/apps/apps-windows-10-app-deploy "التوزيع الجماعي باستخدام Microsoft Intune")</span><span class="sxs-lookup"><span data-stu-id="3d153-195">For more details on this go to [https://docs.microsoft.com/mem/intune/apps/apps-windows-10-app-deploy](https://docs.microsoft.com/mem/intune/apps/apps-windows-10-app-deploy "Mass deployment with Microsoft Intune")</span></span>  

## <a name="scan-bar-codes-by-using-a-camera-in-supply-chain-management"></a><span data-ttu-id="3d153-196">مسح الرموز الشريطية ضوئياً باستخدام كاميرا في Supply Chain Management</span><span class="sxs-lookup"><span data-stu-id="3d153-196">Scan bar codes by using a camera in Supply Chain Management</span></span>

<span data-ttu-id="3d153-197">في **إعدادات العرض** الخاصة بالتطبيق الذي يتم تخزينه، يمكنك تحديد ما إذا كان يجب استخدام الكاميرا لمسح الرموز الشريطية ضوئياً.</span><span class="sxs-lookup"><span data-stu-id="3d153-197">In the **Display settings** of the Warehousing application, you can select if the camera should be used for bar code scanning.</span></span> <span data-ttu-id="3d153-198">إذا قمت بتمكين **استخدام الكاميرا كماسح ضوئي**، يمكنك استخدام الكاميرا على كل حقل إدخال تم تعيين وضع الإدخال المفضل له على **المسح الضوئي**.</span><span class="sxs-lookup"><span data-stu-id="3d153-198">If you enable **Use the camera as scanner**, you can use the camera on every input field that has the preferred input mode set to **Scanning**.</span></span>

<span data-ttu-id="3d153-199">للتحكم في ما إذا كان يجب أن يكون حقل الإدخال قابلاً للمسح الضوئي، في صفحة **أسماء حقول تطبيق المستودع** في Supply Chain Management، قم بتعيين **وضع الإدخال المفضل** على **المسح الضوئي**.</span><span class="sxs-lookup"><span data-stu-id="3d153-199">To control whether an input field should be scannable, on the **Warehouse app field names** page in Supply Chain Management, set **Preferred input mode** to **Scanning**.</span></span> <span data-ttu-id="3d153-200">عند تحديد هذا الخيار، يمكن استخدام الكاميرا للمسح الضوئي في تطبيق التخزين.</span><span class="sxs-lookup"><span data-stu-id="3d153-200">When this option is selected, a camera can be used for scanning in the Warehousing app.</span></span>

<span data-ttu-id="3d153-201">يتم دعم أكثر تنسيقات الرموز الشريطية شيوعاً، بما في ذلك الكود 128، الكود 39، الكود 93، EAN-8، EAN-13، UPC-E، UPC-A، وشفرات الاستجابة السريعة.</span><span class="sxs-lookup"><span data-stu-id="3d153-201">The most common bar code formats are supported, including Code 128, Code 39, Code 93, EAN-8, EAN-13, UPC-E, UPC-A, and QR codes.</span></span>

<span data-ttu-id="3d153-202">ستبدأ صفحة **الكاميرا** على كل صفحة حيث يكون لحقل الإدخال وضع إدخال مفضل يتم تعيينه على **المسح الضوئي** عندما تكون في صفحة **الكاميرا**.</span><span class="sxs-lookup"><span data-stu-id="3d153-202">The **Camera** page will be initiated on each page where the input field has the preferred input mode set to **Scanning** when you are on the **Camera** page.</span></span> <span data-ttu-id="3d153-203">استخدم الخيارات التالية للتنقل خلال الصفحة:</span><span class="sxs-lookup"><span data-stu-id="3d153-203">Use the following options to navigate the page:</span></span>

-   <span data-ttu-id="3d153-204">حدد الزر **"رجوع"** للرجوع إلى **صفحة المهام والتفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="3d153-204">Select the **Back** button to go back to the **Task and details** page.</span></span>

-   <span data-ttu-id="3d153-205">حدد القلم في صفحة **المهمة والتفاصيل** للانتقال إلى الصفحة حيث يمكنك كتابة الإدخال يدوياً.</span><span class="sxs-lookup"><span data-stu-id="3d153-205">Select the pencil on the **Task and details** page to go to the page where you can manually type input.</span></span>

    ![لقطة شاشة لمهام تطبيق الأجهزة المحمولة وعلامات تبويب التفاصيل.](../media/task-details-page-ss.png)

-   <span data-ttu-id="3d153-207">حدد الكاميرا في صفحة **المهمة والتفاصيل** للرجوع إلى صفحة **الكاميرا**.</span><span class="sxs-lookup"><span data-stu-id="3d153-207">Select the camera on the **Task and details** page to go back to the **Camera** page.</span></span>

    ![لقطة شاشة لصفحة الكاميرا الخاصة بالمسح الضوئي للصنف.](../media/camera-page-ss.png)

<span data-ttu-id="3d153-209">في صفحة **الكاميرا**، عند تحديد زر **الكاميرا**، فإنه يظهر بشكل باهت أثناء محاولة تحديد الرمز الشريطي.</span><span class="sxs-lookup"><span data-stu-id="3d153-209">On the **Camera** page, when you select the **Camera** button, it will appear dimmed while trying to identify a bar code.</span></span> <span data-ttu-id="3d153-210">في حالة عدم تعريف الرمز الشريطي خلال خمس ثوانٍ، سيؤدي ذلك إلى انتهاء مهلة العملية وسيصبح زر **الكاميرا** متاحاً مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="3d153-210">If a bar code is not identified within five seconds, the process will time out and the **Camera** button will become available again.</span></span> <span data-ttu-id="3d153-211">سيمكنك عندئذ محاولة مسح أحد الرموز الشريطية ضوئياً مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="3d153-211">You will then be able to try to scan a bar code again.</span></span>

<span data-ttu-id="3d153-212">عندما توجه الكاميرا نحو رمز شريطي، حافظ على محاذاة الرمز الشريطي داخل الأقواس للحصول على أفضل النتائج.</span><span class="sxs-lookup"><span data-stu-id="3d153-212">When you aim the camera at a bar code, keep the bar code aligned within the brackets for best results.</span></span> <span data-ttu-id="3d153-213">عند مسح الرمز الشريطي ضوئياً بنجاح، ستتم معالجة النتيجة، وسيتم نقلك إلى الخطوة التالية.</span><span class="sxs-lookup"><span data-stu-id="3d153-213">When a bar code is scanned successfully, the result will be processed, and you will be taken to the next step.</span></span> <span data-ttu-id="3d153-214">إذا كانت الخطوة التالية تحتوي على حقل إدخال آخر مع تعيين وضع الإدخال المفضل على **المسح الضوئي**، فستبدأ صفحة **الكاميرا** مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="3d153-214">If the next step contains another input field with the preferred input mode set to **Scanning**, the **Camera** page will start again.</span></span> <span data-ttu-id="3d153-215">إذا لم تكن الخطوة التالية حقل مسح ضوئي، فلن يتم بدء تشغيل صفحة **الكاميرا**.</span><span class="sxs-lookup"><span data-stu-id="3d153-215">If the next step is not a scanning field, then the **Camera** page will not be initiated.</span></span>

## <a name="remove-access-for-a-device"></a><span data-ttu-id="3d153-216">إزالة الوصول لجهاز</span><span class="sxs-lookup"><span data-stu-id="3d153-216">Remove access for a device</span></span>

<span data-ttu-id="3d153-217">في حالة وجود جهاز مفقود أو مكسور، يجب إزالة إمكانية الوصول إلى Supply Chain Management الخاصة بالجهاز.</span><span class="sxs-lookup"><span data-stu-id="3d153-217">In case of a lost or compromised device, you must remove access to Supply Chain Management for the device.</span></span> <span data-ttu-id="3d153-218">تصف الخطوات التالية العملية المستحسنة لإزالة الوصول.</span><span class="sxs-lookup"><span data-stu-id="3d153-218">The following steps describe the recommended process to remove access.</span></span>

1.  <span data-ttu-id="3d153-219">في Supply Chain Management، انتقل إلى **نظام > إدارة > إعداد > Azure Active Directory > تطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="3d153-219">In Supply Chain Management, go to **System > Administration > Setup > Azure Active Directory > Applications**.</span></span>

2.  <span data-ttu-id="3d153-220">قم بحذف السطر المتوافق مع الجهاز الذي ترغب في إزالة صلاحية الوصول اليه.</span><span class="sxs-lookup"><span data-stu-id="3d153-220">Delete the line that corresponds to the device to which you want to remove access.</span></span> <span data-ttu-id="3d153-221">تذكر **معرف العميل** الذي يتم استخدامه للجهاز الذي تمت إزالته، ستحتاجه لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="3d153-221">Remember the **Client ID** that is used for the removed device, you will need it later.</span></span>


3.  <span data-ttu-id="3d153-222">سجل الدخول إلى مدخل Azure على [https://portal.azure.com](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3d153-222">Sign in to the Azure portal at [https://portal.azure.com](https://portal.azure.com/).</span></span>

4.  <span data-ttu-id="3d153-223">حدد رمز **Active Directory** في القائمة اليمنى وتأكد من أنك في الدليل الصحيح.</span><span class="sxs-lookup"><span data-stu-id="3d153-223">Select the **Active Directory** icon on the left menu and ensure that you are in the correct directory.</span></span>

5.  <span data-ttu-id="3d153-224">في القائمة، حدد **تسجيلات التطبيقات** ثم حدد التطبيق الذي ترغب في تكوينه.</span><span class="sxs-lookup"><span data-stu-id="3d153-224">In the list, select **App registrations** and then select the application that you want to configure.</span></span> <span data-ttu-id="3d153-225">ستظهر صفحة **إعدادات** مع معلومات التكوين.</span><span class="sxs-lookup"><span data-stu-id="3d153-225">The **Settings** page will appear with configuration information.</span></span>

6.  <span data-ttu-id="3d153-226">تأكد من أن **معرف العميل** للتطبيق هو نفس الشكل كما في الخطوة 2 في هذا القسم.</span><span class="sxs-lookup"><span data-stu-id="3d153-226">Ensure that the **Client ID** of the application is the same as in step 2 in this section.</span></span>

7.  <span data-ttu-id="3d153-227">حدد الزر **حذف** في الجزء العلوي.</span><span class="sxs-lookup"><span data-stu-id="3d153-227">Select the **Delete** button in the top pane.</span></span>

8.  <span data-ttu-id="3d153-228">حدد **موافق** في رسالة التأكيد.</span><span class="sxs-lookup"><span data-stu-id="3d153-228">Select **Yes** in the confirmation message.</span></span>
