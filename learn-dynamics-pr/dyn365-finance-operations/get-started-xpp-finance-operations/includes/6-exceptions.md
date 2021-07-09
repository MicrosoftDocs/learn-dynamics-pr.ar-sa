---
ms.openlocfilehash: cd10136b4eb5d53689344f8de12c0995baf1b11b
ms.sourcegitcommit: 1385575708da232750c0993c3bc45466592d057e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "6072337"
---
<span data-ttu-id="9d6bb-101">بينما تكون العبارات الشرطية رائعة لمعالجة تشغيل كتل الأكواد المختلفة، يتم استخدام معالجة الاستثناءات للتعامل مع الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-101">While conditional statements are great for handling the running of different code blocks, exception handling is used to deal with errors.</span></span>
<span data-ttu-id="9d6bb-102">يمكن استخدام العبارات مثل `throw`و `try...catch`و `finally`و `retry` لمعالجة الاستثناءات.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-102">Statements like `throw`, `try...catch`, `finally`, and `retry` can be used to handle exceptions.</span></span> <span data-ttu-id="9d6bb-103">الاستثناء هو طريقة للأكواد للابتعاد عن الأكواد القابلة للتشغيل عند حدوث خطأ.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-103">An exception is a way for the code to jump away from the runnable code when an error occurs.</span></span> 

<span data-ttu-id="9d6bb-104">يمكن استخدام عبارة throw لإصدار استثناء أثناء الخطأ.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-104">The throw statement can be used to give an error exception.</span></span> <span data-ttu-id="9d6bb-105">يمكن لعبارة throw تحديد قيمة تعداد استثنائية، لكنها أفضل ممارسة لاستخدام أساليب الخطأ العامة أو المعلومات أو أساليب التحذير.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-105">A throw statement can specify an exception enum value, but it is best practice to use the global error, info, or warning methods.</span></span> <span data-ttu-id="9d6bb-106">يسمح لك هذا الأسلوب باستخدام تسمية لعرض المستخدم في سجل المعلومات، كما هو موضح في المثال التالي:</span><span class="sxs-lookup"><span data-stu-id="9d6bb-106">This method allows you to use a label to display to the user in an Infolog, as shown in the following example:</span></span>
```xpp
throw error("This is an error.");
```
<span data-ttu-id="9d6bb-107">فيما يلي الشكل الذي تبدو عليه رسالة الخطأ والتحذير والمعلومات في واجهة المستخدم:</span><span class="sxs-lookup"><span data-stu-id="9d6bb-107">Here is what an error, warning, and info message looks like in the user interface:</span></span>

![تُظهر لقطة الشاشة رسائل الخطأ والتحذير والمعلومات.](../media/error-1.png)

