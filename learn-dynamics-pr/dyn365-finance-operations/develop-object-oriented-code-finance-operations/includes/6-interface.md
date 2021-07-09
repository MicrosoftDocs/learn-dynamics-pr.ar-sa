---
ms.openlocfilehash: 4b8e952e1d240d1b57a3d0fbf0f398f9b5302d72
ms.sourcegitcommit: 45337c216dae17eda3fd77996e054b20515eb8dc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "6072101"
---
<span data-ttu-id="ab9d9-101">تُعد *الواجهة* مواصفة لمجموعة من أساليب المثيل العام.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-101">An *interface* is a specification for a set of public instance methods.</span></span>
<span data-ttu-id="ab9d9-102">تحدد الواجهة أوجه التشابه بين الفئات غير المرتبطة وتفرضها دون الحاجة إلى اشتقاق فئة واحدة من الأخرى.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-102">An interface defines and enforces similarities between unrelated classes without having to derive one class from the other.</span></span> <span data-ttu-id="ab9d9-103">تعتبر جميع الواجهات عامة، حتى إذا لم تضف بشكل صريح الكلمة الرئيسية `public` أمام الكلمة الرئيسية `interface` في الكود `classDeclaration` .</span><span class="sxs-lookup"><span data-stu-id="ab9d9-103">All interfaces are public, even if you don't explicitly add the `public` keyword in front of the `interface` keyword in the `classDeclaration` code.</span></span> <span data-ttu-id="ab9d9-104">تعتبر الأساليب الموجودة بالواجهة عامة أيضاً.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-104">The methods on an interface are also public.</span></span>  

<span data-ttu-id="ab9d9-105">لإنشاء واجهة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ab9d9-105">To create an interface, follow these steps:</span></span>

1.  <span data-ttu-id="ab9d9-106">في مستكشف الحلول، انقر بزر الماوس الأبيض فوق مشروع ثم حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-106">In Solution Explorer, right-click the project, and then select **Add**.</span></span>
2.  <span data-ttu-id="ab9d9-107">في مربع الحوار **عنصر جديد** ، حدد **الواجهة** ثم أدخل اسماً للواجهة.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-107">In the **New Item** dialog box, select **Interface** and then enter a name for the interface.</span></span>
3.  <span data-ttu-id="ab9d9-108">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-108">Select **Add**.</span></span>

<span data-ttu-id="ab9d9-109">عندما تضيف الكلمة الأساسية `implements` في إقرار الفئة، يجب أن تقر الفئة بالأساليب التي تحددها الواجهة.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-109">When you add the `implements` keyword on a class declaration, the class must declare the methods that are specified by the interface.</span></span> <span data-ttu-id="ab9d9-110">يمكن لإقرار الفئة تطبيق واجهات متعددة.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-110">A class declaration can implement multiple interfaces.</span></span> <span data-ttu-id="ab9d9-111">اسرد الواجهات بعد تكرار واحد للكلمة الأساسية `implements` وافصل أسماء الواجهات باستخدام الفواصل.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-111">List the interfaces after the single occurrence of the `implements` keyword and separate the interface names by using commas.</span></span> <span data-ttu-id="ab9d9-112">يجب الإقرار صراحةً بجميع أساليب الواجهة التي تُنفذها فئة بأنها **عامة** باستخدام الكلمة الأساسية `public` في الفئة.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-112">All interface methods that a class implements must be explicitly declared as **public** by using the `public` keyword in the class.</span></span> <span data-ttu-id="ab9d9-113">يجب أيضاً إقرار أي فئة تطبق واجهة بأنها **عامة**.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-113">A class that implements an interface must also be declared as **public**.</span></span> <span data-ttu-id="ab9d9-114">يمكن لواجهة أن توسع واجهة أخرى باستخدام الكلمة الأساسية `extends` .</span><span class="sxs-lookup"><span data-stu-id="ab9d9-114">An interface can extend another interface by using the `extends` keyword.</span></span> <span data-ttu-id="ab9d9-115">ومع ذلك، لا يمكن لأي واجهة توسيع أكثر من واجهة واحدة.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-115">However, an interface can't extend more than one interface.</span></span>

### <a name="interface-example"></a><span data-ttu-id="ab9d9-116">مثال لواجهة</span><span class="sxs-lookup"><span data-stu-id="ab9d9-116">Interface example</span></span> 

<span data-ttu-id="ab9d9-117">في المثال التالي، تقوم فئة **Automobile‎** بتنفيذ واجهة **IDrivable‎** .</span><span class="sxs-lookup"><span data-stu-id="ab9d9-117">In the following example, an **Automobile** class implements an **IDrivable** interface.</span></span> <span data-ttu-id="ab9d9-118">يتم دعم الكلمة الأساسية `is` وهي تتيح لك اختبار ما إذا كانت الفئة تقوم بتنفيذ واجهة أم لا.</span><span class="sxs-lookup"><span data-stu-id="ab9d9-118">The `is` keyword is supported and lets you test whether a class implements an interface.</span></span>

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
