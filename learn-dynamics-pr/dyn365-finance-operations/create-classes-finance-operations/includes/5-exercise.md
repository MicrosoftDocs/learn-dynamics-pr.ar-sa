---
ms.openlocfilehash: ba9e48e9ce4fa01db9dc8f9be69789abe4c37ebd
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072624"
---
## <a name="scenario"></a>السيناريو
باعتبارك مطور تطبيقات Finance and Operations، تم تكليفك بمهمة إدراج سجلات عملاء في جدول شركة Fleet Management. حيث تحتاج إلى إنشاء فئة قابلة للتشغيل وإضافة الكود الذي ستُدرج سجلين في جدول `FMCustomer`.


## <a name="create-a-runnable-class"></a>إنشاء فئة قابلة للتشغيل 

1. قم بتصغير نافذة Internet Explorer.
1. افتح Visual Studio.
1. حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.
1. ابدأ في إنشاء مشروع جديد عن طريق فتح قائمة **الملف** وتحديد **مشروع > جديد**.
1. في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.
1. في الجزء الأوسط، حدد **العمليات المالية**.
1. قم بتسمية المشروع **FleetManagementSecurityProject**.
1. حدد **موافق**.
1. افتح القائمة **Dynamics 365** في الشريط.
1. حدد **الخيارات**.
1. ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.
1. تأكد من تحديد خانتي الاختيار لكل من **تنظيم المشروعات حسب نوع العنصر** و **مزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.
1. حدد **موافق**.
1. في **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **FleetManagementClassProject**.
1. حدد **إضافة > عنصر جديد**.
1. في الجزء الأيمن، حدد **عناصر Dynamics 365** ثم حدد **الرمز**.
1. في الجزء الأوسط، حدد **فئة قابلة للتشغيل (مهمة)**.
1. أدخل **FMInsertCustomers** في حقل **الاسم**.
1. حدد **إضافة**. سيتم فتح فئة **FMInsertCustomers** الآن في نافذة **مصمم الأكواد**.

## <a name="add-code-to-insert-customer-records"></a>إضافة كود لإدراج سجلات العملاء 

1. في نافذة **مصمم الأكواد**، قم بإدراج سطر فارغ بين السطرين 6 و7 باستخدام مفتاح **Enter** وقم بإزالة الشُرط المائلة (///).
2. أدخل الكود التالي في السطر 7:

    ```xpp
       FMCustomer FMCustomer;
    ```

3. في نافذة **مصمم الأكواد**، قم بإدراج سطر فارغ بين الأقواس المتعرجة في السطرين 9 و10 باستخدام مفتاح **Enter**.
4. انسخ الكود التالي والصقه في المساحة الخالية في السطر 10:

    ```xpp
       FMInsertCustomers FMInsertCustomers = new  FMInsertCustomers();
       FMInsertCustomers.run();
    ``` 

5. وفي السطر 13، انسخ الكود التالي والصقه:

    ```xpp
          public void run()
         {
          this.insertRecords();
         }
         private void insertRecords()
         {
             ttsBegin;

                FMCustomer.FirstName = "John";
                FMCustomer.LastName = "Smith";
                FMCustomer.Email = "johnsmith@contoso.com";

                FMCustomer.insert();

                FMCustomer.clear();
                FMCustomer.FirstName = "Sally";
                FMCustomer.LastName = "Smith";
                FMCustomer.Email = "sallysmith@contoso.com";

                FMCustomer.insert();

             ttsCommit;
        }
    ```

6. في **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق فئة `FMInsertCustomers`.
7. حدد **تعيين ككائن بدء التشغيل**.
8. قم بتنفيذ بناء بالنقر بزر الماوس الأيمن فوق مشروع **FleetManagementClassProject** في نافذة **مستكشف الحلول** ثم حدد **البناء**.
9. قم بتشغيل الفئة دون التصحيح بتحديد القائمة **تصحيح**. حدد **ابدأ بدون تصحيح**. يمكنك أيضا استخدام اختصار لوحة المفاتيح **Ctrl + F5**.