<span data-ttu-id="9d6bb-109&quot;>يمكن استدعاء الأساليب الثابتة في الفئة العمومية بدون البادئة `Global::` حتى يمكن أيضاً استدعاء الأسلوب `Global::error` كما هو موضح في المثال التالي:</span><span class=&quot;sxs-lookup&quot;><span data-stu-id=&quot;9d6bb-109&quot;>Static methods on the Global class can be called without the `Global::` prefix, so the `Global::error` method can also be called as shown in the following example:</span></span>
```xpp
error(&quot;This is an error.");
```
<span data-ttu-id="9d6bb-110">يمكنك أيضاً استخدام عبارة `try...catch` لمعالجة بعض الأكواد في كتلة try، ثم استخدم كتلة catch لمعالجة الاستثناء إذا وقع.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-110">You can also use a `try...catch` statement to process some code in the try block, and then use the catch block to handle an exception if it occurs.</span></span> <span data-ttu-id="9d6bb-111">في المثال التالي، تعمل الكتلة `try` على تشغيل بعض الأكواد.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-111">In the following example, the `try` block runs some code.</span></span> <span data-ttu-id="9d6bb-112">في حالة حدوث استثناء رقمي، تصدر كتلة `catch` الأولى رسالة معلومات لعرضها: "تم العثور على رقم".</span><span class="sxs-lookup"><span data-stu-id="9d6bb-112">If a numeric exception occurs, the first `catch` block gives an info message to display: "Found a Numeric."</span></span> <span data-ttu-id="9d6bb-113">تعالج الكتلة الثانية `catch` أية أخطاء أخرى قد يتم العثور عليها.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-113">The second `catch` block handles any other errors that might be found.</span></span> <span data-ttu-id="9d6bb-114">يجب عليك فقط التقاط الاستثناءات التي تعرف أن الأكواد الخاصة بك داخل الكتلة `try` ستطرحها.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-114">You should only catch exceptions that you know your code inside the `try` block might throw.</span></span> <span data-ttu-id="9d6bb-115">يجب أن ترتفع كافة الاستثناءات الأخرى إلى إطار المكدس التالي.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-115">All other exceptions should rise to the next stack frame.</span></span>
```xpp
try
{
    //Run some code that might throw a numeric or other type of exception.
}
catch (Exception::Numeric)
{
    info('Found a Numeric exception.');
}
catch
{
    info('Caught an exception');
    retry;
}
finally
{
        // Executed no matter how the try block exits.
}
```
<span data-ttu-id="9d6bb-116">يمكن كتابة `retry` في كتلة catch للانتقال مرة أخرى إلى أول سطر من الكود ضمن كتلة try.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-116">A `retry` can be written in a catch block to jump back to the first line of code within the try block.</span></span> <span data-ttu-id="9d6bb-117">يمكن استخدام هذا إذا كان من الممكن إصلاح المشكلة أثناء التطبيق عن طريق الكود في كتلة catch.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-117">This can be used if the issue in the implementation can be fixed by code in the catch block.</span></span> <span data-ttu-id="9d6bb-118">بعد ذلك، سيتم تشغيل كتلة try مرة أخرى لإعطاءها فرصة ثانية لنجاح العملية.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-118">Then, the try block will run again to give it a second chance to succeed.</span></span> <span data-ttu-id="9d6bb-119">تأكد من أن إعادة المحاولة لا تتسبب في تكرار لا نهائي.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-119">Make sure that the retry does not cause an infinite loop.</span></span> <span data-ttu-id="9d6bb-120">يمكن إضافة عبارة `finally` إلى عبارة `try...catch`.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-120">A `finally` clause can be added to a `try...catch` statement.</span></span> <span data-ttu-id="9d6bb-121">يتم تشغيل العبارات في عبارة `finally` عندما يترك تنفيذ الكود الكتلة `try`.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-121">Statements in the `finally` clause are run when the implementation of the code leaves the `try` block.</span></span> <span data-ttu-id="9d6bb-122">سيتم تنفيذ العبارات في الكتلة `finally` بغض النظر عن الطريقة التي يتم بها إنهاء الكتلة `try`.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-122">The statements in the `finally` block will run no matter how the `try` block exits.</span></span>

<span data-ttu-id="9d6bb-123">إذا لم تتم معالجة الاستثناء، فسيتم تفكيك استدعاء الأسلوب الحالي وستتم معالجة الاستثناء أو عدم معالجته، في نطاق المستدعي.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-123">If an exception is not handled, then the call to the current method is unraveled and the exception will be handled, or not handled, in the caller's scope.</span></span>

## <a name="user-messages"></a><span data-ttu-id="9d6bb-124">رسائل المستخدم</span><span class="sxs-lookup"><span data-stu-id="9d6bb-124">User messages</span></span>

<span data-ttu-id="9d6bb-125">باستخدام واجهة API **للرسالة**، يمكنك الحصول على مزيد من التحكم في دورة حياة الرسالة، ويمكنك بشكل صريح إضافة الرسائل وإزالتها.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-125">By using the **Message()** API, you can have more control over the lifecycle of a message, you can explicitly add and remove messages.</span></span> <span data-ttu-id="9d6bb-126">يمكن استخدام هذا إذا كنت بحاجة إلى إزالة رسائل التحقق من الصحة في أوقات غير متقاطعة الحد، أو لعرض رسالة معلومات حول جانب معين من خبرة المستخدم التي ترتبط مباشرة بالتحقق من صحة البيانات.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-126">This can be used if you need validation messages removed at times other than when a save boundary has been crossed, or for displaying an informational message about a specific aspect of the user’s experience that is directly related to data validation.</span></span> 

