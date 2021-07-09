---
ms.openlocfilehash: 1fc4649baafd88d5e0d0303de1bd2b8d1764209b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071363"
---
<span data-ttu-id="b1612-101">عندما تحتاج إلى تغيير سلوك عنصر ما، فإنك تنشئ ملحقاً لذلك العنصر.</span><span class="sxs-lookup"><span data-stu-id="b1612-101">When you need to change the behavior of an element, you create an extension of that element.</span></span> <span data-ttu-id="b1612-102">تتطلب بعض العناصر كتابة تعليمات برمجية لتغيير سلوكها، مثل إضافة معالج الأحداث.</span><span class="sxs-lookup"><span data-stu-id="b1612-102">Some elements require code to be written to change their behavior, such as adding an event handler.</span></span> <span data-ttu-id="b1612-103">في حالات أخرى، يمكنك إنشاء ملحق للفئة لتغيير تكوين العنصر.</span><span class="sxs-lookup"><span data-stu-id="b1612-103">In other cases, you might create a class extension to change an element's makeup.</span></span>

## <a name="class-extensions"></a><span data-ttu-id="b1612-104">ملحقات الفئة</span><span class="sxs-lookup"><span data-stu-id="b1612-104">Class extensions</span></span> 

<span data-ttu-id="b1612-105">لتوسيع منطق الأعمال المرتبط بجدول، يمكنك إنشاء فئة زيادة.</span><span class="sxs-lookup"><span data-stu-id="b1612-105">To extend the business logic that is related to a table, you create an augmentation class.</span></span> <span data-ttu-id="b1612-106">إذا كنت ترغب في إضافة حقل معرّف آخر إلى الجدول وتعبئته، فيمكنك إنشاء معالج أحداث البيانات لحدث الإدراج، ثم تنفيذ المنطق لملء الحقل الجديد في معالج الأحداث هذا.</span><span class="sxs-lookup"><span data-stu-id="b1612-106">If you wanted to add another ID field to the table and have it filled, you would create a data event handler for the Inserting event and then implement the logic to fill the new field in that event handler.</span></span> <span data-ttu-id="b1612-107">يمكنك إنشاء فئة تقوي الجدول وتتيح الوصول إلى حقول الجدول وطرقه بطريقة سهلة القراءة.</span><span class="sxs-lookup"><span data-stu-id="b1612-107">You can create a class that augments the table and enables access to the table's fields and methods in an easy-to-read manner.</span></span> <span data-ttu-id="b1612-108">عند إنشاء ملحق فئة، يجب عليك تزيينه بالسمة `ExtensionOf`، واستخدام اللاحقة`_Extension`، والإشارة إلى الفئة باعتبارها `final`.</span><span class="sxs-lookup"><span data-stu-id="b1612-108">When creating a class extension, you must decorate it with the `ExtensionOf` attribute, use the `_Extension` suffix, and indicate the class as `final`.</span></span>

<span data-ttu-id="b1612-109">فيما يلي مثال لإنشاء فئة توسع `InventTable`.</span><span class="sxs-lookup"><span data-stu-id="b1612-109">The following is an example of creating a class that extends `InventTable`.</span></span> <span data-ttu-id="b1612-110">يمكن بعد ذلك إضافة الطرق إلى هذه الفئة المعززة حيث يتم استخدام التعليق.</span><span class="sxs-lookup"><span data-stu-id="b1612-110">Methods can then be added to this augmented class where the comment is used.</span></span>
```xpp
[ExtensionOf(tableStr(InventTable))]
final class InventTableNew_Extension
{
    public void newDefaultInventLocationId()
     {
     //enter your code here
     }
}
```
## <a name="event-handlers"></a><span data-ttu-id="b1612-111">معالجات الأحداث</span><span class="sxs-lookup"><span data-stu-id="b1612-111">Event handlers</span></span> 

