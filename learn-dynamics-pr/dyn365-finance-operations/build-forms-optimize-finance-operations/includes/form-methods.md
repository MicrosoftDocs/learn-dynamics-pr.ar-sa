---
ms.openlocfilehash: 6e925260f197c7c940782f004e14b4123b014d1b
ms.sourcegitcommit: 442020b85a494c94b76f90102daf2916649c8c2e
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/28/2022
ms.locfileid: "8490167"
---
تعتبر النماذج عناصر رئيسة للنظام الأساسي لتطوير التمويل والعمليات. العديد من النماذج القياسية متوفرة بالفعل في التطبيق. 

يمكنك أيضاً إنشاء نماذج جديدة. يتكون كل نموذج من أساليب النماذج، والتي يمكن تصنيفها كأساليب قياسية أو أساليب مخصصة. يجب أن يكون للأساليب القياسية استدعاء `super()` لتنفيذ الأسلوب الأصلي. تتوفر الأساليب القياسية والمخصصة مع كافة النماذج القياسية والمخصصة. يمكنك توسيع أساليب النموذج الموجودة وتضمين التعليمات البرمجية باستخدام ‏‫سلسله الأوامر‬. 

## <a name="standard-form-methods"></a>أساليب النماذج القياسية
توضح الأقسام التالية أساليب النماذج القياسية في النظام الأساسي لتطوير تطبيقات التمويل والعمليات.

### <a name="init"></a>init()
الأسلوب `init()` هو أسلوب قياسي يتم استدعاؤه عند فتح نموذج. يساعد هذا الأسلوب في تهيئة النموذج، ويتم تشغيله بعد أسلوب الدالة الإنشائية `new()`. يعد الأسلوب `init()` مسؤولاً عن إنشاء واجهة وقت التشغيل الخاصة بالنموذج. غالباً، ما ستستخدم هذا الأسلوب عند الحاجة إلى:

- تهيئة متغيرات مستوى النموذج.
- الحصول على بيانات المعلمة من args().
- تهيئة استعلام مصدر البيانات.
- تعيين خصائص عناصر التحكم التي لا تعتمد على السجل.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل من النوع تعداد يسمى **TrainingType‎** ويحتوي على قيمتين: **عبر الإنترنت** و **الفصل الدراسي**. يجب فتح النموذج باستخدام تلك السجلات التي يكون **TrainingType‎** بها **متصلاً**. 

ويكون نمط التعليمات البرمجية على النحو التالي:

```xpp
public void init()
    {
        super();
        TrainingMaster_ds.query().dataSourceName("TrainingMaster")
        .addRange(fieldNum(TrainingMaster,TrainingType))
        .value(enum2Str(TrainingType::Online));
    }
```

> [!NOTE]
> يجب إجراء التعديلات على مصدر البيانات بعد استدعاء `super()` فقط لأن التهيئة الأساسية تحدث هناك.

### <a name="close"></a>close() 
الأسلوب `close()` هو أسلوب قياسي يتم استدعاؤه عند إغلاق نموذج. ويقوم الاستدعاء `super()` في هذا الأسلوب بإغلاق النموذج وإدارة تحديثات قاعدة البيانات وتعيين الأسلوب `closed()` على صحيح. يمكنك استخدام الأسلوبين `closeCancel()` أو `closeOK()` لبدء الأسلوب `close()`. بالإضافة إلى ذلك، يمكنك استخدام الأسلوب `close()` لإجبار مسح القيم لمتغير معين أو إلغاء تخصيص فئة. تأكد من إكمال هذه الإجراءات قبل الاستدعاء `super()`. غالباً ما يتم استدعاء فئات **NumberSequence‎** من الأسلوب `close()` لتسهيل عملية الإيقاف.

### <a name="closecancel"></a>closeCancel()
الأسلوب `closeCancel()` هو أسلوب قياسي يتم استدعاؤه عند إلغاء نموذج. يقوم الاستدعاء `super()` في هذا الأسلوب بتحديث القيمة المنطقية لـ `closedCancel()`ويضمن عدم حفظ التعديلات في النموذج.
 
