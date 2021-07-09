---
ms.openlocfilehash: 419327129c0bfcde7510eb68f8940870f3b69a0c
ms.sourcegitcommit: d9d731bb071133aa102da6c7c602825acae008a2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2021
ms.locfileid: "6073711"
---
<span data-ttu-id="9208f-101">البحث عن الكلمة الأساسية قابل للتطبيق على الكيانات الثلاثة للعميل والمنتج والعميل المتوقع، ويتطلب إنشاء جدول فهرس، من خلال صفحة **معايير البحث**.</span><span class="sxs-lookup"><span data-stu-id="9208f-101">Search on keyword is applicable for the three entities of Customer, Product, and Prospect, and requires building up an index table, through the **Search criteria** page.</span></span>

 
<span data-ttu-id="9208f-102">البحث في الحقول المحددة مسبقاً متاح فقط للعميل والعميل المتوقع (عند إنشاء مستندات جديدة)، مما يعني أن البحث عن المنتج يعتمد دائماً على الكلمة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="9208f-102">Search on predefined fields is only available for Customer and Prospect (when you are creating new documents), which means that the Product search is always based on keyword.</span></span>


<span data-ttu-id="9208f-103">عند البحث عن الكلمة الأساسية:</span><span class="sxs-lookup"><span data-stu-id="9208f-103">When searching on keyword:</span></span>

-   <span data-ttu-id="9208f-104">يستخدم بحث التطابق الكامل أسلوب SQL CONTAINS وهو فعال للغاية ولكنه يقتصر على الرموز/العبارات الكاملة.</span><span class="sxs-lookup"><span data-stu-id="9208f-104">The Full match search uses the SQL CONTAINS method and is highly effective but limited to whole token/phrases.</span></span>

-   <span data-ttu-id="9208f-105">يستخدم بحث المطابقة الجزئية أسلوب SQL LIKE ولا يقدم الأداء الأمثل للبيانات كبيرة الحجم.</span><span class="sxs-lookup"><span data-stu-id="9208f-105">The Partial match search uses the SQL LIKE method and does not offer optimal performance on large volume data.</span></span>

<span data-ttu-id="9208f-106">عند البحث في حقول محددة مسبقاً، تستخدم عمليات البحث الكاملة والجزئية SQL LIKE وتكون فعالة للغاية.</span><span class="sxs-lookup"><span data-stu-id="9208f-106">When you are searching on predefined fields, both Full and Partial searches use SQL LIKE and are highly effective.</span></span>

## <a name="search-for-products-and-product-variants-during-order-entry"></a><span data-ttu-id="9208f-107">البحث عن المنتجات ومتغيرات المنتجات أثناء إدخال الأمر</span><span class="sxs-lookup"><span data-stu-id="9208f-107">Search for products and product variants during order entry</span></span>

<span data-ttu-id="9208f-108">يمكنك استخدام حقل **رقم الصنف** في بند أمر المبيعات كحقل بحث للبحث عن المنتجات ومتغيرات المنتجات عندما تقوم يدوياً بإنشاء بند أمر مبيعات أو بند أمر شراء.</span><span class="sxs-lookup"><span data-stu-id="9208f-108">You can use the **Item number** field on a sales order line as a search field to search for products and product variants when you manually create a sales order line or a purchase order line.</span></span>

<span data-ttu-id="9208f-109">يمكنك إدخال أي جزء من اسم المنتج أو الرقم أو البعد والحصول على بحث يعرض جميع الأصناف التي تطابق كلمة البحث.</span><span class="sxs-lookup"><span data-stu-id="9208f-109">You can enter any part of a product name, number, or dimension and get a lookup that displays all the items that match the search word.</span></span> <span data-ttu-id="9208f-110">يتيح لك ذلك العثور بسرعة على متغيرات المنتج عندما يكون لديك فقط سلسلة التكوين أو أحد أبعاد المنتج المتاحة.</span><span class="sxs-lookup"><span data-stu-id="9208f-110">This lets you quickly find product variants when you only have the configuration string or one of the product dimensions available.</span></span>

<span data-ttu-id="9208f-111">في بعض الأحيان، لا يكون الحصول على الكثير من شيء ما هو الأمثل.</span><span class="sxs-lookup"><span data-stu-id="9208f-111">Occasionally, having too much of something is not optimal.</span></span> <span data-ttu-id="9208f-112">هذه النظرية صحيحة بشكل خاص إذا كنت تبيع عدداً من المنتجات المتشابهة وتحاول تذكر أرقام العناصر أو أسماء البحث عن المنتج للعثور على المنتج المناسب لوضعه في أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="9208f-112">This theory is especially true if you sell a number of products that are similar and you are trying to remember item numbers or product search names to find the right product to put on a sales order.</span></span>

