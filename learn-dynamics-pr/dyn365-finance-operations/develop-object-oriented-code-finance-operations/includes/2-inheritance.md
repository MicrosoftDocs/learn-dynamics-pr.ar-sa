---
ms.openlocfilehash: 81b8339facfd84f38038606ad2185eeda1ad04f2
ms.sourcegitcommit: 5f1b010cd85c10b9a38b34f6b4500016961439d2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/25/2021
ms.locfileid: "6307656"
---
فئتا التوريث والخلاصة هما نوعان من بنيات البرمجة المهمة التي توجد في لغات البرمجة الموجهة للكائنات. تُستخدم هذه المفاهيم لإنشاء علاقات الأصل والتابع بين الفئات.
يسمح التوريث للفئة الفرعية بتوسيع فئة أعلى. ترث الفئة الفرعية جميع سمات الفئة الأعلى وأساليبها. يمكن للفئات الفرعية أيضاً تجاوز سلوك أو إضافة المزيد من الوظائف إلى الأساليب الموروثة من الفئة الأعلى. 

## <a name="inheritance"></a>التوريث

لفهم مفهوم التوريث بشكل أفضل في البرمجة الموجهة للكائنات، دعنا نراجع مثالاً من العالم الحقيقي. في هذا المثال، **المركبة** هي الفئة الأصل. هناك العديد من أنواع المركبات المختلفة، على سبيل المثال: السيارات والحافلات والشاحنات. في هذا السيناريو، **المركبة** هي الفئة الأصل. السيارات والحافلات والشاحنات هي فئات ترث من **المركبة**. تحتوي فئة **المركبة** على الخصائص التي تتم مشاركتها عبر جميع أنواع المركبات (السرعة واللون والتروس مثلاً). قد تختلف خصائص كل نوع من أنواع المركبات. على سبيل المثال، قد تحتوي الشاحنة على نظام دفع رباعي، لكن السيارة ليست كذلك.

![رسم تخطيطي للميراث من فئة أصل السيارة لفئات مشتقة من السيارة والحافلة والشاحنة.](../media/inheritance.png)

### <a name="example"></a>مثال

يوضح المثال التالي كيف يستخدم الفصل الميراث. تقوم فئة "السيارة" بتوسيع فئة "المركبة" للحصول على الطول والعرض ولكنها تضيف أيضاً متغير عدد الركاب. 

```xpp
class Vehicle
   {
    // Instance fields.
        real height;
        real width;
    // Constructor to initialize fields height and width.
    new(real _height, real _width)
    {
            height = _ height;
        width = _ width;
     }
   }

class Car extends Vehicle
    {
      // Additional instance field numberOfPassengers. Fields height and width are inherited.
      int numberOfPassengers;

     // Constructor is overridden to initialize z.
     new(real _height, real _width, int _numberOfPassengers)
     {
       // Initialize the fields.
       super(_height, _ width);
       numberOfPassengers = _numberOfPassengers;
     }
    }
 ```

## <a name="abstract"></a>الخلاصة 

يتم تحيد فئات الخلاصة بواسطة الكلمة الأساسية *الخلاصة*. لا يمكن إنشاء مثيل لها ولكنها تتطلب فئة فرعية موروثة من فئة الخلاصة. تُستخدم فئات الخلاصة لتنفيذ مفهوم ستكمله الفئة الفرعية بعد ذلك. يمكن أيضاً الإعلان عن أساليب الخلاصة في فئات الخلاصة. لا تسمح أساليب الخلاصة بالرمز أو الإعلانات في الأسلوب. يجب أن تقوم الفئة الفرعية بتوسيع فئة الخلاصة لاستخدام أسلوب الخلاصة.

### <a name="example"></a>مثال

فيما يلي مثال لفئة خلاصة. تقوم فئة "السيارة" بتوسيع فئة الخلاصة "المركبة" يسمح هذا لفئة "السيارة" بتجاوز أسلوب `printInfo()` ويسمح لك بإضافة وظيفة إلى أسلوب `operate()` الذي لم يتم تضمينه في فئة الخلاصة.

```xpp
abstract class Vehicle
{
      str owner;
      int age;

    void printInfo()
      {
        Info(strfmt("%1, %2",owner, age));
      }
    abstract void operate()
    {
    }
 }

class Car extends Vehicle
{
     str model;
     void printInfo()
     {
            // overriding default functionality
            Info(strfmt("%1, %2, %3",owner, age, model));
     }
   void operate()
   {
        Info('running');
   }
}
 ```
