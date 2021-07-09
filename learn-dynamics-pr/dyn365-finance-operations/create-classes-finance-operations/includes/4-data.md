---
ms.openlocfilehash: ac5f0b5fba462596066f781d0a3f8b342d27e973
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071560"
---
<span data-ttu-id="80ca8-101">يمكنك كتابة التعليمات البرمجية لمعالجة البيانات المخزنة في قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="80ca8-101">You can write code to manipulate data that is stored in the database.</span></span> 

- <span data-ttu-id="80ca8-102">استخدم طريقة `select` لتعريف البيانات التي سيتم تعديلها.</span><span class="sxs-lookup"><span data-stu-id="80ca8-102">Use a `select` method to declare the data that will be modified.</span></span>
- <span data-ttu-id="80ca8-103">تُستخدم طريقة `insert` لإضافة سجل واحد أو أكثر إلى جدول.</span><span class="sxs-lookup"><span data-stu-id="80ca8-103">An `insert` method is used to add one or more records to a table.</span></span>
- <span data-ttu-id="80ca8-104">تُستخدم طريقة `update` لتعديل السجل الحالي في حقول النظام المناسبة.</span><span class="sxs-lookup"><span data-stu-id="80ca8-104">An `update` method is used to modify the current record in the appropriate system fields.</span></span>
- <span data-ttu-id="80ca8-105">تُستخدم عبارة `where` لتحديد الحالة التي ستختبرها طريقة `update` أثناء معالجة كل صف بالجدول.</span><span class="sxs-lookup"><span data-stu-id="80ca8-105">Use a `where` clause to specify a condition that the `update` method will test as it processes each row of the table.</span></span>
- <span data-ttu-id="80ca8-106">تُستخدم طريقة `delete` لإزالة سجلات من جدول.</span><span class="sxs-lookup"><span data-stu-id="80ca8-106">A `delete` method is used to remove records from a table.</span></span> <span data-ttu-id="80ca8-107">قبل استخدام طريقة `update` أو `delete`، يجب استخدام طريقة `select` لتعريف البيانات التي ستقوم بتحديثها أو حذفها.</span><span class="sxs-lookup"><span data-stu-id="80ca8-107">Before using an `update` or `delete` method, you must use a `select` method to define the data that you will be updating or deleting.</span></span>
- <span data-ttu-id="80ca8-108">لتحديد عدة سجلات أو حقول، ستستخدم طريقة `select` بالبداية ثم تستخدم طريقة `next` لإحضار السجل التالي في جدول.</span><span class="sxs-lookup"><span data-stu-id="80ca8-108">To select multiple records or fields, you will initially use a `select` method and then use a `next` method to fetch the next record in a table.</span></span>
- <span data-ttu-id="80ca8-109">لتكرار الحلقة عبر العديد من السجلات التي تحقق معيار محدد، يمكنك استخدام `while select` طريقة.</span><span class="sxs-lookup"><span data-stu-id="80ca8-109">To loop over many records that meet specific criteria, you can use a `while select` method.</span></span>

<span data-ttu-id="80ca8-110">فيما يلي نماذج من التعليمات البرمجية لطرق الإدراج والتحديث والحذف.</span><span class="sxs-lookup"><span data-stu-id="80ca8-110">The following are code samples for insert, update, and delete methods.</span></span> <span data-ttu-id="80ca8-111">تستخدم النماذج جدول `MyCustomerTable` وهمياً يحتوي علي حقول وهمية لـ `AccountNumber` و`CustomerName`.</span><span class="sxs-lookup"><span data-stu-id="80ca8-111">The samples use a fictitious `MyCustomerTable` table containing fictitious fields for `AccountNumber` and `CustomerName`.</span></span>


- <span data-ttu-id="80ca8-112">طريقة `insert`</span><span class="sxs-lookup"><span data-stu-id="80ca8-112">`insert` method</span></span>

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

- <span data-ttu-id="80ca8-113">طريقة `update`</span><span class="sxs-lookup"><span data-stu-id="80ca8-113">`update` method</span></span>

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

- <span data-ttu-id="80ca8-114">طريقة `delete`</span><span class="sxs-lookup"><span data-stu-id="80ca8-114">`delete` method</span></span>


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