### <a name="closeok"></a>closeOK()
الأسلوب `closeOK()` هو أسلوب قياسي يتم استدعاؤه عند إغلاق النموذج عن طريق تحديد الزر **موافق**. يقوم الاستدعاء `super()` في هذا الأسلوب بتحديث القيمة المنطقية لـ `closedOK()` ويستدعي الأسلوب `close()`.

### <a name="run"></a>run()
الأسلوب `run()`هو أسلوب قياسي يتم استدعاؤه مباشرة بعد الأسلوب `init()`. يؤدي الاستدعاء `super()` في هذا الأسلوب إلى ظهور نافذة النموذج على الشاشة ويقوم بالبحث عن قاعدة بيانات لعرض البيانات في النموذج.

تتضمن الأسباب النموذجية لتجاوز هذا الأسلوب:

- تنشيط بعض الحقول أو إلغاء تنشيطها.
- تعديل الاستعلام.

## <a name="standard-form-data-source-methods"></a>أساليب مصدر بيانات النماذج القياسية
توضح الأقسام التالية أساليب مصدر بيانات النماذج القياسية في النظام الأساسي لتطوير تطبيقات التمويل والعمليات.

### <a name="init"></a>init()
الأسلوب `init()` هو أسلوب قياسي لمصدر بيانات نموذج والذي يتم استدعاؤه عند فتح نموذج بعد تطبيق أسلوب النموذج `init()`. يساعد هذا الأسلوب على إنشاء استعلام مصدر البيانات استناداً إلى خصائص مصدر البيانات.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل من النوع تعداد يسمى **TrainingType‎** ويحتوي على قيمتين: **عبر الإنترنت** و **الفصل الدراسي**. يجب فتح النموذج باستخدام تلك السجلات، التي يكون **TrainingType‎** بها **متصلاً**. 

ويجب أن يكون نمط التعليمات البرمجية على النحو التالي:

```xpp
[DataSource]
    class TrainingMaster
    {

        public void init()
        {
            super();
            this.query().dataSourceName("TrainingMaster")
            .addRange(fieldNum(TrainingMaster,TrainingType))
            .value(enum2Str(TrainingType::Online));
        }

    }
```

### <a name="active"></a>active()
الأسلوب `active()` هو أسلوب قياسي لمصدر بيانات النموذج الذي يتم استدعاؤه عند انتقال أحد المستخدمين إلى سجل جديد.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل يسمى **المكان** وحقل من النوع تعداد يسمى **TrainingType**، والذي يحتوي على قيمتين **عبر الإنترنت‏‎** و **الفصل الدراسي‏‎**. بينما تقوم بالتنقل خلال السجلات، لن يمكن تحرير حقل **المكان** إذا كان **TrainingType‎** **متصلاً**. وإلا، سيكون حقل **المكان** قابلاً للتحرير. 

ويجب أن يكون نمط التعليمات البرمجية على النحو التالي:

```xpp
[DataSource]
    class TrainingMaster
    {
        public int active()
        {
            int ret;
        
            ret = super();
            TrainingMaster_ds.object(fieldNum(TrainingMaster, 
            Venue)).allowEdit(TrainingMaster.TrainingType == TrainingType::Classroom);
        
            return ret;
        }

    }
```

### <a name="validatewrite"></a>validateWrite()
يعد الأسلوب `validateWrite()` أسلوباً قياسياً لمصدر بيانات نموذج، والذي يتم استدعاؤه عند محاولة أحد المستخدمين حفظ سجل لتحديد ما إذا كانت البيانات صالحة وجاهزة للكتابة أم لا.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل تاريخ يسمى **TrainingDate‎**. يجب عدم السماح ببيانات التدريب القديمة. 

يمكن أن يكون نمط التعليمات البرمجية التالي وسيلة لتحقيق هذه النتيجة:

```xpp
    [DataSource]
    class TrainingMaster
    {
        public boolean validateWrite()
        {
            boolean ret;
        
            ret = super() && (TrainingMaster.TrainingDate >= today());
        
            return ret;
        }
    }
```

> [!NOTE]
> لا تريد السماح للأسلوب `validateWrite()` بالفشل دون رسالة فيما يتعلق بالسبب. أفضل ممارسة هي إرسال خطأ برسالة معينة بدلاً من استخدام الرجوع المنطقي للعبارة `if`.

