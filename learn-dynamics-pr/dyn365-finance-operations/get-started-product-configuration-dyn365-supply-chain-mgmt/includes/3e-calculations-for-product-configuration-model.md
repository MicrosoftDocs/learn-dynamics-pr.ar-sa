---
ms.openlocfilehash: 9ebe31d0b78e2c4a9c85aa34f4f2ca9063327b62
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6073737"
---


<span data-ttu-id="f1a41-101">يمكن استخدام الحسابات للعمليات الحسابية أو المنطقية.</span><span class="sxs-lookup"><span data-stu-id="f1a41-101">Calculations can be used for arithmetic or logical operations.</span></span> <span data-ttu-id="f1a41-102">وهي تستكمل قيود التعبيرات في نماذج تكوين المنتج.</span><span class="sxs-lookup"><span data-stu-id="f1a41-102">They complement expression constraints in product configuration models.</span></span> <span data-ttu-id="f1a41-103">يمكنك تحديد الحسابات في صفحة **تفاصيل نموذج تكوين المنتج المستند إلى قيد** ثم إنشاء تعبيرات للعمليات الحسابية في محرر التعبير.</span><span class="sxs-lookup"><span data-stu-id="f1a41-103">You can define calculations on the **Constraint-based product configuration model details** page and then build expressions for the calculations in the expression editor.</span></span> 

<span data-ttu-id="f1a41-104">الحساب هو العنصر الذي يمكنك استخدامه في نموذج تكوين المنتج.</span><span class="sxs-lookup"><span data-stu-id="f1a41-104">A calculation is an element that you can use in a product configuration model.</span></span> <span data-ttu-id="f1a41-105">تستكمل العمليات الحسابية القيود عن طريق السماح لك باستخدام الأرقام العشرية لحساب القيم عند تكوين منتج.</span><span class="sxs-lookup"><span data-stu-id="f1a41-105">Calculations complement constraints by letting you use decimal numbers to calculate values when you configure a product.</span></span> <span data-ttu-id="f1a41-106">بالإضافة إلى ذلك، تحتوي العمليات الحسابية على مجموعة أكبر من عوامل التشغيل المتوفرة بخلاف ما تحتويه القيود.</span><span class="sxs-lookup"><span data-stu-id="f1a41-106">Additionally, calculations have a larger set of available operators than constraints have.</span></span>

<span data-ttu-id="f1a41-107">مثل القيد، يتم ربط الحساب بمكون محدد في نموذج تكوين منتج ولا يمكن إعادة استخدامه بواسطة مكون آخر أو مشاركته معه.</span><span class="sxs-lookup"><span data-stu-id="f1a41-107">Like a constraint, a calculation is associated with a specific component in a product configuration model and can't be reused by or shared with another component.</span></span> <span data-ttu-id="f1a41-108">والاختلاف الهام بين العمليات الحسابية والقيود هو أن العمليات الحسابية إلزامية (أحادية الاتجاه)، بينما تعتبر القيود توضيحية (ثنائية الاتجاه).</span><span class="sxs-lookup"><span data-stu-id="f1a41-108">One important difference between calculations and constraints is that calculations are imperative (unidirectional), whereas constraints are declarative (bi-directional).</span></span>

<span data-ttu-id="f1a41-109">تتكون عملية الحساب من سمة هدف وتعبير حساب.</span><span class="sxs-lookup"><span data-stu-id="f1a41-109">A calculation consists of a target attribute and a calculation expression.</span></span>

### <a name="target-attribute"></a><span data-ttu-id="f1a41-110">سمة الهدف</span><span class="sxs-lookup"><span data-stu-id="f1a41-110">Target attribute</span></span>

<span data-ttu-id="f1a41-111">السمة الهدف هي سمة تستلم نتيجة تعبير الحساب.</span><span class="sxs-lookup"><span data-stu-id="f1a41-111">A target attribute is an attribute that receives the result of the calculation expression.</span></span>

<span data-ttu-id="f1a41-112">في التعبير التالي، السمة الهدف هي مقاس مفرض المائدة:</span><span class="sxs-lookup"><span data-stu-id="f1a41-112">In the following expression, the target attribute is a tablecloth measurement:</span></span>

> <span data-ttu-id="f1a41-113">**التعبير:** إذا كان [decimalAttribute1 <= decimalAttribute2, صواب، خطأ]</span><span class="sxs-lookup"><span data-stu-id="f1a41-113">**Expression:** If [decimalAttribute1 <= decimalAttribute2, True, False]</span></span>

