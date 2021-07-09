---
ms.openlocfilehash: 5a45158dfccef3b5a511c209d137dd0de74d2df9
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070216"
---
## <a name="prerequisites"></a><span data-ttu-id="f85da-101">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="f85da-101">Prerequisites</span></span>
<span data-ttu-id="f85da-102">يجب عليك استخدام البيانات التجريبية في الكيان القانوني USRT لممارسة التمرينات.</span><span class="sxs-lookup"><span data-stu-id="f85da-102">You should use the demo data in the USRT legal entity to go through the exercises.</span></span> 

> [!NOTE]
> <span data-ttu-id="f85da-103">لاستخدام توصيات المنتج، يجب أن يكون لديك حق الوصول إلى اشتراك Azure وتنشيط الاتصال بـ Azure Data Lake storage.</span><span class="sxs-lookup"><span data-stu-id="f85da-103">To use product recommendations, you must have access to an Azure subscription and activate the connection to the Azure Data Lake storage.</span></span>
 
<span data-ttu-id="f85da-104">إذا لم يكن لديك اشتراك Azure، فلن تتمكن من تشغيل التمرينات التالية.</span><span class="sxs-lookup"><span data-stu-id="f85da-104">If you do not have an Azure subscription, you will not be able to run the following exercises.</span></span> <span data-ttu-id="f85da-105">إذا كان لديك اشتراك Azure، فتأكد من تشغيل توصيات المنتج من خلال اتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f85da-105">If you do have an Azure subscription, make sure that you turn on the product recommendations by following these steps:</span></span>

1.  <span data-ttu-id="f85da-106">انتقل إلى **البيع بالتجزئة وCommerce > توصيات المنتج > معلمات التوصيات**.</span><span class="sxs-lookup"><span data-stu-id="f85da-106">Go to **Retail and Commerce > Product recommendations > Recommendation parameters**.</span></span> 
2.  <span data-ttu-id="f85da-107">حدد **نعم** في الحقل **تمكين التوصيات**.</span><span class="sxs-lookup"><span data-stu-id="f85da-107">Select **Yes** in the **Enable recommendations** field.</span></span> 


## <a name="configure-market-parameters-and-adjust-recommendation-results"></a><span data-ttu-id="f85da-108">تكوين معلمات السوق وضبط نتائج التوصيات</span><span class="sxs-lookup"><span data-stu-id="f85da-108">Configure market parameters and adjust recommendation results</span></span>

### <a name="scenario"></a><span data-ttu-id="f85da-109">السيناريو</span><span class="sxs-lookup"><span data-stu-id="f85da-109">Scenario</span></span>
<span data-ttu-id="f85da-110">أنت مدير منتج في شركة Fabrikam وتريد تكوين معلمات السوق لخوارزميات التوصيات الخاصة بأنواع **قائمة المنتجات المتداولة**.</span><span class="sxs-lookup"><span data-stu-id="f85da-110">You are a product manager at Fabrikam and want to configure market parameters for the algorithmically generated **Trending list** type of product recommendations.</span></span> <span data-ttu-id="f85da-111">في هذا السيناريو، تريد إزالة حقيبة يد من قائمة المنتجات المتداولة.</span><span class="sxs-lookup"><span data-stu-id="f85da-111">In this scenario, you want to remove a handbag from the trending list.</span></span>