### <a name="validatedelete"></a>validateDelete()
الأسلوب `validateDelete()` هو أسلوب قياسي لمصدر بيانات نموذج، والذي يتم استدعاؤه عندما يحاول مستخدم حذف سجل، وذلك لتأكيد الحذف.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل تاريخ يسمى **TrainingDate‎**. يجب عدم حذف أي بيانات تدريب قديمة. 

يمكن أن يكون نمط التعليمات البرمجية التالي وسيلة لتحقيق هذه النتيجة:

```xpp
    [DataSource]
    class TrainingMaster
    {
        public boolean validateDelete()
        {
            boolean ret;
        
            ret = super() && (TrainingMaster.TrainingDate >= today());
        
            return ret;
        }
    }
```

> [!NOTE]
> يجب عليك إرسال خطأ برسالة بدلاً من أن تدع أسلوب `validateDelete()` يفشل في صمت.

### <a name="executequery"></a>executeQuery()
يعد الأسلوب `executeQuery()` أسلوباً قياسياً لمصدر بيانات نموذج يقوم بتشغيل استعلام مصدر البيانات ويعرض السجلات التي تم استردادها. يمكنك تطبيق عامل تصفية على مصدر البيانات الذي يستخدم استعلام عن طريق تجاوز `executeQuery()`. الفرق الرئيسي بين هذا الأسلوب والأسلوب `init()` هو أن الأسلوب `init()` يعمل مرة واحدة أثناء فتح النموذج، بينما يتم تشغيل الأسلوب `executeQuery() ` عند تحديث النموذج. 

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل من النوع تعداد يسمى **TrainingType‎** ويحتوي على قيمتين: **عبر الإنترنت** و **الفصل الدراسي**. يجب تصفية البيانات الموجودة في النموذج من خلال **Trainingtype‎** **متصل** فقط.

```xpp
[DataSource]
    class TrainingMaster
    {
        public void executeQuery()
        {
            QueryBuildDataSource  queryBuildDataSource;
 
            queryBuildDataSource = 
               this.query().dataSourceTable(tablenum(TrainingMaster));
            queryBuildDataSource.clearRanges();
            queryBuildDataSource.addRange(fieldnum(TrainingMaster, 
               TrainingType)).value(enum2Str(TrainingType::Online));

            super();
        }
        }
```

### <a name="initvalue"></a>initValue()
الأسلوب `initValue()` هو أسلوب قياسي لمصدر بيانات النموذج. بينما تقوم بإدراج سجل جديد، يمكن أن يساعدك `initValue()` على تهيئة قيم الحقول. يتم استدعاء هذا الأسلوب عند إنشاء سجل جديد. 

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل تاريخ يسمى **TrainingDate‎**. أثناء إنشاء سجل جديد، يجب تهيئة حقل **TrainingDate‎** بتاريخ اليوم. 

ويمكن أن يكون نمط الترميز على النحو التالي:

```xpp
[DataSource]
    class TrainingMaster
    {
        public void initValue()
        {
            super();
            TrainingMaster.TrainingDate = today();
        }
         }
```

### <a name="write"></a>write()

الأسلوب `write()` هو أسلوب قياسي لمصدر بيانات النموذج. يتم استدعاء هذا الأسلوب عند تعديل سجل وعند محاولة حفظه بواسطة تحديد الزر **حفظ** أو التنقل خارج السجل.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل حقيقي يسمي **السعر** والذي يشير إلى السعر الإجمالي للمدرب. ويحتوي أيضاً على حقل عدد صحيح يسمي **NoofDays‎** والذي يشير إلى مدة التدريب. بالإضافة إلى ذلك، يحتوي الجدول على حقل يسمي **TrainerID‎**، والذي يقوم بإنشاء مفتاح خارجي مع **TrainerTable‎**. يحتوي **TrainerTable‎** على حقل حقيقي يسمي **المعدل**، والذي يلتقط المعدل اليومي للمدربين. 

وبعد حفظ السجل في الجدول **TrainingMaster‎**، يجب تحديث حقل **السعر** الخاص بجدول **TrainerMaster‎** بضرب **NoofDays‎** و **معدل** **TrainerTable‎**. 

ويكون نمط الترميز على النحو التالي:

```xpp
[DataSource]
    class TrainingMaster
    {
        public void write()
        {
            TrainingMaster.Price = TrainerTable::find(TrainingMaster.TrainerID).Rate * TrainingMaster.NoofDays;
            super();
        }
    }
```

### <a name="delete"></a>delete()
الأسلوب `delete()` هو أسلوب قياسي لمصدر بيانات النموذج. يتم استدعاء هذا الأسلوب عند حذف سجل. 

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل يسمي **TrainerID‎**، والذي له علاقة مفتاح خارجي مع **TrainerTable‎**. **TrainerTable** يحتوي على حقل يسمى **TrainingCount**. المتطلب هو تقليل رقم **TrainingCount‎** بمقدار واحد إذا تم حذف سجل من الجدول **TrainingMaster‎**. 

ويمكن أن يكون نمط الترميز على النحو التالي:

```xpp
public void delete()
        {
            TrainerTable    trainerTable;
            ttsbegin;
            trainerTable = TrainerTable::find(TrainingMaster.TrainerID, true);
            trainerTable.TrainingCount = trainerTable.TrainingCount - 1;
            trainerTable.update();
            ttscommit;
            super();
            
        }
```

## <a name="standard-form-data-source-field-methods"></a>أساليب حقل مصدر بيانات النماذج القياسية
توضح الأقسام التالية أساليب حقل مصدر بيانات النماذج القياسية في النظام الأساسي لتطوير تطبيقات التمويل والعمليات.

#### <a name="modified"></a>modified()
الأسلوب `modified()` هو أسلوب قياسي لحقل مصدر بيانات النموذج. يتم استدعاء هذا الأسلوب عند تعديل قيمة حقل معين.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل يسمى **المكان** وحقل من النوع تعداد يسمى **TrainingType** والذي يحتوي على قيمتين: **عبر الإنترنت‏‎** و **الفصل الدراسي‏‎**. إذا تم تحديد **متصل** لـ **TrainingType‎**، فإن حقل **المكان** يجب أن يصبح فارغاً.

ويمكن أن يكون نمط الترميز على النحو التالي:

```xpp
[DataSource]
    class TrainingMaster
    {
        [DataField]
        class TrainingType 
        {
            public void modified()
            {
                super();
                if(TrainingMaster.TrainingType == TrainingType::Online)
                    TrainingMaster.Venue = "";
            }

        }

    }
```

### <a name="validate"></a>validate()
الأسلوب `validate()` هو أسلوب قياسي لحقل مصدر بيانات النموذج. يتم استدعاء هذا الأسلوب عند إدخال قيمة في حقل معين، ويتم تجاوزها في حالة الحاجة إلى التحقق من صحة الحقل الإضافي.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل يسمى **المشاركون**، حيث لا يسمح بإدخال رقم أعلى من **20**. 

ويمكن أن يكون نمط الترميز على النحو التالي:

```xpp
    [DataSource]
    class TrainingMaster
    {
        [DataField]
        class Participants 
        {
            public boolean validate()
            {
                boolean ret;
                ret = super() && (TrainingMaster.Participants <= 20);
                return ret;
            }

        }

    }
```

تأكد من تقديم سبب للأخطاء التي تم طرحها، كما هو موضح في المثال التالي للتعليمات البرمجية:
 
```xpp
    [DataSource]
    class TrainingMaster
    {
        [DataField]
        class Participants 
        {
            public boolean validate()
            {
                boolean ret;
                if (TrainingMaster.Participants > 20)
                {
                    throw error("Maximum 20 participants");
                    return false;
                }
                ret = super();
                return ret;
            }
        }
    }

```

### <a name="lookup"></a>lookup()
الأسلوب `lookup()` هو أسلوب قياسي لحقل مصدر بيانات النموذج. يتم استدعاء هذا الأسلوب عند محاولة إجراء عملية بحث على حقل مصدر بيانات. إذا كان يجب تخصيص البيانات المعروضة في نموذج البحث مع بعض عوامل التصفية، فإنه يجب تجاوز الأسلوب `lookup()`.

**مثال**

