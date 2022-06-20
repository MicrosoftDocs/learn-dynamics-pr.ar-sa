---
ms.openlocfilehash: 39b7ae853013491b7ecbe50a0f3ea88bbb318532
ms.sourcegitcommit: aba63fc581b771b49a7826609e64b544c917af16
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2022
ms.locfileid: "8841225"
---
قد تحتاج أحيانًا إلى تشغيل منطق لمستخدم آخر. في سياق Microsoft Dataverse، يقوم المنطق الذي تقوم بتشغيله بتطبيق كافة الأدوار المناسبة والأمان المستند إلى الكائن استناداً إلى المستخدم الذي تقوم بانتحاله. يمكن أن يكون هذا الأسلوب فعالاً بشكل خاص عندما تؤدي إلى تكامل الأنظمة الخارجية مع أحد حلول Dataverse التي يكون فيها حساب التكامل حساب نظام مقابل المستخدم الذي قام بالفعل باستدعاء الطلب.

## <a name="implement-a-web-api-request-with-user-impersonation"></a>تطبيق طلب Web API مع انتحال المستخدم

عند استدعاء أي أسلوب Web API، يمكنك توفير CallerObjectId في عنوان الرسالة للإشارة إلى أنك تريد تشغيل الرسالة لذلك المستخدم المحدد. قيمة هذه المعلمة هي معرف كائن Azure Active Directory (Azure AD). توفر Azure Graph API أسلوبًا للاستعلام عن بيانات مستخدم Azure AD. لمزيد من المعلومات، راجع [Azure AD مرجع Graph API](/previous-versions/azure/ad/graph/api/users-operations/?azure-portal=true).

## <a name="determine-the-user-who-performed-an-operation"></a>تحديد المستخدم الذي قام بإجراء العملية

إذا كنت بحاجة إلى عرض معرف المستخدم الذي قام بالفعل بإجراء عملية لمستخدم آخر، فيمكنك الاستعلام عن قيمه createdonbehalfby بالسجل، والتي ستحتوي على هذه التفاصيل. علي سبيل المثال، إذا كنت ترغب في معرفة ما إذا كان قد تم إنشاء سجل حساب من خلال انتحال المستخدم بدلاً من المستخدم الفعلي، فيمكنك الاستعلام من سجل الحساب هذا لمقارنة قيم createdby وcreatedonbehalfby الخاصة بهم باستخدام الاستعلام التالي:

```odata
GET [Organization URI]/api/data/v9.2/accounts(00000000-0000-0000-000000000003)?$select=name&$expand=createdby($select=fullname),createdonbehalfby($select=fullname),owninguser($select=fullname) HTTP/1.1   
Accept: application/json  
OData-MaxVersion: 4.0  
OData-Version: 4.0  
```

إذا تم إنشاء السجل بواسطة حساب انتحال، فيمكن أن تتوقع استجابة مشابهة للمثال التالي:

```odata
HTTP/1.1 200 OK  
Content-Type: application/json; odata.metadata=minimal  
ETag: W/"506868"  
  
{
  "@odata.context": "[Organization URI]/api/data/v9.2/$metadata#accounts(name,createdby(fullname,azureactivedirectoryobjectid),createdonbehalfby(fullname,azureactivedirectoryobjectid),owninguser(fullname,azureactivedirectoryobjectid))/$entity",
  "@odata.etag": "W/"2751197"",
  "name": "Sample Account created using impersonation",
  "accountid": "00000000-0000-0000-000000000003",
  "createdby": {
    "@odata.etag": "W/"2632435"",
    "fullname": "Impersonated User",
    "azureactivedirectoryobjectid": "e39c5d16-675b-48d1-8e67-667427e9c084",
    "systemuserid": "75df116d-d9da-e711-a94b-000d3a34ed47",
    "ownerid": "75df116d-d9da-e711-a94b-000d3a34ed47"
  },
  "createdonbehalfby": {
    "@odata.etag": "W/"2632445"",
    "fullname": "Actual User",
    "azureactivedirectoryobjectid": "3d8bed3e-79a3-47c8-80cf-269869b2e9f0",
    "systemuserid": "278742b0-1e61-4fb5-84ef-c7de308c19e2",
    "ownerid": "278742b0-1e61-4fb5-84ef-c7de308c19e2"
  },
  "owninguser": {
    "@odata.etag": "W/"2632435"",
    "fullname": "Impersonated User",
    "azureactivedirectoryobjectid": "e39c5d16-675b-48d1-8e67-667427e9c084",
    "systemuserid": "75df116d-d9da-e711-a94b-000d3a34ed47",
    "ownerid": "75df116d-d9da-e711-a94b-000d3a34ed47"
  }
}
```

