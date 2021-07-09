---
ms.openlocfilehash: 81a82d634a02428f67202814bfe15c1beab48ee4
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070088"
---
<span data-ttu-id="a97f0-101">في هذا التمرين، ستقوم بتنفيذ مشغل ثم تسجيل الملحق وتصحيح CRT، والتحقق من صحة الملحق.</span><span class="sxs-lookup"><span data-stu-id="a97f0-101">In this exercise, you will implement a trigger and then register the extension, debug the CRT, and validate the extension.</span></span>

## <a name="implement-a-trigger"></a><span data-ttu-id="a97f0-102">تنفيذ مشغل</span><span class="sxs-lookup"><span data-stu-id="a97f0-102">Implement a trigger</span></span> 

<span data-ttu-id="a97f0-103">لتنفيذ مشغل، أكمل المهام كما هو موضح في مثال التعليمات البرمجية التالي.</span><span class="sxs-lookup"><span data-stu-id="a97f0-103">To implement a trigger, complete the tasks as shown in the following code example.</span></span>

1. <span data-ttu-id="a97f0-104">تنفيذ **IrequestTriggerAsync**.</span><span class="sxs-lookup"><span data-stu-id="a97f0-104">Implement **IrequestTriggerAsync**.</span></span>
2. <span data-ttu-id="a97f0-105">حدد **أنواع الطلبات المدعومة** لتحديد أنواع الطلبات التي يجب أن يتم تنفيذ المشغل عليها.</span><span class="sxs-lookup"><span data-stu-id="a97f0-105">Specify **SupportedRequestTypes** to define the request types that the trigger must be implemented for.</span></span>
3. <span data-ttu-id="a97f0-106">اكتب تنفيذ المشغل في طريقة **OnExecuting** إذا كان من الضروري تشغيل منطق الأعمال قبل معالجة الطلب.</span><span class="sxs-lookup"><span data-stu-id="a97f0-106">Write a trigger implementation in the **OnExecuting** method if business logic must be run before the request is addressed.</span></span>
4. <span data-ttu-id="a97f0-107">اكتب تنفيذ المشغل في طريقة **OnExecuted** إذا كان من الضروري تشغيل منطق الأعمال بعد معالجة الطلب.</span><span class="sxs-lookup"><span data-stu-id="a97f0-107">Write a trigger implementation in the **OnExecuted** method if business logic must be run after the request is addressed.</span></span>

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
    
## <a name="register-the-extension"></a><span data-ttu-id="a97f0-108">تسجيل الملحق</span><span class="sxs-lookup"><span data-stu-id="a97f0-108">Register the extension</span></span>

<span data-ttu-id="a97f0-109">لتسجيل الملحق، أكمل المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="a97f0-109">To register the extension, complete these tasks:</span></span>

1.  <span data-ttu-id="a97f0-110">قم بنسخ ولصق مكتبة الملحقات إلى المجلد **...\RetailServer\webroot\bin\ext** ثم قم بتحديث ملف **commerceRuntime.ext.config** بمعلومات مكتبة الملحقات المخصصة الموجودة ضمن قسم التركيب.</span><span class="sxs-lookup"><span data-stu-id="a97f0-110">Copy and paste the extension library to the **...\RetailServer\webroot\bin\ext** folder and then update the **commerceRuntime.ext.config** file with the custom extension library information under the composition section.</span></span> <span data-ttu-id="a97f0-111">في هذا المثال، يُعد **Contoso.Commerce.Runtime.Services** اسم الملحق المخصص.</span><span class="sxs-lookup"><span data-stu-id="a97f0-111">In this example, **Contoso.Commerce.Runtime.Services** is the custom extension name.</span></span>
2.  <span data-ttu-id="a97f0-112">لكي يعمل ملحق CRT في وضع دون الاتصال‬، قم بتحديث **...\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext\CommerceRuntime.MPOSOffline.ext.config** ‫بمعلومات مكتبة الملحقات المخصصة الموجودة ضمن قسم التركيب.</span><span class="sxs-lookup"><span data-stu-id="a97f0-112">For the CRT extension to work in offline mode, update **...\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext\CommerceRuntime.MPOSOffline.ext.config** with the extension library information under the composition section.</span></span> 
3.  <span data-ttu-id="a97f0-113">‏‫قم بنسخ ولصق مكتبة الملحقات إلى **...\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext**.</span><span class="sxs-lookup"><span data-stu-id="a97f0-113">Copy and paste the extension library to **...\Microsoft Dynamics 365\70\Retail Modern POS\ClientBroker\ext**.</span></span>

## <a name="debug-crt"></a><span data-ttu-id="a97f0-114">تصحيح CRT</span><span class="sxs-lookup"><span data-stu-id="a97f0-114">Debug CRT</span></span>
<span data-ttu-id="a97f0-115">لتصحيح أخطاء CRT من نقطة البيع، قم بإرفاق المشروع الملحق CRT بعملية **w3wp.exe** (عملية IIS لخادم البيع بالتجزئة) عندما تكون نقطة البيع متصلة بخادم البيع بالتجزئة.</span><span class="sxs-lookup"><span data-stu-id="a97f0-115">To debug CRT from POS, attach the CRT extension project to the **w3wp.exe** (IIS process for Retail server) process when POS is connected to the Retail server.</span></span> 

<span data-ttu-id="a97f0-116">بالنسبة لوضع عدم الاتصال، قم بإرفاق المشروع الملحق CRT بعملية **dllhost.exe**.</span><span class="sxs-lookup"><span data-stu-id="a97f0-116">For offline mode, attach the CRT extension project to the **dllhost.exe** process.</span></span>

## <a name="validate-the-extension"></a><span data-ttu-id="a97f0-117">التحقق من صحة الملحق</span><span class="sxs-lookup"><span data-stu-id="a97f0-117">Validate the extension</span></span>

<span data-ttu-id="a97f0-118">للتحقق من صحة الملحق، أكمل المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="a97f0-118">To validate the extension, complete these tasks:</span></span>

1.  <span data-ttu-id="a97f0-119">تسجيل الدخول إلى نقطة البيع</span><span class="sxs-lookup"><span data-stu-id="a97f0-119">Sign in to POS.</span></span>
2.  <span data-ttu-id="a97f0-120">البحث عن أي عميل في نقطة البيع ثم الانتقال إلى تفاصيل العميل.</span><span class="sxs-lookup"><span data-stu-id="a97f0-120">Search for any customer in POS and then go to the customer details.</span></span> <span data-ttu-id="a97f0-121">سيتم استدعاء طلب CRT السابق.</span><span class="sxs-lookup"><span data-stu-id="a97f0-121">The preceding CRT request will be called.</span></span>