لديك نموذج مخصص يحتوي على جدول مسمى **TrainingMaster‎**. يحتوي الجدول على حقل يسمي **TrainerID‎**، والذي يقوم بإنشاء مفتاح خارجي مع **TrainerTable‎**. يحتوي **TrainerTable** على حقل تعداد يسمى **TrainerType** والذي يحتوي على قيمتين: **فني** و **وظيفي**. يجب أن يقوم البحث في حقل **TrainerID** بعرض المدربين الفنيين فقط. 

ويمكن أن يكون نمط الترميز على النحو التالي:

```xpp
    [DataSource]
    class TrainingMaster
    {
        [DataField]
        class TrainerID 
        {
            public void lookup(FormControl _formControl, str _filterStr)
            {
                SysTableLookup sysTableLookup = 
                   SysTableLookup::newParameters(tableNum(TrainerTable),_formControl);
                
                Query query = new Query();
                QueryBuildDataSource qbds;
                qbds= query.addDataSource(tableNum(TrainerTable));
                qbds.addRange(fieldNum(TrainerTable, 
                     TrainerType)).value(enum2Str(TrainerType::Technical));

                sysTableLookup.addLookupfield(fieldNum(TrainerTable,TrainerID));
                sysTableLookup.addLookupfield(fieldNum(TrainerTable,TrainerName));

                sysTableLookup.parmQuery(query);
                sysTableLookup.performFormLookup();
            }
        }
    }
```

## <a name="extension-of-a-form-method"></a>ملحق أسلوب النموذج
سلسلة الأوامر عبارة عن خيار يساعدك على تحسين وظيفة أسلوب النموذج. ينطبق هذا الخيار على الأساليب القياسية والأساليب المخصصة للنموذج.

يمكنك استخدام نمط التعليمات البرمجية التالي إذا كنت بحاجة إلى توسيع أسلوب النموذج `init()`:

```xpp
[ExtensionOf(formStr(Currency))]
final class CurrencyForm_Extension
{
    public void init()
    {
        //code
        next init();
        //code
    }

}
```

## <a name="extension-of-a-form-data-source-method"></a>ملحق أسلوب مصدر بيانات النموذج
سلسلة الأوامر عبارة عن خيار يساعدك على تحسين وظيفة أسلوب مصدر بيانات النموذج. ينطبق هذا الخيار على الأساليب القياسية والأساليب المخصصة للنموذج.

يمكنك استخدام نمط التعليمات البرمجية التالي إذا كنت بحاجة إلى توسيع أسلوب مصدر بيانات النموذج `initValue()`:

```xpp
[ExtensionOf(FormDataSourceStr(Currency, Currency))]
final class CurrencyFormCurrencyTableDataSource_Extension
{
    public void initValue()
    {
        //code
        next initValue();
        //code
    }

}
```

## <a name="extension-of-a-form-data-source-field-method"></a>ملحق أسلوب حقل مصدر بيانات النموذج
سلسلة الأوامر عبارة عن خيار يساعدك على تحسين وظيفة أسلوب حقل مصدر بيانات النموذج. ينطبق هذا الخيار على الأساليب القياسية والأساليب المخصصة للنموذج.

يمكنك استخدام نمط التعليمات البرمجية التالي إذا كنت بحاجة إلى توسيع أسلوب حقول مصدر بيانات النموذج `lookup()`:

```xpp
[ExtensionOf(formDataFieldStr(CustTable, CustTable, CustGroup))]
final class CustTableFormDataFieldCustGroup_Extension
{
    public void lookup(FormControl _formControl, str _filterStr)
    {
        //Code
        next lookup(_formControl, _filterStr);
        //Code
    }

}
```

## <a name="extension-of-a-form-control-method"></a>ملحق أسلوب التحكم في النموذج
سلسلة الأوامر عبارة عن خيار يساعدك على تحسين وظيفة أسلوب التحكم في النموذج. ينطبق هذا الخيار على الأساليب القياسية والأساليب المخصصة للنموذج.

يمكنك استخدام نمط التعليمات البرمجية التالي إذا كنت بحاجة إلى توسيع أسلوب عنصر تحكم زر النموذج `clicked()`:

```xpp
[ExtensionOf(formControlStr(CustTable, DirPartyEntityAssociationUpdate))]
final class CustTableFormControlDirPartyEntityAssociationUpdate_Extension
{
    public void clicked()
    {
        //code
        next clicked();
        //Code
    }

}
```
