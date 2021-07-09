---
ms.openlocfilehash: 6e56d2591866181ce25b677b9fa5fc8fe11a85ce
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070085"
---
<span data-ttu-id="75301-101">يتم استخدام ملحقات Retail Server كخدمات لعرض المنطق من Commerce runtime.</span><span class="sxs-lookup"><span data-stu-id="75301-101">Retail Server extensions are used as services to expose the logic from Commerce runtime.</span></span>
<span data-ttu-id="75301-102">لإنشاء ملحق Retail Server، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="75301-102">To create a Retail Server extension, follow these steps:</span></span>

1. <span data-ttu-id="75301-103">قم بإنشاء ملحق CRT قبل إنشاء ملحق Retail Server.</span><span class="sxs-lookup"><span data-stu-id="75301-103">Create the CRT extension before you create the Retail Server extension.</span></span> <span data-ttu-id="75301-104">يجب ألا تشتمل واجهة API لـ Retail Server على منطق فيما عدا ذلك الذي يستدعي CRT مع المعلمات.</span><span class="sxs-lookup"><span data-stu-id="75301-104">A Retail Server API should have no logic except that which calls the CRT with the parameters.</span></span>
2. <span data-ttu-id="75301-105">قم بإنشاء مشروع مكتبة فئة C# جديد يستخدم الإصدار 4.6.1 من Microsoft .NET Framework، أو استخدم أياً من نماذج Retail Server في Retail SDK كقالب.</span><span class="sxs-lookup"><span data-stu-id="75301-105">Create a new C# class library project that uses Microsoft .NET Framework version 4.6.1, or use any of the Retail Server samples in the Retail SDK as a template.</span></span>
3. <span data-ttu-id="75301-106">في مشروع ملحق Retail Server، أضف مرجعاً إلى مشروع أو مكتبة ملحق CRT.</span><span class="sxs-lookup"><span data-stu-id="75301-106">In the Retail Server extension project, add a reference to your CRT extension library or project.</span></span> <span data-ttu-id="75301-107">يتيح لك هذا المرجع إمكانية استدعاء طلب CRT والاستجابة والكيانات.</span><span class="sxs-lookup"><span data-stu-id="75301-107">This reference lets you call the CRT request, response, and entities.</span></span>
4. <span data-ttu-id="75301-108">في مشروع ملحق Retail Server، قم بإضافة الحزمة **Microsoft.Dynamics.Commerce.Hosting.Contracts** باستخدام مدير حزم NuGet.</span><span class="sxs-lookup"><span data-stu-id="75301-108">In the Retail Server extension project, add the **Microsoft.Dynamics.Commerce.Hosting.Contracts** package by using the NuGet package manager.</span></span> <span data-ttu-id="75301-109">يمكن العثور على حزم NuGet في المجلد **retailsdk\pkgs**.</span><span class="sxs-lookup"><span data-stu-id="75301-109">NuGet packages can be found in the **RetailSDK\pkgs** folder.</span></span>
5. <span data-ttu-id="75301-110">قم بإنشاء فئة وحدة تحكم جديدة، ثم قم بتوسيعها من **IController**.</span><span class="sxs-lookup"><span data-stu-id="75301-110">Create a new controller class and then extend it from **IController**.</span></span> <span data-ttu-id="75301-111">ستحتوي فئة وحدة التحكم هذه على الطريقة التي يجب عرضها بواسطة واجهة API لـ Retail Server.</span><span class="sxs-lookup"><span data-stu-id="75301-111">This controller class will contain the method that must be exposed by the Retail Server API.</span></span> <span data-ttu-id="75301-112">داخل فئة وحدة التحكم، أضف طرق استدعاء طلب CRT.</span><span class="sxs-lookup"><span data-stu-id="75301-112">Inside the controller class, add methods to call the CRT request.</span></span> <span data-ttu-id="75301-113">لا تقم بتوسيع فئة وحدة التحكم الجديدة من فئات وحدات التحكم الموجودة مثل **CustomerController** و **ProductController**.</span><span class="sxs-lookup"><span data-stu-id="75301-113">Don’t extend the new controller class from existing controller classes such as **CustomerController** and **ProductController**.</span></span> <span data-ttu-id="75301-114">يجب أن توسع فئات الملحق الفئة **IController** فقط.</span><span class="sxs-lookup"><span data-stu-id="75301-114">Extension classes must extend the **IController** class only.</span></span>
6. <span data-ttu-id="75301-115">أضف السمة **RoutePrefix** في فئة وحدة التحكم لربطها بكيان ما.</span><span class="sxs-lookup"><span data-stu-id="75301-115">Add the **RoutePrefix** attribute on the controller class to bind it to an entity.</span></span> <span data-ttu-id="75301-116">وإذا لم تكن هذا السمة مرتبطة بكيان ما، فهي غير مطلوبة.</span><span class="sxs-lookup"><span data-stu-id="75301-116">If it is not bound to an entity, this attribute is not required.</span></span>
   <span data-ttu-id="75301-117">تكون السمة **BindEntity** مطلوبة في فئة وحدة التحكم إذا كنت تقوم بإنشاء وحدة تحكم جديدة وتعرض أحد الكيانات.</span><span class="sxs-lookup"><span data-stu-id="75301-117">The **BindEntity** attribute is required on a controller class if you are creating a new controller and exposing an entity.</span></span>

