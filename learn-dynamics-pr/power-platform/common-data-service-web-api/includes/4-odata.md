---
ms.openlocfilehash: 6e9ddab0620f9fc6084922f34a0fb214815c268c
ms.sourcegitcommit: aba63fc581b771b49a7826609e64b544c917af16
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2022
ms.locfileid: "8841267"
---
OData هي لغة تم اختبارها عبر الزمن للاستعلام عن RESTful APIs. يستكشف هذا الدرس عدة طرق لأداء عمليات CRUD ضد بيانات Microsoft Dataverse.

## <a name="create-records"></a>إنشاء سجلات

استخدم الأسلوب HTTP POST لإنشاء سجلات.

```odata
POST [Organization URI]/api/data/v9.0/accounts HTTP/1.1
Content-Type: application/json; charset=utf-8
OData-MaxVersion: 4.0
OData-Version: 4.0
Accept: application/json

{
    "name": "Sample Account",
    "creditonhold": false,
    "address1_latitude": 47.639583,
    "description": "This is the description of the sample account",
    "revenue": 5000000,
    "accountcategorycode": 1
}

```

## <a name="retrieve-records"></a>استرجاع السجلات

استخدم الأسلوب HTTP GET لاسترجاع السجلات.

يسترجع النموذج التالي حسابًا بمعرف 00000000-0000-0000-0000-000000000001:

```odata
GET [Organization URI]/api/data/v9.2/accounts(00000000-0000-0000-0000-000000000001)
```

باستخدام بناء جملة استعلام OData القياسي، تتوفر طرق أخرى للاستعلام عن البيانات. لمزيد من المعلومات حول هذه العملية، راجع [استرجاع سجل كيان باستخدام Web API](/power-apps/developer/common-data-service/webapi/retrieve-entity-using-web-api/?azure-portal=true).

## <a name="update-records"></a>تحديث السجلات

بناءً على ما تحاول تحقيقه، يمكنك الاختيار بين أحد الأسلوبين لتحديث السجلات:

-   استخدم الأسلوب HTTP PATCH، إذا كنت تقوم بتحديث قيم سمات متعددة. حيث توفر طرق PATCH إمكانية upert إذا قمت بتوفير قيمة معرف كجزء من طلبك، وهي ميزة مفيدة عندما تقوم بمزامنة البيانات بين الأنظمة.

-   استخدم الأسلوب HTTP PUT إذا كنت تقوم بتحديث قيمة سمة واحدة.
    لا يمكن استخدام هذا الأسلوب مع خصائص التنقل مثل عمليات البحث لأن ذلك يتطلب إزالة مرجع أيضًا.

يقوم المثال التالي بتحديث أحد كيانات الحساب:

```odata
PATCH [Organization URI]/api/data/v9.2/accounts(00000000-0000-0000-0000-000000000001) HTTP/1.1  
Content-Type: application/json  
OData-MaxVersion: 4.0  
OData-Version: 4.0  
  
{  
    "name": "Updated Sample Account ",  
    "creditonhold": true,  
    "address1_latitude": 47.639583,  
    "description": "This is the updated description of the sample account",  
    "revenue": 6000000,  
    "accountcategorycode": 2  
}  
```

يمكنك استخدام عنوان الطلب return=representation، إذا كنت ترغب في استرداد البيانات من الكيان الذي تقوم بتحديثه. يمكنك إضافة استعلام `$select` إلى PATCH URL، إذا كنت تريد التحكم في الخصائص التي يتم إرجاعها. في المثال التالي، تمت إضافة العنوان وتم تعديله ليشمل فقط سمات الاسم `$select` وتم تعديله ليشمل فقط السمات name وcreditonhold وaddress1.

### <a name="request"></a>طلب

```odata
PATCH [Organization URI]/api/data/v9.2/accounts(00000000-0000-0000-0000-000000000001)?$select=name,creditonhold,address1_latitude,description,revenue,accountcategorycode,createdon HTTP/1.1  
OData-MaxVersion: 4.0  
OData-Version: 4.0  
Accept: application/json  
Content-Type: application/json; charset=utf-8  
Prefer: return=representation  
  
{"name":"Updated Sample Account"}  
```

### <a name="response"></a>الاستجابة

```odata
HTTP/1.1 200 OK  
Content-Type: application/json; odata.metadata=minimal  
Preference-Applied: return=representation  
OData-Version: 4.0  
  
{  
    "@odata.context": "[Organization URI]/api/data/v9.2/$metadata#accounts/$entity",  
    "@odata.etag": "W/"536537"",  
    "accountid": "00000000-0000-0000-0000-000000000001",  
    "accountcategorycode": 1,  
    "description": "This is the description of the sample account",  
    "address1_latitude": 47.63958,  
    "creditonhold": false,  
    "name": "Updated Sample Account",  
    "createdon": "2022-09-28T23:14:00Z",  
    "revenue": 5000000.0000,  
    "_transactioncurrencyid_value": "048dddaa-6f7f-e611-80d3-00155db5e0b6"  
}  
```

ما يلي هو نموذج لطلب PUT حيث يتم تحديث اسم حساب لسجل معيّن:

```odata
PUT [Organization URI]/api/data/v9.2/accounts(00000000-0000-0000-0000-000000000001)/name HTTP/1.1  
Content-Type: application/json  
OData-MaxVersion: 4.0  
OData-Version: 4.0  
  
{"value": "Updated Sample Account Name"}  
```

## <a name="delete-records"></a>حذف السجلات

استخدم الأسلوب HTTP DELETE لحذف السجلات. العملية مباشرة، حيث تقوم بتوفير URI لسجل الكيان الذي تريد حذفه، كما هو موضح في الطلب التالي:

```odata
DELETE [Organization URI]/api/data/v9.2/accounts(00000000-0000-0000-0000-000000000001) HTTP/1.1  
Content-Type: application/json  
OData-MaxVersion: 4.0  
OData-Version: 4.0
```

## <a name="additional-operations"></a>العمليات الإضافية

يوفر Dataverse عدداً من العمليات الأخرى المحددة مسبقاً والتي يمكنك تشغيلها من خلال طلبات Web API. للحصول على قائمة المخزون الكاملة للإمكانيات المتاحة، راجع [تنفيذ العمليات باستخدام Web API](/power-apps/developer/common-data-service/webapi/perform-operations-web-api/?azure-portal=true).
