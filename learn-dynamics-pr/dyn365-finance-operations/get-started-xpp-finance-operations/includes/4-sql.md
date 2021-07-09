---
ms.openlocfilehash: c4c6cf5520040de2c20012601817f1fcef45fb12
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071676"
---
يمكنك استخدام عبارات SQL في X++ لمعالجة البيانات باستخدام الكلمات الأساسية `select`، `insert_recordset`، `update_recordset`، و`delete`. 

تُستخدم عبارات التحديد لاختيار البيانات التي سيتم استردادها من قاعدة البيانات. في عبارة `select`، يمكنك اختيار الجداول التي تسحب منها، واختيار الحقول التي تريد استردادها من تلك الجداول، وتعيين شروط لتصفية البيانات بشكل أكبر، وتحديد الترتيب الذي يتم به إدراج البيانات. تحتوي عبارة `select` على الكلمة الأساسية "select" والمعلمات. وتحتوي المعلمات على الأجزاء المختلفة من عبارة التحديد التي تحدد البيانات التي يتم سحبها وكيفية ذلك.

فيما يلي مثال على بناء عبارة التحديد:
```xpp
Select [FindOptions] [FieldList] from [Table] [Options] [OrderByClause] [WhereClause] [JoinClause]
```
توفر معلمات **خيارات البحث** خيارات إضافية لسحب البيانات. على سبيل المثال، تسحب `crossCompany` البيانات عبر الكيانات القانونية، وتسحب `firstOnly` فقط السجل الأول، وتقوم `firstOnly10` بإحضار السجلات العشرة الأولى، وتحدد `forUpdate` البيانات مع وسمها بقفل.

تحدد **قائمة الحقول** البيانات المطلوب استردادها. يمكنك أيضاً استخدام دالات تجميعية مثل `sum`، أو `avg`، `minof`، أو `maxof` أو `count`. إذا كنت تستخدم حرف البدل النجمي (*) في **قائمة الحقول**، فسوف يسحب كل الحقول لسجل معين، لكننا لا نوصي بهذا الإجراء.

بعد **قائمة الحقول**، تستخدم الكلمة الأساسية "from"، متبوعة بالجدول المراد سحب البيانات منه. يمكنك بعد ذلك تضمين خيارات لترتيب البيانات أو تجميعها باستخدام الكلمات الرئيسية "order by" و"group by". تستخدم عبارة WHERE تعبيرات لتحديد معايير العبارة.

ويمكن استخدام عبارة JOIN لضم جداول إضافية إلى عبارة SELECT. كما يمكنك استخدام عوامل تشغيل ارتباطية في عبارات WHERE ضمن عبارات SELECT. ستقوم العبارة بإحضار كل السجلات التي يكون هذا التعبير فيها صحيحاً. الحد الأدنى لمتطلبات عبارة التحديد هي الكلمة الأساسية "select" والكلمة الأساسية "from" والجدول.

فيما يلي مثال على عبارة تحديد: تحدد العبارة الأولى الحقل المراد سحبه وتستخدم العبارة الثانية حرف البدل النجمي. نوصي بتحديد الحقول المراد سحبها عند كتابة عبارة تحديد.
```xpp
    Select AccountNum from CustTable;
        
    Select * from CustTable;
```
ويمكنك إضافة معلمات أخرى لعمل عبارات تحديد أكثر تعقيداً. في هذا المثال، يؤدي القيام بذلك إلى سحب كافة السجلات من CustTable حيث تكون قيم AccountNum أكبر من 1000 وأقل من 2000. يتم أيضاً فرز السجلات التي تم سحبها حسب قيم AccountNum بترتيب تنازلي.
```xpp
Select forUpdate  CustTable order by AccountNum desc
    where custTable.accountNum > '1000'
    && custTable.accountNum < '2000';
```
فيما يلي مثال على الشكل الذي قد تبدو عليه عبارة الانضمام. يوضح المثال انضمام سجل SalesLine إلى SalesTable ذي الصلة حيث يتطابق معرّف المبيعات في سطر المبيعات مع معرّف مبيعات جدول المبيعات.
```xpp
Select * from SalesLine
join SalesTable where SalesLine.SalesId == SalesTable.SalesId;
```
تُعيد عبارة `select` جميع السجلات، ويمكن إحضار السجلات المتبقية باستخدام عبارة `next`. تتكرر عبارة `while select` خلال كل سجل يُطابق معايير التحديد، وهو أمر شائع لمعالجة البيانات. في المثال التالي، بدلاً من سحب السجل الأول الذي يطابق المعايير، ستُكرر عبارة `while select` خلال كل سجل يكون فيه المعيار صحيحاً. عند تحديد كل سجل، سيتم تشغيله بعد ذلك من خلال المنطق الإضافي المُدرج بين الأقواس.

```xpp
While select forUpdate * from CustTable 
    order by AccountNum desc
    where custTable.accountNum > '1000'
    && custTable.accountNum < '2000'
{
    (Additional logic here.)
}
```
يمكن استخدام أساليب الإدراج لإضافة سجل جديد إلى أحد الجداول. لن تُدرج أساليب الإدراج سوى الأعمدة التي حُددت بواسطة الاستعلام. يمكنك تجاوز عمليات التحقق من صحة أسلوب الإدراج وعمليات المعالجة باستخدام أسلوب `doInsert()`. يمكن لعبارة `insert_recordset` إدراج سجلات متعددة عن طريق نسخ السجلات من أحد الجداول وإدراجها في جدول آخر.

فيما يلي مثال على استخدام أسلوب `insert` وعبارة `Insert_recordset`:
```xpp
ttsbegin;
salesLine.unitPrice = 4;
salesline.insert();
ttscommit;

insert_recordSet myTable (myNum)
    select myNum
        from anotherTable;
```
يمكن لأساليب التحديث تغيير القيم الموجودة في سجل أحد الجداول. لتحديث سجل، يجب عليك استخدام أمر `select forUpdate` للإشارة إلى أن السجلات مخصصة للتحديث. يجب أيضاً تضمين أساليب التحديث في عبارة ttsbegin وttscommit. يمكنك أيضاً استخدام `update_recordset` لتحديث سجلات متعددة في الوقت نفسه.

فيما يلي مثال على استخدام أحد أساليب التحديث وعبارة `update_recordset`.
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
يمكن لأساليب الحذف إزالة سجل موجود من أحد الجداول. يمكنك استخدام أسلوب `doDelete()` لاستبدال سلوك أسلوب الحذف القياسي. يمكنك أيضاً حذف سجلات متعددة مرة واحدة باستخدام عبارة `delete_from`.

فيما يلي مثال على استخدام أحد أساليب الحذف وعبارة `delete_from`.
```xpp
ttsbegin;
Select forupdate salesLine where salesline.salesId == 'S0001';
salesLine.delete();
ttsCommit;
            
delete_from salesLine
where salesLine.salesId == 'S0001';
```
يمكنك استخدام هذه المعلومات ككتل إنشاء لإنشاء استعلامات أكثر تعقيداً.
