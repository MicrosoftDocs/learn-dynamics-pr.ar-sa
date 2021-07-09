---
ms.openlocfilehash: 6e56d2591866181ce25b677b9fa5fc8fe11a85ce
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070085"
---
يتم استخدام ملحقات Retail Server كخدمات لعرض المنطق من Commerce runtime.
لإنشاء ملحق Retail Server، اتبع الخطوات التالية:

1. قم بإنشاء ملحق CRT قبل إنشاء ملحق Retail Server. يجب ألا تشتمل واجهة API لـ Retail Server على منطق فيما عدا ذلك الذي يستدعي CRT مع المعلمات.
2. قم بإنشاء مشروع مكتبة فئة C# جديد يستخدم الإصدار 4.6.1 من Microsoft .NET Framework، أو استخدم أياً من نماذج Retail Server في Retail SDK كقالب.
3. في مشروع ملحق Retail Server، أضف مرجعاً إلى مشروع أو مكتبة ملحق CRT. يتيح لك هذا المرجع إمكانية استدعاء طلب CRT والاستجابة والكيانات.
4. في مشروع ملحق Retail Server، قم بإضافة الحزمة **Microsoft.Dynamics.Commerce.Hosting.Contracts** باستخدام مدير حزم NuGet. يمكن العثور على حزم NuGet في المجلد **retailsdk\pkgs**.
5. قم بإنشاء فئة وحدة تحكم جديدة، ثم قم بتوسيعها من **IController**. ستحتوي فئة وحدة التحكم هذه على الطريقة التي يجب عرضها بواسطة واجهة API لـ Retail Server. داخل فئة وحدة التحكم، أضف طرق استدعاء طلب CRT. لا تقم بتوسيع فئة وحدة التحكم الجديدة من فئات وحدات التحكم الموجودة مثل **CustomerController** و **ProductController**. يجب أن توسع فئات الملحق الفئة **IController** فقط.
6. أضف السمة **RoutePrefix** في فئة وحدة التحكم لربطها بكيان ما. وإذا لم تكن هذا السمة مرتبطة بكيان ما، فهي غير مطلوبة.
   تكون السمة **BindEntity** مطلوبة في فئة وحدة التحكم إذا كنت تقوم بإنشاء وحدة تحكم جديدة وتعرض أحد الكيانات.

تُنشئ التعليمة البرمجية العينة التالية واجهة API بسيطة لـ Retail Server لإرجاع كيان وسلسلة وقيمة منطقية. لم يتم تضمين طلب CRT والاستجابة المستخدمة في العينة في هذه العينة. للحصول على مثال لطلب CRT والاستجابة، راجع قابلية التوسعة والمُشغلات الخاصة بـ Commerce runtime (CRT).

    ```csharp
    /// <summary>
        /// New extended controller.
        /// </summary>
        [RoutePrefix("SimpleExtension")]  
        [BindEntity(typeof(SimpleEntity))]

        public class SimpleExtensionController : IController
        {
            /// <summary>
            /// The action to get the string value.
            /// </summary>
            /// <param name="context">The context parameters.</param>
            /// <param name="stringValue">The string value parameters.</param>
            /// <returns>The string value.</returns>
            [HttpPost]
            [Authorization(CommerceRoles.Customer, CommerceRoles.Employee)]
            public async Task<string> GetStringValue(IEndpointContext context, string stringValue)
            {
                GetStringValueResponse resp = await     context.ExecuteAsync<GetStringValueResponse>
                (new GetStringValueRequest(stringValue)).ConfigureAwait(false);
                return resp.StringValue;
            }
    
            /// <summary>
            /// The action to get the bool value.
            /// </summary>
            /// <param name="context">The context parameters.</param>
            /// <param name="boolValue">The string value parameters.</param>
            /// <returns>The bool value.</returns>
            [HttpPost]
            [Authorization(CommerceRoles.Customer, CommerceRoles.Employee)]
            public async Task<bool> GetBoolValue(IEndpointContext context, string boolValue)
            {
            GetBoolValueResponse resp = await context.ExecuteAsync<GetBoolValueResponse>
            (new GetBoolValueRequest(boolValue)).ConfigureAwait(false);
            return resp.BoolValue;
        }

            /// <summary>
            /// The action to get the simple entity.
            /// </summary>
            /// <param name="context">The context parameters.</param>
            /// <param name="name">The name parameters.</param>
            /// <returns>The simple entity.</returns>
            [HttpPost]
            [Authorization(CommerceRoles.Customer, CommerceRoles.Employee)]
            public async Task<SimpleEntity> GetSimpleEntity(IEndpointContext context, string name)
            {
                GetSimpleEntityResponse resp = await context.ExecuteAsync<GetSimpleEntityResponse>
                (new GetSimpleEntityRequest(name)).ConfigureAwait(false);
                return resp.SimpleEntityObj;
            }
    ```