<span data-ttu-id="75301-118">تُنشئ التعليمة البرمجية العينة التالية واجهة API بسيطة لـ Retail Server لإرجاع كيان وسلسلة وقيمة منطقية.</span><span class="sxs-lookup"><span data-stu-id="75301-118">The following sample code creates a simple Retail Server API to return an entity, a string, and a bool value.</span></span> <span data-ttu-id="75301-119">لم يتم تضمين طلب CRT والاستجابة المستخدمة في العينة في هذه العينة.</span><span class="sxs-lookup"><span data-stu-id="75301-119">The CRT request and response that is used in the sample is not included in this sample.</span></span> <span data-ttu-id="75301-120">للحصول على مثال لطلب CRT والاستجابة، راجع قابلية التوسعة والمُشغلات الخاصة بـ Commerce runtime (CRT).</span><span class="sxs-lookup"><span data-stu-id="75301-120">For an example of the CRT request and response, see Commerce runtime (CRT) extensibility and triggers.</span></span>

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
7. <span data-ttu-id="75301-121">أنشئ مشروع الامتداد وانسخ الملف الثنائي إلى المجلد **\RetailServer\webroot\bin\Ext**.</span><span class="sxs-lookup"><span data-stu-id="75301-121">Build the extension project and copy the binary to the **\RetailServer\webroot\bin\Ext** folder.</span></span>
8. <span data-ttu-id="75301-122">قم بتحديث ملف **web.config** الخاص بـ Commerce Scale Unit في المجلد **\RetailServer\webroot** عن طريق إضافة اسم مكتبة الملحقات الجديدة في القسم **extensionComposition**.</span><span class="sxs-lookup"><span data-stu-id="75301-122">Update the Commerce Scale Unit **web.config** file in the **\RetailServer\webroot** folder by adding the new extension library name in the **extensionComposition** section.</span></span>

    ```csharp
    <extensionComposition>
    <!-- Use fully qualified assembly names for ALL if you need to support loading from the Global Assembly Cache.
    If you host in an application with a bin folder, this is not required. -->
    <add source="assembly" value="SimpleExtensionSample" >
    </extensionComposition>
     ```