<span data-ttu-id="9208f-113">عندما تبحث عن منتجات أو متغيرات منتج، من المهم أن تفهم كيف تعثر ميزة البحث على المنتجات التي تطابق النص الذي تدخله.</span><span class="sxs-lookup"><span data-stu-id="9208f-113">When you search for products or product variants, it is important to understand how the search feature finds the products that match the text that you enter.</span></span>

<span data-ttu-id="9208f-114">يمكنك تكوين معامِلات البحث بناءً على نوع البحث للمطابقة الكاملة أو الجزئية عندما تبحث عن الأصناف و/أو العملاء.</span><span class="sxs-lookup"><span data-stu-id="9208f-114">You can configure the search parameters based on a search type of full or partial match when you are searching for items and/or customers.</span></span>

<span data-ttu-id="9208f-115">قواعد البحث الأساسية في تقديم نتائج البحث هي:</span><span class="sxs-lookup"><span data-stu-id="9208f-115">The key search rules in delivering search results are:</span></span>

-   <span data-ttu-id="9208f-116">ستعيد نتائج البحث أي سجل مطابق، بغض النظر عن الحقل الذي تم إدخال نص البحث فيه.</span><span class="sxs-lookup"><span data-stu-id="9208f-116">Search results will return any matching record, disregarding the field that the search text is entered in.</span></span>

-   <span data-ttu-id="9208f-117">يجب أن يكون نص البحث موجوداً في السجل المطابق بطوله الكامل.</span><span class="sxs-lookup"><span data-stu-id="9208f-117">The search text needs to be present in the matching record in its full length.</span></span>

-   <span data-ttu-id="9208f-118">ستحدث المطابقة حتى إذا تم العثور على نص البحث في منتصف سلسلة نصية في السجل المطابق.</span><span class="sxs-lookup"><span data-stu-id="9208f-118">A match will occur even if the search text is found in the middle of a text string in the matching record.</span></span> <span data-ttu-id="9208f-119">ليس من الضروري أن يظهر نص البحث في بداية سلسلة نصية.</span><span class="sxs-lookup"><span data-stu-id="9208f-119">The search text does not have to appear in the beginning of a text string.</span></span>

-   <span data-ttu-id="9208f-120">يتم التعامل مع نص البحث كسلسلة نصية واحدة حتى إذا كان يحتوي على مسافة بيضاء.</span><span class="sxs-lookup"><span data-stu-id="9208f-120">The search text is treated as a single text string even if it contains white space.</span></span>

## <a name="configure-the-product-search"></a><span data-ttu-id="9208f-121">تكوين البحث عن المنتج</span><span class="sxs-lookup"><span data-stu-id="9208f-121">Configure the product search</span></span>

<span data-ttu-id="9208f-122">فيما يلي خطوات تكوين البحث عن المنتج.</span><span class="sxs-lookup"><span data-stu-id="9208f-122">Here are the steps to configure the product search.</span></span>

### <a name="step-1"></a><span data-ttu-id="9208f-123">الخطوة 1</span><span class="sxs-lookup"><span data-stu-id="9208f-123">Step 1</span></span>

<span data-ttu-id="9208f-124">قم بتضمين جميع معرفات المنتج ومتغيرات المنتج ذات الصلة والأبعاد في معايير البحث.</span><span class="sxs-lookup"><span data-stu-id="9208f-124">Include all the relevant product and product variant identifiers and dimensions in the search criteria.</span></span>

<span data-ttu-id="9208f-125">من أمثلة معرفات متغيرات المنتج والمنتج والأبعاد التي يمكنك البحث عنها اسم المنتج ورقم الصنف وعرض رقم المنتج والتكوين واللون والحجم والنمط واسم البحث وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="9208f-125">Examples of product and product variant identifiers and dimensions that you can search by are Product name, Item number, Display product number, Configuration, Color, Size, Style, Search name, and so on.</span></span>

