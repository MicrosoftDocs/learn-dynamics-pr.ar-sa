---
ms.openlocfilehash: 2decc9411d24ba1ec319bcc45a32808a4d8c6893
ms.sourcegitcommit: 4ce9caef7d38158f172e82412bc70ae36883e42f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "6072138"
---
<span data-ttu-id="38ae1-101">لمتابعة السيناريو الذي ستستخدمه في التمارين الآتية، يجب أولاً إعداد الميزة عن طريق توفير بيانات العرض التوضيحي وإضافة بعض السجلات المخصصة.</span><span class="sxs-lookup"><span data-stu-id="38ae1-101">To follow the scenario that you will use in the following exercises, you must first prepare the feature by making demo data available and adding a few custom records.</span></span>

<span data-ttu-id="38ae1-102">قبل محاولة تنفيذك أي تمارين في بقية هذه الوحدة، اتبع التعليمات الموجودة في كافة الأقسام الفرعية الآتية.</span><span class="sxs-lookup"><span data-stu-id="38ae1-102">Before you try to do any of the exercises in the rest of this module, follow the instructions in all the following subsections.</span></span> <span data-ttu-id="38ae1-103">وتقدم هذه الأقسام الفرعية أيضاً العديد من صفحات الإعدادات المهمة التي ستستخدمها عند إعداد إدارة التغييرات الهندسية لمؤسستك الخاصة.</span><span class="sxs-lookup"><span data-stu-id="38ae1-103">These subsections also introduce several important settings pages that you will use when you set up engineering change management for your own organization.</span></span>

## <a name="make-standard-demo-data-available"></a><span data-ttu-id="38ae1-104">توفير بيانات العرض التوضيحي القياسية</span><span class="sxs-lookup"><span data-stu-id="38ae1-104">Make standard demo data available</span></span>

<span data-ttu-id="38ae1-105">وتعامل مع نظام يتم فيه تثبيت بيانات العرض التوضيحي القياسية.</span><span class="sxs-lookup"><span data-stu-id="38ae1-105">Work on a system where the standard demo data is installed.</span></span> <span data-ttu-id="38ae1-106">وتعمل بيانات العرض التوضيحي القياسية على إضافة بيانات إلى العديد من الكيانات القانونية للعروض التوضيحية (الشركات والمؤسسات).</span><span class="sxs-lookup"><span data-stu-id="38ae1-106">The standard demo data adds data for several demo legal entities (companies and organizations).</span></span> <span data-ttu-id="38ae1-107">وفي أثناء العمل خلال التمارين، ستستخدم منتقي الشركة في الجانب الأيمن من شريط التنقل للتبديل بين إحدى الشركتين وهي *DEMF‎* التي تم إعداداها *كمؤسسه هندسية* وشركة أخرى وهي *USMF‎* التي تم إعداداها *كمؤسسه تشغيليه*.</span><span class="sxs-lookup"><span data-stu-id="38ae1-107">As you work through the exercises, you will use the company picker on the right side of the navigation bar to switch between one company *DEMF* that is set up as an *engineering organization* and another company *USMF* that is set up as an *operational organization*.</span></span>