9. <span data-ttu-id="75301-123">في Microsoft Internet Information Services (IIS)، أعد تشغيل Commerce Scale Unit لتحميل الملحق الجديد.</span><span class="sxs-lookup"><span data-stu-id="75301-123">In Microsoft Internet Information Services (IIS), restart the Commerce Scale Unit to load the new extension.</span></span>
10. <span data-ttu-id="75301-124">للتحقق من تحميل الملحق بنجاح، يمكنك استعراض بيانات تعريف Retail Server.</span><span class="sxs-lookup"><span data-stu-id="75301-124">To verify that the extension loaded successfully, you can browse the Retail Server metadata.</span></span> <span data-ttu-id="75301-125">تأكد من ظهور الكيانات والطرق الخاصة بك في القائمة.</span><span class="sxs-lookup"><span data-stu-id="75301-125">Confirm that your entities and methods appear in the list.</span></span> <span data-ttu-id="75301-126">لتصفح بيانات التعريف، افتح عنوان URL بالتنسيق التالي في مستعرض الويب: **https://RS-URL/Commerce/$metadata**</span><span class="sxs-lookup"><span data-stu-id="75301-126">To browse the metadata, open a URL in the following format in a web browser: **https://RS-URL/Commerce/$metadata**</span></span>
11. <span data-ttu-id="75301-127">لاستدعاء ملحق Retail Server في العميل الخاص بك، يجب إنشاء وكيل Typescript الخاص بالعميل.</span><span class="sxs-lookup"><span data-stu-id="75301-127">To call the Retail Server extension in your client, you must generate the client Typescript proxy.</span></span> <span data-ttu-id="75301-128">يمكنك بعد ذلك استخدام الوكيل لاستدعاء واجهات API خادم الجديدة الخاصة بـ Retail Server من العميل.</span><span class="sxs-lookup"><span data-stu-id="75301-128">You can then use the proxy to call your new Retail Server APIs from the client.</span></span>
<span data-ttu-id="75301-129">لا تحتاج إلى إضافة أو تضمين ملفات **EdmModelExtender** في الملحق مع واجهات API لملحق Retail Server.</span><span class="sxs-lookup"><span data-stu-id="75301-129">You don't need to add or include **EdmModelExtender** files in the extension with the Retail Server extension APIs.</span></span> <span data-ttu-id="75301-130">لا تكون الملفات مطلوبة إلا إذا كنت تستخدم الإصدار 10.0.10 من Retail SDK أو إصدار أقدم.</span><span class="sxs-lookup"><span data-stu-id="75301-130">The files are required only if you are using Retail SDK version 10.0.10 or earlier.</span></span>
<span data-ttu-id="75301-131">ملحق Retail Server الذي تم إنشاؤه باستخدام واجهة API **Microsoft.Dynamics.Commerce.Hosting.Contracts** الجديدة يمكن استخدامه في التنفيذ دون اتصال.</span><span class="sxs-lookup"><span data-stu-id="75301-131">A Retail Server extension that is built by using this new **Microsoft.Dynamics.Commerce.Hosting.Contracts** API can be used in an offline implementation.</span></span> <span data-ttu-id="75301-132">لا تحتاج إلى إنشاء مكتبة وكيل C# منفصلة.</span><span class="sxs-lookup"><span data-stu-id="75301-132">You don't need to generate a separate C# proxy library.</span></span> <span data-ttu-id="75301-133">انسخ مكتبة ملحق خادم البيع بالتجزئة في المجلد **\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext** ثم قم بتحديث ملف التكوين **RetailProxy.MPOSOffline.ext** لتضمين هذه المكتبة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="75301-133">Copy the Retail Server extension library in the **\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext** folder and then update the **RetailProxy.MPOSOffline.ext** config file to include this new library.</span></span> <span data-ttu-id="75301-134">يجب أن يُنشئ الملحق وكيل Typescript فقط.</span><span class="sxs-lookup"><span data-stu-id="75301-134">The extension must generate the Typescript proxy only.</span></span> <span data-ttu-id="75301-135">يمكن العثور على نماذج SDK في المجلد **\RetailSDK\SampleExtensions\TypeScriptProxy**.</span><span class="sxs-lookup"><span data-stu-id="75301-135">SDK samples can be found in the **\RetailSDK\SampleExtensions\TypeScriptProxy** folder.</span></span>
<span data-ttu-id="75301-136">يوضح المثال التالي كيفية تحديث العنصر **إضافة** في ملف التكوين **RetailProxy.MPOSOffline.ext**.</span><span class="sxs-lookup"><span data-stu-id="75301-136">The following example shows how to update the **add** element in the **RetailProxy.MPOSOffline.ext** config file.</span></span>

    ```csharp
    <?xml version="1.0" encoding="utf-8"?> 
    <retailProxyExtensions> 
        <composition> 
            <add source="assembly" value="Contoso.RetailServer.StoreHoursSample" /> 
        </composition> 
    </retailProxyExtensions> 
    ```


