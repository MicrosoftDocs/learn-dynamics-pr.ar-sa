---
ms.openlocfilehash: 1857826e47626c5d44672a98323357172fa3501e
ms.sourcegitcommit: c1e0c2e1de92b19183313a689ec3e6d97664ae20
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/25/2022
ms.locfileid: "8487852"
---
في Dynamics 365، يُمكنك استخدام كائنات الاستعلام في النظام الأساسي للتطوير لإنشاء عبارات SQL. يُمكنك استخدام هذه الاستعلامات لعرض البَيانات في نماذج وتقارير وطرق عرض والمزيد. بالإضافة إلى ذلك، يُمكنك كتابة جمل SQL باستخدام استعلامات التحديد. يساعدك كائن الاستعلام في إنشاء SQL ديناميكيًا في وقت التشغيل. 

بدلاً من استخدام الجداول مباشرةً، نوصي باستخدام كائنات الاستعلام في النماذج. باستخدام كائنات الاستعلام، يُمكنك تحديد تلك الحقول التي تريد عرضها في النموذج، على عكس الجداول. سيساعد هذا الأسلوب في تقليل حجم عبارة SQL التي تعمل خلف النموذج، كما تساعد في تحسين الأداء. ينطبق المفهوم نفسه على التقارير والآراء أيضًا.

## <a name="querybuilddatasource-class"></a>فئة QueryBuildDataSource
فئة **QueryBuildDataSource** هي كتلة الإنشاء لإنشاء الاستعلام. يحدد مصدر البَيانات المراد إضافته إلى الاستعلام. يُمكنه تحديد حقول الجدول المراد إضافتها وترتيب فرز السجلات وما إلى ذلك. بالإضافة إلى ذلك، يُمكنه إنشاء العلاقة من خلال تطبيق الصلات بين مصادر البَيانات.

### <a name="example"></a>مثال
لديك جدول **TrainingMaster** به الحقلين: **TrainingID** و **TrainingDate**. من خلال إنشاء كائن استعلام، تحتاج إلى عرض كلا الحقلين بالترتيب التصاعدي لـ **TrainingID**. ويكون نمط الترميز على النحو التالي:

```xpp
 class TrainingMasterQuery
 {
    public static void main(Args _args)
    {
        QueryBuildDataSource    qbds;

        Query query = new Query();
 
        qbds = query.addDataSource(tableNum(TrainingMaster));
        qbds.addSortField(fieldNum(TrainingMaster, TrainingID), SortOrder::Ascending);

        QueryRun queryRun = new QueryRun(query);
 
        while (queryRun.next())
        {
            TrainingMaster trainingMaster = queryRun.get(tableNum(TrainingMaster));
            info(strFmt("%1, %2", trainingMaster.TrainingID, date2Str(trainingMaster.TrainingDate, 123, DateDay::Digits1or2, DateSeparator::Hyphen, DateMonth::Digits1or2, DateSeparator::Hyphen, DateYear::Digits4)));
        }
    }
}
```

## <a name="querybuildrange-class"></a>فئة QueryBuildRange
تحدد فئة **QueryBuildRange** تصفية السجلات التي يتم جلبها من مصدر البَيانات.

### <a name="example"></a>مثال
في الجدول **TrainingMaster**، تمت إضافة حقل جديد باسم **TrainingType**. يحتوي هذا الحقل الجديد على قيمتين: **Online** و **Classroom**. تحتاج إلى تصفية جميع التدريبات عبر الإنترنت من خلال إنشاء كائن استعلام. ويكون نمط الترميز على النحو التالي:

```xpp
class TrainingMasterQuery
{
    public static void main(Args _args)
    {

        Query query = new Query();
 
        QueryBuildDataSource qbds = query.addDataSource(tableNum(TrainingMaster));
        qbds.addSortField(fieldNum(TrainingMaster, TrainingID), SortOrder::Ascending);

        QueryBuildRange qbr = qbds.addRange(fieldNum(TrainingMaster, TrainingType));
        qbr.value(queryValue(TrainingType::Online));

        QueryRun queryRun = new QueryRun(query);
 
        while (queryRun.next())
        {
            TrainingMaster trainingMaster = queryRun.get(tableNum(TrainingMaster));
            info(strFmt("%1, %2", trainingMaster.TrainingID, date2Str(trainingMaster.TrainingDate, 123, DateDay::Digits1or2, DateSeparator::Hyphen, DateMonth::Digits1or2, DateSeparator::Hyphen, DateYear::Digits4)));
        }
    }

}
```

