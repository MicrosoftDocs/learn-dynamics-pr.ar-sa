---
ms.openlocfilehash: c5ef8445ff9daba1e7c7c3b41d66df35571b721c
ms.sourcegitcommit: 1d9dbd81b128041197540f8687181cc789626fc2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2021
ms.locfileid: "7900571"
---
لاستدعاء إحدى واجهات API لحماية الحساب في Dynamics 365 Fraud Protection، يجب أولاً تحديد نقطة النهاية الصحيحة من مستند Swagger في واجهة API في [Dynamics 365 Fraud Protection](https://apidocs.microsoft.com/services/dynamics365fraudprotection/?azure-portal=true).
(يمكنك الرجوع إلى التمييز الأصفر في لقطة الشاشة التالية).

> [!div class="mx-imgBorder"]
 > [![لقطة شاشة لواجهة API في Dynamics 365 Fraud Protection.](../media/integration-testing.png)](../media/integration-testing.png#lightbox)

لأغراض تتعلق بهذه الوحدة النمطية، ستتنقل عبر عملية استدعاء إحدى واجهات برمجة التطبيقات (API) لحماية الحساب كمثال.

## <a name="call-the-account-create-api"></a>استدعاء واجهة API لإنشاء حساب

لاستدعاء واجهة API لإنشاء حساب، اتبع هذه الخطوات.

1. حدد نقطة نهاية API المحددة لحماية الحساب من مستند Swagger. (في هذا المثال، راجع *واجهة API لإنشاء حساب‬*.)

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لنقطة نهاية API لحماية الحساب من مستند Swagger.](../media/account-create.png)](../media/account-create.png#lightbox)

1. يسرد مستند Swagger أيضاً تفاصيل حول الرؤوس والحمولة التي يمكنك استخدامها والاستجابة التي يمكنك توقعها عند تحديد **ترحيل**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لمستند Swagger، مع سرد تفاصيل الرأس والحمولة.](../media/headers-payloads.png)](../media/headers-payloads.png#lightbox)

1. استخدم تطبيق Postman (أو أي عميل تختاره) لإرسال طلب حماية الحساب إلى Dynamics 365 Fraud Protection:

    1. لإرسال **طلب POST**، أدخِل **`{{API Endpoint}}{{Relative Endpoint}}`** في الحقل **URL**.

        > [!NOTE]
        > **نقطة نهاية API** مأخوذة من الصفحة الرئيسية لمدخل Dynamics 365 Fraud Protection. **نقطة النهاية النسبية** مأخوذة من عينة مستند Swagger التي تظهر في الخطوة 1.

    1. انسخ والصق عينة حمولة JSON م من Swagger، ثم عدّل القيم استناداً إلى احتياجاتك. (تسهيلاً للأمور، تم توفير عينة الحمولة لكل واجهة API لحماية الحساب لاحقاً في هذا المستند.)

1. قم بتمرير رؤوس HTTP المطلوبة التالية عند كل طلب.

    | اسم الرأس | قيمة الرأس |
    |-------------|--------------|
    | التخويل  | استخدم تنسيق *الحامل {{access_token}}* لهذا الرأس، حيث *accesstoken* هو الرمز المميز المرتجع بواسطة Azure AD. تأكد من أنك تضيف أيضاً الكلمة الأساسية **حامل** إذا أضفت هذا الرأس. ومع ذلك، إذا كنت تستخدم علامة التبويب **مصادقة** في Postman، فلا تحتاج إلى إضافة الكلمة الأساسية **حامل**. |
    | x-ms-correlation-id | أرسل قيمة GUID جديدة على كل مجموعة استدعاءات API تتم معاً. (أنت تحتاج إلى هذا الرأس إذا كنت تريد تصحيح الأخطاء التي تحصل عليها من Dynamics 365 Fraud Protection لأن هذه هي الطريقة الوحيدة للبحث عن استدعائك.) |
    | Content-Type  | application/json  |

1. عيّن قيمة **deviceContextId** إلى قيمة **session_id**، معرف جلسة العمل الفريد للجهاز الذي أنشأه التاجر أثناء عملية تطبيق بصمة الجهاز. عندئذٍ، أرسِل الطلب.

    > [!NOTE]
    >
    > إذا لم تكن قد طبقت بصمة الجهاز حتى الآن، فيمكنك المتابعة مع باقي الخطوات لمعرفة كيفية الحصول على نتيجة بدون بيانات بصمة الجهاز. يمكنك تخطي كتلة بصمة الجهاز تماماً في الوقت الحالي.
    >
    > تُرجع واجهات APIs لحماية الحساب أعلى الدرجات (999) في حال عدم التكامل مع بصمة الجهاز. ضع في اعتبارك أن بصمة الجهاز هي شرط لتلقي أي نتائج مفيدة من نموذج مخاطر حماية الحساب في Dynamics 365 Fraud Protection. لمزيد من المعلومات، راجع [تطبيق بصمة الجهاز في Dynamics 365 Fraud Protection](/learn/modules/device-fingerprint-fraud-protection/?azure-portal=true).

## <a name="sample-payload"></a>عينة الحمولة

توفر الأقسام التالية عينات حمولة لواجهة API لحماية الحساب والتي يمكنك تجربتها.

### <a name="account-create"></a>إنشاء حساب

/v1.0/action/account/create/\<signUpId>

يجب أن تكون قيمة **signUpId** فريدة لكل طلب، ويجب أن تكون نفس القيمة الموجودة في قسم بيانات التعريف في العينة التالية.

```http
{ 
 "device": { 
   "deviceContextId": "2cf391cc-62d2-47d4-a9c1-78ec025293da", 
   "ipAddress": "192.168.8.214", 
   "provider": "DFPFingerprinting", 
   "externalDeviceId": "1234567890", 
   "externalDeviceType": "Tablet" }, 
 "user": { 
  "userId": " cf4e1d39-1100-4791-a6cf-98580f3d91cb", 
  "userType": "Consumer", 
  "username": "kayla@contoso.com", 
  "firstName": "Kayla", 
  "lastName": "Goderich", 
  "countryRegion": "US", 
  "zipCode": "44329", 
  "timeZone": "-08:00", 
  "language": "en-us", 
  "membershipId": " CC004567", 
  "isMembershipIdUsername": false }, 
 "metadata": { 
  "signUpId": "f5085b48-0f9d-47f5-85d1-2c95e7842d39", 
  "customerLocalDate": "2020-02-25T15:12:26.9653975-08:00", 
  "assessmentType": "Protect", 
  "trackingId": "d65544f0-f8b4-4249-a5e0-94b32a25548f", 
  "merchantTimeStamp": "2020-08-27T15:12:26.9721842-08:00" }, 
 "name": "AP.AccountCreation", 
 "version": "0.5" 
} 
```

### <a name="account-login"></a>تسجيل الدخول إلى الحساب

/v1.0/action/account/login/\<userId>

يجب أن تكون قيمة **userId** هي نفسها الموجودة في الحمولة. يجب أن يكون لكل مستخدم قيمة فريدة. يمكن استخدام قيمة GUID في هذه العينة.

```http
{ 
 "device": { 
  "deviceContextId": "2ef10376-2ba8-4f36-a911-da438e5e5e27", 
  "ipAddress": "192.168.8.214", 
  "provider": "DFPFingerprinting", 
  "externalDeviceId": "1234567890", 
  "externalDeviceType": "Computer" }, 
 "user": { 
  "userId": "cf4e1d39-1100-4791-a6cf-98580f3d91cb", 
  "userType": "Consumer", 
  "username": "kayla@contoso.com", 
  "firstName": "Kayla", 
  "lastName": "Goderich", 
  "countryRegion": "US", 
  "zipCode": "44329", 
  "timeZone": "-08:00", 
  "language": "en-us", 
  "membershipId": "CC004567", 
  "isMembershipIdUsername": false }, 
 "metadata": { 
  "loginId": "a15d4a5d-fadc-49ab-8022-712fec597e22", 
  "customerLocalDate": "2020-02-25T15:22:42.3397533-08:00", 
  "assessmentType": "Protect", 
  "trackingId": "a14ebdca-9447-49b4-951e-26f6ccc4445c", 
  "merchantTimeStamp": "2020-08-27T15:22:42.3405921-08:00" }, 
 "name": "AP.AccountLogin", 
 "version": "0.5" 
}
```

### <a name="account-create-status"></a>حالة إنشاء الحساب

/v1.0/observe/account/create/status/\<signUpId>

يجب أن تكون قيمة **signUpId** هي نفسها الموجودة في الحمولة. يجب أن يكون لكل مستخدم قيمة فريدة. يمكن استخدام قيمة GUID في هذه العينة.

```http
{ 
 "metadata":{ 
  "signUpId":"a6221a3f-c38c-429e-8fde-3026d8c29ed3", 
  "userId":"34f47dc4-9781-4033-99fd-185649c4b001", 
  "trackingId":"697a6bee-2d30-4132-92a6-c137aaf49c0a", 
  "merchantTimeStamp":"2020-04-03T13:23:32.3226335-07:00" }, 
 "statusDetails":{ 
  "statusType":"Rejected", 
  "reasonType":"ChallengeAbandoned", 
  "challengeType":"Email", 
  "statusDate":"2020-04-03T13:23:32.3817714-07:00" },
 "name":"AP.AccountCreation.Status", 
 "version":"0.5" 
}
```

### <a name="account-login-status"></a>حالة تسجيل الدخول إلى الحساب

/v1.0/observe/account/login/status/\<userId>

يجب أن تكون قيمة **userId** هي نفس القيمة الموجودة في واجهة API لتسجيل الدخول إلى الحساب المقابلة.

```http
{ 
 "metadata":{ 
  "loginId":"dc4ea331-a6e5-4aa0-8eba-16b4d516a07d", 
  "userId":"34f47dc4-9781-4033-99fd-185649c4b001", 
  "trackingId":"dcd65c87-d3db-4a42-8ed3-3e59f443b994", 
  "merchantTimeStamp":"2020-04-03T13:23:32.3759321-07:00"}, 
 "statusDetails":{ 
  "statusType":"Rejected", 
  "reasonType":"ChallengeAbandoned", 
  "challengeType":"Email", 
  "statusDate":"2020-04-03T13:23:32.3884589-07:00"}, 
 "name":"AP.AccountLogin.Status", 
 "version":"0.5" 
}
```

### <a name="label"></a>التسمية

/v1.0/label/account/create/\<userId>

```http
{ 
 "metadata": { 
  "name": "AP.Label.Metadata", 
  "userId": "34f47dc4-9781-4033-99fd-185649c4b001", 
  "merchantTimeStamp": "2020-06-14T21:53:27.8822492-08:00", 
  "trackingId": "34f47dc4-9781-4033-99fd-185649c4b001" }, 
 "label": { 
  "eventTimeStamp": "2020-02-21T21:53:27.8822492-08:00", 
  "labelObjectType": "Account", 
  "labelObjectId": "userid", 
  "labelSource": "ManualReview", 
  "labelState": "AccountCompromised", 
  "labelReasonCode": "AccountFraud" }, 
 "name": "AP.Label", 
 "version": "0.5" 
}
```