<span data-ttu-id="f1a41-114">**DecimalAttribute1** هو طول الطاولة و **decimalAttribute2** هو طول مفرش الطاولة.</span><span class="sxs-lookup"><span data-stu-id="f1a41-114">**DecimalAttribute1** is the table length and  **decimalAttribute2** is the tablecloth length.</span></span> <span data-ttu-id="f1a41-115">يرجع التعبير القيمة **صواب** إلى السمة الهدف إذا كان  **decimalAttribute2** أكبر من أو يساوي **decimalAttribute1**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-115">The expression returns the value **True** to the target attribute if **decimalAttribute2** is greater than or equal to **decimalAttribute1**.</span></span> <span data-ttu-id="f1a41-116">بخلاف ذلك، يُرجع التعبير  **خطأ**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-116">Otherwise, the expression returns **False**.</span></span>
<span data-ttu-id="f1a41-117">بالتالي، يكون مقاس مفرش الطاولة مقبولا إذا كان طول مفرش الطاولة هو نفس طول الطاولة أو يتجاوزه.</span><span class="sxs-lookup"><span data-stu-id="f1a41-117">Therefore, the tablecloth measurement is acceptable if the tablecloth length is the same as or exceeds the length of the table.</span></span>

<span data-ttu-id="f1a41-118">يمكن تعيين كافة أنواع السمات التي تدعمها وحدة تكوين المنتج إلى سمات هدف باستثناء النص بدون قائمة ثابتة.</span><span class="sxs-lookup"><span data-stu-id="f1a41-118">All attribute types that the product configurator supports can be set to target attributes except text without a fixed list.</span></span>

<span data-ttu-id="f1a41-119">لا يمكن لقيمة السمة الهدف تقييد قيم سمات الإدخال نظرا لأن العمليات الحسابية تكون أحادية الاتجاه.</span><span class="sxs-lookup"><span data-stu-id="f1a41-119">The value of a target attribute cannot restrict the values of the input attributes because calculations are unidirectional.</span></span> <span data-ttu-id="f1a41-120">بالتالي، يتم تعيين قيمة السمة الهدف استناداً إلى التغييرات في قيمة سمات الإدخال ولكن التغيير في قيمة الهدف لا يؤثر على قيمة سمات الإدخال.</span><span class="sxs-lookup"><span data-stu-id="f1a41-120">Therefore, the value of the target attribute is set based on changes in the value of the input attributes, but a change in the value of the target doesn't affect the value of the input attributes.</span></span> <span data-ttu-id="f1a41-121">يختلف هذا السلوك عن سلوك القيود.</span><span class="sxs-lookup"><span data-stu-id="f1a41-121">This behavior differs from the behavior for constraints.</span></span> <span data-ttu-id="f1a41-122">تحدث القيود في كلا الاتجاهين.</span><span class="sxs-lookup"><span data-stu-id="f1a41-122">Constraints occur in both directions.</span></span>

<span data-ttu-id="f1a41-123">**مثال:**</span><span class="sxs-lookup"><span data-stu-id="f1a41-123">**Example:**</span></span>

<span data-ttu-id="f1a41-124">في التعبير التالي، يكون الهدف من عملية الحساب هو طول سلك الطاقة وقيمة الإدخال هي لون.</span><span class="sxs-lookup"><span data-stu-id="f1a41-124">In the following expression, the target for the calculation is the length of a power cord and the input value is a color.</span></span>

> <span data-ttu-id="f1a41-125">**التعبير:** [إذا كان اللون == "أخضر"، 1.5، 1.0]</span><span class="sxs-lookup"><span data-stu-id="f1a41-125">**Expression:** [If Color == "Green", 1.5, 1.0]</span></span>

<span data-ttu-id="f1a41-126">عند تكوين الصنف، يتم تعيين طول سلك الطاقة إلى  **1.5** إذا قمت بتحديد  **أخضر** كقيمة لسمة اللون.</span><span class="sxs-lookup"><span data-stu-id="f1a41-126">When you configure the item, the length of the power cord is set to **1.5** if you specify **Green** as the value of the color attribute.</span></span> <span data-ttu-id="f1a41-127">إذا قمت بتحديد لون آخر، يتم تعيين الطول إلى  **1.0**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-127">If you specify any other color, the length is set to **1.0**.</span></span> <span data-ttu-id="f1a41-128">ومع ذلك، نظراً لأن العمليات الحسابية تكون أحادية الاتجاه، لا تقوم عملية الحساب بتعيين قيمة سمة اللون إلى اللون  **الأخضر**  إذا قمت بتحديد طول  **1.5**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-128">However, because calculations are unidirectional, the calculation doesn't set the value of the color attribute to **Green** if you specify a length of **1.5**.</span></span>


