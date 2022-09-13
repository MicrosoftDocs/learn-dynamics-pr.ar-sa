---
ms.openlocfilehash: 9a72997da10917e6db0e424bcbccf4daeecf8de6
ms.sourcegitcommit: d9a5d6ce9de95633830f18fa2a3df6346ad0fd4f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/26/2022
ms.locfileid: "9356125"
---
وبشكل عام، تحتاج المؤسسات إلى مزامنة البيانات عبر أنظمة متعددة. يوفر Microsoft Dataverse ميزة لإدارة هذا السيناريو بكفاءة، وهو ما يسمى بـ *تعقب التغيير*. مع تمكين تعقب التغييرات، يمكنك إنشاء تطبيقات للاستعلام عن هذه التغييرات.

## <a name="enable-change-tracking-for-a-table"></a>تمكين تعقب التغييرات لأحد الجداول

يمكنك تمكين تعقب التغييرات على جدول عن طريق تعيين علامة **تعقب التغييرات** في إعدادات الجدول في Maker Portal Power Apps، الموجود ضمن قسم **الخيارات المتقدمة > لهذا الجدول**. 

## <a name="delta-links"></a>ارتباطات Delta

وفقا لوثائق OData 4.0، تُعد ارتباطات delta هي "الارتباطات غير الشفافة، المنشأة من قبل الخدمة التي يستخدمها العميل لاسترداد التغييرات اللاحقة لناتج ما." قامت Microsoft بإنشاء معيار Dataverse هذا في تعقب التغييرات لتوفير أسلوب عام قياسي للربط مع تغيير البيانات أثناء حدوثها بمرور الوقت. للمزيد من المعلومات حول ارتباطات delta، راجع [ارتباطات delta الخاصة بالإصدار 4.0 من OData](https://docs.oasis-open.org/odata/odata/v4.0/cs01/part1-protocol/odata-v4.0-cs01-part1-protocol.html#_Toc365046305).
بعد إصدار طلب تعقب التغيير، ستحتوي الاستجابة الخاصة بك على ارتباط delta، والذي ستقوم بتمريره إلى الطلب التالي للحصول على التغييرات التي حدثت منذ الطلب الأولي. سيتم الحصول على التطبيق الخاص بك للمحافظة على ارتباط delta، وذلك بشكل مشابه لكيفية تتبع الارتباط مع طوابع التاريخ/الوقت في الماضي.

## <a name="retrieve-changes-in-tables-by-using-the-web-api"></a>استرداد التغييرات في الجداول باستخدام API للويب

بعد تمكين تعقب التغييرات على جدول ما، يمكنك استرداد التغييرات التي قام بها من خلال Web API عن طريق إضافة odata.track-changes كعنوان تفضيلي في طلب الويب الخاص بك. يطلب المثال التالي إجراء تغييرات من جدول الحساب لمجموعة محددة من الحقول (الاسم ورقم الحساب ورقم الهاتف 1 ورقم الفاكس).

```odata
GET [Organization URI]/org1/api/data/v9.2/accounts?$select=name,accountnumber,telephone1,fax HTTP/1.1
Prefer: odata.track-changes
Cache-Control: no-cache
OData-Version: 4.0
Content-Type: application/json
```

وفي الطلب الأولي، ستتلقى مجموعة كاملة من البيانات التي تنطبق على الاستعلام نظراً لعدم تطبيق delta. ومع ذلك، ستعرض الاستجابة إحدى قيم @odata.deltaLink. يحتوي هذا الارتباط على معلمة deltatoken، المخصصة لتمريرها إلى طلبك اللاحق عندما تريد معرفة التغييرات التي تم تطبيقها منذ تشغيل هذا الاستعلام. يمكنك التفكير في هذه العملية بنفس طريقة معالجة الترحيل في OData.

المثال التالي هو الاستجابة لطلب الحساب السابق:

```odata
{
          "@odata.context":"[Organization URI]/data/v9.2/$metadata#accounts(name,telephone1,fax)/$delta",
          "@odata.deltaLink":"[Organization URI]/api/data/v9.2/accounts?$select=name,telephone1,fax&$deltatoken=919042%2108%2f22%2f2017%2008%3a10%3a44",
"value":
    [
        {
            "@odata.etag":"W/\"915244\"",
            "name":"Monte Orton",
            "telephone1":"555000",
            "fax":"10101",
            "accountid":"60c4e274-0d87-e711-80e5-00155db19e6d"
        },
        {
            "@odata.context":"[Organization URI]/api/data/v9.2/$metadata#accounts/$deletedEntity",
            "id":"2e451703-c686-e711-80e5-00155db19e6d",
            "reason":"deleted"
        }
    ]
}
```

في هذا السيناريو، يجب مراعاة أن بعض الوقت قد انقضى، وترغب الآن في معرفة ما إذا كان قد تم تطبيق أي تغييرات أخرى. يمكنك استخدام معلمة @odata.deltaLink لتشغيل الاستعلام الخاص (أو لاستخراج deltatoken، إذا كنت تقوم بإدارة سلاسل الاتصال بشكل مختلف)، ورؤية التغييرات التي حدثت منذ الطلب الأخير.

يوضح المثال التالي كيفية استرداد التغييرات التي تمت منذ الطلب الأخير بواسطة تشغيل \@odata.deltaLink الذي تم إرجاعه:

```odata
GET [Organization URI]/api/data/v9.2/accounts?$select=name,accountnumber,telephone1,fax&$deltatoken=919042%2108%2f22%2f2017%2008%3a10%3a44
```

في هذا السيناريو، تخيل أنه تم إنشاء حساب جديد وتم حذف آخر. ردك سيكون مشابهاً للمثال التالي بعد ذلك:

```odata
{
          "@odata.context":"[Organization URI]/data/v9.2/$metadata#accounts(name,telephone1,fax)/$delta",
          "@odata.deltaLink":"[Organization URI]/api/data/v9.2/accounts?$select=name,telephone1,fax&$deltatoken=919058%2108%2f22%2f2017%2008%3a21%3a20",
"value":
    [
        {
            "@odata.etag":"W/\"915244\"",
            "name":"Monte Orton",
            "telephone1":"555000",
            "fax":"10101",
            "accountid":"60c4e274-0d87-e711-80e5-00155db19e6d"
        },
        {
            "@odata.context":"[Organization URI]/api/data/v9.1/$metadata#accounts/$deletedEntity",
            "id":"2e451703-c686-e711-80e5-00155db19e6d",
            "reason":"deleted"
        }
    ]
}
```

كما هو موضح في المثال، تم إرسال ارتباط delta آخر، ويمكنك استخدامه في المرة التالية التي تحتاج إليها لمعرفة التغييرات التي حدثت.

## <a name="retrieve-the-number-of-changes-in-a-delta"></a>استرداد عدد التغييرات في delta

يمكنك أيضاً استرداد عدد التغييرات التي تم إجراؤها في وحدة delta معينة عن طريق إضافة المعلمة $count إلى الطلب الخاص بك.

```odata
GET [Organization URI]/api/data/v9.2/accounts/$count?$deltatoken=919042%2108%2f22%2f2017%2008%3a10%3a44
```

