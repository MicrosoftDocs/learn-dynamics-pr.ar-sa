---
ms.openlocfilehash: b6a173f4c8ea173f36067afd486d1e4d6c64aad4
ms.sourcegitcommit: c1858cd3b2bd6663edff36e214795d4934ad3ddf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2022
ms.locfileid: "9581844"
---
الجداول هي العناصر الرئيسية للنظام الأساسي لتطوير تطبيقات التمويل والعمليات. تتوفر بالفعل العديد من الجداول القياسية في التطبيق. يُمكنك أيضًا إنشاء جدول مخصص جديد. 

يحتوي كل جدول على أساليب يُمكن تصنيفها على أنها أساليب قياسية أو أساليب مخصصة. يجب أن تحتوي الجداول القياسية على استدعاء `super()` لتشغيل منطق إطار العمل. ينطبق هذا المطلب أيضًا على الجداول المخصصة لأنها مشتقة من نفس النوع الأساسي. 

يُمكنك توسيع طرق الجدول الحالية وتضمين التعليمات البرمجية باستخدام خيار سلسلة الأوامر. بالإضافة إلى ذلك، يُمكنك إنشاء مفوضي الجدول لتضمين التعليمات البرمجية في أسلوب موجود. لإضافة وظائف إلى أسلوب جدول موجود، يجب أن يتم اشتراك هؤلاء المفوضين.

## <a name="standard-table"></a>جدول قياسي
توضح الأقسام التالية الأساليب المختلفة المستخدمة في الجداول القياسية في النظام الأساسي لتطوير تطبيقات التمويل والعمليات.

### <a name="initvalue"></a>initValue()
أسلوب `initValue()` هي طريقة قياسية يتم استدعاؤها عند إنشاء سجل جديد. يُمكنك استخدام هذا الأسلوب لمعالجة متطلبات تهيئة بعض قيم الحقول أثناء إنشاء سجل جديد.

**مثال**

لديك جدول مخصص يسمى **TrainingMaster**. الشرط هو تهيئة الحقل **TrainingType** لهذا الجدول باستخدام عنصر التعداد **عبر الإنترنت** أثناء إدراج سجل جديد في هذا الجدول. 

ويكون نمط الترميز على النحو التالي:

```xpp

    public void initValue()
    {
        super();
        this.TrainingType = TrainingType::Online;
    }
```

### <a name="find"></a>find()

الأسلوب `find()` هي طريقة مخصصة يتم إنشاؤها عادةً باستخدام جميع الجداول. يقوم الأسلوب `find()` بإرجاع سجل معين بناءً على المفتاح الأساسي أو المفاتيح الفريدة الأخرى. يمثل هذا الأسلوب أسلوبًا ثابتًا.

**مثال**

لديك جدول مخصص باسم **معلمات التدريب**. تحتاج إلى إنشاء أسلوب `find()` التي ستُرجع سجلًا واحدًا.

ويكون نمط الترميز على النحو التالي:

```xpp
static TrainingParameters find(boolean _forupdate = false)
    {
        TrainingParameters parameter;

        if (_forupdate)
        {
            parameter.selectForUpdate(_forupdate);
        }

        select firstonly parameter
            index Key
            where parameter.Key == 0;

        if (!parameter && !parameter.isTmp())
        {
            Company::createParameter(parameter);
        }

        return parameter;
    }
```
 
### <a name="insert"></a>insert()
أسلوب `insert()` هو طريقة قياسية يتم استدعاؤها عند إدراج سجل جديد في أحد الجداول. يُمكنك استخدام هذا الأسلوب في هذه السيناريوهات:

- قم بتعبئة البَيانات في حقل بناءً على قيمة بعض الحقول الأخرى في الجدول.
- قم بتشغيل عملية أثناء إدراج البَيانات في جدول.

**مثال**

في الجدول المخصص **TrainingMaster**، تحتاج إلى ملء البَيانات في الحقل **السعر**. قيمة هذا الحقل هي مضاعفة الحقلين التاليين:

- حقل **NoofDays** من جدول **TrainingMaster**
- الحقل **السعر لكل يوم** من جدول **معلمة التدريب**

ويكون نمط الترميز على النحو التالي:

```xpp
public void insert()
    {
        this.Price = this.NoofDays * TrainingParameters::find().PerDayPrice;
        super();
    }
```