<span data-ttu-id="9d6bb-127">هيا نلقي النظر على مثال:</span><span class="sxs-lookup"><span data-stu-id="9d6bb-127">Let’s look at an example:</span></span>

```xpp
messageId = Message::Add(MessageSeverity::Informational, "The customer is marked as inactive");
```

<span data-ttu-id="9d6bb-128">في هذا المثال، يمكن إلغاء تحديد الرسالة عند ظهور سجل جديد في الصفحة.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-128">In this example, the message can then be cleared when a new record is shown on the page.</span></span> 

<span data-ttu-id="9d6bb-129">بالإضافة إلى استخدام واجهة API **للرسالة()**، يمكنك استخدام الأسلوب `Message::AddAction()` بحيث يمكنك تضمين إجراء داخل رسالة سيتم إرسالها إلى شريط الرسائل.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-129">In addition to using the **Message()** API, you can use the `Message::AddAction()` method so you can embed an action within a message that is sent to the message bar.</span></span> <span data-ttu-id="9d6bb-130">يدعم هذا الأسلوب إضافة إجراء مفرد مقترن بعرض أو عنصر قائمة إجراء، والذي يمكن تصوره كزر **ارتباط**.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-130">This method supports adding a single action that is associated with a display or action menu item, that can then be visualized as a **Link** button.</span></span> 

<span data-ttu-id="9d6bb-131">في المثال التالي، يتم تشغيل رسالة لمسؤول النظام لإعلامه بعدم تشغيل وظيفة المجموعة ثم يتم كشف إجراء للانتقال مباشرة إلى الصفحة **وظائف المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-131">In the following example, a message is triggered for a system administrator letting them know that a batch job is not running and then exposes an action to go directly to the **Batch jobs** page.</span></span> 

```xpp
MenuItemMessageAction actionData = new MenuItemMessageAction();

actionData.MenuItemName("BatchJob");

str jsonData = FormJsonSerializer::serializeClass(actionData);

int64 messageId = Message::AddAction(MessageSeverity::Informational, "The Test batch job is not currently running", "Go to Batch jobs", MessageActionType::DisplayMenuItem, jsonData);
```

<span data-ttu-id="9d6bb-132">وفيما يلي الناتج:</span><span class="sxs-lookup"><span data-stu-id="9d6bb-132">Here is the output:</span></span>

![لقطة الشاشة التي تظهر رسالة الناتج لم يتم تشغيل وظيفة مجموعة الاختبار حالياً.](../media/add-action-method-ss.png)

## <a name="exceptions-inside-transactions"></a><span data-ttu-id="9d6bb-134">استثناءات داخل الحركات</span><span class="sxs-lookup"><span data-stu-id="9d6bb-134">Exceptions inside transactions</span></span> 

<span data-ttu-id="9d6bb-135">في حالة طرح استثناء داخل إحدى الحركات، فسيتم إيقاف الحركة تلقائياً (تحدث العملية `ttsAbort`).</span><span class="sxs-lookup"><span data-stu-id="9d6bb-135">If an exception is thrown inside a transaction, the transaction is automatically aborted (a `ttsAbort` operation occurs).</span></span> <span data-ttu-id="9d6bb-136">ينطبق هذا على الاستثناءات التي يتم طرحها يدوياً والاستثناءات التي يتم طرحها بواسطة النظام.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-136">This applies for exceptions that are thrown manually and for exceptions that are thrown by the system.</span></span>

<span data-ttu-id="9d6bb-137">عند طرح استثناء داخل كتلة transaction `ttsBegin - ttsCommit`، فلا يمكن لعبارة catch داخل كتلة transaction معالجة الاستثناء.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-137">When an exception is thrown inside a `ttsBegin - ttsCommit` transaction block, no catch statement inside that transaction block can process the exception.</span></span> <span data-ttu-id="9d6bb-138">بدلاً من ذلك، تعتبر عبارات catch الأعمق التي تقع خارج كتلة transaction هي أول عبارات catch التي سيتم اختبارها.</span><span class="sxs-lookup"><span data-stu-id="9d6bb-138">Instead, the innermost catch statements that are outside the transaction block are the first catch statements to be tested.</span></span>


