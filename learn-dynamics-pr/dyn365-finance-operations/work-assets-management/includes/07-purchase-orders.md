---
ms.openlocfilehash: 449b69576085ec08c4fec663796f40fecdef1047
ms.sourcegitcommit: 9134765f329ce8893f21b7a57a08277d75913363
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/16/2021
ms.locfileid: "6072530"
---
<span data-ttu-id="5407b-101">هذه الوحدة توضح كيفية إنشاء أصول استناداً إلى أوامر الشراء.</span><span class="sxs-lookup"><span data-stu-id="5407b-101">This unit explains how you can create assets based on purchase orders.</span></span> <span data-ttu-id="5407b-102">ومع ذلك، لإكمال هذه العملية، تحتاج أولاً إلى قائمة بأصناف الأصول التي يمكن استخدامها كأساس لإنشاء أصول لمهام الصيانة في إدارة الأصول.</span><span class="sxs-lookup"><span data-stu-id="5407b-102">However, to complete this process, you first need a list of asset items that can then be used as a basis for creating assets for maintenance jobs in Asset Management.</span></span> 

<span data-ttu-id="5407b-103">تتيح لك أصناف الأصول إمكانية عرض قائمة بكافة بنود أمر الشراء التي تم إنشاؤها في هذه الأصناف.</span><span class="sxs-lookup"><span data-stu-id="5407b-103">Asset items allow you to view a list of all purchase order lines that were created on those items.</span></span> <span data-ttu-id="5407b-104">والغرض من هذه الوظيفة هو مساعدتك على إنشاء أصل في إدارة الأصول استناداً إلى أمر شراء.</span><span class="sxs-lookup"><span data-stu-id="5407b-104">The purpose of this functionality is to help you create an asset in Asset Management based on a purchase order.</span></span>

<span data-ttu-id="5407b-105">المهمة الأولي هي إعداد الأصناف التي سيتم استخدامها لإنشاء أصول من أمر شراء في **أصناف الأصول**.</span><span class="sxs-lookup"><span data-stu-id="5407b-105">Your first task is to set up the items that will be used for creating assets from a purchase order in **Asset items**.</span></span> <span data-ttu-id="5407b-106">بعد إنشاء بند أمر شراء، ستقوم بعد ذلك بإنشاء الأصول في "الأصول قيد الانتظار".</span><span class="sxs-lookup"><span data-stu-id="5407b-106">After creating a purchase order line, you will then create the assets in Pending assets.</span></span> <span data-ttu-id="5407b-107">ومن الممكن تحديد مرحلة أمر الشراء التي يجب فيها إنشاء الأصل.</span><span class="sxs-lookup"><span data-stu-id="5407b-107">It is possible to decide at which stage of the purchase order that the asset should be created.</span></span>

> [!NOTE]
> <span data-ttu-id="5407b-108">يجب إعداد كافة المنتجات في وحدة إدارة معلومات المنتجات في Supply Chain Management، قبل أن تتمكن من إنشاء هذه الأصناف.</span><span class="sxs-lookup"><span data-stu-id="5407b-108">All products must be set up in the Product information management module in Supply Chain Management, before you can establish these items.</span></span>

## <a name="create-asset-items"></a><span data-ttu-id="5407b-109">إنشاء أصناف الأصول</span><span class="sxs-lookup"><span data-stu-id="5407b-109">Create asset items</span></span>
<span data-ttu-id="5407b-110">اتبع الخطوات الآتية لإنشاء أصناف الأصول:</span><span class="sxs-lookup"><span data-stu-id="5407b-110">Follow these steps to create asset items:</span></span>

1.  <span data-ttu-id="5407b-111">انتقل إلى **إدارة الأصول > الإعداد > الأصول > الأصناف** ثم حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="5407b-111">Go to **Asset Management > Setup > Assets > Items** and then select **New**.</span></span>
2.  <span data-ttu-id="5407b-112">في حقل **رقم الصنف**، حدد رقم الصنف من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="5407b-112">In the **Item number** field, select the item number from the drop-down menu.</span></span> 
3.  <span data-ttu-id="5407b-113">في علامة التبويب السريعة **عام** في حقل **نوع الأصل**، حدد نوع الأصل من القائمة المنسدلة.</span><span class="sxs-lookup"><span data-stu-id="5407b-113">On the **General** FastTab, in the **Asset type** field, select the asset type from the drop-down menu.</span></span>
4.  <span data-ttu-id="5407b-114">وإذا لزم الأمر، يمكنك تحديد **الشركة المصنعة** و **والطراز** للصنف.</span><span class="sxs-lookup"><span data-stu-id="5407b-114">If required, you can select the **Manufacturer** and **Model** for the item.</span></span>
5.  <span data-ttu-id="5407b-115">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5407b-115">Select **Save**.</span></span> <span data-ttu-id="5407b-116">وبعد حفظ صنف الأصل، يظهر اسم المنتج تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="5407b-116">After you have saved the asset item, the product name automatically appears.</span></span>

