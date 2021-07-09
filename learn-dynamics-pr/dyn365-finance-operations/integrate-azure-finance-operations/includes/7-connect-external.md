---
ms.openlocfilehash: 1f9fc6c8edf95ad94c0977d86b3089c410ea492d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071962"
---
<span data-ttu-id="050a2-101">بفضل كيانات البيانات وOData، يمكن توصيل تطبيقات Finance and Operations بالعديد من الخدمات الخارجية.</span><span class="sxs-lookup"><span data-stu-id="050a2-101">Thanks to data entities and OData, Finance and Operations apps can connect to several external services.</span></span> <span data-ttu-id="050a2-102">ومع ذلك، للقيام بذلك، يجب تسجيل الخدمات باستخدام Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="050a2-102">However, to do that, the services must be registered with the Azure Active Directory (Azure AD).</span></span>

<span data-ttu-id="050a2-103">لتسجيل خدمة باستخدام Azure AD، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="050a2-103">To register a service with the Azure AD, follow these steps:</span></span>

1.  <span data-ttu-id="050a2-104">انتقل إلى علامة التبويب **Azure Active Directory** الموجودة في مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="050a2-104">Go to the **Azure Active Directory** tab of the Azure portal.</span></span>
2.  <span data-ttu-id="050a2-105">حدد **خصائص** ولاحظ معرف المستأجر في الحقل **معرف الدليل**.</span><span class="sxs-lookup"><span data-stu-id="050a2-105">Select **Properties** and note the tenant ID in the **Directory ID** field.</span></span> <span data-ttu-id="050a2-106">ستحتاج إلى معرف المستأجر لاحقاً لاسترداد رمز مصادقة Azure AD المميز.</span><span class="sxs-lookup"><span data-stu-id="050a2-106">You will need the tenant ID later to retrieve an Azure AD authentication token.</span></span>
3.  <span data-ttu-id="050a2-107">في علامة التبويب **Azure Active Directory**، حدد **تسجيلات التطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="050a2-107">On the **Azure Active Directory** tab, select **App registrations**.</span></span>
4.  <span data-ttu-id="050a2-108">حدد **تسجيل تطبيق جديد**.</span><span class="sxs-lookup"><span data-stu-id="050a2-108">Select **New application registration**.</span></span>
5.  <span data-ttu-id="050a2-109">أدخل اسماً يعرّف التطبيق الخارجي الذي تقوم بتسجيله.</span><span class="sxs-lookup"><span data-stu-id="050a2-109">Enter a name that identifies the external application that you're registering.</span></span> <span data-ttu-id="050a2-110">بالنسبة للتطبيق الذي ستجري مصادقته باستخدام سر مشترك، حدد **‎تطبيق ويب/ API**.</span><span class="sxs-lookup"><span data-stu-id="050a2-110">For an application that will authenticate by using a shared secret, select **Web app / API**.</span></span>
6.  <span data-ttu-id="050a2-111">حدد التطبيق الجديد وانسخ معرف التطبيق.</span><span class="sxs-lookup"><span data-stu-id="050a2-111">Select the new application and copy the application ID.</span></span>
7.  <span data-ttu-id="050a2-112">حدد **الأذونات المطلوبة**.</span><span class="sxs-lookup"><span data-stu-id="050a2-112">Select **Required permissions**.</span></span>
8.  <span data-ttu-id="050a2-113">حدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="050a2-113">Select **Add**.</span></span>
9.  <span data-ttu-id="050a2-114">اختر **تحديد API**.</span><span class="sxs-lookup"><span data-stu-id="050a2-114">Choose **Select an API**.</span></span>
10. <span data-ttu-id="050a2-115">حدد **Microsoft Dynamics ERP (Microsoft.ERP)**.</span><span class="sxs-lookup"><span data-stu-id="050a2-115">Select **Microsoft Dynamics ERP (Microsoft.ERP)**.</span></span>
11. <span data-ttu-id="050a2-116">ضمن **الأذونات المفوضة**، يجب عليك تحديد الخيارات التالية، بحدٍ أدنى:</span><span class="sxs-lookup"><span data-stu-id="050a2-116">Under **Delegated permissions**, you must select, at a minimum, the following options:</span></span>
    - <span data-ttu-id="050a2-117">**الوصول إلى خدمة Dynamics AX المخصصة**</span><span class="sxs-lookup"><span data-stu-id="050a2-117">**Access Dynamics AX Custom Service**</span></span>
    - <span data-ttu-id="050a2-118">**الوصول إلى بيانات Dynamics AX**</span><span class="sxs-lookup"><span data-stu-id="050a2-118">**Access Dynamics AX data**</span></span>
    - <span data-ttu-id="050a2-119">**الوصول إلى Dynamics AX عبر الإنترنت كمستخدمي المؤسسة**</span><span class="sxs-lookup"><span data-stu-id="050a2-119">**Access Dynamics AX online as organization users**</span></span>
12. <span data-ttu-id="050a2-120">حدد **تم**.</span><span class="sxs-lookup"><span data-stu-id="050a2-120">Select **Done**.</span></span>
13. <span data-ttu-id="050a2-121">حدد **المفاتيح**.</span><span class="sxs-lookup"><span data-stu-id="050a2-121">Select **Keys**.</span></span>
14. <span data-ttu-id="050a2-122">في مربع الحوار الذي يظهر، أدخل وصفاً، ثم اضبط قيمة **انتهاء الصلاحية** إلى **عدم انتهاء مدة الصلاحية مطلقاً**.</span><span class="sxs-lookup"><span data-stu-id="050a2-122">In the dialog box that appears, enter a description, and then set the **Expires** value to **Never expires**.</span></span>
15. <span data-ttu-id="050a2-123">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="050a2-123">Select **Save**.</span></span>

<span data-ttu-id="050a2-124">عندما تقوم بتسجيل خدمتك في Azure AD، فستحتاج أيضاً إلى تسجيلها في تطبيقات Finance and Operations باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="050a2-124">When you've registered your service in Azure AD, you'll also need to register it in Finance and Operations apps by using the following steps:</span></span>

1.  <span data-ttu-id="050a2-125">في تطبيقات Finance and Operations، انتقل إلى **إدارة النظام > إعداد > تطبيقات Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="050a2-125">In Finance and Operations apps, go to **System administration > Setup > Azure Active Directory applications**.</span></span>
2.  <span data-ttu-id="050a2-126">حدد **جديد‎**.</span><span class="sxs-lookup"><span data-stu-id="050a2-126">Select **New**.</span></span>
3.  <span data-ttu-id="050a2-127">في الحقل **معرف العميل**، أدخل معرف التطبيق الذي قمت بتسجيله فيه Azure AD.</span><span class="sxs-lookup"><span data-stu-id="050a2-127">In the **Client ID** field, enter the application ID that you registered in Azure AD.</span></span>
4.  <span data-ttu-id="050a2-128">في الحقل **الاسم**، أدخِل اسماً للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="050a2-128">In the **Name** field, enter a name for the application.</span></span>
5.  <span data-ttu-id="050a2-129">في الحقل **معرف المستخدم**، حدد معرّف مستخدم حساب الخدمة المناسب.</span><span class="sxs-lookup"><span data-stu-id="050a2-129">In the **User ID** field, select an appropriate service account user ID.</span></span>
6.  <span data-ttu-id="050a2-130">**احفظ** السجل.</span><span class="sxs-lookup"><span data-stu-id="050a2-130">**Save** the record.</span></span> 
