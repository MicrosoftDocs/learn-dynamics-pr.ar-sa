---
ms.openlocfilehash: fb751ede1394008570e271438ad279c20438ad66
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071453"
---
<span data-ttu-id="f6a18-101">تُستخدم العبارات المستندة إلى مجموعة لتحديث سجلات بيانات متعددة أو إدراجها أو حذفها من أحد الجداول.</span><span class="sxs-lookup"><span data-stu-id="f6a18-101">Set-based statements are used to update, insert, or delete multiple records of data from a table.</span></span>

<span data-ttu-id="f6a18-102">وتُستخدم العمليات المستندة إلى صف أو غير المستندة إلى مجموعة لتحديث سجل مفرد من أحد الجداول أو إدراجه أو حذفه.</span><span class="sxs-lookup"><span data-stu-id="f6a18-102">Row-based, or non-set-based, operations are used to update, insert, or delete a single record from a table.</span></span>

<span data-ttu-id="f6a18-103">يمكن أن يؤدي استخدام الاستعلامات المستندة إلى مجموعة إلى زيادة الأداء بشكل كبير عن طريق تقليل عدد الاستدعاءات التي يتم اجراؤها على قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="f6a18-103">Using set-based queries can greatly increase performance by reducing the number of calls that are made to the database.</span></span>
 
<span data-ttu-id="f6a18-104">تتطلب العملية المستندة إلى صف استدعاءً إلى قاعدة البيانات لكل سجل يلزم معالجته، بينما تستدعي العبارة المستندة إلى مجموعة قاعدة البيانات مرة واحدة فقط.</span><span class="sxs-lookup"><span data-stu-id="f6a18-104">A row-based operation requires a call to the database for each record that needs to be manipulated, while a set-based statement only calls the database once.</span></span>

<span data-ttu-id="f6a18-105">على سبيل المثال، إذا كنت بحاجة إلى تحديث 100 سجل في جدول، فإن العملية المستندة إلى صف ستستدعي طريقة التحديث وتستدعي قاعدة البيانات 100 مرة لتحديث جميع السجلات.</span><span class="sxs-lookup"><span data-stu-id="f6a18-105">For example, if you need to update 100 records on a table, a row-based operation would call the update method and call the database 100 times to update all the records.</span></span> <span data-ttu-id="f6a18-106">ستستدعي العبارة المستندة إلى مجموعة طريقة `update_recordset` مرة واحدة وستستدعي قاعدة البيانات مرة واحدة لتحديث جميع السجلات.</span><span class="sxs-lookup"><span data-stu-id="f6a18-106">A set-based statement would call the `update_recordset` method once and call the database once to update all the records.</span></span>

<span data-ttu-id="f6a18-107">فيما يلي ثلاثة أمثلة على العبارات المستندة إلى مجموعة التي يمكن استخدامها:</span><span class="sxs-lookup"><span data-stu-id="f6a18-107">Three examples of set-based statements that can be used are:</span></span>

-   <span data-ttu-id="f6a18-108">**`Update_recordset`** - تُستخدم لتحديث سجلات متعددة في وقت واحد.</span><span class="sxs-lookup"><span data-stu-id="f6a18-108">**`Update_recordset`** - Used to update multiple records at once.</span></span>
-   <span data-ttu-id="f6a18-109">**`Delete_from`** - تُستخدم لحذف سجلات متعددة في وقت واحد.</span><span class="sxs-lookup"><span data-stu-id="f6a18-109">**`Delete_from`** - Used to delete multiple records at once.</span></span>
-   <span data-ttu-id="f6a18-110">**`Insert_recordset`** - تُستخدم لنسخ سجلات متعددة من جدول واحد أو أكثر إلى جدول آخر.</span><span class="sxs-lookup"><span data-stu-id="f6a18-110">**`Insert_recordset`** - Used to copy multiple records from one or more tables into another table.</span></span>

