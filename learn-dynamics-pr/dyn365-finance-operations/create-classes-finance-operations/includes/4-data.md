---
ms.openlocfilehash: ac5f0b5fba462596066f781d0a3f8b342d27e973
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071560"
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