1.  <span data-ttu-id="f85da-112">انتقل إلى **البيع بالتجزئة وCommerce > توصيات المنتج > معلمات التوصيات**</span><span class="sxs-lookup"><span data-stu-id="f85da-112">Go to **Retail and Commerce > Product recommendations > Recommendation parameters**</span></span> 
2.  <span data-ttu-id="f85da-113">انتقل إلى علامة تبويب **المنتجات المتداولة**. يحتوي نوعان من معلمات السوق على قيم افتراضية.</span><span class="sxs-lookup"><span data-stu-id="f85da-113">Go to the **Trending products** tab.Two types of market parameters contain default values.</span></span> <span data-ttu-id="f85da-114">يمكنك ترك القيم الافتراضية، أو يمكنك تغييرها في أي وقت لتعكس سير عملك بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="f85da-114">You can leave the default values, or you can change them at any time to better reflect your flow of business.</span></span>
3.  <span data-ttu-id="f85da-115">من علامة التبويب **المنتجات المتداولة**، يمكنك أيضاً إضافة منتجات إلى مقدمة قائمة التوصيات (تضمين) أو إزالة منتج (استبعاد).</span><span class="sxs-lookup"><span data-stu-id="f85da-115">From the **Trending products** tab, you can also add products to the front of a recommendations list (include) or remove a product (exclude).</span></span> 
4.  <span data-ttu-id="f85da-116">من علامة التبويب **المنتجات المتداولة**، حدد في الجدول **إضافة بند**.</span><span class="sxs-lookup"><span data-stu-id="f85da-116">On the **Trending products** tab, in the table, select **Add line**.</span></span>
5.  <span data-ttu-id="f85da-117">في الحقل **المنتج**، أدخل قيمة تمثل المنتج الذي تتم إزالته من قائمة **المنتجات المتداولة**.</span><span class="sxs-lookup"><span data-stu-id="f85da-117">In the **Product** field, enter a value that represents the product that is being removed from the **Trending products** list.</span></span> <span data-ttu-id="f85da-118">حدد موقع **حقيبة اليد المصنوعة من الجلد الطبيعي** أو أدخل رقم الصنف **91032**.</span><span class="sxs-lookup"><span data-stu-id="f85da-118">Locate and select the **Genuine leather handbag** or enter the item number **91032**.</span></span>
6.  <span data-ttu-id="f85da-119">في الحقل **نوع البند**، يمكنك تقرير ما إذا كان سيتم تضمين منتج ما أو استبعاده.</span><span class="sxs-lookup"><span data-stu-id="f85da-119">In the **Line type** field, you can decide whether to include or exclude a product.</span></span> <span data-ttu-id="f85da-120">بالنسبة لهذا السيناريو، حدد **استبعاد**.</span><span class="sxs-lookup"><span data-stu-id="f85da-120">For this scenario, select **Exclude**.</span></span> 
7.  <span data-ttu-id="f85da-121">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="f85da-121">Select **Save**.</span></span> 

> [!NOTE]
> <span data-ttu-id="f85da-122">في سيناريوهات العالم الحقيقي، ستكون قادراً على رؤية التغييرات على الصفحات المباشرة بعد اتفاقية مستوى الخدمة المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="f85da-122">In real-world scenarios, you would be able to see the changes on live pages after the required service-level agreement.</span></span> <span data-ttu-id="f85da-123">بالنسبة لهذا السيناريو، يمكنك افتراض أنه قد تمت إزالة المنتج بنجاح.</span><span class="sxs-lookup"><span data-stu-id="f85da-123">For this scenario, you can assume that the product was successfully removed.</span></span>

## <a name="create-an-editorial-recommendation-list"></a><span data-ttu-id="f85da-124">إنشاء قائمة توصيات تحريرية</span><span class="sxs-lookup"><span data-stu-id="f85da-124">Create an editorial recommendation list</span></span>

### <a name="scenario"></a><span data-ttu-id="f85da-125">السيناريو</span><span class="sxs-lookup"><span data-stu-id="f85da-125">Scenario</span></span>
<span data-ttu-id="f85da-126">أنت بائع أحذية بالتجزئة وتريد أن تعرض للعملاء مجموعة موسمية من أحذية الرجال لموسم الخريف.</span><span class="sxs-lookup"><span data-stu-id="f85da-126">You are a shoe retailer who wants to show customers a seasonal collection of men’s shoes for the Autumn season.</span></span> <span data-ttu-id="f85da-127">تشرح الخطوات التالية كيفية إنشاء قائمة توصيات تحريرية لأحذية الخريف وإضافة منتجات إلى القائمة.</span><span class="sxs-lookup"><span data-stu-id="f85da-127">The following steps explain how to create an editorial recommendation list for Autumn shoes and to add products to the list.</span></span>

