---
ms.openlocfilehash: 9bc5c6684d673303b5f9316229c0e398e0f37880
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072277"
---

يأتي Visual Studio مع SysTest Framework الذي يسمح لك بكتابة كود اختبار الوحدة، ودمج الاختبارات، ثم تشغيل الاختبار لأتمتة اختبار الكود. يمكنك إعداد SysTest Framework لإنشاء اختبار وحدة نمطية من الكود. يمكنك أيضاً استيراد تسجيلات مسجل المهام إلى Visual Studio لإنشاء كود اختبار. يتم توفير مزيد من المعلومات حول مسجل المهام لاحقاً في هذه الوحدة النمطية.  

يمكن بعد ذلك دمج اختبارك في وحدة اختبار نمطية يمكن استخدامها لإدارة كود الاختبار و`FormAdaptors`. ستسمح لك إضافة وحدة الاختبار النمطية إلى عنصر التحكم في المصدر بدمج اختبارك مع عملية الإنشاء. ستعمل هذه الإضافة بعد ذلك على تشغيل كود الاختبار أثناء الإنشاء للتحقق من أن جميع الوظائف تعمل بالشكل المتوقع.

يمكنك أيضاً تشغيل كود الاختبار بشكل فردي. يعد تشغيل أكواد الاختبار عملية قابلة للتكرار، لذلك عند إنشاء فئة الاختبار، يمكنك تشغيلها عدة مرات. تسمح لك هذه التكرارات بالتحقق من صحة تغييرات الأكواد باستمرار. بالإضافة إلى ذلك، يعد تشغيل الاختبارات بسرعة للتحقق مما إذا كانت وظيفتك لا تزال تعمل بعد تعديل مطور آخر للعنصر أمراً أساسياً لتحقيق الإنتاجية. 

يمكن أن يكون خيار إعادة تشغيل الاختبارات مفيداً أيضاً لإنتاجية مؤسستك خلال الترقيات التي تم إصدارها بواسطة Microsoft. بدلاً من طلب موارد المستخدم لاختبار انحدار جميع الوظائف من واجهة المستخدم، يمكنك تشغيل اختبارات الوحدة النمطية هذه التي ستدخل البيانات المطلوبة وتشغيل عمليات الاختبار لتحديد ما إذا كانت الوظيفة تعمل على النحو المتوقع.

![مخطط لعملية نموذج اختبار الوحدة النمطية من اختبارات المؤلف، ودمج الاختبارات ثم تنفيذها.](../media/unit-test.jpg)

لإنشاء حالة اختبار جديدة لاختبار الوظائف في أحد التطبيقات، اتبع الخطوات التالية:

1.  افتح Visual Studio كمسؤول.
2.  قم بإنشاء مشروع جديد.
3.  أضف فئة جديدة إلى المشروع.
4.  قم بتوسيع فئة **SysTestCase** في إقرار الفئة.
5.  أضف أساليب إلى الفئة لتحديد الاختبار. ويجب أن تستخدم هذه الأساليب سمة **[SysTestMethodAttribute]**.
6.  يمثل الكود التالي مثالاً لفئة اختبار باستخدام نموذج "إدارة الأسطول".

```xpp
class FMUnitTestSample extends SysTestCase
 {
   public void setup()
   {
     // Reset the test data to be sure things are clean
     FMDataHelper::main(null);
   }
    
  [SysTestMethodAttribute]
   public void testFMTotalsEngine()
   {
      FMRental rental;
      FMTotalsEngine fmTotals;
      FMRentalTotal fmRentalTotal;
      FMRentalCharge rentalCharge;
      FMRentalTotal expectedtotal;
      str rentalID = '000022';

      // Find a known rental
      rental = FMRental::find(rentalID);

     // Get the rental charges associated with the rental
     // Data is seeded randomly, so this will change for each run
     select sum(ExtendedAmount) from rentalCharge
         where rentalCharge.RentalId == rental.RentalId;

     fmTotals = FMTotalsEngine::construct();
     fmTotals.calculateRentalVehicleRate(rental);

     // Get the totals from the engine
     fmRentalTotal = fmTotals.totals(rental);

     // Set the expected amount
     expectedTotal = rental.VehicleRateTotal + rentalCharge.ExtendedAmount;

     this.assertEquals(expectedTotal,fmRentalTotal);

   }

   [SysTestMethodAttribute]
   public void testFMCarValidateField()
   {
     FMCarClass fmCar;

     fmCar.NumberOfDoors = -1;
     this.assertFalse(fmCar.validateField(Fieldnum("FMCarClass", "NumberOfDoors")));
  }

 }
```
7.  احفظ الفئة. ستتوفر حالتا اختبار في "مستكشف الاختبارات".
8.  أنشئ المشروع.
9. في قائمة **الاختبار**، افتح **Windows > "مستكشف الاختبارات"**.
10. حدد **تشغيل الاختبار المحدد** لتشغيل حالة اختبار محددة. سيتم عرض النتائج بعد اكتمال **مستكشف الاختبارات**.

يمكنك إنشاء وحدة اختبار نمطية للمساعدة في إدارة أكواد الاختبار. تسمح إضافة وحدات اختبار نمطية للتحكم في المصادر لعملية الإنشاء بالعثور على الوحدات النمطية التي تحتوي على كلمة "اختبار" في الاسم وتنفيذ تشغيل الاختبار.

لإنشاء وحدة اختبار نمطية، اتبع الخطوات التالية:

1.  في Visual Studio، افتح **Dynamics 365 > إدارة النماذج > إنشاء نموذج**.
2.  أدخِل اسم النموذج الذي يتضمن كلمة "اختبار".
3.  أضف مراجع إلى النماذج التالية:
    -   النظام الأساسي للتطبيق
    -   أساس التطبيق
    -   أساسيات الاختبار
    -   محول نموذج أساس التطبيق
    -   محول نموذج النظام الأساسي للتطبيق
    -   تكامل التقارير الإلكترونية لمجموعة التطبيقات
    -   محول نموذج مجموعة التطبيقات
4.  حدد **التالي**.
5.  حدد **إنهاء**.