<span data-ttu-id="5407b-117">الصورة الآتية مثال لصفحة **أصناف الأصول** في **إدارة الأصول > الإعداد > الأصول > الأصناف**.</span><span class="sxs-lookup"><span data-stu-id="5407b-117">The following image is an example of the **Asset items** page in **Asset Management > Setup > Assets > Items**.</span></span>

![لقطة شاشة لصفحة "أصناف الأصول" توضح زر "جديد".](../media/asset-items-ssm.png)
 

<span data-ttu-id="5407b-119">شاهد الفيديو الآتي لمعرفة كيفية إنشاء الأصول استناداً إلى أوامر الشراء.</span><span class="sxs-lookup"><span data-stu-id="5407b-119">Watch the following video to see how to create assets based on purchase orders.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4oXeq]


## <a name="create-assets-from-pending-assets"></a><span data-ttu-id="5407b-120">إنشاء أصول من أصول قيد الانتظار</span><span class="sxs-lookup"><span data-stu-id="5407b-120">Create assets from pending assets</span></span>
<span data-ttu-id="5407b-121">لإنشاء أصول من أصول قيد الانتظار، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="5407b-121">To create assets from pending assets, follow these steps:</span></span>

1.  <span data-ttu-id="5407b-122">انتقل إلى **إدارة الأصول > عام > الأصول > أصول قيد الانتظار**، حيث ستشاهد قائمة بكافة أوامر الشراء التي تستند إلى الأصناف المحددة في **أصناف الأصول**.</span><span class="sxs-lookup"><span data-stu-id="5407b-122">Go to **Asset Management > Common > Assets > Pending Assets**, where you will see a list of all of the purchase orders that are based on the items that are selected in **Asset items**.</span></span>

    <span data-ttu-id="5407b-123">[![لقطة شاشة لصفحة "الأصول قيد الانتظار" توضح أبعاد العرض.](../media/pending-assets-ssm.png)](../media/pending-assets-ssm.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="5407b-123">[![Screenshot of the Pending assets page highlighting Display dimensions.](../media/pending-assets-ssm.png)](../media/pending-assets-ssm.png#lightbox)</span></span>

2.  <span data-ttu-id="5407b-124">إذا كنت ترغب في معرفة المزيد عن صنف أصل محدد، فحدد الرقم المرجعي في بند أمر الشراء، حيث ستشاهد علامات التبويب السريعة **نظرة عامة** و **الأصل** و **أبعاد المخزون**.</span><span class="sxs-lookup"><span data-stu-id="5407b-124">If you want to learn more about a specific asset item, select the Reference number on a purchase order line, where you will see the **Overview**, **Asset**, and **Inventory dimensions** FastTabs.</span></span>
3.  <span data-ttu-id="5407b-125">يمكنك تعديل البُعد الذي يجب عرضه في علامة التبويب السريعة **أبعاد المخزون**.</span><span class="sxs-lookup"><span data-stu-id="5407b-125">You can modify which dimension should be displayed in the **Inventory dimensions** FastTab.</span></span> <span data-ttu-id="5407b-126">حدد **أبعاد العرض** من القائمة الرئيسية في أعلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="5407b-126">Select **Display dimensions** from the main menu at the top of the page.</span></span> <span data-ttu-id="5407b-127">سيتم فتح مربع حوار **أبعاد العرض**، وستتمكن من إجراء التحديدات.</span><span class="sxs-lookup"><span data-stu-id="5407b-127">The **Display dimensions** dialog box will open, and you will be able to make your selections.</span></span> 
1. <span data-ttu-id="5407b-128">بعد مراجعة المعلومات فيما يتعلق بهذا الأصل، ستقوم بإنشاء أصل استناداً إلى بند أمر الشراء.</span><span class="sxs-lookup"><span data-stu-id="5407b-128">After reviewing information regarding this asset, you will create an asset based on a purchase order line.</span></span> <span data-ttu-id="5407b-129">قم بالرجوع إلى صفحة قائمة **الأصول قيد الانتظار** وحدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="5407b-129">Go back to the **Pending assets** list page and select **Edit**.</span></span>
6.  <span data-ttu-id="5407b-130">عندما تكون في وضع **تحرير**، حدد خانة الاختيار في عمود **وضع علامة** لهذا البند وحدد **إنشاء أصول** من شريط القوائم.</span><span class="sxs-lookup"><span data-stu-id="5407b-130">When you are in **Edit** mode, select the check box in the **Mark** column for that line and select **Create assets** from the menu bar.</span></span> <span data-ttu-id="5407b-131">سيتم عرض رسالة تخبرك بمعرِّف الأصل.</span><span class="sxs-lookup"><span data-stu-id="5407b-131">A message will display informing you of the asset ID.</span></span>
7.  <span data-ttu-id="5407b-132">إذا كنت ترغب في إضافة مزيد من المعلومات، فيمكنك الانتقال إلى قائمة **جميع الأصول** وتحديد الأصل ثم تحديد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="5407b-132">If you want to add more information, you can go to the **All assets** list, select the asset, and then select **Edit**.</span></span>


<span data-ttu-id="5407b-133">وإذا لم تعد هناك حاجة إليه، فيمكنك أيضاً حذف أصل قيد الانتظار.</span><span class="sxs-lookup"><span data-stu-id="5407b-133">If it is no longer needed, you can also delete a pending asset.</span></span> 

1. <span data-ttu-id="5407b-134">حدد **تحرير** وحدد مربع علامة الاختيار أمام البند، ثم حدد **تجاهل الأصول قيد الانتظار** من شريط القوائم.</span><span class="sxs-lookup"><span data-stu-id="5407b-134">Select **Edit**, select the check mark box in front of the line, and then select **Discard pending assets** from the menu bar.</span></span> 
1. <span data-ttu-id="5407b-135">سيتم عرض رسالة تخبرك بمعرِّف الأصل.</span><span class="sxs-lookup"><span data-stu-id="5407b-135">A message will display informing you of the asset ID.</span></span> <span data-ttu-id="5407b-136">لا تؤدي هذه العملية إلى حذف أمر الشراء أو أمر المبيعات.</span><span class="sxs-lookup"><span data-stu-id="5407b-136">This process does not delete the purchase order or the sales order.</span></span>

> [!NOTE]
> <span data-ttu-id="5407b-137">يتم تحويل كافة أبعاد المنتجات (الحجم واللون والتكوين وما إلى ذلك) تلقائياً إلى سمات الأصول.</span><span class="sxs-lookup"><span data-stu-id="5407b-137">All product dimensions (size, color, configuration, and so on) are automatically transferred to the asset attributes.</span></span> <span data-ttu-id="5407b-138">ويتم تخزين أبعاد التعقب (رقم تسلسلي) مباشرةً إلى الأصل عند إنشاء الأصل.</span><span class="sxs-lookup"><span data-stu-id="5407b-138">Tracking dimensions (serial number) are stored directly on the asset when the asset is created.</span></span>


## <a name="find-pending-assets"></a><span data-ttu-id="5407b-139">البحث عن الأصول قيد الانتظار</span><span class="sxs-lookup"><span data-stu-id="5407b-139">Find pending assets</span></span>
<span data-ttu-id="5407b-140">للمساعدة على تنظيم إنشاء أصول من عملية الأصول قيد الانتظار، ويمكنك استلام إخطار في كل مرة يكون الأصل قيد الانتظار جاهزاً للإنشاء كأصل.</span><span class="sxs-lookup"><span data-stu-id="5407b-140">To help streamline the create assets from pending assets process, you can receive a notification every time a pending asset is ready to be created as an asset.</span></span> 

1.  <span data-ttu-id="5407b-141">انتقل إلى **إدارة الأصول > دوري > الأصل > عدد الأصول قيد الانتظار**.</span><span class="sxs-lookup"><span data-stu-id="5407b-141">Go to **Asset Management > Periodic > Asset > Pending asset count**.</span></span>
2.  <span data-ttu-id="5407b-142">في علامة التبويب السريعة **إجراء في الخلفية**، يمكنك إعداد هذه المهمة لإجرائها كمهمة دُفعات، مرة يومياً مثلاً.</span><span class="sxs-lookup"><span data-stu-id="5407b-142">On the **Run in background** FastTab, you can set up this job to run as a batch job, for example, once each day.</span></span> 
3.  <span data-ttu-id="5407b-143">حدد **تكرار** لفتح مربع حوار **تحديد التكرار**.</span><span class="sxs-lookup"><span data-stu-id="5407b-143">Select **Recurrence** to open the **Define recurrence** dialog box.</span></span> <span data-ttu-id="5407b-144">من مربع الحوار، يمكنك تحديد **تاريخ البدء** و **المنطقة الزمنية** و **تاريخ الانتهاء** و **نمط التكرار**.</span><span class="sxs-lookup"><span data-stu-id="5407b-144">From the dialog box, you can define the **Start date**, **Time zone**, **End date**, and **Recurrence pattern**.</span></span>
4.  <span data-ttu-id="5407b-145">عند الانتهاء، حدد **موافق** لإجراء المهمة وتحديث القائمة في **الأصول قيد الانتظار**.</span><span class="sxs-lookup"><span data-stu-id="5407b-145">When you are finished, select **OK** to run the job and update the list in **Pending assets**.</span></span>

> [!CAUTION]
> <span data-ttu-id="5407b-146">إذا تغيرت البيانات في أمر شراء بعد إنشاء الأصل استناداً إلى صنف محدد، فلن يتم تطبيق هذه التغييرات على الأصل.</span><span class="sxs-lookup"><span data-stu-id="5407b-146">If data is changed on a purchase order after you have created an asset based on the appertaining item, those changes will not be reflected on the asset.</span></span>

