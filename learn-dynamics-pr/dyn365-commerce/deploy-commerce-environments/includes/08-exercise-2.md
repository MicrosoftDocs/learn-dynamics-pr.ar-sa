---
ms.openlocfilehash: fe6f37a41a2cc49d696a10ad7d3e4aca4bd2c060
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070095"
---
<span data-ttu-id="c1330-101">طُلب من مطور Commerce توزيع موقع تجارة إلكترونية لإحدى الشركات.</span><span class="sxs-lookup"><span data-stu-id="c1330-101">The Commerce developer, has been asked to deploy an e-Commerce site for a company.</span></span> 
 

## <a name="before-you-begin"></a><span data-ttu-id="c1330-102">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="c1330-102">Before you begin</span></span> 
<span data-ttu-id="c1330-103">ستحتاج إلى الوصول إلى Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="c1330-103">You will need Microsoft Dynamics Lifecycle Services (LCS) access.</span></span> 
 
### <a name="to-deploy-an-e-commerce-site-follow-these-steps"></a><span data-ttu-id="c1330-104">لتوزيع موقع تجارة إلكترونية، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c1330-104">To deploy an e-Commerce site, follow these steps:</span></span>

1.  <span data-ttu-id="c1330-105">قم بتسجيل الدخول إلى LCS باستخدام بيانات الاعتماد الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="c1330-105">Sign in to LCS with your credentials.</span></span> 
2.  <span data-ttu-id="c1330-106">من **كل المشروعات**، حدد مشروعك.</span><span class="sxs-lookup"><span data-stu-id="c1330-106">From **All projects**, select your project.</span></span> 
3.  <span data-ttu-id="c1330-107">حدد بيئتك ضمن قسم **البيئات**.</span><span class="sxs-lookup"><span data-stu-id="c1330-107">Select your environment under the **Environments** section.</span></span>
4.  <span data-ttu-id="c1330-108">من صفحة **تفاصيل البيئة**، حدد **إدارة**.</span><span class="sxs-lookup"><span data-stu-id="c1330-108">From the **Environment details** page, select **Manage**.</span></span> 
5.  <span data-ttu-id="c1330-109">انتقل إلى صفحة **إعداد وتوزيع Commerce** وحدد علامة التبويب **التجارة الإلكترونية**. يظهر مربع حوار، حيث يجب عليك إدخال المعلومات المطلوبة للتشغيل.</span><span class="sxs-lookup"><span data-stu-id="c1330-109">Go to the **Commerce Deployment & Setup** page and select the **e-Commerce** tab. A dialog box appears, where you must enter the information that is required for provisioning.</span></span> 
7.  <span data-ttu-id="c1330-110">في الحقل **اسم بيئة التجارة الإلكترونية**، أدخل **D365EcommDemo**.</span><span class="sxs-lookup"><span data-stu-id="c1330-110">In the **e-Commerce environment name** field, enter **D365EcommDemo**.</span></span>
8.  <span data-ttu-id="c1330-111">في حقل **Commerce Scale unit**، أدخل **east-us-1**.</span><span class="sxs-lookup"><span data-stu-id="c1330-111">In the **Commerce Scale unit** field, enter **east-us-1**.</span></span>
9.  <span data-ttu-id="c1330-112">في الحقل **الموقع الجغرافي للتجارة الإلكترونية**، أدخل **أمريكا الشمالية**.</span><span class="sxs-lookup"><span data-stu-id="c1330-112">In the **e-Commerce geography** field, enter **North America**.</span></span>
10. <span data-ttu-id="c1330-113">حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="c1330-113">Select **Next**.</span></span>
11. <span data-ttu-id="c1330-114">في الحقل **أسماء المضيفين المدعومين**، أدخل https:\//www.fabrikam.com.</span><span class="sxs-lookup"><span data-stu-id="c1330-114">In the **Supported host names** field, enter https:\//www.fabrikam.com.</span></span>
12. <span data-ttu-id="c1330-115">في الحقل **مجموعة أمان AAD لمسؤول النظام**، أدخل **التجارة الإلكترونية**.</span><span class="sxs-lookup"><span data-stu-id="c1330-115">In the **AAD security group for system admin** field, enter **e-commerce**.</span></span> <span data-ttu-id="c1330-116">من القائمة الموجودة على اليسار، سترى التجارة الإلكترونية المحددة تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="c1330-116">From the list on the right, you will see the automatically selected e-commerce.</span></span>
13. <span data-ttu-id="c1330-117">حدد **تمكين التقييمات وخدمة المراجعة**.</span><span class="sxs-lookup"><span data-stu-id="c1330-117">Select **Enable ratings and review service**.</span></span>
14. <span data-ttu-id="c1330-118">في حقل البحث **مجموعة أمان AAD للمشرف على التقييمات والمراجعة**، أدخل **التقييمات**.</span><span class="sxs-lookup"><span data-stu-id="c1330-118">In the **AAD security group for ratings and review moderator** search field, enter **ratings**.</span></span> <span data-ttu-id="c1330-119">سيحدد تلقائياً سياسة الإشراف على التقييمات والمراجعات.</span><span class="sxs-lookup"><span data-stu-id="c1330-119">It will automatically select  a ratings and reviews moderation policy.</span></span>
15. <span data-ttu-id="c1330-120">حدد **تهيئة**.</span><span class="sxs-lookup"><span data-stu-id="c1330-120">Select **Initialize**.</span></span>
16. <span data-ttu-id="c1330-121">يمكنك عرض حالة التهيئة إما بتحديد **تحديث** أو العودة إلى علامة التبويب **التجارة الإلكترونية** لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="c1330-121">View the initialization status by either selecting **Refresh** or returning to the **e-Commerce** tab later.</span></span>

