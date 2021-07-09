---
ms.openlocfilehash: c4c6cf5520040de2c20012601817f1fcef45fb12
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071676"
---
<span data-ttu-id="40083-101">يمكنك استخدام عبارات SQL في X++ لمعالجة البيانات باستخدام الكلمات الأساسية `select`، `insert_recordset`، `update_recordset`، و`delete`.</span><span class="sxs-lookup"><span data-stu-id="40083-101">You can use SQL statements in X++ to manipulate data by using `select`, `insert_recordset`, `update_recordset`, and `delete` keywords.</span></span> 

<span data-ttu-id="40083-102">تُستخدم عبارات التحديد لاختيار البيانات التي سيتم استردادها من قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="40083-102">Select statements are used to choose what data will be retrieved from the database.</span></span> <span data-ttu-id="40083-103">في عبارة `select`، يمكنك اختيار الجداول التي تسحب منها، واختيار الحقول التي تريد استردادها من تلك الجداول، وتعيين شروط لتصفية البيانات بشكل أكبر، وتحديد الترتيب الذي يتم به إدراج البيانات.</span><span class="sxs-lookup"><span data-stu-id="40083-103">In a `select` statement, you can choose which tables you are pulling from, choose which fields that you want to retrieve from those tables, set conditions to further filter the data, and select the order in which the data is listed.</span></span> <span data-ttu-id="40083-104">تحتوي عبارة `select` على الكلمة الأساسية "select" والمعلمات.</span><span class="sxs-lookup"><span data-stu-id="40083-104">The `select` statement contains the keyword "select" and parameters.</span></span> <span data-ttu-id="40083-105">وتحتوي المعلمات على الأجزاء المختلفة من عبارة التحديد التي تحدد البيانات التي يتم سحبها وكيفية ذلك.</span><span class="sxs-lookup"><span data-stu-id="40083-105">Parameters contain the different pieces of the select statement that determine how and what data is pulled.</span></span>

<span data-ttu-id="40083-106">فيما يلي مثال على بناء عبارة التحديد:</span><span class="sxs-lookup"><span data-stu-id="40083-106">The following is an example of the select statement syntax:</span></span>
```xpp
Select [FindOptions] [FieldList] from [Table] [Options] [OrderByClause] [WhereClause] [JoinClause]
```
<span data-ttu-id="40083-107">توفر معلمات **خيارات البحث** خيارات إضافية لسحب البيانات.</span><span class="sxs-lookup"><span data-stu-id="40083-107">The **Find options** parameters give additional options for pulling data.</span></span> <span data-ttu-id="40083-108">على سبيل المثال، تسحب `crossCompany` البيانات عبر الكيانات القانونية، وتسحب `firstOnly` فقط السجل الأول، وتقوم `firstOnly10` بإحضار السجلات العشرة الأولى، وتحدد `forUpdate` البيانات مع وسمها بقفل.</span><span class="sxs-lookup"><span data-stu-id="40083-108">For example, `crossCompany` pulls data across legal entities, `firstOnly` pulls only the first record, `firstOnly10` only fetches the first ten records, and `forUpdate` selects the data with a lock.</span></span>

<span data-ttu-id="40083-109">تحدد **قائمة الحقول** البيانات المطلوب استردادها.</span><span class="sxs-lookup"><span data-stu-id="40083-109">The **Field list** specifies which data to retrieve.</span></span> <span data-ttu-id="40083-110">يمكنك أيضاً استخدام دالات تجميعية مثل `sum`، أو `avg`، `minof`، أو `maxof` أو `count`.</span><span class="sxs-lookup"><span data-stu-id="40083-110">You can also use aggregate functions like `sum`, `avg`, `minof`, `maxof` or `count`.</span></span> <span data-ttu-id="40083-111">إذا كنت تستخدم حرف البدل النجمي (\*) في **قائمة الحقول**، فسوف يسحب كل الحقول لسجل معين، لكننا لا نوصي بهذا الإجراء.</span><span class="sxs-lookup"><span data-stu-id="40083-111">If you use the asterisk (\*) in the **Field list**, it will pull all fields for a given record, but we do not recommend that procedure.</span></span>