<span data-ttu-id="b1612-112">معالج الأحداث هو وسيلة لك لكتابة أو نسخ التعليمات البرمجية إلى عنصر يتم تشغيله عند حدوث حدث معين، بالمثل عندما يتم تعديل حقل أو عندما يتم مسح أحد السجلات.</span><span class="sxs-lookup"><span data-stu-id="b1612-112">An event handler is a way for you to write or copy code to an element that runs when a certain event occurs, such as when a field is modified or a record is deleted.</span></span> <span data-ttu-id="b1612-113">تحتوي بعض العناصر، مثل الجداول والنماذج، على عقدة **الأحداث** في نافذة المصمم والتي، عند توسيعها، تسرد كافة الاحداث المرتبطة بهذا العنصر.</span><span class="sxs-lookup"><span data-stu-id="b1612-113">Some elements, like tables and forms, contain an **Events** node in the designer window that, when expanded, lists all the events that are associated with that element.</span></span> <span data-ttu-id="b1612-114">إذا كنت بحاجة إلى إضافة سلوك إضافي غير موجود حالياً في عنصر ما، فيجب عليك إنشاء ملحق لهذا العنصر، ثم إضافة معالج الأحداث إلى العنصر الممتد.</span><span class="sxs-lookup"><span data-stu-id="b1612-114">If you need to add supplementary behavior that doesn't currently exist in an element, you should create an extension of that element, and then add an event handler to the extended element.</span></span>

<span data-ttu-id="b1612-115">فيما يلي طرق معالجات الأحداث التي يتم سحبها من جدول `CustTable`.</span><span class="sxs-lookup"><span data-stu-id="b1612-115">The following are methods for event handlers that are pulled from the `CustTable` table.</span></span> <span data-ttu-id="b1612-116">يمكن نسخ هذه الأساليب وإضافتها إلى العنصر الممتد أو الفئة الخاصة بك بالنقر بزر الماوس الأيمن فوق الحدث في نافذة مصمم العناصر ثمّ تحديد **نسخ طريقة معالج الأحداث**.</span><span class="sxs-lookup"><span data-stu-id="b1612-116">These methods can be copied and added to your extended element or class by right-clicking the event in the element designer window and selecting **Copy event handler method**.</span></span>

