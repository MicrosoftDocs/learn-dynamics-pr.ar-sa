---
ms.openlocfilehash: d5f8e19076a7d47d3ffd102fc9223b2591a63f0c
ms.sourcegitcommit: f6819b06b09bea4edfb42315bfe2f17231c1ac8b
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/20/2022
ms.locfileid: "8015644"
---
يمكنك كتابة التعليمات البرمجية لمعالجة البيانات المخزنة في قاعدة البيانات. 

- استخدم طريقة `select` لتعريف البيانات التي سيتم تعديلها.
- تُستخدم طريقة `insert` لإضافة سجل واحد أو أكثر إلى جدول.
- تُستخدم طريقة `update` لتعديل السجل الحالي في حقول النظام المناسبة.
- تُستخدم عبارة `where` لتحديد الحالة التي ستختبرها طريقة `update` أثناء معالجة كل صف بالجدول.
- تُستخدم طريقة `delete` لإزالة سجلات من جدول. قبل استخدام طريقة `update` أو `delete`، يجب استخدام طريقة `select` لتعريف البيانات التي ستقوم بتحديثها أو حذفها.
- لتحديد عدة سجلات أو حقول، ستستخدم طريقة `select` بالبداية ثم تستخدم طريقة `next` لإحضار السجل التالي في جدول.
- لتكرار الحلقة عبر العديد من السجلات التي تحقق معيار محدد، يمكنك استخدام `while select` طريقة.

ستقوم العبارة `select` بإحضار التاريخ أو التحكم فيه من قاعده البيانات باستخدام X++. يمكنك استخدام عبارة `select` لإحضار سجل أو حقل واحد. يمكنك استخدام العبارات الأخرى مثل `next` لإحضار سجلات إضافية أو استخدام `while select` لاجتياز سجلات متعددة. 

على سبيل المثال، سوف يجلب نموذج الرمز التالي جميع الأعمدة في الصف الأول من **CustTable**، ثم سيطبع القيمة في عمود **AccountNum** لهذا الصف:

```xpp
CustTable custTable;
select firstonly custTable; //this is a short notation for 'select firstonly * from custTable;'  
info("AccountNum: " + custTable.AccountNum); 
 ```
 
فيما يلي نماذج من التعليمات البرمجية لطرق `insert`، و`update`، و`delete`. تستخدم العينات جدولاً وهمياً هو **MyCustomerTable** يحتوي على حقول وهمية لـ **AccountNumber** و **CustomerName**.


- طريقة `insert`

    ```xpp
    //This will insert a new record into a sample MyCustomerTable table. The only mandatory field that is set on this table is AccountNumber.

    private void AddCustomer()
    {
        MyCustomerTable myCustomerTable;
        ttsBegin;
             myCustomerTable.AccountNumber = "1234";
             //The new record will have the account number 1234.
             myCustomerTable.insert();
        ttsCommit;
    }
    ```

- طريقة `update`

    ```xpp
    //This will update the record where the AccountNumber field is set to 1234 by adding more information in the CustomerName field.
    
    private void UpdateCustomer()
    {
        MyCustomerTable myCustomerTable
        ttsBegin;
            select forUpdate myCustomerTable
            where myCustomerTable.AccountNumber == "1234";
            //Now we will update the CustomerName field to be Sally
            myCustomerTable.CustomerName = "Sally";
            myCustomerTable.update();
            ttsCommit;
    }
    ```

- طريقة `delete`


    ```xpp
    //This will delete the record from the MyCustomerTable table where the AccountNumber field is set to 1234.
    
    private void DeleteCustomer()
    {
        ttsBegin;
            while select forUpdate myCustomerTable
            where myCustomerTable.AccountNumber == "1234"
        {
            myCustomerTable.delete();
        }
        ttsCommit;
    }

    ```