<span data-ttu-id="9208f-126">انتقل إلى صفحة **المبيعات والتسويق > الإعداد > البحث > معايير البحث**.</span><span class="sxs-lookup"><span data-stu-id="9208f-126">Go to **Sales and marketing > Setup > Search > Search criteria** page.</span></span> <span data-ttu-id="9208f-127">تتيح لك صفحة **معايير البحث** تحديد معايير البحث عن العملاء والعملاء المتوقعين والمنتجات.</span><span class="sxs-lookup"><span data-stu-id="9208f-127">The **Search criteria** page allows you to define criteria for customer, prospect, and product search.</span></span> <span data-ttu-id="9208f-128">تأكد من تصفية الصفحة باستخدام معايير البحث عن المنتج، والتي يمكنك القيام بها بالتبديل إلى **المنتج** في قائمة الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9208f-128">Make sure that you filter the page by using product search criteria, which you can do by switching to **Product** in the page's menu.</span></span>

![لقطة شاشة لصفحة معايير البحث تمت تصفيتها حسب المنتج.](../media/search-criteria-product.png)

<span data-ttu-id="9208f-130">لإضافة رقم منتج العرض إلى معايير البحث، حدد **جديد** في قائمة الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9208f-130">To add the display product number to the search criteria, select **New** in the page's menu.</span></span> <span data-ttu-id="9208f-131">سيضيف هذا التحديد رقماً قياسياً جديداً في شبكة **معايير البحث**.</span><span class="sxs-lookup"><span data-stu-id="9208f-131">This selection will add a new record in the **Search criteria** grid.</span></span> <span data-ttu-id="9208f-132">افتح البحث عن عمود **اسم الحقل** وحدد **DisplayProductNumber**.</span><span class="sxs-lookup"><span data-stu-id="9208f-132">Open the **Field name** column lookup and select **DisplayProductNumber**.</span></span>

<span data-ttu-id="9208f-133">لإضافة تكوين المنتج إلى معايير البحث، قم بإنشاء سجل جديد في شبكة **معايير البحث** وحدد **configId** في عمود حقل الاسم.</span><span class="sxs-lookup"><span data-stu-id="9208f-133">To add the product's configuration to the search criteria, create a new record in the **Search criteria** grid and select **configId** in the Field name column.</span></span> <span data-ttu-id="9208f-134">بنفس الطريقة، أنشئ سجلاً باستخدام **اسم الحقل**، و **InventColorId** لبُعد اللون، و **InventSizeId** لبُعد الحجم، و **InventStyleId** لبُعد النمط.</span><span class="sxs-lookup"><span data-stu-id="9208f-134">In the same manner, create a record with **Field name**, **InventColorId** for the color dimension, **InventSizeId** for the size dimension, and **InventStyleId** for the style dimension.</span></span>

### <a name="step-2"></a><span data-ttu-id="9208f-135">الخطوة 2</span><span class="sxs-lookup"><span data-stu-id="9208f-135">Step 2</span></span> 

<span data-ttu-id="9208f-136">قم بتعبئة جدول قاعدة البيانات المستخدم للبحث عن المنتج.</span><span class="sxs-lookup"><span data-stu-id="9208f-136">Populate the database table that is used for product search.</span></span>

<span data-ttu-id="9208f-137">في صفحة **معايير البحث**، حدد زر **تحديث بيانات البحث**.</span><span class="sxs-lookup"><span data-stu-id="9208f-137">In the **Search criteria** page, select the **Update search data** button.</span></span>

<span data-ttu-id="9208f-138">في مربع الحوار **تحديث بيانات البحث**، تأكد من تعيين **المصدر** إلى **المنتج**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="9208f-138">In the **Update search data** dialog box, make sure that **Source** is set to **Product** and then select **OK**.</span></span> <span data-ttu-id="9208f-139">سيقوم النظام بتجميع جميع معايير البحث المحددة التي تم تحديدها في الخطوة 1 في جدول واحد.</span><span class="sxs-lookup"><span data-stu-id="9208f-139">The system will aggregate in one table all the selected search criteria that was specified in step 1.</span></span>

<span data-ttu-id="9208f-140">إذا كان لديك الكثير من المنتجات ومتغيرات المنتجات، فقد تكون هذه العملية طويلة جداً، وقد تتلقى تحذيراً.</span><span class="sxs-lookup"><span data-stu-id="9208f-140">If you have a lot of products and product variants, this operation can be quite lengthy, and you might receive a warning.</span></span> <span data-ttu-id="9208f-141">نوصي بجدولة عدد سكان جدول البحث على خادم الدُفعات في وقت لا يكون فيه الخادم مشغولاً للغاية.</span><span class="sxs-lookup"><span data-stu-id="9208f-141">We recommend that you schedule the search table population on the batch server at a time when the server is not too busy.</span></span>

