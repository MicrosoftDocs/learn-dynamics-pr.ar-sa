---
ms.openlocfilehash: 41a51f54418f8549b09520d2556b9188cb8332352d5329fb5ad9a2640b9a1e18
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7116030"
---
تُعد *الواجهة* مواصفة لمجموعة من أساليب المثيل العام.
تحدد الواجهة أوجه التشابه بين الفئات غير المرتبطة وتفرضها دون الحاجة إلى اشتقاق فئة واحدة من الأخرى. تعتبر جميع الواجهات عامة، حتى إذا لم تضف بشكل صريح الكلمة الرئيسية `public` أمام الكلمة الرئيسية `interface` في الكود `classDeclaration` . تعتبر الأساليب الموجودة بالواجهة عامة أيضاً.  

لإنشاء واجهة، اتبع الخطوات التالية:

1.  في مستكشف الحلول، انقر بزر الماوس الأبيض فوق مشروع ثم حدد **إضافة**.
2.  في مربع الحوار **عنصر جديد** ، حدد **الواجهة** ثم أدخل اسماً للواجهة.
3.  حدد **إضافة**.

عندما تضيف الكلمة الأساسية `implements` في إقرار الفئة، يجب أن تقر الفئة بالأساليب التي تحددها الواجهة. يمكن لإقرار الفئة تطبيق واجهات متعددة. اسرد الواجهات بعد تكرار واحد للكلمة الأساسية `implements` وافصل أسماء الواجهات باستخدام الفواصل. يجب الإقرار صراحةً بجميع أساليب الواجهة التي تُنفذها فئة بأنها **عامة** باستخدام الكلمة الأساسية `public` في الفئة. يجب أيضاً إقرار أي فئة تطبق واجهة بأنها **عامة**. يمكن لواجهة أن توسع واجهة أخرى باستخدام الكلمة الأساسية `extends` . ومع ذلك، لا يمكن لأي واجهة توسيع أكثر من واجهة واحدة.

### <a name="interface-example"></a>مثال لواجهة 

في المثال التالي، تقوم فئة **Automobile‎** بتنفيذ واجهة **IDrivable‎** . يتم دعم الكلمة الأساسية `is` وهي تتيح لك اختبار ما إذا كانت الفئة تقوم بتنفيذ واجهة أم لا.

```xpp
public interface IDrivable
{
    public int getSpeed()
     {
     }

    public void setSpeed(int newSpeed)
     {
     }
}

class Automobile implements IDrivable
 {
   int m_speed;

   public int getSpeed()
    {
         return m_speed;
    }

   public void setSpeed(int newSpeed)
    {
         m_speed = newSpeed;
    }
 }

class UseAnAutomobile
 {
   void DriveAutomobile()
    {
       IDrivable yourIDrivable;
       Automobile myAutomobile;
       str sTemp = "object is not an IDrivable";
    
       myAutomobile = new Automobile();

       if (myAutomobile is IDrivable)
       {
          yourIDrivable = myAutomobile;
          yourIDrivable.setSpeed(42);
          sTemp = int2str(yourIDrivable.getSpeed());
       }

       Global::info(sTemp);
       return;
    }
}
```