<span data-ttu-id="40083-112">بعد **قائمة الحقول**، تستخدم الكلمة الأساسية "from"، متبوعة بالجدول المراد سحب البيانات منه.</span><span class="sxs-lookup"><span data-stu-id="40083-112">After the **Field list**, the keyword "from" is used, followed by the table to pull from.</span></span> <span data-ttu-id="40083-113">يمكنك بعد ذلك تضمين خيارات لترتيب البيانات أو تجميعها باستخدام الكلمات الرئيسية "order by" و"group by".</span><span class="sxs-lookup"><span data-stu-id="40083-113">You can then include options to order or group the data by using "order by" and "group by" keywords.</span></span> <span data-ttu-id="40083-114">تستخدم عبارة WHERE تعبيرات لتحديد معايير العبارة.</span><span class="sxs-lookup"><span data-stu-id="40083-114">The where clause uses expressions to define the criteria for the statement.</span></span>

<span data-ttu-id="40083-115">ويمكن استخدام عبارة JOIN لضم جداول إضافية إلى عبارة SELECT.</span><span class="sxs-lookup"><span data-stu-id="40083-115">The join clause can be used to join additional tables to a select statement.</span></span> <span data-ttu-id="40083-116">كما يمكنك استخدام عوامل تشغيل ارتباطية في عبارات WHERE ضمن عبارات SELECT.</span><span class="sxs-lookup"><span data-stu-id="40083-116">You can use relational operators in where clauses in select statements.</span></span> <span data-ttu-id="40083-117">ستقوم العبارة بإحضار كل السجلات التي يكون هذا التعبير فيها صحيحاً.</span><span class="sxs-lookup"><span data-stu-id="40083-117">The statement will fetch all records where this expression yields true.</span></span> <span data-ttu-id="40083-118">الحد الأدنى لمتطلبات عبارة التحديد هي الكلمة الأساسية "select" والكلمة الأساسية "from" والجدول.</span><span class="sxs-lookup"><span data-stu-id="40083-118">The minimum requirements for a select statement are the keyword "select," the keyword "from," and the table.</span></span>