<span data-ttu-id="f1a41-129">إذا كانت السمة الهدف من نوع عدد صحيح، ولكن عملية الحساب تقوم بإنشاء رقم عشري، يتم إرجاع جزء العدد الصحيح فقط من النتيجة المحسوبة، وتتم إزالة الجزء العشري، ولا يتم تقريب النتيجة.</span><span class="sxs-lookup"><span data-stu-id="f1a41-129">If a target attribute is of the integer type, but a calculation generates a decimal number, only the integer part of the calculated result is returned, the decimal part is removed, and the result isn't rounded.</span></span> <span data-ttu-id="f1a41-130">على سبيل المثال، يتم عرض نتيجة 12.70 في صورة 12.</span><span class="sxs-lookup"><span data-stu-id="f1a41-130">For example, a result of 12.70 is shown as 12.</span></span>

<span data-ttu-id="f1a41-131">تحدث العمليات الحسابية عند توفير قيمة لكافة سمات الإدخال.</span><span class="sxs-lookup"><span data-stu-id="f1a41-131">Calculations occur when a value has been provided for all input attributes.</span></span> <span data-ttu-id="f1a41-132">يمكنك الكتابة فوق القيمة التي يتم حسابها للسمة الهدف ما لم يتم تعيين السمة الهدف كمخفية أو للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="f1a41-132">You can overwrite the value that is calculated for the target attribute unless the target attribute is set as hidden or read-only.</span></span>

### <a name="set-up-a-target-attribute-as-hidden-or-read-only"></a><span data-ttu-id="f1a41-133">إعداد سمة هدف كمخفية أو للقراءة فقط</span><span class="sxs-lookup"><span data-stu-id="f1a41-133">Set up a target attribute as hidden or read-only</span></span>

<span data-ttu-id="f1a41-134">لتعيين سمة كمخفية أو للقراءة فقط، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="f1a41-134">To set an attribute as hidden or read-only, follow these steps.</span></span>

1.  <span data-ttu-id="f1a41-135">حدد  **إدارة معلومات المنتج > المنتجات > نماذج تكوين المنتجات**</span><span class="sxs-lookup"><span data-stu-id="f1a41-135">Select **Product information management > Products > Product configuration models**.</span></span>

2.  <span data-ttu-id="f1a41-136">حدد نموذج تكوين منتج، ثم في جزء الإجراء، حدد  **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-136">Select a product configuration model and then, on the Action Pane, select **Edit**.</span></span>

3.  <span data-ttu-id="f1a41-137">في صفحة  **تفاصيل نموذج تكوين المنتج المستند إلى قيد** ، حدد السمة المطلوب استخدامها كسمة هدف.</span><span class="sxs-lookup"><span data-stu-id="f1a41-137">On the **Constraint-based product configuration model details** page, select the attribute to use as a target attribute.</span></span>

