---
ms.openlocfilehash: a12da6c49bd9f52938c2704bfaffb824820b2303
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071669"
---
بإضافة مكتبات الفئات الجديدة لتطبيقات Finance and Operations، يمكنك استهلاك خدمات الويب.

توضح لك الخطوات التالية كيفية استهلاك خدمة `StockQuote` خارجية باستخدام X++‎.

يمكنك استخدام مكتبه فئات C#‎ للسماح لـ Visual Studio بإنشاء أوامر Boilerplate برمجية تُستخدم للوصول إلى خدمة الويب. يستخدم نموذج الأوامر البرمجية هذا عينة خدمة ويب Contoso، لذا ستقوم باستبدال عنوان الويب بخدمة الويب الخاصة بمؤسستك.

1.  افتح **Visual Studio** كمسؤول.
2.  انتقل إلى **ملف > جديد > مشروع**.
3.  في مربع حوار **مشروع جديد** في العمود الأيمن، حدد **Visual C#** ضمن عُقدة **القوالب**.
4.  حدد **مكتبة الصنف** من القائمة في العمود الأوسط.
5.  أدخل **ExternalServiceLibrary** للاسم.
6.  حدد **موافق**.
7.  في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق عقدة **ExternalServiceLibrary**.
8.  حدد **إضافة مرجع خدمة**.
9.  أدخل خدمة الويب الخاصة بمؤسسك في حقل **العنوان**.
10. حدد **موافق**.
11. في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق عقدة **ExternalServiceLibrary**.
12. حدد **إضافة > عنصر جديد**.
13. حدد **‏‏الكود** في العمود الأيمن، ثم حدد **فئة** في العمود الأوسط.
14. قم بتسمية الفئة **ExternalServiceClass**.
15. قم بإجراء التفاف لعملية خدمة StockQuote، كما هو موضح في نموذج الأوامر البرمجية التالي. 

```xpp  
public static string GetQuote(string s)
{
//Code has been formatted for online viewing
        var binding = new System.ServiceModel.BasicHttpBinding();
        var endpointAddress = new EndpointAddress("http://www.contoso.net/stockquote.asmx");
        ServiceLibrary.QuoteReference.StockQuoteSoapClient client = new
        ServiceLibrary.QuoteReference.StockQuoteSoapClient(binding, endpointAddress); 

//GetQuote is the operation on the StockQuote service
return client.GetQuote(s);
}
```

16. قم بتنفيذ إنشاء عن طريق النقر بزر الماوس الأيمن فوق مشروع **ExternalServiceLibrary** في **مستكشف الحلول**.
17. حدد **إنشاء**. يتم إنشاء الملف الثنائي ExternalServiceLibrary.dll.
18. حدد **ملف > جديد > مشروع**.
19. في مربع حوار **مشروع جديد** في العمود الأيمن، حدد **Dynamics 365** ضمن عُقدة **القوالب**.
20. حدد **Finance Operations** من الجزء الأوسط.
21. أدخل **ExternalServiceLibrary** في الحقل **الاسم** وحدد **موافق**.
22. في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق عقدة **ExternalServiceLibrary**.
23. حدد **إضافة مرجع**.
24. حدد **ExternalServiceLibrary.dll** من مربع حوار **إضافة مرجع**.
25. حدد **موافق**.
26. افتح **فئة** في عقدة **المراجع** في نافذة **مستكشف الحلول**.
27. استخدم خدمات الويب الخارجية التي تمت الإشارة إليها في **ExternalServiceLibrary.dll**. فيما يلي نموذج لأمر برمجي.
```xpp
public static void main(Args _args)
{
    info(ServiceLibrary.StockQuoteClass::GetQuote("MSFT"));
}
```