<span data-ttu-id="40083-119">فيما يلي مثال على عبارة تحديد:</span><span class="sxs-lookup"><span data-stu-id="40083-119">The following is an example of a select statement.</span></span> <span data-ttu-id="40083-120">تحدد العبارة الأولى الحقل المراد سحبه وتستخدم العبارة الثانية حرف البدل النجمي.</span><span class="sxs-lookup"><span data-stu-id="40083-120">The first statement defines the field to pull and the second statement uses the asterisk.</span></span> <span data-ttu-id="40083-121">نوصي بتحديد الحقول المراد سحبها عند كتابة عبارة تحديد.</span><span class="sxs-lookup"><span data-stu-id="40083-121">We recommend that you define the fields to pull in when writing a select statement.</span></span>
```xpp
    Select AccountNum from CustTable;
        
    Select * from CustTable;
```
<span data-ttu-id="40083-122">ويمكنك إضافة معلمات أخرى لعمل عبارات تحديد أكثر تعقيداً.</span><span class="sxs-lookup"><span data-stu-id="40083-122">You can add other parameters to make more complex select statements.</span></span> <span data-ttu-id="40083-123">في هذا المثال، يؤدي القيام بذلك إلى سحب كافة السجلات من CustTable حيث تكون قيم AccountNum أكبر من 1000 وأقل من 2000.</span><span class="sxs-lookup"><span data-stu-id="40083-123">In this example, doing so pulls all the records from CustTable where the AccountNum values are greater than 1000 and less than 2000.</span></span> <span data-ttu-id="40083-124">يتم أيضاً فرز السجلات التي تم سحبها حسب قيم AccountNum بترتيب تنازلي.</span><span class="sxs-lookup"><span data-stu-id="40083-124">The pulled records are also sorted by the AccountNum values in descending order.</span></span>
```xpp
Select forUpdate  CustTable order by AccountNum desc
    where custTable.accountNum > '1000'
    && custTable.accountNum < '2000';
```
<span data-ttu-id="40083-125">فيما يلي مثال على الشكل الذي قد تبدو عليه عبارة الانضمام.</span><span class="sxs-lookup"><span data-stu-id="40083-125">The following is an example of how a join statement might look.</span></span> <span data-ttu-id="40083-126">يوضح المثال انضمام سجل SalesLine إلى SalesTable ذي الصلة حيث يتطابق معرّف المبيعات في سطر المبيعات مع معرّف مبيعات جدول المبيعات.</span><span class="sxs-lookup"><span data-stu-id="40083-126">The example shows the joining of the SalesLine record to the related SalesTable where the sales ID on the sales line matches the sales table sales ID.</span></span>
```xpp
Select * from SalesLine
join SalesTable where SalesLine.SalesId == SalesTable.SalesId;
```
<span data-ttu-id="40083-127">تُعيد عبارة `select` جميع السجلات، ويمكن إحضار السجلات المتبقية باستخدام عبارة `next`.</span><span class="sxs-lookup"><span data-stu-id="40083-127">A `select` statement returns all records, and remaining records can be fetched by using a `next` statement.</span></span> <span data-ttu-id="40083-128">تتكرر عبارة `while select` خلال كل سجل يُطابق معايير التحديد، وهو أمر شائع لمعالجة البيانات.</span><span class="sxs-lookup"><span data-stu-id="40083-128">A `while select` statement loops through every record that matches the select criteria, which is common for data manipulation.</span></span> <span data-ttu-id="40083-129">في المثال التالي، بدلاً من سحب السجل الأول الذي يطابق المعايير، ستُكرر عبارة `while select` خلال كل سجل يكون فيه المعيار صحيحاً.</span><span class="sxs-lookup"><span data-stu-id="40083-129">In the following example, instead of pulling the first record that matches the criteria, the `while select` statement will loop through each record where the criterion is true.</span></span> <span data-ttu-id="40083-130">عند تحديد كل سجل، سيتم تشغيله بعد ذلك من خلال المنطق الإضافي المُدرج بين الأقواس.</span><span class="sxs-lookup"><span data-stu-id="40083-130">When each record is selected, it will then run through the additional logic that is inserted between the brackets.</span></span>

```xpp
While select forUpdate * from CustTable 
    order by AccountNum desc
    where custTable.accountNum > '1000'
    && custTable.accountNum < '2000'
{
    (Additional logic here.)
}
```
<span data-ttu-id="40083-131">يمكن استخدام أساليب الإدراج لإضافة سجل جديد إلى أحد الجداول.</span><span class="sxs-lookup"><span data-stu-id="40083-131">Insert methods can be used to add a new record to a table.</span></span> <span data-ttu-id="40083-132">لن تُدرج أساليب الإدراج سوى الأعمدة التي حُددت بواسطة الاستعلام.</span><span class="sxs-lookup"><span data-stu-id="40083-132">Insert methods will only insert the columns that are selected by the query.</span></span> <span data-ttu-id="40083-133">يمكنك تجاوز عمليات التحقق من صحة أسلوب الإدراج وعمليات المعالجة باستخدام أسلوب `doInsert()`.</span><span class="sxs-lookup"><span data-stu-id="40083-133">You can override the insert method's validations and processes by using the `doInsert()` method.</span></span> <span data-ttu-id="40083-134">يمكن لعبارة `insert_recordset` إدراج سجلات متعددة عن طريق نسخ السجلات من أحد الجداول وإدراجها في جدول آخر.</span><span class="sxs-lookup"><span data-stu-id="40083-134">The `insert_recordset` statement can insert multiple records by copying the records from one table and inserting them into another.</span></span>

