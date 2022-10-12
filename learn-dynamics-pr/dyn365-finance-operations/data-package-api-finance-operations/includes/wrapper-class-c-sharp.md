---
ms.openlocfilehash: 1dfdb0e9fc2ffb2aab64dc777bd2e6d2a5be64d1
ms.sourcegitcommit: c1858cd3b2bd6663edff36e214795d4934ad3ddf
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2022
ms.locfileid: "9576398"
---
لإنشاء فئة مجمعة، ستحتاج إلى استخدام بعض لغات البرمجة من .NET لاستهلاك خدمة ويب خارجية. يُمكن لتطبيقات التمويل والعمليات إنشاء مرجع لفئة التضمين والوصول إلى خدمة الويب الخارجية من خلال فئة التضمين.

تُظهر التعليمة البرمجية التالية مثالاً حول إنشاء مكتبة فئة C#. سيتم إنشاء مرجع خدمة لخدمة الويب SOAP في مكتبة الفئات.

```csharp
using System.ServiceModel;

namespace <WebServiceProviderName>
{
      public class <classname>
      {
             public static string <methodname>()
             {
                     var binding = new System.ServiceModel.BasicHttpBinding();
                     var endpointAddress = new EndpointAddress(“SOAP web service url”);
                     WebServiceSoapClient client = new WebServiceSoapClient(binding, endpointAddress);

                      return client.<web service method name>();
               }
       }
} 
```
تتضمن بيئة تطوير تطبيقات التمويل والعمليات عنصرًا يسمى **مراجع** ضمن **مستكشف التطبيقات**. يجب تضمين تجميع فئة الغلاف في المرجع. يُمكنك استدعاء الطريقة التي تم إنشاؤها في فئة الغلاف مباشرة باستخدام المرجع الذي تم إنشاؤه. 

ستشبه التعليمة البرمجية المثال التالي:

`WebServiceDataProvider.<classname>::<methodname>();`

يُمكنك إنشاء طرق منفصلة في فئة التضمين للوصول إلى جميع طرق خدمة الويب، والتي يُمكنك الاتصال بها في النهاية من التعليمة البرمجية لتطبيقات التمويل والعمليات حيثما كان ذلك مطلوبًا.