1.  <span data-ttu-id="f85da-128">انتقل إلى **Retail وCommerce > توصيات المنتج > قوائم التوصيات**.</span><span class="sxs-lookup"><span data-stu-id="f85da-128">Go to **Retail and Commerce > Product recommendations > Recommendation lists**.</span></span> 
2.  <span data-ttu-id="f85da-129">حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="f85da-129">Select **New**.</span></span> 
3.  <span data-ttu-id="f85da-130">في الحقل **معرف القائمة**، حدد **أحذية_موسم_الخريف**.</span><span class="sxs-lookup"><span data-stu-id="f85da-130">In the **List ID** field, enter **Autumn_shoes**.</span></span> 
4.  <span data-ttu-id="f85da-131">في الحقل **‏‫عنوان القائمة‬**، أدخل **مجموعة أحذية موسم الخريف**.</span><span class="sxs-lookup"><span data-stu-id="f85da-131">In the **List title** field, enter **Autumn shoes selection**.</span></span> 
5.  <span data-ttu-id="f85da-132">حدد **إضافة منتجات‬**.</span><span class="sxs-lookup"><span data-stu-id="f85da-132">Select **Add products**.</span></span> 
6.  <span data-ttu-id="f85da-133">في الشجرة، حدد **الكل (الكل)/الملابس والأحذية (الملابس والأحذية)/الأحذية (الأحذية)/الأحذية الرجالية (الأحذية الرجالية)**.</span><span class="sxs-lookup"><span data-stu-id="f85da-133">In the tree, select **ALL (ALL)\Apparel and Footwear (Apparel and Footwear)\Footwear (Footwear)\Men's Footwear (Men's Footwear)**.</span></span> 
7.  <span data-ttu-id="f85da-134">في القائمة، قم بوضع علامة للصف المحدد.</span><span class="sxs-lookup"><span data-stu-id="f85da-134">In the list, mark the selected row.</span></span> 
8.  <span data-ttu-id="f85da-135">في القائمة، حدد الصنف **0159** والصنف **991105**.</span><span class="sxs-lookup"><span data-stu-id="f85da-135">In the list, select items **0159** and **991105**.</span></span> 
9.  <span data-ttu-id="f85da-136">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="f85da-136">Select **Add**.</span></span>
10. <span data-ttu-id="f85da-137">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="f85da-137">Select **OK**.</span></span> 
11. <span data-ttu-id="f85da-138">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="f85da-138">Select **Save**.</span></span>
 
## <a name="add-recommendations-to-an-e-commerce-page"></a><span data-ttu-id="f85da-139">إضافة توصيات إلى صفحة تجارة إلكترونية</span><span class="sxs-lookup"><span data-stu-id="f85da-139">Add recommendations to an e-Commerce page</span></span>

### <a name="scenario"></a><span data-ttu-id="f85da-140">السيناريو</span><span class="sxs-lookup"><span data-stu-id="f85da-140">Scenario</span></span>
<span data-ttu-id="f85da-141">تريد إضافة قوائم توصيات إلى صفحة تجارة إلكترونية موجودة.</span><span class="sxs-lookup"><span data-stu-id="f85da-141">You want to add recommendation lists to an existing e-Commerce page.</span></span> <span data-ttu-id="f85da-142">لإكمال هذا التمرين، ستحتاج إلى الوصول إلى منشئ موقع التجارة الإلكترونية والتوصيات الممكّنة.</span><span class="sxs-lookup"><span data-stu-id="f85da-142">To complete this exercise, you will need access to the e-Commerce site builder and enabled recommendations.</span></span> 

1.  <span data-ttu-id="f85da-143">من منشئ موقع التجارة الإلكترونية، انتقل إلى صفحة موجودة.</span><span class="sxs-lookup"><span data-stu-id="f85da-143">From the e-Commerce site builder, go to an existing page.</span></span> <span data-ttu-id="f85da-144">انتقل إلى **الصفحة الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="f85da-144">Go to **Homepage**.</span></span>
2.  <span data-ttu-id="f85da-145">قم بتشغيل وضع **التحرير** في الزاوية العليا اليمنى.</span><span class="sxs-lookup"><span data-stu-id="f85da-145">Turn on **Edit** mode in the upper-right corner.</span></span>
3.  <span data-ttu-id="f85da-146">في الوحدة النمطية **الحاوية**، حدد زر علامة الحذف (...) ثم حدد **إضافة وحدة نمطية**.</span><span class="sxs-lookup"><span data-stu-id="f85da-146">In the **Container** module, select the ellipsis button (…) and then select **Add module**.</span></span>
4.  <span data-ttu-id="f85da-147">في مربع الحوار **إضافة وحدة نمطية**، حدد **مجموعة المنتجات** ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="f85da-147">In the **Add module** dialog box, select **Product collection** and then select **OK**.</span></span>
5.  <span data-ttu-id="f85da-148">في جزء **الخصائص** الخاص بالوحدة النمطية لمجموعة المنتجات، حدد **إضافة قائمة منتجات**.</span><span class="sxs-lookup"><span data-stu-id="f85da-148">In the **Properties** pane for the product collection module, select **Add a product list**.</span></span>
6.  <span data-ttu-id="f85da-149">حدد نوع قائمة التوصيات التي تريد إضافتها، ثم قم **بحفظ** الصفحة و **نشرها**.</span><span class="sxs-lookup"><span data-stu-id="f85da-149">Select the type of recommendation list that you want to add, and then **Save** and **Publish** the page.</span></span>
7.  <span data-ttu-id="f85da-150">انتقل إلى الصفحة المباشرة لعرض قائمة التوصيات.</span><span class="sxs-lookup"><span data-stu-id="f85da-150">Go to the live page to view the recommendations list.</span></span> 