<span data-ttu-id="40083-135">فيما يلي مثال على استخدام أسلوب `insert` وعبارة `Insert_recordset`:</span><span class="sxs-lookup"><span data-stu-id="40083-135">The following is an example of using an `insert` method and the `Insert_recordset` statement:</span></span>
```xpp
ttsbegin;
salesLine.unitPrice = 4;
salesline.insert();
ttscommit;

insert_recordSet myTable (myNum)
    select myNum
        from anotherTable;
```
<span data-ttu-id="40083-136">يمكن لأساليب التحديث تغيير القيم الموجودة في سجل أحد الجداول.</span><span class="sxs-lookup"><span data-stu-id="40083-136">Update methods can change existing values on a table record.</span></span> <span data-ttu-id="40083-137">لتحديث سجل، يجب عليك استخدام أمر `select forUpdate` للإشارة إلى أن السجلات مخصصة للتحديث.</span><span class="sxs-lookup"><span data-stu-id="40083-137">To update a record, you must use a `select forUpdate` command to indicate that the records are for update.</span></span> <span data-ttu-id="40083-138">يجب أيضاً تضمين أساليب التحديث في عبارة ttsbegin وttscommit.</span><span class="sxs-lookup"><span data-stu-id="40083-138">Update methods also need to be wrapped in a ttsbegin and ttscommit statement.</span></span> <span data-ttu-id="40083-139">يمكنك أيضاً استخدام `update_recordset` لتحديث سجلات متعددة في الوقت نفسه.</span><span class="sxs-lookup"><span data-stu-id="40083-139">You can also use the `update_recordset` to update multiple records at the same time.</span></span>

<span data-ttu-id="40083-140">فيما يلي مثال على استخدام أحد أساليب التحديث وعبارة `update_recordset`.</span><span class="sxs-lookup"><span data-stu-id="40083-140">The following is an example of using an update method and the `update_recordset` statement.</span></span>
```xpp
ttsbegin;
Select forupdate salesLine where salesline.salesId == 'S0001';
salesLine.unitPrice = 10;
salesLine.update();
ttsCommit;
        
update_recordset salesLine
setting unitPrice = 10
where salesId =='S0001';
```
<span data-ttu-id="40083-141">يمكن لأساليب الحذف إزالة سجل موجود من أحد الجداول.</span><span class="sxs-lookup"><span data-stu-id="40083-141">Delete methods can remove an existing record from a table.</span></span> <span data-ttu-id="40083-142">يمكنك استخدام أسلوب `doDelete()` لاستبدال سلوك أسلوب الحذف القياسي.</span><span class="sxs-lookup"><span data-stu-id="40083-142">You can use the `doDelete()` method to override the standard delete method behavior.</span></span> <span data-ttu-id="40083-143">يمكنك أيضاً حذف سجلات متعددة مرة واحدة باستخدام عبارة `delete_from`.</span><span class="sxs-lookup"><span data-stu-id="40083-143">You can also delete multiple records at once with the `delete_from` statement.</span></span>

<span data-ttu-id="40083-144">فيما يلي مثال على استخدام أحد أساليب الحذف وعبارة `delete_from`.</span><span class="sxs-lookup"><span data-stu-id="40083-144">The following is an example of using a delete method and the `delete_from` statement.</span></span>
```xpp
ttsbegin;
Select forupdate salesLine where salesline.salesId == 'S0001';
salesLine.delete();
ttsCommit;
            
delete_from salesLine
where salesLine.salesId == 'S0001';
```
<span data-ttu-id="40083-145">يمكنك استخدام هذه المعلومات ككتل إنشاء لإنشاء استعلامات أكثر تعقيداً.</span><span class="sxs-lookup"><span data-stu-id="40083-145">You can use this information as the building blocks to creating more complex queries.</span></span>