## <a name="advanced-query-syntax"></a>بناء جملة الاستعلام المتقدم
يوجد نطاق من صياغة الاستعلام المتقدمة لحقول السلسلة أو الرقم أو التاريخ. بالنسبة لحقول السلسلة، يُمكنك التصفية حسب النطاق المتساوي، وليس المتساوي، وحرف البدل، وما إلى ذلك. بالنسبة لحقول الأرقام، يُمكن أن تكون خيارات التصفية متساوية، وليست متساوية، وأكبر من، وأقل من، وهكذا. بالنسبة لحقول التاريخ، يُمكن أن تكون خيارات التصفية مستندة إلى اليوم، ونطاق اليوم، ونطاق الشهر، ونطاق السنة، وتاريخي أكبر / أقل من، وما إلى ذلك.

### <a name="example"></a>مثال
تمت إضافة حقل جديد يسمى **NoofDays** إلى جدول **TrainingMaster**. سيتم تطبيق عامل تصفية متقدم على الاستعلام لإظهار جميع التدريبات التي يزيد عدد أيامها عن **2**. ويكون نمط الترميز على النحو التالي:

```xpp
class TrainingMasterQuery
{
    public static void main(Args _args)
    {

        Query query = new Query();
 
        QueryBuildDataSource qbds1 = query.addDataSource(tableNum(TrainingMaster));
        qbds1.addSortField(fieldNum(TrainingMaster, TrainingID), SortOrder::Ascending);

        QueryBuildRange qbr1 = qbds1.addRange(fieldNum(TrainingMaster, NoofDays));
        qbr1.value(queryValue(">2"));

        QueryRun queryRun = new QueryRun(query);
 
        while (queryRun.next())
        {
            TrainingMaster trainingMaster = queryRun.get(tableNum(TrainingMaster));
            info(strFmt("%1, %2", trainingMaster.TrainingID, date2Str(trainingMaster.TrainingDate, 123, DateDay::Digits1or2, DateSeparator::Hyphen, DateMonth::Digits1or2, DateSeparator::Hyphen, DateYear::Digits4)));
        }
    }

}
```

## <a name="build-a-query-that-includes-a-relational-table"></a>إنشاء استعلام يتضمن جدولاً علائقيًا
يُمكنك إنشاء استعلام يتضمن جداول مرتبطة، وذلك باستخدام أحد كائنات الاستعلام. يُمكنك تحديد جميع أنواع الصلات على النحو المطلوب بواسطة الاستعلام الخاص بك.

### <a name="example"></a>مثال
تم إنشاء جدول جديد يسمى **جدول المدرب** به ثلاثة حقول: **معرف المدرب** و **اسم المدرب** و **نوع المدرب** (قيم التعداد: **Functional** و **Technical** و **Softskill**). بالإضافة إلى ذلك، تمت إضافة حقل **معرّف المدرب** إلى جدول **المدرب الرئيسي**، مما يؤدي إلى إنشاء علاقة مفتاح خارجي بين الجداول. تحتاج إلى تصفية جميع التدريبات عبر الإنترنت التي يقدمها المدربون الفنيون من خلال إنشاء أحد كائنات الاستعلام. 

ويكون نمط الترميز على النحو التالي:

```xpp
class TrainingMasterQuery
{
    public static void main(Args _args)
    {

        Query query = new Query();
 
        QueryBuildDataSource qbds1 = query.addDataSource(tableNum(TrainingMaster));
        qbds1.addSortField(fieldNum(TrainingMaster, TrainingID), SortOrder::Ascending);

        QueryBuildRange qbr1 = qbds1.addRange(fieldNum(TrainingMaster, TrainingType));
        qbr1.value(queryValue(TrainingType::Online));

        QueryBuildDataSource qbds2 = qbds1.addDataSource(tableNum(TrainerTable));
        qbds2.relations(true);
        qbds2.joinMode(JoinMode::ExistsJoin);

        QueryBuildRange qbr2 = qbds2.addRange(fieldNum(TrainerTable, TrainerType));
        qbr2.value(queryValue(TrainerType::Technical));

        QueryRun queryRun = new QueryRun(query);
 
        while (queryRun.next())
        {
            TrainingMaster trainingMaster = queryRun.get(tableNum(TrainingMaster));
            info(strFmt("%1, %2", trainingMaster.TrainingID, date2Str(trainingMaster.TrainingDate, 123, DateDay::Digits1or2, DateSeparator::Hyphen, DateMonth::Digits1or2, DateSeparator::Hyphen, DateYear::Digits4)));
        }
    }

}
```

لمزيد من المعلومات حول كائنات الاستعلام ومنشئ الاستعلام، راجع المواقع التالية:

[التصفية المتقدمة وبنية الاستعلام](/dynamics365/fin-ops-core/fin-ops/get-started/advanced-filtering-query-options/?azure-portal=true)

[فئة QueryBuildDataSource](/dotnet/api/dynamics.ax.application.querybuilddatasource/?azure-portal=true)

[الكيفية: إنشاء استعلامات باستخدام X++](/dynamicsax-2012/developer/how-to-create-queries-by-using-x/?azure-portal=true)

[قسم نموذج كائن الاستعلام](/dynamics365/fin-ops-core/dev-itpro/dev-ref/xpp-library-objects/?azure-portal=true)