<span data-ttu-id="f6a18-111">يمكن لـ `update_recordset` تحديث حقول متعددة في جدول.</span><span class="sxs-lookup"><span data-stu-id="f6a18-111">The `update_recordset` can update multiple fields on a table.</span></span> <span data-ttu-id="f6a18-112">يمكنك أيضاً تحديد عبارة WHERE لتحديد السجلات التي يتم تحديثها.</span><span class="sxs-lookup"><span data-stu-id="f6a18-112">You can also specify a where clause to determine what records are updated.</span></span> <span data-ttu-id="f6a18-113">فيما يلي مثال على `update_recordset` حيث تعلن عن الجدول وتستدعي `update_recordset` لتحديث حقلي **PaymMode‎** و **العملة** فقط للعملاء الذين لديهم حقل `CustGroup` يساوي "US".</span><span class="sxs-lookup"><span data-stu-id="f6a18-113">The following is an example of an `update_recordset` where you declare the table and call the `update_recordset` to update the customer **PaymMode** and **Currency** fields only for the customers with a `CustGroup` field that equals "US."</span></span>
<span data-ttu-id="f6a18-114">ضع في اعتبارك أنه في حال تجاوز طريقة التحديث، فإن `update_recordset` ستستدعي طريقة التحديث كل على حدة بدلاً من الكل في وقت واحد.</span><span class="sxs-lookup"><span data-stu-id="f6a18-114">Keep in mind that if the update method is overridden, the `update_recordset` will call the update method one at a time instead of all at once.</span></span>
```xpp
CustTable;
Update_recordset custTable
Setting
     PaymMode = 'Check',
     Currency = 'USD'
Where custTable.CustGroup == 'US';
```
<span data-ttu-id="f6a18-115">تبدو طريقة `delete_from` مماثلة لـ `update_recordset`.</span><span class="sxs-lookup"><span data-stu-id="f6a18-115">The `delete_from` method is like the `update_recordset`.</span></span> <span data-ttu-id="f6a18-116">يمكنك حذف سجلات متعددة في نفس الوقت من أحد الجداول، ويمكنك استخدام عبارة WHERE لتحديد السجلات المراد حذفها.</span><span class="sxs-lookup"><span data-stu-id="f6a18-116">You can delete multiple records at the same time from a table, and you can use a where clause to determine which records to delete.</span></span> <span data-ttu-id="f6a18-117">في المثال التالي، يتم الإعلان عن الجدول ثم استدعاء `delete_from` لحذف جميع السجلات حيث يساوي حقل `CustGroup` الخاص بالعميل "US".</span><span class="sxs-lookup"><span data-stu-id="f6a18-117">In the following example, the table is declared and then the `delete_from` is called to delete all the records where the customer's `CustGroup` field equals "US."</span></span>
```xpp
CustTable;
Delete_from custTable
    Where custTable.CustGroup == 'US';
```
<span data-ttu-id="f6a18-118">يُتيح لك `Insert_recordset` إدخال سجلات متعددة من جدول ما في جدول آخر.</span><span class="sxs-lookup"><span data-stu-id="f6a18-118">`Insert_recordset` lets you insert multiple records from one table into another table.</span></span> <span data-ttu-id="f6a18-119">ويمكنك استخدام عبارة WHERE لتحديد السجلات المراد إدراجها، كما يمكنك استخدام المتغيرات لإدراجها.</span><span class="sxs-lookup"><span data-stu-id="f6a18-119">You can use a where clause to determine which records to insert, and you can use variables to insert.</span></span> <span data-ttu-id="f6a18-120">في المثال التالي، يتم الإعلان عن الجدول الذي سيتم إدراجه والجدول الذي تسحب البيانات منه.</span><span class="sxs-lookup"><span data-stu-id="f6a18-120">In the following example, the table that will be inserted into and the table that you are pulling data from are declared.</span></span> <span data-ttu-id="f6a18-121">ثم يتم استدعاء `insert_recordset` لإدراج البيانات في الحقول المدرجة بين قوسين.</span><span class="sxs-lookup"><span data-stu-id="f6a18-121">The `insert_recordset` is then called to insert data into the fields that are listed in parentheses.</span></span> <span data-ttu-id="f6a18-122">وبعد ذلك، يتم استدعاء الحقول من الجدول المرحلي بالترتيب الذي تم به إدراج الحقول بين الأقواس.</span><span class="sxs-lookup"><span data-stu-id="f6a18-122">The fields from the staging table are then called in the order that the fields were listed in the parentheses.</span></span> <span data-ttu-id="f6a18-123">الآن، سيتم إدراج تلك الحقول في `CustTable` حيث يساوي حقل `CustGroup` الخاص بالعميل المرحلي "US".</span><span class="sxs-lookup"><span data-stu-id="f6a18-123">Now, those fields will be inserted into the `CustTable` where the staged customer's `CustGroup` field equals "US."</span></span>
```xpp
CustTable custTable;
StagingCustTable stagingCustTable;

Insert_recordset custTable (accountNum, custGroup, paymMode, currency)
    Select stagingAccountNum, stagingCustGroup, stagingPaymMode, stagingCurrency
        From stagingCustTable
        Where stagingCustTable.stagingCustGroup == 'US';
```