### <a name="modifiedfield"></a>modifiedField()
يمثل الأسلوب `modifiedField()` طريقة قياسية يتم استدعاؤها عند تعديل حقل من السجل. يُمكنك استخدام هذا الأسلوب في هذه السيناريوهات:

- قم بتعبئة البَيانات في حقل بينما يتم تعديل حقل آخر في نفس السجل.
- قم بتشغيل عملية بينما يتم تعديل بعض الحقول في أحد السجلات.

**مثال**

الشرط هو محو القيمة من الحقل **مكان إقامة الحدث** في جدول **TrainingMaster**، بينما يكون **TrainingType** **عبر الإنترنت**. 

ويكون نمط الترميز على النحو التالي:

```xpp
public void modifiedField(FieldId _fieldId)
    {
        super(_fieldId);

        switch (_fieldId)
        {
            case fieldNum(TrainingMaster, TrainingType):
                this.Venue = (this.TrainingType == TrainingType::Online ? "" : this.venue);
                break;
        }
    }
```

### <a name="validatefield"></a>validateField()
يمثل الأسلوب `validateField()` الطريقة القياسية للتحقق من صحة البَيانات التي تم إدخالها في الحقل. يُمكنك استخدام هذا الأسلوب لإجراء التحقق من صحة البَيانات أثناء إدخال البَيانات في الحقل.

**مثال**

الشرط هو تقييد إدخال البَيانات في حقل مكان جدول **TrainingMaster**، إذا كان **TrainingType** هو **عبر الإنترنت**. 

ويكون نمط الترميز على النحو التالي:

```xpp
public boolean validateField(FieldId _fieldIdToCheck)
    {
        boolean ret = super(_fieldIdToCheck);
        
        switch(_fieldIdToCheck)
        {
            case fieldNum(TrainingMaster, Venue):
                if (this.TrainingType == TrainingType::Online && this.Venue)
                {
                    ret = ret && checkFailed("Online training does not require venue");
                }
                break;
        }
        return ret;
    }
```

### <a name="validatewrite"></a>validateWrite()
يمثل الأسلوب `validateWrite()` طريقة قياسية على الجداول. يتم استدعاء هذه الطريقة عند تحديد الزر **حفظ** أو عندما يحاول المستخدم الخروج من سجل بعد إدخال سجل جديد أو تحديث سجل موجود. تجاوز هذا الأسلوب إذا كان يجب التحقق من صحة الشرط قبل ترك السجل.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل يسمي **TrainerID‎**، والذي يقوم بإنشاء مفتاح خارجي مع **TrainerTable‎**. يمتلك **TrainerTable** الحقل الحقيقي **المعدّل**، والذي يرصد المعدّل اليومي للمدربين. عند حفظ السجل في الجدول **TrainingMaster**، يجب على النظام التحقق مما إذا كان **المعدّل** محددًا للمدرب المطابق. 

ويمكن أن يكون نمط الترميز على النحو التالي:

```xpp
public boolean validateWrite()
    {
        boolean ret;
         
        ret = super();

        if(!TrainerTable::find(this.TrainerID).Rate)
        {
            ret = checkFailed("Please enter Trainer's rate");
        }
    
        return ret;
    }
```

## <a name="extension-of-table-methods"></a>ملحق أساليب الجدول
سلسلة الأوامر هي خيار يساعدك على تحسين وظائف أسلوب الجدول. هذا الخيار قابل للتطبيق على الأساليب القياسية والأساليب المخصصة.

في المثال التالي، يكون المتطلب هو تهيئة القاعدة **تقريب السعر** لجدول **العملة** بـ **0.01** كلما تم إنشاء سجل جديد. سيتم إنشاء فئة امتداد الجدول باستخدام القصاصة البرمجية للأسلوب `initValue()` هذا.

```xpp
 [ExtensionOf(tableStr(Currency))]
final class CurrencyTable_Extension
{
    public void initValue()
    {
        this.RoundOffPrice = 0.01;
        next initValue();
    }

}
```

تستدعي الكلمة الأساسية `next` الأسلوب الأصل من الأسلوب الموسّع. لن تحتاج إلى استخدام الكلمة الأساسية `next`، إذا تم إنشاء أسلوب مخصص جديد في الجدول الموسع. 
