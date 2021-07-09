---
ms.openlocfilehash: a12da6c49bd9f52938c2704bfaffb824820b2303
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071669"
---
<span data-ttu-id="ab1f1-101">بإضافة مكتبات الفئات الجديدة لتطبيقات Finance and Operations، يمكنك استهلاك خدمات الويب.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-101">By adding new class libraries to Finance and Operations apps, you can consume web services.</span></span>

<span data-ttu-id="ab1f1-102">توضح لك الخطوات التالية كيفية استهلاك خدمة `StockQuote` خارجية باستخدام X++‎.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-102">The following steps show you how to consume an external `StockQuote` service by using X++.</span></span>

<span data-ttu-id="ab1f1-103">يمكنك استخدام مكتبه فئات C#‎ للسماح لـ Visual Studio بإنشاء أوامر Boilerplate برمجية تُستخدم للوصول إلى خدمة الويب.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-103">You can use a C# class library to allow Visual Studio to create the boilerplate code that is used to access the web service.</span></span> <span data-ttu-id="ab1f1-104">يستخدم نموذج الأوامر البرمجية هذا عينة خدمة ويب Contoso، لذا ستقوم باستبدال عنوان الويب بخدمة الويب الخاصة بمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-104">This code sample uses a sample Contoso web service, so you will replace the web address with your organization's specific web service.</span></span>

1.  <span data-ttu-id="ab1f1-105">افتح **Visual Studio** كمسؤول.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-105">Open **Visual Studio** as an administrator.</span></span>
2.  <span data-ttu-id="ab1f1-106">انتقل إلى **ملف > جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-106">Go to **File > New > Project**.</span></span>
3.  <span data-ttu-id="ab1f1-107">في مربع حوار **مشروع جديد** في العمود الأيمن، حدد **Visual C#** ضمن عُقدة **القوالب**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-107">In the **New project** dialog box in the left column, select   **Visual C#** under the **Templates** node.</span></span>
4.  <span data-ttu-id="ab1f1-108">حدد **مكتبة الصنف** من القائمة في العمود الأوسط.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-108">Select **Class Library** from the list in the middle column.</span></span>
5.  <span data-ttu-id="ab1f1-109">أدخل **ExternalServiceLibrary** للاسم.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-109">Enter **ExternalServiceLibrary** for the name.</span></span>
6.  <span data-ttu-id="ab1f1-110">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-110">Select **OK**.</span></span>
7.  <span data-ttu-id="ab1f1-111">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق عقدة **ExternalServiceLibrary**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-111">In the **Solution Explorer** window, right-click the    **ExternalServiceLibrary** node.</span></span>
8.  <span data-ttu-id="ab1f1-112">حدد **إضافة مرجع خدمة**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-112">Select **Add Service Reference**.</span></span>
9.  <span data-ttu-id="ab1f1-113">أدخل خدمة الويب الخاصة بمؤسسك في حقل **العنوان**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-113">Enter your organization's web service in the **Address** field.</span></span>
10. <span data-ttu-id="ab1f1-114">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-114">Select **OK**.</span></span>
11. <span data-ttu-id="ab1f1-115">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق عقدة **ExternalServiceLibrary**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-115">In the **Solution Explorer** window, right-click the    **ExternalServiceLibrary** node.</span></span>
12. <span data-ttu-id="ab1f1-116">حدد **إضافة > عنصر جديد**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-116">Select **Add > New Item**.</span></span>
13. <span data-ttu-id="ab1f1-117">حدد **‏‏الكود** في العمود الأيمن، ثم حدد **فئة** في العمود الأوسط.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-117">Select **Code** in the left column, and then select **Class** in the middle column.</span></span>
14. <span data-ttu-id="ab1f1-118">قم بتسمية الفئة **ExternalServiceClass**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-118">Name the class **ExternalServiceClass**.</span></span>
15. <span data-ttu-id="ab1f1-119">قم بإجراء التفاف لعملية خدمة StockQuote، كما هو موضح في نموذج الأوامر البرمجية التالي.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-119">Wrap the StockQuote service operation, as shown in the following code sample.</span></span> 

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

16. <span data-ttu-id="ab1f1-120">قم بتنفيذ إنشاء عن طريق النقر بزر الماوس الأيمن فوق مشروع **ExternalServiceLibrary** في **مستكشف الحلول**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-120">Perform a build by right-clicking the **ExternalServiceLibrary** project in the **Solution Explorer**.</span></span>
17. <span data-ttu-id="ab1f1-121">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-121">Select **Build**.</span></span> <span data-ttu-id="ab1f1-122">يتم إنشاء الملف الثنائي ExternalServiceLibrary.dll.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-122">The binary ExternalServiceLibrary.dll is created.</span></span>
18. <span data-ttu-id="ab1f1-123">حدد **ملف > جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-123">Select **File > New > Project**.</span></span>
19. <span data-ttu-id="ab1f1-124">في مربع حوار **مشروع جديد** في العمود الأيمن، حدد **Dynamics 365** ضمن عُقدة **القوالب**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-124">In the **New project** dialog box in the left column, select    **Dynamics 365** under the **Templates** node.</span></span>
20. <span data-ttu-id="ab1f1-125">حدد **Finance Operations** من الجزء الأوسط.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-125">Select **Finance Operations** from the middle column.</span></span>
21. <span data-ttu-id="ab1f1-126">أدخل **ExternalServiceLibrary** في الحقل **الاسم** وحدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-126">Enter **ExternalServiceLibrary** in the **Name** field and select **OK**.</span></span>
22. <span data-ttu-id="ab1f1-127">في نافذة **مستكشف الحلول**، انقر بزر الماوس الأيمن فوق عقدة **ExternalServiceLibrary**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-127">In the **Solution Explorer** window, right-click the    **ExternalServiceLibrary** node.</span></span>
23. <span data-ttu-id="ab1f1-128">حدد **إضافة مرجع**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-128">Select **Add Reference**.</span></span>
24. <span data-ttu-id="ab1f1-129">حدد **ExternalServiceLibrary.dll** من مربع حوار **إضافة مرجع**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-129">Select **ExternalServiceLibrary.dll** from the **Add reference** dialog box.</span></span>
25. <span data-ttu-id="ab1f1-130">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-130">Select **OK**.</span></span>
26. <span data-ttu-id="ab1f1-131">افتح **فئة** في عقدة **المراجع** في نافذة **مستكشف الحلول**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-131">Open the **Class** in the **References** node in the **Solution  Explorer** window.</span></span>
27. <span data-ttu-id="ab1f1-132">استخدم خدمات الويب الخارجية التي تمت الإشارة إليها في **ExternalServiceLibrary.dll**.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-132">Use the external web services that were referenced in     **ExternalServiceLibrary.dll**.</span></span> <span data-ttu-id="ab1f1-133">فيما يلي نموذج لأمر برمجي.</span><span class="sxs-lookup"><span data-stu-id="ab1f1-133">The following is a code sample.</span></span>
```xpp
public static void main(Args _args)
{
    info(ServiceLibrary.StockQuoteClass::GetQuote("MSFT"));
}
```