<span data-ttu-id="9208f-142">حتى يتم ملء الجدول، لن يوفر البحث عن المنتج النتائج الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="9208f-142">Until the table is populated, product search will not provide the correct results.</span></span> <span data-ttu-id="9208f-143">إذا لم تتلق أي نتائج بحث، فتأكد من تعبئة هذا الجدول.</span><span class="sxs-lookup"><span data-stu-id="9208f-143">If you do not receive any search results, make sure that this table is populated.</span></span>

<span data-ttu-id="9208f-144">يجب تعبئة الجدول فقط عند تعديل معايير البحث.</span><span class="sxs-lookup"><span data-stu-id="9208f-144">The table must be populated only when the search criteria is modified.</span></span>
<span data-ttu-id="9208f-145">تتم إضافة المنتجات والمتغيرات التي تم إصدارها حديثاً إلى الجدول تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="9208f-145">Newly released products and variants are automatically added to the table.</span></span> <span data-ttu-id="9208f-146">تتم إزالة المنتجات والمتغيرات المحذوفة تلقائياً من الجدول.</span><span class="sxs-lookup"><span data-stu-id="9208f-146">Deleted products and variants are automatically removed from the table.</span></span>

### <a name="step-3"></a><span data-ttu-id="9208f-147">الخطوة 3</span><span class="sxs-lookup"><span data-stu-id="9208f-147">Step 3</span></span>

<span data-ttu-id="9208f-148">قم بتمكين البحث عن البحث عن المنتج في بنود أوامر الشراء والمبيعات.</span><span class="sxs-lookup"><span data-stu-id="9208f-148">Enable the lookup for product search on sales and purchase order lines.</span></span>

<span data-ttu-id="9208f-149">يمكنك تمكين هذه الوظيفة بالانتقال إلى **المبيعات والتسويق > الإعداد > البحث > معلمات البحث** وتعيين **تمكين البحث للبحث** إلى **نعم** في علامة التبويب **عام**.</span><span class="sxs-lookup"><span data-stu-id="9208f-149">You can enable this functionality by going to **Sales and marketing > Setup > Search > Search parameters** and setting **Enable lookup for search** to **Yes** on the **General** tab.</span></span>

<span data-ttu-id="9208f-150">[![لقطة شاشة لصفحة معلمات البحث.](../media/search-parameters.png)](../media/search-parameters.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9208f-150">[![Screenshot of the search parameters page.](../media/search-parameters.png)](../media/search-parameters.png#lightbox)</span></span>

<span data-ttu-id="9208f-151">بالنسبة لإدخال بند أمر المبيعات، يكون السلوك الافتراضي هو فتح صفحة **البحث عن المنتج** عندما تبدأ في إدخال حقل **رقم الصنف**، ثم اضغط على المفتاح **Tab**.</span><span class="sxs-lookup"><span data-stu-id="9208f-151">For sales order line entry, the default behavior is to open the **Product search** page when you start typing in the **Item number** field and then press the **Tab** key.</span></span>

<span data-ttu-id="9208f-152">[![لقطة شاشة لصفحة البحث عن المنتج تعرض جدولاً بالمنتجات التي تم العثور عليها.](../media/product-search.png)](../media/product-search.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="9208f-152">[![Screenshot of the Product search page showing a table of found products.](../media/product-search.png)](../media/product-search.png#lightbox)</span></span>

<span data-ttu-id="9208f-153">تقوم صفحة **البحث عن المنتج** بتغيير السياق أثناء إنشاء بند الأمر ويمكن اعتباره تدخلياً دون داعٍ.</span><span class="sxs-lookup"><span data-stu-id="9208f-153">The **Product search** page changes the context during order line creation and might be considered unnecessarily intrusive.</span></span>

<span data-ttu-id="9208f-154">إذا كنت تفضل الحصول على نتائج البحث في عملية بحث ولا تفقد السياق أثناء إدخال بند الأمر، فيمكنك استخدام بحث البحث بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="9208f-154">If you prefer to get the search results in a lookup and not lose context during order line entry, you can use the search lookup instead.</span></span> <span data-ttu-id="9208f-155">إذا كنت تبحث عن منتج أو متغير منتج، لكنك لم تحدد أي شيء في البحث وتضغط على المفتاح **Tab**، فسيتم عرض صفحة **البحث عن المنتج**.</span><span class="sxs-lookup"><span data-stu-id="9208f-155">If you search for a product or product variant, but you don't select anything in the lookup and press the **Tab** key, the **Product search** page will display.</span></span>
