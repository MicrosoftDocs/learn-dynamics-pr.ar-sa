---
ms.openlocfilehash: 699f7efa8c29ec500c6b89de2b2db0b1465552758270777952c8a156a056deaf
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7100092"
---
يمكنك كتابة التعليمات البرمجية لمعالجة البيانات المخزنة في قاعدة البيانات. 

- استخدم طريقة `select` لتعريف البيانات التي سيتم تعديلها.
- تُستخدم طريقة `insert` لإضافة سجل واحد أو أكثر إلى جدول.
- تُستخدم طريقة `update` لتعديل السجل الحالي في حقول النظام المناسبة.
- تُستخدم عبارة `where` لتحديد الحالة التي ستختبرها طريقة `update` أثناء معالجة كل صف بالجدول.
- تُستخدم طريقة `delete` لإزالة سجلات من جدول. قبل استخدام طريقة `update` أو `delete`، يجب استخدام طريقة `select` لتعريف البيانات التي ستقوم بتحديثها أو حذفها.
- لتحديد عدة سجلات أو حقول، ستستخدم طريقة `select` بالبداية ثم تستخدم طريقة `next` لإحضار السجل التالي في جدول.
- لتكرار الحلقة عبر العديد من السجلات التي تحقق معيار محدد، يمكنك استخدام `while select` طريقة.

فيما يلي نماذج من التعليمات البرمجية لطرق الإدراج والتحديث والحذف. تستخدم النماذج جدول `MyCustomerTable` وهمياً يحتوي علي حقول وهمية لـ `AccountNumber` و`CustomerName`.


- طريقة `insert`

    ```xpp
    //This will insert a new record into a sample MyCustomerTable table. The only mandatory field that is set on this table is AccountNumber.

    private void AddCustomer()
    {
        MyCustomerTable myCustomerTable;
        ttsBegin;
             select forUpdate myCustomerTable;
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