4.  <span data-ttu-id="f1a41-138">في علامة التبويب السريعة  **السمات** ، حدد  **مخفية**  أو  **للقراءة فقط**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-138">On the **Attributes** FastTab, select **Hidden** or **Read-only**.</span></span>

    <span data-ttu-id="f1a41-139">[![لقطة شاشة لعلامة التبويب السريعة السمات مع تمييز سمة "للقراءة فقط".](../media/read-only-attribute.png)](../media/read-only-attribute.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f1a41-139">[![Screenshot of the Atrributes FastTab highlighting the Read-only attribute.](../media/read-only-attribute.png)](../media/read-only-attribute.png#lightbox)</span></span>

<span data-ttu-id="f1a41-140">لا يمكن الكتابة فوق عملية الحساب بالقيم التي قمت بتعيينها.</span><span class="sxs-lookup"><span data-stu-id="f1a41-140">A calculation cannot overwrite the values that you set.</span></span> <span data-ttu-id="f1a41-141">القيم التي تقوم بتعيينها عند تكوين منتج هي القيم التي يتم استخدامها.</span><span class="sxs-lookup"><span data-stu-id="f1a41-141">The values that you set when you configure a product are the values that are used.</span></span> <span data-ttu-id="f1a41-142">لا يمكن لعملية الحساب التي تحدث عند تغيير قيم الإدخال في الحساب الكتابة فوق القيم التي توفرها لسمة معينة.</span><span class="sxs-lookup"><span data-stu-id="f1a41-142">The calculation that occurs when the input values in a calculation are changed can't overwrite the values that you provide for a specific attribute.</span></span>

<span data-ttu-id="f1a41-143">إذا قمت بإزالة قيمة إدخال في عملية حساب، ستتم إزالة قيمة السمة الهدف أيضاًً.</span><span class="sxs-lookup"><span data-stu-id="f1a41-143">If you remove an input value in a calculation, the value of the target attribute is also removed.</span></span>

## <a name="error-message---model-is-in-contradiction"></a><span data-ttu-id="f1a41-144">رسالة الخطأ - النموذج متعارض</span><span class="sxs-lookup"><span data-stu-id="f1a41-144">Error message - Model is in contradiction</span></span>

<span data-ttu-id="f1a41-145">تظهر رسالة الخطأ **النموذج متعارض** عندما تتضمن العملية الحسابية خطأ أو عندما توجد تعارضات في واحد أو أكثر من القيود.</span><span class="sxs-lookup"><span data-stu-id="f1a41-145">The **Model is in contradiction** error message is shown when a calculation includes an error or when a contradiction exists in one or more constraints.</span></span>

<span data-ttu-id="f1a41-146">فيما يلي المواقف التي يمكن أن تحدث فيها أخطاء في العمليات الحسابية:</span><span class="sxs-lookup"><span data-stu-id="f1a41-146">Situations where errors can occur in calculations are when:</span></span>

-   <span data-ttu-id="f1a41-147">قسمة القيمة على 0 (صفر).</span><span class="sxs-lookup"><span data-stu-id="f1a41-147">A value is divided by 0 (zero).</span></span>

-   <span data-ttu-id="f1a41-148">وجود تعارض بين العنصرين التاليين:</span><span class="sxs-lookup"><span data-stu-id="f1a41-148">A conflict exists between the following two elements:</span></span>

    -   <span data-ttu-id="f1a41-149">القيم المتوفرة لسمة ولكنها محدودة بقيد</span><span class="sxs-lookup"><span data-stu-id="f1a41-149">The values that are available for an attribute and are limited by a constraint</span></span>

    -   <span data-ttu-id="f1a41-150">قيمة تم إنشاؤها بواسطة عملية حساب</span><span class="sxs-lookup"><span data-stu-id="f1a41-150">A value that is generated by a calculation</span></span>

-   <span data-ttu-id="f1a41-151">القيم التي يتم إرجاعها بواسطة عملية الحساب تقع خارج مجال السمة، على سبيل المثال، عدد صحيح من [1.. 10] يتم حسابه إلى 0.</span><span class="sxs-lookup"><span data-stu-id="f1a41-151">The values that are returned by the calculation are outside the domain of the attribute, for example, an integer from [1..10] that is calculated to 0.</span></span>

## <a name="error-message---after-successfully-validating-a-product-model"></a><span data-ttu-id="f1a41-152">رسالة الخطأ - بعد التحقق من صحة طراز منتج بنجاح</span><span class="sxs-lookup"><span data-stu-id="f1a41-152">Error message - After successfully validating a product model</span></span>

<span data-ttu-id="f1a41-153">إذا استلمت رسالة الخطأ **بعد التحقق من صحة طراز منتج بنجاح**، لا يتم تضمين العمليات الحسابية في عملية التحقق من الصحة.</span><span class="sxs-lookup"><span data-stu-id="f1a41-153">If you receive the **After successfully validating a product model** error message, calculations are not included in the validation.</span></span> <span data-ttu-id="f1a41-154">يجب اختبار نموذج تكوين المنتج للبحث عن الأخطاء في العمليات الحسابية.</span><span class="sxs-lookup"><span data-stu-id="f1a41-154">You must test the product configuration model to find errors in calculations.</span></span> <span data-ttu-id="f1a41-155">لاختبار نموذج تكوين منتج، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f1a41-155">To test a product configuration model, follow these steps:</span></span>

1.  <span data-ttu-id="f1a41-156">حدد  **إدارة معلومات المنتج > المنتجات > نماذج تكوين المنتجات**</span><span class="sxs-lookup"><span data-stu-id="f1a41-156">Select **Product information management > Products > Product configuration models**.</span></span>

2.  <span data-ttu-id="f1a41-157">حدد نموذج تكوين منتج، ثم في جزء الإجراء، في المجموعة  **تشغيل** ، حدد  **اختبار**.</span><span class="sxs-lookup"><span data-stu-id="f1a41-157">Select a product configuration model and then, on the Action Pane, in the **Run** group, select **Test**.</span></span>

