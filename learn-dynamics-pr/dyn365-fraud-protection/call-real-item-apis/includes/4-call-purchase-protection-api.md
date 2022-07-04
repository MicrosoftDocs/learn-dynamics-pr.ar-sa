---
ms.openlocfilehash: 51d65f681c81ca59ad32dfa63b38a7486361dc56
ms.sourcegitcommit: 24d9968aa50d817923b7ffaef674b71d2c06238a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/16/2022
ms.locfileid: "9021524"
---
لإرسال طلب إلى خدمة Dynamics 365 Fraud Protection، تأكد من استدعاء نقطة النهاية الصحيحة على خدمة Dynamics 365 Fraud Protection لبيئة التكامل أو التشغيل، كما تقتضي الحاجة. يمكنك اختيار نقطة نهاية لاستخدامها من إعلام تغيير وSwagger API من خلال الانتقال إلى واجهة API‎ في [Dynamics 365 Fraud Protection](/fraud-protection-rest/api/fraud-protection-rest/).

لأغراض تتعلق بهذه الوحدة النمطية، ستتنقل عبر عملية استدعاء إحدى واجهات API لحماية المشتريات كمثال. 

إذا كنت مهتماً بشكل أساسي بتنفيذ تقييمات واجهة API لحماية الحساب فقط، فيمكنك تخطي هذه الوحدة والانتقال إلى الوحدة **استدعاء واجهات API لحماية الحساب** في هذه الوحدة النمطية.

## <a name="make-a-purchase-assessment-call"></a>إجراء استدعاء لتقييم الشراء
اتبع الخطوات التالية لإجراء استدعاء Dynamics 365 Fraud Protection لتقييم الشراء.

