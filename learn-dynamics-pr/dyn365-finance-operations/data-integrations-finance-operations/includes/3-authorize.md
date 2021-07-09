---
ms.openlocfilehash: ff32e2e799af9c001129fbdd1833bdff10d99b0f
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071551"
---
<span data-ttu-id="1c8f8-101">تستخدم حزمة واجهة برمجة تطبيقات (API) إطار عمل إدارة البيانات OAuth 2.0 لتفويض الوصول.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-101">The Data management framework's package API uses OAuth 2.0 to authorize access.</span></span> <span data-ttu-id="1c8f8-102">لكي تتمكن من استخدام واجهة برمجة التطبيقات (API)، يجب أن تكون متصلة برمز وصول OAuth مميز صالح.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-102">For you to use the API, it must be connected with a valid OAuth access token.</span></span> <span data-ttu-id="1c8f8-103">بالنسبة للمؤسسات التي تقوم بنشر محلي، ستستخدم Active Directory Federation Services ‏(AD FS).</span><span class="sxs-lookup"><span data-stu-id="1c8f8-103">For organizations that are doing an on-premises deployment, you will use Active Directory Federation Services (AD FS).</span></span> 

<span data-ttu-id="1c8f8-104">يستخدم Azure Active Directory (Azure AD)‏ OAuth 2.0 لتمكينك من السماح بالوصول إلى تطبيقات الويب وواجهات برمجة تطبيقات الويب داخل مستأجر Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-104">Azure Active Directory (Azure AD) uses OAuth 2.0 to enable you to authorize access to web applications and web Application Programming Interfaces within your Azure AD tenant.</span></span> <span data-ttu-id="1c8f8-105">للبدء، يجب تسجيل التطبيق مع مستأجر Azure AD الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-105">To begin, you must register the application with your Azure AD tenant.</span></span> <span data-ttu-id="1c8f8-106">يتم القيام بهذا من خلال [مدخل Microsoft Azure](https://ms.portal.azure.com/#home/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="1c8f8-106">This is done through the [Microsoft Azure portal](https://ms.portal.azure.com/#home/?azure-portal=true).</span></span>

<span data-ttu-id="1c8f8-107">فيما يلي نظرة عامة على تدفق طلب رمز مصادقة OAuth 2.0:</span><span class="sxs-lookup"><span data-stu-id="1c8f8-107">The following is an overview of the OAuth 2.0 authorization code request flow:</span></span>

1. <span data-ttu-id="1c8f8-108">يوجه العميل المستخدم إلى `/authorize endpoint`.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-108">The client directs the user to the `/authorize endpoint`.</span></span>
2. <span data-ttu-id="1c8f8-109">مع هذا الطلب، يشير العميل إلى الأذونات التي يحتاج إلى الحصول عليها من المستخدم الذي يحتاج إلى الوصول.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-109">With this request, the client indicates the permissions that it needs to acquire from the user who is needing access.</span></span> <span data-ttu-id="1c8f8-110">للحصول على نقطة نهاية تفويض OAuth 2.0 للمستأجر الخاص بك، يمكنك الانتقال إلى **تسجيلات التطبيقات > نقاط النهاية** في مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-110">To get your OAuth 2.0  authorization endpoint for your tenant, you can go to **App registrations > Endpoints** in the Azure portal.</span></span>
3. <span data-ttu-id="1c8f8-111">في التطبيق الأصلي، يتم توجيه المستخدم لتسجيل الدخول والموافقة على الأذونات التي يطلبها التطبيق.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-111">In the native application, the user is directed to sign in and  consent to permissions that are requested by the app.</span></span> <span data-ttu-id="1c8f8-112">عند قيام المستخدم بالمصادقة ومنح الموافقة، سيقوم Azure AD بإرسال استجابة إلى التطبيق الخاص بك في عنوان `redirect_uri` الموجود في طلبك.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-112">When the user authenticates and grants consent, Azure AD will send a response to your application at the `redirect_uri` address in your request.</span></span>

    ```odata
    // Line breaks for legibility only

    https://login.microsoftonline.com/{tenant}/oauth2/authorize?
    client_id=6731de76-14a6-49ae-97bc-6eba6914391e
    &response_type=code
    &redirect_uri=http%3A%2F%2Flocalhost%3A12345
    &response_mode=query
    &resource=https%3A%2F%2Fservice.contoso.com%2F
    &state=12345
    ```
    <span data-ttu-id="1c8f8-113">نوعا الاستجابات هما:</span><span class="sxs-lookup"><span data-stu-id="1c8f8-113">The two types of responses are:</span></span>

    -   <span data-ttu-id="1c8f8-114">**الاستجابة الناجحة** - ستمنح الاستجابة الناجحة حق الوصول وتشمل موافقة المسؤول، ورمز التفويض الذي طلبه التطبيق، وقيمة جلسة فريدة، ومعلمة حالة.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-114">**Successful response** - A successful response will grant access and include the admin consent, the authorization code that the application requested, a unique session value, and a state parameter.</span></span>
    -   <span data-ttu-id="1c8f8-115">**الاستجابة لخطأ** - الاستجابة لخطأ لن تمنح رمز التفويض.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-115">**Error response** - An error response will not grant an authorization code.</span></span> <span data-ttu-id="1c8f8-116">تتضمن استجابة الخطأ قيمة رمز الخطأ ووصف الخطأ وقيمة الحالة.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-116">The error response includes the error code value, error description, and state value.</span></span>

    <span data-ttu-id="1c8f8-117">مع الاستجابة الناجحة، يتم منح رمز التفويض ويتم منح حق الوصول إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-117">With a successful response, an authorization code is granted and access is given to the user.</span></span>

4. <span data-ttu-id="1c8f8-118">يمكن الآن استرداد الرمز لرمز وصول مميز إلى المورد المطلوب.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-118">The code can now be redeemed for an access token to the desired resource.</span></span> <span data-ttu-id="1c8f8-119">ويتم تحقيق ذلك عن طريق إرسال طلب POST إلى نقطة نهاية `/token`.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-119">This is accomplished by sending a POST request to the `/token` endpoint.</span></span>
5. <span data-ttu-id="1c8f8-120">عند الاستجابة الناجحة، يقوم Azure AD بإرجاع رمز وصول مميز.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-120">Upon a successful response, Azure AD returns an access token.</span></span> <span data-ttu-id="1c8f8-121">الرمز المميز للوصول هو رمز ويب Json المميز (JWT).</span><span class="sxs-lookup"><span data-stu-id="1c8f8-121">The access token is a Json Web Token (JWT).</span></span>
6. <span data-ttu-id="1c8f8-122">عند طلب الرمز المميز للوصول، يقوم Azure AD بإرجاع بيانات التعريف حول رمز المميز للوصول لاستهلاك التطبيق.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-122">When the access token is requested, Azure AD returns metadata about the access token for the application's consumption.</span></span> <span data-ttu-id="1c8f8-123">يجب على العميل تخزين رموز الوصول مؤقتاً لمدة الرمز المميز المحدد ضمن استجابة OAuth2.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-123">The client should cache access tokens for the specified token lifetime within the OAuth2 response.</span></span> <span data-ttu-id="1c8f8-124">قد ترجع واجهة برمجة التطبيقات (API) الخاصة بالويب استجابة `invalid_token`؛ قد يرجع السبب في ذلك إلى وجود رمز مميز منتهي الصلاحية.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-124">A web API might return an `invalid_token` response; this could be due to an expired token.</span></span>
7. <span data-ttu-id="1c8f8-125">عند الحصول على الرمز المميز للوصول، يمكن استخدام الرمز المميز في طلبات واجهات برمجة التطبيقات (API) للويب.</span><span class="sxs-lookup"><span data-stu-id="1c8f8-125">When the access token is obtained, the token can be used in requests to web APIs.</span></span>