7. أنشئ مشروع الامتداد وانسخ الملف الثنائي إلى المجلد **\RetailServer\webroot\bin\Ext**.
8. قم بتحديث ملف **web.config** الخاص بـ Commerce Scale Unit في المجلد **\RetailServer\webroot** عن طريق إضافة اسم مكتبة الملحقات الجديدة في القسم **extensionComposition**.

    ```csharp
    <extensionComposition>
    <!-- Use fully qualified assembly names for ALL if you need to support loading from the Global Assembly Cache.
    If you host in an application with a bin folder, this is not required. -->
    <add source="assembly" value="SimpleExtensionSample" >
    </extensionComposition>
     ```

9. في Microsoft Internet Information Services (IIS)، أعد تشغيل Commerce Scale Unit لتحميل الملحق الجديد.
10. للتحقق من تحميل الملحق بنجاح، يمكنك استعراض بيانات تعريف Retail Server. تأكد من ظهور الكيانات والطرق الخاصة بك في القائمة. لتصفح بيانات التعريف، افتح عنوان URL بالتنسيق التالي في مستعرض الويب: **https://RS-URL/Commerce/$metadata**
11. لاستدعاء ملحق Retail Server في العميل الخاص بك، يجب إنشاء وكيل Typescript الخاص بالعميل. يمكنك بعد ذلك استخدام الوكيل لاستدعاء واجهات API خادم الجديدة الخاصة بـ Retail Server من العميل.
لا تحتاج إلى إضافة أو تضمين ملفات **EdmModelExtender** في الملحق مع واجهات API لملحق Retail Server. لا تكون الملفات مطلوبة إلا إذا كنت تستخدم الإصدار 10.0.10 من Retail SDK أو إصدار أقدم.
ملحق Retail Server الذي تم إنشاؤه باستخدام واجهة API **Microsoft.Dynamics.Commerce.Hosting.Contracts** الجديدة يمكن استخدامه في التنفيذ دون اتصال. لا تحتاج إلى إنشاء مكتبة وكيل C# منفصلة. انسخ مكتبة ملحق خادم البيع بالتجزئة في المجلد **\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext** ثم قم بتحديث ملف التكوين **RetailProxy.MPOSOffline.ext** لتضمين هذه المكتبة الجديدة. يجب أن يُنشئ الملحق وكيل Typescript فقط. يمكن العثور على نماذج SDK في المجلد **\RetailSDK\SampleExtensions\TypeScriptProxy**.
يوضح المثال التالي كيفية تحديث العنصر **إضافة** في ملف التكوين **RetailProxy.MPOSOffline.ext**.

    ```csharp
    <?xml version="1.0" encoding="utf-8"?> 
    <retailProxyExtensions> 
        <composition> 
            <add source="assembly" value="Contoso.RetailServer.StoreHoursSample" /> 
        </composition> 
    </retailProxyExtensions> 
    ```


