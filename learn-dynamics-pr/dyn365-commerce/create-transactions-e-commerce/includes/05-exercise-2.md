---
ms.openlocfilehash: f69f39d196041008e603bd470604a7e04b87772c
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070352"
---
<span data-ttu-id="e3506-101">أنت مسؤول النظام في شركة Fabrikam وتحتاج إلى التحقق من مزامنة أمر عميل معين مع المركز الرئيسي لـ Commerce (HQ).</span><span class="sxs-lookup"><span data-stu-id="e3506-101">You are the system administrator of Fabrikam and need to verify that a certain customer order has been synchronized with Commerce Headquarters (HQ).</span></span> <span data-ttu-id="e3506-102">في هذا التمرين، سوف تتحقق من مزامنة الأمر عبر الإنترنت الذي تم إنشاؤه في التمرين السابق بنجاح في المركز الرئيسي.</span><span class="sxs-lookup"><span data-stu-id="e3506-102">For this exercise, you will verify that the online order that was created in the previous exercise is successfully synchronized in HQ.</span></span>

<span data-ttu-id="e3506-103">يتم تنفيذ الخطوات الواردة في هذا التمرين من خلال وظائف دفعية في سيناريوهات واقعية.</span><span class="sxs-lookup"><span data-stu-id="e3506-103">The steps in this exercise are implemented by batch jobs in real-life scenarios.</span></span> <span data-ttu-id="e3506-104">نوصي بمراجعتها يدوياً لفهم العملية والتأكد من حدوث المزامنة المطلوبة في بيئة الاختبار قبل المتابعة إلى التمرين التالي.</span><span class="sxs-lookup"><span data-stu-id="e3506-104">We recommend that you go through them manually to understand the process and ensure that the needed synchronization has happened in the test environment before you proceed to the next exercise.</span></span>

1.  <span data-ttu-id="e3506-105">انتقل إلى المركز الرئيسي لـ Commerce وتحقق من أنك في الكيان القانوني **USRT**.</span><span class="sxs-lookup"><span data-stu-id="e3506-105">Go to Commerce Headquarters and verify that you are in legal entity **USRT**.</span></span>
2.  <span data-ttu-id="e3506-106">انتقل إلى **Retail وCommerce > Retail وCommerce IT > جدول التوزيع > P-0001**.</span><span class="sxs-lookup"><span data-stu-id="e3506-106">Go to **Retail and Commerce > Retail and Commerce IT > Distribution schedule > P-0001**.</span></span>
3.  <span data-ttu-id="e3506-107">حدد **تشغيل الآن** ثم حدد **نعم** في الرسالة التي سيتم عرضها.</span><span class="sxs-lookup"><span data-stu-id="e3506-107">Select **Run now** and then select **Yes** on the message that displays.</span></span> 
4.  <span data-ttu-id="e3506-108">في شريط **ابحث عن صفحة** في الجزء العلوي من الشاشة، ابحث عن **تحميل جلسات العمل‬**.</span><span class="sxs-lookup"><span data-stu-id="e3506-108">In the **Search for a page** bar on the top of the screen, search for and select **Upload sessions**.</span></span>
5.  <span data-ttu-id="e3506-109">تحقق من تسجيل وظيفة تحميل تطبيقية بعد قيامك بتشغيل الوظيفة **P-0001**.</span><span class="sxs-lookup"><span data-stu-id="e3506-109">Verify that an applied Upload job recorded after you ran the **P-0001** job.</span></span>
6.  <span data-ttu-id="e3506-110">انتقل إلى **Retail وCommerce > Retail وCommerce IT > Synchronize orders**.</span><span class="sxs-lookup"><span data-stu-id="e3506-110">Go to **Retail and Commerce > Retail and Commerce IT > Synchronize orders**.</span></span>
7.  <span data-ttu-id="e3506-111">في قسم **عقد المؤسسة المتاحة**، حدد جميع القنوات المتاحة وحدد السهم الأيمن لنقلها إلى قسم **عقد المؤسسة المحددة**.</span><span class="sxs-lookup"><span data-stu-id="e3506-111">In the **Available organization nodes** section, select all available channels and select the right arrow to move them to the **Selected organization nodes** section.</span></span>
8.  <span data-ttu-id="e3506-112">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="e3506-112">Select **OK**.</span></span>
9.  <span data-ttu-id="e3506-113">في شريط **ابحث عن صفحة** في الجزء العلوي من الشاشة، ابحث عن **حالة مزامنة الأمر** وحددها.</span><span class="sxs-lookup"><span data-stu-id="e3506-113">In the **Search for a page** bar on the top of the screen, search for and select **Order synchronization status**.</span></span>
10. <span data-ttu-id="e3506-114">تحقق من أن الأمر عبر الإنترنت الذي قمت بإنشائه متاح في القائمة وتحقق من تعيين **حالة الأمر معلقة** على **تم النجاح**.</span><span class="sxs-lookup"><span data-stu-id="e3506-114">Verify that the online order that you have created is available in the list and has a **Pending order status** set to **Succeeded**.</span></span>
11. <span data-ttu-id="e3506-115">استخدم الرقم المرجعي للطلب من التمرين السابق للعثور على الترتيب الصحيح في حقل **معرف مرجع القناة**.</span><span class="sxs-lookup"><span data-stu-id="e3506-115">Use the order reference number from the previous exercise to find the correct order in the **Channel reference ID** field.</span></span> 