<span data-ttu-id="38ae1-108">لقراءة المزيد حول إعداد نظام يتضمن بيانات عرض توضيحي راجع [توزيع بيئة العرض التوضيحي](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="38ae1-108">To read more about setting up a system with demo data see [Deploy a demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment/?azure-portal=true).</span></span> <span data-ttu-id="38ae1-109">يمكن للمسؤول مساعدتك على إعداد النظام.</span><span class="sxs-lookup"><span data-stu-id="38ae1-109">Your administrator can help you set up the system.</span></span>

## <a name="set-up-an-engineering-organization"></a><span data-ttu-id="38ae1-110">إعداد مؤسسة هندسية</span><span class="sxs-lookup"><span data-stu-id="38ae1-110">Set up an engineering organization</span></span>

<span data-ttu-id="38ae1-111">مؤسسه هندسية تمتلك بيانات هندسية، وتكون مسؤولة عن تصميم المنتج وتغييرات المنتج.</span><span class="sxs-lookup"><span data-stu-id="38ae1-111">An engineering organization owns the engineering data, and is responsible for product design and product changes.</span></span> <span data-ttu-id="38ae1-112">لإعداد المؤسسات الهندسية، اتبع الخطوات الآتية.</span><span class="sxs-lookup"><span data-stu-id="38ae1-112">To set up your engineering organizations, follow these steps.</span></span>

1. <span data-ttu-id="38ae1-113">انتقل إلى **إدارة التغيير الهندسي > الإعداد > المؤسسات الهندسية**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-113">Go to **Engineering change management > Setup > Engineering organizations**.</span></span>
1. <span data-ttu-id="38ae1-114">حدد **جديد** لإضافة صف إلى الشبكة، وعيِّن له القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-114">Select **New** to add a row to the grid, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-115">**المؤسسة الهندسية**: *DEMF*</span><span class="sxs-lookup"><span data-stu-id="38ae1-115">**Engineering organization**: *DEMF*</span></span>
    - <span data-ttu-id="38ae1-116">**اسم المؤسسة**: *Contoso Entertainment System Germany*</span><span class="sxs-lookup"><span data-stu-id="38ae1-116">**Organization name**: *Contoso Entertainment System Germany*</span></span>

    ![لقطة شاشة لإضافة مؤسسة هندسية.](../media/engineering-org-ss.png)
    
## <a name="set-up-the-version-product-dimension-group"></a><span data-ttu-id="38ae1-118">إعداد مجموعه أبعاد منتج الإصدار</span><span class="sxs-lookup"><span data-stu-id="38ae1-118">Set up the version product dimension group</span></span>

<span data-ttu-id="38ae1-119">لإعداد مجموعة أبعاد منتج الإصدار، اتبع الخطوات الآتية.</span><span class="sxs-lookup"><span data-stu-id="38ae1-119">To set up the version product dimension group, follow these steps.</span></span>

1. <span data-ttu-id="38ae1-120">انتقل إلى **إدارة معلومات المنتجات > الإعداد > مجموعات الأبعاد والمتغيرات > مجموعات أبعاد المنتج**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-120">Go to **Product information management > Setup > Dimensions and variant groups > Product dimension groups**.</span></span>
1. <span data-ttu-id="38ae1-121">حدد **جديد** لإنشاء مجموعة أبعاد المنتج.</span><span class="sxs-lookup"><span data-stu-id="38ae1-121">Select **New** to create a product dimension group.</span></span>
1. <span data-ttu-id="38ae1-122">قم بتعيين حقل **الاسم** إلى **الإصدار**</span><span class="sxs-lookup"><span data-stu-id="38ae1-122">Set the **Name** field to **Version**.</span></span>
1. <span data-ttu-id="38ae1-123">حدد **حفظ** لحفظ البُعد الجديد وتحميل القيم إلى علامة التبويب السريعة **أبعاد المنتج**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-123">Select **Save** to save the new dimension and load values onto the **Product dimensions** FastTab.</span></span>
1. <span data-ttu-id="38ae1-124">في علامة التبويب السريعة **أبعاد المنتج**، قم بتعيين **الإصدار** كبُعد نشط للمنتج.</span><span class="sxs-lookup"><span data-stu-id="38ae1-124">On the **Product dimensions** FastTab, set **Version** as an active product dimension.</span></span>


    ![لقطة شاشة لإضافة مجموعة أبعاد المنتج.](../media/product-dimension-groups-ss.png)

## <a name="set-up-product-lifecycle-states"></a><span data-ttu-id="38ae1-126">إعداد حالات دورة حياة المنتج</span><span class="sxs-lookup"><span data-stu-id="38ae1-126">Set up product lifecycle states</span></span>

<span data-ttu-id="38ae1-127">نظراً إلى أن المنتج الهندسي يمر عبر دورة حياته، من المهم أن تكون قادراً على التحكم في الحركات المسموح بها لكل حالة دورة حياة.</span><span class="sxs-lookup"><span data-stu-id="38ae1-127">As an engineering product goes through its lifecycle, it's important that you be able to control which transactions are allowed for each lifecycle state.</span></span> <span data-ttu-id="38ae1-128">لإعداد حالات دورة حياة المنتج، اتبع الخطوات الآتية.</span><span class="sxs-lookup"><span data-stu-id="38ae1-128">To set up the product lifecycle states, follow these steps.</span></span>

1. <span data-ttu-id="38ae1-129">انتقل إلى **إدارة التغيير الهندسي > الإعداد > حالة دورة حياة المنتج**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-129">Go to **Engineering change management > Setup > Product lifecycle state**.</span></span>
1. <span data-ttu-id="38ae1-130">حدد **جديد** لإضافة حالة دورة حياة، وعيِّن لها القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-130">Select **New** to add a lifecycle state, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-131">**الحالة** : *تشغيلية*</span><span class="sxs-lookup"><span data-stu-id="38ae1-131">**State**: *Operational*</span></span>
    - <span data-ttu-id="38ae1-132">**الوصف**: *تشغيلية*</span><span class="sxs-lookup"><span data-stu-id="38ae1-132">**Description**: *Operational*</span></span>

1. <span data-ttu-id="38ae1-133">حدد **حفظ** لحفظ حالة دورة الحياة الجديدة وتحميل القيم إلى **إجراءات العمل الممكنة**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-133">Select **Save** to save the new lifecycle state and load values onto the **Enabled business processes** FastTab.</span></span>
1. <span data-ttu-id="38ae1-134">في علامة التبويب السريعة **إجراءات العمل الممكنة**، حدد إجراءات العمل التي يجب توفرها.</span><span class="sxs-lookup"><span data-stu-id="38ae1-134">On the **Enabled business processes** FastTab, select the business processes that should be available.</span></span> <span data-ttu-id="38ae1-135">بالنسبة إلى هذا المثال، اترك الحقل **السياسة** مضبوطاً على **ممكن** لكافة إجراءات العمل.</span><span class="sxs-lookup"><span data-stu-id="38ae1-135">For this example, leave the **Policy** field set to **Enabled** for all business processes.</span></span>

    ![تمكين إجراءات العمل لحالة دورة الحياة.](../media/product-lifecycle-states-1-ss.png)

1. <span data-ttu-id="38ae1-137">حدد **جديد** لإضافة حالة دورة حياة أخرى، وعيِّن لها القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-137">Select **New** to add another lifecycle state, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-138">**الحالة:** *نموذج أولي*</span><span class="sxs-lookup"><span data-stu-id="38ae1-138">**State:** *Prototype*</span></span>
    - <span data-ttu-id="38ae1-139">**الوصف:** *نموذج أولي*</span><span class="sxs-lookup"><span data-stu-id="38ae1-139">**Description:** *Prototype*</span></span>

1. <span data-ttu-id="38ae1-140">حدد **حفظ** لحفظ حالة دورة الحياة الجديدة وتحميل القيم إلى **إجراءات العمل الممكنة**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-140">Select **Save** to save the new lifecycle state and load values onto the **Enabled business processes** FastTab.</span></span>
1. <span data-ttu-id="38ae1-141">في علامة التبويب السريعة **إجراءات العمل الممكنة**، حدد إجراءات العمل التي يجب توفرها.</span><span class="sxs-lookup"><span data-stu-id="38ae1-141">On the **Enabled business processes** FastTab, select the business processes that should be available.</span></span> <span data-ttu-id="38ae1-142">بالنسبة إلى هذا المثال، اترك الحقل **السياسة** مضبوطاً على *ممكن مع تحذير* لكافة إجراءات العمل.</span><span class="sxs-lookup"><span data-stu-id="38ae1-142">For this example, set the **Policy** field to *Enabled with warning* for all business processes.</span></span>

    ![تمكين (مع تحذيرات) إجراءات العمل لحالة دورة الحياة.](../media/product-lifecycle-states-2-ss.png)

## <a name="set-up-a-version-number-rule"></a><span data-ttu-id="38ae1-144">إعداد قاعدة رقم الإصدار</span><span class="sxs-lookup"><span data-stu-id="38ae1-144">Set up a version number rule</span></span>

<span data-ttu-id="38ae1-145">لإعداد قاعدة رقم الإصدار، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-145">To set up a version number rule, follow these steps.</span></span>

1. <span data-ttu-id="38ae1-146">انتقل إلى **إدارة التغيير الهندسي > إعداد > قاعدة رقم إصدار المنتج**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-146">Go to **Engineering change management > Setup > Product version number rule**.</span></span>
1. <span data-ttu-id="38ae1-147">حدد **جديد** لإضافة قاعدة، وعيِّن لها القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-147">Select **New** to add a rule, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-148">**الاسم:** *تلقائي*</span><span class="sxs-lookup"><span data-stu-id="38ae1-148">**Name:** *Auto*</span></span>
    - <span data-ttu-id="38ae1-149">**قاعدة الرقم:** *تلقائي*</span><span class="sxs-lookup"><span data-stu-id="38ae1-149">**Number Rule:** *Auto*</span></span>
    - <span data-ttu-id="38ae1-150">**التنسيق:** *V-\#\#*</span><span class="sxs-lookup"><span data-stu-id="38ae1-150">**Format:** *V-\#\#*</span></span>

    ![لقطة شاشة لإضافة قاعدة رقم إصدار منتج.](../media/version-number-rule-ss.png)

## <a name="set-up-a-product-release-policy"></a><span data-ttu-id="38ae1-152">إعداد سياسية إصدار المنتج</span><span class="sxs-lookup"><span data-stu-id="38ae1-152">Set up a product release policy</span></span>

<span data-ttu-id="38ae1-153">لإعداد سياسية إصدار المنتج، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-153">To set up a product release policy, follow these steps.</span></span>

1. <span data-ttu-id="38ae1-154">انتقل إلى **إدارة التغيير الهندسي > الإعداد > سياسات إصدار المنتج**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-154">Go to **Engineering change management > Setup > Product release policies**.</span></span>
1. <span data-ttu-id="38ae1-155">حدد **جديد** لإضافة سياسة إصدار، وعيِّن لها القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-155">Select **New** to add a release policy, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-156">**الاسم:** *مكونات*</span><span class="sxs-lookup"><span data-stu-id="38ae1-156">**Name:** *Components*</span></span>
    - <span data-ttu-id="38ae1-157">**الوصف:** *مكونات*</span><span class="sxs-lookup"><span data-stu-id="38ae1-157">**Description:** *Components*</span></span>

1. <span data-ttu-id="38ae1-158">في علامة التبويب السريعة **عام**، عيّن القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-158">On the **General** FastTab, set the following values:</span></span>

    - <span data-ttu-id="38ae1-159">**نوع المنتج:** *سلعة*</span><span class="sxs-lookup"><span data-stu-id="38ae1-159">**Product type:** *Item*</span></span>
    - <span data-ttu-id="38ae1-160">**تطبيق القوالب:** *دائماً*</span><span class="sxs-lookup"><span data-stu-id="38ae1-160">**Apply templates:** *Always*</span></span>
    - <span data-ttu-id="38ae1-161">**نشط:** *نعم*</span><span class="sxs-lookup"><span data-stu-id="38ae1-161">**Active:** *Yes*</span></span>

1. <span data-ttu-id="38ae1-162">في علامة التبويب السريعة **جميع المنتجات**، حدد **إضافة** لإضافة سطر وعيِّن له القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-162">On the **All products** FastTab, select **Add** to add a line, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-163">**معرف حساب الشركة:** *DEMF*</span><span class="sxs-lookup"><span data-stu-id="38ae1-163">**Company account ID:** *DEMF*</span></span>
    - <span data-ttu-id="38ae1-164">**قالب المنتج المُصدر:** *D0006*</span><span class="sxs-lookup"><span data-stu-id="38ae1-164">**Template released product:** *D0006*</span></span>

1. <span data-ttu-id="38ae1-165">حدد **جديد** لإضافة سطر آخر، وعيِّن له القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-165">Select **Add** to add another line, and set the following values for it:</span></span>

    - <span data-ttu-id="38ae1-166">**معرف حساب الشركة:** *USMF*</span><span class="sxs-lookup"><span data-stu-id="38ae1-166">**Company account ID:** *USMF*</span></span>
    - <span data-ttu-id="38ae1-167">**قالب المنتج المُصدر:** *D0006*</span><span class="sxs-lookup"><span data-stu-id="38ae1-167">**Template released product:** *D0006*</span></span>
    - <span data-ttu-id="38ae1-168">**استلام ‏‫قائمة مكونات الصنف‬ (BOM):** حدد خانة الاختيار هذه.</span><span class="sxs-lookup"><span data-stu-id="38ae1-168">**Receive BOM:** Select this check box.</span></span>
    - <span data-ttu-id="38ae1-169">**نسخ اعتماد قائمة مكونات الصنف:** حدد خانة الاختيار هذه.</span><span class="sxs-lookup"><span data-stu-id="38ae1-169">**Copy BOM approval:** Select this check box.</span></span>
    - <span data-ttu-id="38ae1-170">**نسخ تنشيط قائمة مكونات الصنف:** حدد خانة الاختيار هذه.</span><span class="sxs-lookup"><span data-stu-id="38ae1-170">**Copy BOM activation:** Select this check box.</span></span>
    - <span data-ttu-id="38ae1-171">**استلام ‏‫مسار:** حدد خانة الاختيار هذه.</span><span class="sxs-lookup"><span data-stu-id="38ae1-171">**Receive route:** Select this check box.</span></span>
    - <span data-ttu-id="38ae1-172">**نسخ اعتماد المسار:** حدد خانة الاختيار هذه.</span><span class="sxs-lookup"><span data-stu-id="38ae1-172">**Copy route approval:** Select this check box.</span></span>
    - <span data-ttu-id="38ae1-173">**نسخ تنشيط المسار:** حدد خانة الاختيار هذه.</span><span class="sxs-lookup"><span data-stu-id="38ae1-173">**Copy route activation:** Select this check box.</span></span>

    ![لقطة شاشة لإضافة سياسة إصدار المنتج.](../media/product-release-policy-ss.png)

## <a name="set-up-an-engineering-product-category"></a><span data-ttu-id="38ae1-175">إعداد فئة المنتج الهندسي</span><span class="sxs-lookup"><span data-stu-id="38ae1-175">Set up an engineering product category</span></span> 

<span data-ttu-id="38ae1-176">توفر فئات المنتجات الهندسية أساساً لإنشاء المنتجات الهندسية (أي المنتجات التي يتم إصدارها والتحكم فيها من خلال إدارة التغيير الهندسي).</span><span class="sxs-lookup"><span data-stu-id="38ae1-176">Engineering product categories provide the basis for creating engineering products (that is, products that are versioned and controlled through engineering change management).</span></span> <span data-ttu-id="38ae1-177">لإعداد فئات المنتجات الهندسية، اتبع الخطوات الآتية.</span><span class="sxs-lookup"><span data-stu-id="38ae1-177">To set up engineering product categories, follow these steps.</span></span>

1. <span data-ttu-id="38ae1-178">انتقل إلى **إدارة تغيير الهندسة > تفاصيل فئة المنتج الهندسي**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-178">Go to **Engineering change management > Engineering product category details**.</span></span>
1. <span data-ttu-id="38ae1-179">حدد **جديد** لإنشاء فئة، وعيِّن لها القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-179">Select **New** to create a category, and set the following values for it:</span></span>
    
    - <span data-ttu-id="38ae1-180">**الاسم:** *مكونات*</span><span class="sxs-lookup"><span data-stu-id="38ae1-180">**Name:** *Components*</span></span>
    - <span data-ttu-id="38ae1-181">**المؤسسة الهندسية:** *DEMF*</span><span class="sxs-lookup"><span data-stu-id="38ae1-181">**Engineering organization:** *DEMF*</span></span>

1. <span data-ttu-id="38ae1-182">في علامة التبويب السريعة **التفاصيل**، عيّن القيم الآتية:</span><span class="sxs-lookup"><span data-stu-id="38ae1-182">On the **Details** FastTab, set the following values:</span></span>

    - <span data-ttu-id="38ae1-183">**نوع المنتج:** *سلعة*</span><span class="sxs-lookup"><span data-stu-id="38ae1-183">**Product type:** *Item*</span></span>
    - <span data-ttu-id="38ae1-184">**إصدار المسار في الحركات:** *نعم*</span><span class="sxs-lookup"><span data-stu-id="38ae1-184">**Track version in transactions:** *Yes*</span></span>
    - <span data-ttu-id="38ae1-185">**مجموعة أبعاد المنتج** *الإصدار*</span><span class="sxs-lookup"><span data-stu-id="38ae1-185">**Product dimension group:** *Version*</span></span>
    - <span data-ttu-id="38ae1-186">**حالة دورة حياة المنتج عند الإنشاء:** *تشغيلي*</span><span class="sxs-lookup"><span data-stu-id="38ae1-186">**Product lifecycle state at creation:** *Operational*</span></span>
    - <span data-ttu-id="38ae1-187">**قاعدة رقم الإصدار:** *تلقائي*</span><span class="sxs-lookup"><span data-stu-id="38ae1-187">**Version number rule:** *Auto*</span></span>
    - <span data-ttu-id="38ae1-188">**فرض السريان:** *لا*</span><span class="sxs-lookup"><span data-stu-id="38ae1-188">**Enforce effectivity:** *No*</span></span>
    - <span data-ttu-id="38ae1-189">**استخدام مصطلح قاعدة الرقم:** *لا*</span><span class="sxs-lookup"><span data-stu-id="38ae1-189">**Use number rule nomenclature:** *No*</span></span>
    - <span data-ttu-id="38ae1-190">**استخدام مصطلح قاعدة الاسم:** *لا*</span><span class="sxs-lookup"><span data-stu-id="38ae1-190">**Use name rule nomenclature:** *No*</span></span>
    - <span data-ttu-id="38ae1-191">**استخدام مصطلح قاعدة الوصف:** *لا*</span><span class="sxs-lookup"><span data-stu-id="38ae1-191">**Use description rule nomenclature:** *No*</span></span>

1. <span data-ttu-id="38ae1-192">في علامة التبويب السريعة **سياسة الاستعداد**، عيِّن حقل **سياسة إصدار المنتج** على *مكونات*.</span><span class="sxs-lookup"><span data-stu-id="38ae1-192">On the **Readiness policy** FastTab, set the **Product release policy** field to *Components*.</span></span>
1. <span data-ttu-id="38ae1-193">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-193">Select **Save**.</span></span>

    <span data-ttu-id="38ae1-194">[![لقطة شاشة لإضافة فئة المنتج الهندسي.](../media/product-category-details-ss.png)](../media/product-category-details-ss.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="38ae1-194">[![Screenshot of adding an engineering product category.](../media/product-category-details-ss.png)](../media/product-category-details-ss.png#lightbox)</span></span>

### <a name="set-up-product-acceptance-conditions"></a><span data-ttu-id="38ae1-195">إعداد شروط قبول المنتج</span><span class="sxs-lookup"><span data-stu-id="38ae1-195">Set up product acceptance conditions</span></span>

1. <span data-ttu-id="38ae1-196">استخدم منتقي الشركة في الجانب الأيمن من شريط التنقل للتبديل إلى الكيان القانوني *USMF)‎)* (الشركة).</span><span class="sxs-lookup"><span data-stu-id="38ae1-196">Use the company picker on the right side of the navigation bar to switch to the *USMF* legal entity (company).</span></span>
1. <span data-ttu-id="38ae1-197">انتقل إلى **إدارة التغيير الهندسي > الإعداد > معلمات إدارة التغيير الهندسي**.</span><span class="sxs-lookup"><span data-stu-id="38ae1-197">Go to **Engineering change management > Setup > Engineering change management parameters**.</span></span>
1. <span data-ttu-id="38ae1-198">في علامة التبويب **التحكم في الإصدار**، في القسم **قبول المنتج**، عيِّن الحقل **قبول المنتج** على *يدوي*.</span><span class="sxs-lookup"><span data-stu-id="38ae1-198">On the **Release control** tab, in the **Product acceptance** section, set the **Product acceptance** field to *Manual*.</span></span>

    ![لقطة شاشة لإعداد شروط قبول المنتج.](../media/engineering-change-management-parameters-ss.png)
