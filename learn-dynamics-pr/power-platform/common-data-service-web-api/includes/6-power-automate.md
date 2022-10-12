---
ms.openlocfilehash: 83bf5182341d39637bf796b5a23dcfc005f83c8e
ms.sourcegitcommit: 42a0faa4dc64a860f6457449b0792257c2254757
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/23/2022
ms.locfileid: "9584202"
---
يحتوي Dataverse على ميزة تسمح للمستخدمين المحترفين بإنشاء مجموعاتهم المخصصة لمنطق الأعمال التي تُسمى بـ *إجراءات*. ومن منظور المطوِّر، يتعرف Microsoft Learn على الإجراء كـ "عملية قابلة لإعادة الاستخدام قد يكون لها تأثيرات جانبية ملحوظة". تتضمن هذه الآثار الجانبية إنشاء السجلات أو تحديثها.

الميزة الأخرى للإجراءات هي قدرتها على الاستدعاء من خلال API للويب. ونتيجة لذلك، يمكنك تغليف عمليات أتمتة التعليمات البرمجية المنخفضة بطريقة ما يمكنك من خلالها استخدام هذه العمليات في أي سيناريو تقريباً، وذلك بالتعامل معها طلب Web API ذي الصلة والاستجابة له.

بينما لا يغطي هذا الدرس كيفية إنشاء إجراءات بالتفصيل، فإنه من المفترض أن يكون لديك بالفعل فهم أساسي لكيفيه إنشائها. إذا كنت بحاجة إلى مزيد من المعلومات حول كيفية إنشاء إجراء، فيمكنك مراجعة وثائق ذات صلة به. راجع قسم [إنشاء واجهات API المخصصة](/power-apps/developer/data-platform/custom-api/?azure-portal=true) للاطلاع على تعليمات مفصلة حول كيفية إنشاء إجراءات Dataverse.

## <a name="run-actions-with-the-web-api"></a>تشغيل الإجراءات باستخدام Web API

عند إنشاء إجراء جديد في حل Dataverse الخاص بك، فسينشئ إطار العمل أيضاً رسالة طلب Web API مطابق. يمكنك تشغيل هذه الطلبات باستخدام عملية POST مشابهة للمثال التالي:

```odata
POST [Organization URI]/api/data/v9.2/WinOpportunity HTTP/1.1
Accept: application/json
Content-Type: application/json; charset=utf-8
OData-MaxVersion: 4.0
OData-Version: 4.0

{
 "Status": 3,
 "OpportunityClose": {
  "subject": "Won Opportunity",
  "opportunityid@odata.bind": "[Organization URI]/api/data/v9.2/opportunities(b3828ac8-917a-e511-80d2-00155d2a68d2)"
 }
}
```

المثال أعلاه هو استدعاء طلب HTTP لإجراء WinOpportunity فيما يتعلق بأي فرصة بقيمة opportunityid التي تبلغ ```b3828ac8-917a-e511-80d2-00155d2a68d2```.

## <a name="call-pre-built-dataverse-actions"></a>استدعاء إجراءات Dataverse المُنشأة مسبقاً

Dataverse يتضمن مجموعة من الإجراءات الموجودة التي يمكنك استخدامها لتنفيذ العمليات الشائعة. قد تُطبَّقُ بعض هذه الإجراءات فقط على تطبيقات تستند إلى النماذج أو تطبيقات Dynamics 365. علي سبيل المثال، يحسب إجراء CalculatePrice السعر في الفرصة/عرض الأسعار/الأمر/الفاتورة، لذلك لا ينطبق إلا على تطبيق Dynamics 365 Sales حيث توجد هذه الوظيفة.

للمزيد من المعلومات حول الإجراءات المُنشاة مسبقاً المتوفرة للاستخدام من خلال Web API، راجع [مرجع إجراءات Web API](/dynamics365/customer-engagement/web-api/actions?view=dynamics-ce-odata-9/?azure-portal=true&preserve-view=true).

## <a name="unbound-vs-bound-actions"></a>الإجراءات غير المقيدة مقابل الإجراءات المقيدة

يمكن إنشاء الاجراء كإجراء غير مقيد (أي أنه لا يتضمن كيان Dataverse مرتبط به) أو مقيد (أي أن المنطق مرتبط بسجل كيان معين). يمكن لمطوِّري SQL  
أخذ هذه الإجراءات بعين الاعتبار كـ"الإجراءات المخزنة" (إجراءات غير مقيدة) مقابل المشغلات (الإجراءات مقيدة). ومع ذلك، فعلى عكس مشغلات SQL، يمكنك أيضاً تشغيل الإجراءات المقيدة عند الطلب بتوفير معرِّف سجل كيان مماثل مع تقديم المعلمة الخاصة به.

الإجراءات غير المقيدة تعتبر مفيدة تبعاً للمنطق العام، حيث إن قد يتعين تشغيلها خارج سياق أي سجل يخص كياناً معيناً، مثل إجراء WinOpportunity الذي تمت الإشارة إليه سابقاً. لتشغيل إجراء مقيد مقابل سجل محدد، يجب عليك تقديم معرِّف هذا السجل في عنوان URI الخاص بطلبك:

```odata
POST [Organization URI]/api/data/v9.2/contacts(94d8c461-a27a-e511-80d2-00155d2a68d2)/Microsoft.Dynamics.CRM.new_AddNoteToContact HTTP/1.1
Accept: application/json
Content-Type: application/json; charset=utf-8
OData-MaxVersion: 4.0
OData-Version: 4.0

{
 "NoteTitle": "New Note Title",
 "NoteText": "This is the text of the note"
}
```

يستدعي المثال السابق الإجراء المخصص الذي تم إنشاؤه مسبقاً في الحل المسمى بـ new_AddNoteToContact الخاص بجهة اتصال مزودة بمعرف 94d8c461-a27a-e511-80d2-00155d2a68d2 ثم يمرر المعلمات NoteTitle وNoteText إلى الإجراء. سيكون السلوك المتوقع لهذا الإجراء هو أنه ستتم إضافة ملاحظة جديدة إلى جهة الاتصال المقابلة بصحبة العنوان والنص المقدَّمان.

## <a name="more-details"></a>مزيد من التفاصيل

لمزيد من المعلومات حول كيفية استدعاء الإجراءات في التعليمات البرمجية، راجع [استخدام إجراءات API للويب](/power-apps/developer/common-data-service/webapi/use-web-api-actions/?azure-portal=true).
