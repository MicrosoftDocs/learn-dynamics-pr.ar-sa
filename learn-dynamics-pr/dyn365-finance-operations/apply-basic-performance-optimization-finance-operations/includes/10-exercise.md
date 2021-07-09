---
ms.openlocfilehash: bf3c65d487e950d6a341bc3082cf206fd09ed977
ms.sourcegitcommit: 977539219691830a564399fa637ced040d24475e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "6072561"
---

## <a name="scenario"></a>السيناريو
تم تكليف مطور تطبيقات Finance and Operations بإنشاء مهمة لتحديث تفاوت "السعر" إلى 2 بالمائة لجميع الأصناف الموجودة في مجموعة منتجات التلفزيون.


## <a name="create-a-new-project"></a>إنشاء مشروع جديد

1. قم بتصغير نافذة Internet Explorer. 
2. افتح Visual Studio
3. حدد **نعم** في النافذة **هل ترغب في السماح لهذا التطبيق بإجراء تغييرات على الجهاز؟**.
4. افتح القائمة **ملف** وحدد **جديد > مشروع**.
5. في مربع الحوار **مشروع جديد**، تأكد من تحديد **Dynamics 365** في الجزء الأيسر ضمن **مثبت**.
6. في الجزء الأوسط، حدد **العمليات المالية**.
7. قم بتسمية المشروع **PriceToleranceUpdateJob**.
8. حدد **موافق**.
9. لضمان الرجوع إلى مجموعة التطبيقات الصحيحة، انتقل إلى قائمة **Dynamics 365**
10. حدد **إدارة النماذج > تحديث معلمات النموذج**
11. حدد نموذج **FleetManagement** من القائمة المنسدلة **اسم النموذج**. 
12. حدد **التالي**، ثم تأكد من تحديد **ApplicationSuite** في القائمة المنسدلة **الحزم المشار إليها**. 
13. حدد **التالي** ثم **إنهاء**.
14. افتح القائمة **Dynamics 365** في الشريط.
15. حدد **الخيارات**.
16. ضمن عُقدة **Dynamics 365** في الجزء الأيمن، حدد **المشاريع**.
17. تأكد من تحديد مربعي الاختيار الخاصتين بكل من **تنظيم المشروعات حسب نوع العنصر** و **ومزامنة قاعدة البيانات في البناء الخاص بالمشروع الذي تم إنشاؤه حديثاً**.
18. حدد **موافق**.


## <a name="create-a-runnable-class"></a>إنشاء فئة قابلة للتشغيل 

1. في النافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق مشروع **PriceToleranceUpdateJob**.
2. حدد **إضافة > عنصر جديد**.
3. في الجزء الأيمن، حدد **عناصر Dynamics 365** ثم حدد **الرمز**.
4. في الجزء الأوسط، حدد **فئة قابلة للتشغيل (مهمة)**.
5. أدخل **PriceToleranceUpdate** في الحقل **الاسم**.
6. حدد **إضافة**.
7. سيتم الآن فتح الفئة القابلة للتشغيل **PriceToleranceUpdate** في النافذة "مصمم العناصر".
8. قم بإزالة الكود الموجود في النافذة "مصمم العناصر"، ثم قم بإدخال الكود الآتي سطراً بسطر:
   
   ```xpp
   class PriceToleranceUpdate
   {
        Public static void main(Args _args)
        {
        InventTable inventTable;
        InventItemGroupItem inventItemGroupItem;
                UPDATE_RECORDSET inventTable
                SETTING
                     ItemPriceToleranceGroupId = "2%"
                JOIN inventItemGroupItem
                      Where inventItemGroupItem.Itemid == inventTable.itemid
                      && inventItemGroupItem.ItemGroupId == 'Television';
       }
   }
   ```
9. احفظ الفئة القابلة للتشغيل.
10. انقر بزر الماوس الأيمن فوق مشروع **PriceToleranceUpdateJob** وحدد **بناء**.
11. انقر بزر الماوس الأيمن فوق الفئة القابلة للتشغيل **PriceToleranceUpdate** وحدد **تعيين ككائن بدء التشغيل**.
12. من شريط الأدوات، حدد الخيار **تصحيح الأخطاء > البدء دون تصحيح الأخطاء** لتشغيل الفئة.