<span data-ttu-id="b1612-117">[![Visual Studio لقطة شاشة تُظهر كيفية نسخ طريقة معالج الأحداث من نافذة مصمم الجداول.](../media/copy-event-handler.png)](../media/copy-event-handler.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="b1612-117">[![Visual Studio screenshot showing how to copy event handler method from the table designer window.](../media/copy-event-handler.png)](../media/copy-event-handler.png#lightbox)</span></span>

-   <span data-ttu-id="b1612-118">**`OnDeleted` حدث** - هذا هو معالج ما بعد الأحداث الذي يتم تشغيله عند حذف سجل في الجدول.</span><span class="sxs-lookup"><span data-stu-id="b1612-118">**`OnDeleted` event** - This is a post-event handler that triggers when a record is deleted in the table.</span></span> <span data-ttu-id="b1612-119">يمكنك استخدام هذا، على سبيل المثال، لعرض رسالة سجل معلومات بعد حذف أحد السجلات.</span><span class="sxs-lookup"><span data-stu-id="b1612-119">You could use this, for example, to display an Infolog message after a record is deleted.</span></span>
```xpp
/// <summary>
///
/// </summary>
/// <param name="sender"></param>
/// <param name="e"></param>
[DataEventHandler(tableStr(CustTable), DataEventType::Deleted)]
public static void CustTable_onDeleted(Common sender, DataEventArgs e)
{
}
```
-   <span data-ttu-id="b1612-120">**`OnInserting` حدث** - يتم تشغيل هذا عند إدخال البيانات.</span><span class="sxs-lookup"><span data-stu-id="b1612-120">**`OnInserting` event** - This is triggered when data is being inserted.</span></span> <span data-ttu-id="b1612-121">علي سبيل المثال، يمكن أن يتم تشغيل هذا عند إضافة عميل جديد إلى تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="b1612-121">For example, this could trigger when you add a  new customer to Finance and Operations apps.</span></span>
```xpp
/// <summary>
///
/// </summary>
/// <param name="sender"></param>
/// <param name="e"></param>
[DataEventHandler(tableStr(CustTable), DataEventType::Inserting)]
public static void CustTable_onInserting(Common sender, DataEventArgs e)
{
}
```
-   <span data-ttu-id="b1612-122">**`OnValidatedWrite` حدث** - هذا هو معالج ما بعد الأحداث الذي يتم تشغيله بعد إدخال البيانات.</span><span class="sxs-lookup"><span data-stu-id="b1612-122">**`OnValidatedWrite` event** - This is a post-event handler that triggers after data is entered.</span></span> <span data-ttu-id="b1612-123">يستخدم هذا للتحقق من صحة البيانات التي تتم كتابتها على صفحة، مثل التأكد من أن عمر العميل لا يقل عن 18 عاماً عن طريق التحقق من تاريخ الميلاد.</span><span class="sxs-lookup"><span data-stu-id="b1612-123">This is used to validate data that is being written to a page, such as ensuring that a customer is at least 18 years old by verifying a birth date.</span></span>
```xpp
/// <summary>
///
/// </summary>
/// <param name="sender"></param>
/// <param name="e"></param>
[DataEventHandler(tableStr(CustTable), DataEventType::ValidatedWrite)]
public static void CustTable_onValidatedWrite(Common sender, DataEventArgs e)
{
}
```

## <a name="chain-of-command"></a><span data-ttu-id="b1612-124">سلسله الأوامر</span><span class="sxs-lookup"><span data-stu-id="b1612-124">Chain of Command</span></span> 

<span data-ttu-id="b1612-125">يمكنك تضمين المنطق حول الطرق المحددة في الفئة الأساسية التي تقوم بزيادتها.</span><span class="sxs-lookup"><span data-stu-id="b1612-125">You can wrap logic around methods that are defined in the base class that you're augmenting.</span></span> <span data-ttu-id="b1612-126">يمكنك أيضاً توسيع منطق الطرق العامة والمحمية دون الحاجة إلى استخدام معالجات الأحداث.</span><span class="sxs-lookup"><span data-stu-id="b1612-126">You can also extend the logic of public and protected methods without having to use event handlers.</span></span>

<span data-ttu-id="b1612-127">عند تضمين طريقة، يمكنك الوصول إلى الطرق العامة والمحمية بالإضافة إلى متغيرات الفئة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="b1612-127">When wrapping a method, you can access public and protected methods as well as variables of the base class.</span></span> <span data-ttu-id="b1612-128">يؤدي استخدام برنامج تضمين حول طريقة والكلمة الأساسية `next` إلى إنشاء سلسلة أوامر (CoC).</span><span class="sxs-lookup"><span data-stu-id="b1612-128">Using a wrapper around a method and the `next` keyword creates a Chain of Command (CoC).</span></span>

<span data-ttu-id="b1612-129">سلسلة الأوامر هي نموذج تصميم يتم فيه معالجة الطلب بواسطة سلسلة من أجهزة الاستقبال.</span><span class="sxs-lookup"><span data-stu-id="b1612-129">CoC is a design pattern where a request is handled by a series of receivers.</span></span> <span data-ttu-id="b1612-130">ويتم استخدام فئة الملحق لتضمين الطرق المحمية أو العامة للفئات والجداول وكيانات البيانات والنماذج.</span><span class="sxs-lookup"><span data-stu-id="b1612-130">An extension class is used to wrap protected or public methods of classes, tables, data entities, and forms.</span></span> <span data-ttu-id="b1612-131">يجب أن تكون على دراية ببعض القيود عند تضمين الطرق:</span><span class="sxs-lookup"><span data-stu-id="b1612-131">You should be aware of some restrictions when wrapping methods:</span></span>

-   <span data-ttu-id="b1612-132">يجب أن يكون لطريقة برنامج التضمين نفس توقيع الطريقة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="b1612-132">The wrapper method must have the same signature as the base method.</span></span>
-   <span data-ttu-id="b1612-133">عند زيادة فئات النموذج، يمكن تضمين الطرق على مستوى الجذر فقط، وليس الطرق المحددة في الفئات المتداخلة.</span><span class="sxs-lookup"><span data-stu-id="b1612-133">When you augment form classes, only root-level methods can be    wrapped, not methods that are defined in nested classes.</span></span>

<span data-ttu-id="b1612-134">تلزم طرق برنامج التضمين في فئة ملحقة لاستدعاء `next` دائماً بحيث يتم استدعاء طريقة `next` في السلسلة وأخيراً، يتم استدعاء التنفيذ الأصلي دائماً.</span><span class="sxs-lookup"><span data-stu-id="b1612-134">Wrapper methods in an extension class are required to always call `next` so that the `next` method in the chain and, finally, the original implementation is always called.</span></span> <span data-ttu-id="b1612-135">تضمن هذه العملية أن كل طريقة في السلسلة تدخل في النتيجة.</span><span class="sxs-lookup"><span data-stu-id="b1612-135">This process ensures that every method in the chain factors into the result.</span></span> <span data-ttu-id="b1612-136">يجب أن تستدعي الطريقة **`next()`** دون شروط.</span><span class="sxs-lookup"><span data-stu-id="b1612-136">The method must call **`next()`** unconditionally.</span></span>
