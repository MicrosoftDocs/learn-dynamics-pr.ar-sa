---
ms.openlocfilehash: 81a82d634a02428f67202814bfe15c1beab48ee4
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070088"
---
في هذا التمرين، ستقوم بتنفيذ مشغل ثم تسجيل الملحق وتصحيح CRT، والتحقق من صحة الملحق.

## <a name="implement-a-trigger"></a>تنفيذ مشغل 

لتنفيذ مشغل، أكمل المهام كما هو موضح في مثال التعليمات البرمجية التالي.

1. تنفيذ **IrequestTriggerAsync**.
2. حدد **أنواع الطلبات المدعومة** لتحديد أنواع الطلبات التي يجب أن يتم تنفيذ المشغل عليها.
3. اكتب تنفيذ المشغل في طريقة **OnExecuting** إذا كان من الضروري تشغيل منطق الأعمال قبل معالجة الطلب.
4. اكتب تنفيذ المشغل في طريقة **OnExecuted** إذا كان من الضروري تشغيل منطق الأعمال بعد معالجة الطلب.

    ```csharp
    using Microsoft.Dynamics.Commerce.Runtime;
    using Microsoft.Dynamics.Commerce.Runtime.DataServices.Messages;
    using Microsoft.Dynamics.Commerce.Runtime.Messages;
    using System;
    using System.Collections.Generic;
    using System.Threading.Tasks;
        
    public class GetCustomerTriggers : IRequestTriggerAsync
    {
       /// <summary>
       /// Gets the supported requests for this trigger.
       /// </summary>
       public IEnumerable<Type> SupportedRequestTypes
       {
           get
             {
               return new[] { typeof(GetCustomerDataRequest) };
             }
       }
    
       /// <summary>
       /// Post trigger code.
       /// </summary>
       /// <param name="request">The request.</param>
       /// <param name="response">The response.</param>
       public async Task OnExecuted(Request request, Response response)
       {
          //Custom logic
                
         // The only stub to handle async signature 
            await Task.CompletedTask;
        }

        /// <summary>
        /// Pre trigger code
        /// </summary>
        /// <param name="request">The request.</param>
        public async Task OnExecuting(Request request)
        {
            // custom logic 
            await Task.CompletedTask;
        }
    }
    ```
    
## <a name="register-the-extension"></a>تسجيل الملحق

لتسجيل الملحق، أكمل المهام التالية:

1.  قم بنسخ ولصق مكتبة الملحقات إلى المجلد **...\RetailServer\webroot\bin\ext** ثم قم بتحديث ملف **commerceRuntime.ext.config** بمعلومات مكتبة الملحقات المخصصة الموجودة ضمن قسم التركيب. في هذا المثال، يُعد **Contoso.Commerce.Runtime.Services** اسم الملحق المخصص.
2.  لكي يعمل ملحق CRT في وضع دون الاتصال‬، قم بتحديث **...\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext\CommerceRuntime.MPOSOffline.ext.config** ‫بمعلومات مكتبة الملحقات المخصصة الموجودة ضمن قسم التركيب. 
3.  ‏‫قم بنسخ ولصق مكتبة الملحقات إلى **...\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext**.

## <a name="debug-crt"></a>تصحيح CRT
لتصحيح أخطاء CRT من نقطة البيع، قم بإرفاق المشروع الملحق CRT بعملية **w3wp.exe** (عملية IIS لخادم البيع بالتجزئة) عندما تكون نقطة البيع متصلة بخادم البيع بالتجزئة. 

بالنسبة لوضع عدم الاتصال، قم بإرفاق المشروع الملحق CRT بعملية **dllhost.exe**.

## <a name="validate-the-extension"></a>التحقق من صحة الملحق

للتحقق من صحة الملحق، أكمل المهام التالية:

1.  تسجيل الدخول إلى نقطة البيع
2.  البحث عن أي عميل في نقطة البيع ثم الانتقال إلى تفاصيل العميل. سيتم استدعاء طلب CRT السابق.