1.  حدد نقطة النهاية الصحيحة من مستند Swagger. في هذا المثال، يتم إجراء الاستدعاء مع نقطة نهاية **الشراء**.

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لمستند Swagger يُظهر نقطة نهاية الشراء.](../media/purchase-endpoint-ss.png)](../media/purchase-endpoint-ss.png#lightbox) 

    يذكر مستند Swagger أيضاً تفاصيل حول الرؤوس والحمولة التي يمكنك استخدامها والاستجابة التي يمكنك توقعها.

2.  استخدم تطبيق Postman (أو أي عميل تختاره) لإرسال طلب الشراء إلى Dynamics 365 Fraud Protection. أرسل **طلب POST**، كما يظهر في الصورة التالية.
    - في حقل **URL**، أدخل **{{API Endpoint}}{{Relative Endpoint}}**.
    - حدد **تخويل**، وضمن **النوع**، حدد **الرمز المميز للحامل**.
    - أدخل قيمة الرمز المميز التي تلقيتها في الطلب السابق. 

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لطلب Post، تُظهر الحقلين "تخويل" و"Content-Type".](../media/post-request-ss.png)](../media/post-request-ss.png#lightbox) 

4.  حدد **النص**، وحدد **خام**، ثم حدد **JSON** من القائمة المنسدلة. 

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لطلب Post، تُظهر تحديد النص > خام > JSON.](../media/json-1.png)](../media/json-1.png#lightbox)
 

5.  انسخ والصق عينة حمولة JSON م من Swagger، ثم عدّل القيم استناداً إلى احتياجاتك. (تسهيلاً للأمور، تم أيضاً تضمين عينة الحمولة في القسم **عينة حمولة حدث الشراء** لاحقاً في هذه الوحدة.)

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لطلب Post مع عينة حمولة JSON من Swagger.](../media/json-2-sample-ss.png)](../media/json-2-sample-ss.png#lightbox) 

6.  قم بتمرير رؤوس HTTP المطلوبة التالية عند كل طلب. 

    |      اسم الرأس            |      قيمة الرأس                                                                                                                                                                                                                                                                                                                                    |
    |-----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    |     التخويل           |     استخدم تنسيق *الحامل {{access_token}}* لهذا الرأس، حيث *accesstoken* هو الرمز المميز المرتجع بواسطة Azure AD. تأكد من أنك تضيف أيضاً الكلمة الأساسية **حامل** إذا أضفت هذا الرأس. ومع ذلك، إذا كنت تستخدم علامة التبويب **مصادقة** في Postman، فلا تحتاج إلى إضافة الكلمة الأساسية **حامل**.    |
    |     x-ms-correlation-id     |     أرسل قيمة GUID جديدة على كل مجموعة استدعاءات API تتم معاً. (أنت تحتاج إلى هذا الرأس إذا كنت تريد تصحيح الأخطاء التي تحصل عليها من Dynamics 365 Fraud Protection لأن هذه هي الطريقة الوحيدة للبحث عن استدعائك.)                                                                                                                       |
    |     Content-Type            |     application/json                                                                                                                                                                                                                                                                                                                                 |


7.  عيّن قيمة **deviceContextId** في الحمولة إلى قيمة **session_id**، معرف جلسة العمل الفريد للجهاز الذي أنشأه التاجر أثناء عملية تطبيق بصمة الجهاز. لمزيد من المعلومات، راجع [إعداد بصمة الجهاز](/dynamics365/fraud-protection/device-fingerprinting/?azure-portal=true).
 
    > [!NOTE]
    > إذا لم تكن قد طبقت بصمة الجهاز حتى الآن، فإن وحدة نمطية أخرى توفر لك فرصة إجراء ذلك. لمزيد من المعلومات، راجع [تطبيق بصمة الجهاز في Dynamics 365 Fraud Protection](/learn/modules/device-fingerprint-fraud-protection//?azure-portal=true). يمكنك متابعة الجزء المتبقي من هذه الوحدة النمطية لمعرفة كيفية الحصول على درجة من Dynamics 365 Fraud Protection عند إجراء استدعاء ناجح لواجهة API. يمكنك تخطي كتلة بصمة الجهاز تماماً في الوقت الحالي. (راجع الأسطر تحت التعليمات البرمجية التالية **"‏deviceContext":** في القسم **عينة حمولة حدث الشراء‬‏‫** لكتلة التعليمات البرمجية التي يجب تخطيها.) ومع ذلك، إذا توفرت لديك بيانات الجهاز، مثل عنوان IP، أضف **PurchaseId** باعتباره **deviceContextId**، ثم قدم المعلومات المتوفرة لديك لتلك الكتلة. 

8.  تحقق من **حالة** و **نص** الاستجابة، ثم حدد **إرسال**. 

    > [!div class="mx-imgBorder"]
    > [![لقطة شاشة لطلب Post مع موقع الزر "إرسال".](../media/post-request-send-ss.png)](../media/post-request-send-ss.png#lightbox)

 
 
## <a name="sample-purchase-event-payload"></a>عينة حمولة حدث الشراء‬‏‫‬‏‫
يبيّن المثال التالي عينة حمولة حدث الشراء التي يمكنك استخدامها لهذه الوحدة.

```http
{
  "purchaseId": "string",
  "assessmentType": "string",
  "originalOrderId": "string",
  "customerLocalDate": "2020-08-05T18:06:00.180Z",
  "merchantLocalDate": "2020-08-05T18:06:00.180Z",
  "totalAmount": 0,
  "salesTax": 0,
  "currency": "string",
  "shippingMethod": "string",
  "customData": {
    "additionalProp1": {},
    "additionalProp2": {},
    "additionalProp3": {}
  },
  "user": {
    "userId": "string",
    "creationDate": "2020-08-05T18:06:00.180Z",
    "updateDate": "2020-08-05T18:06:00.180Z",
    "firstName": "string",
    "lastName": "string",
    "country": "string",
    "zipCode": "string",
    "timeZone": "string",
    "language": "string",
    "phoneNumber": "string",
    "email": "string",
    "membershipId": "string",
    "profileType": "string",
    "profileName": "string",
    "authenticationProvider": "string",
    "displayName": "string",
    "isEmailValidated": true,
    "emailValidatedDate": "2020-08-05T18:06:00.180Z",
    "isPhoneNumberValidated": true,
    "phoneNumberValidatedDate": "2020-08-05T18:06:00.180Z"
  },
  **"deviceContext": {
    "deviceContextId": "string",
    "provider": "string",
    "externalDeviceId": "string",
    "externalDeviceType": "string",
    "ipAddress": "string"**
  },
  "paymentInstrumentList": [
    {
      "merchantPaymentInstrumentId": "string",
      "type": "string",
      "creationDate": "2020-08-05T18:06:00.180Z",
      "updateDate": "2020-08-05T18:06:00.180Z",
      "state": "string",
      "cardType": "string",
      "holderName": "string",
      "bin": "string",
      "expirationDate": "string",
      "lastFourDigits": "string",
      "email": "string",
      "billingAgreementId": "string",
      "payerId": "string",
      "payerStatus": "string",
      "addressStatus": "string",
      "imei": "string",
      "encryptedCreditCardNumber": "string",
      "purchaseAmount": 0,
      "billingAddress": {
        "street1": "string",
        "street2": "string",
        "street3": "string",
        "city": "string",
        "state": "string",
        "district": "string",
        "zipCode": "string",
        "country": "string",
        "firstName": "string",
        "lastName": "string",
        "phoneNumber": "string"
      }
    }
  ],
  "productList": [
    {
      "productId": "string",
      "productName": "string",
      "type": "string",
      "sku": "string",
      "category": "string",
      "market": "string",
      "salesPrice": 0,
      "currency": "string",
      "cogs": 0,
      "isRecurring": true,
      "isFree": true,
      "language": "string",
      "purchasePrice": 0,
      "margin": 0,
      "quantity": 0,
      "isPreorder": true,
      "shippingMethod": "string"
    }
  ],
  "shippingAddress": {
    "street1": "string",
    "street2": "string",
    "street3": "string",
    "city": "string",
    "state": "string",
    "district": "string",
    "zipCode": "string",
    "country": "string",
    "firstName": "string",
    "lastName": "string",
    "phoneNumber": "string"
  },
  "_metadata": {
    "trackingId": "string",
    "merchantTimeStamp": "2020-08-05T18:06:00.180Z"
  }
}
```
