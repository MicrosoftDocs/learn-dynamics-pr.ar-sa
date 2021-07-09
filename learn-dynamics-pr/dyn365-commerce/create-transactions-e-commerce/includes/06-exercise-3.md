---
ms.openlocfilehash: 1e61271343aa5060d9f55ca3ec3dfdf8fc439e80
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070332"
---
<span data-ttu-id="c04c3-101">انت عامل متجر في فرع سان فرانسيسكو لشركة البيع بالتجزئة **Fabrikam**.</span><span class="sxs-lookup"><span data-stu-id="c04c3-101">You are a San Francisco store worker for the **Fabrikam** retailer.</span></span> <span data-ttu-id="c04c3-102">يدخل عميل غير معروف إلى المتجر ويطلب استلام الأمر الخاص به: حذاء أكسفورد بني.</span><span class="sxs-lookup"><span data-stu-id="c04c3-102">An unknown customer walks into the store with the request to pick up their order: brown Oxford shoes.</span></span> <span data-ttu-id="c04c3-103">قام بتقديم أمر الشراء من خلال موقع التجارة الإلكترونية لشركة Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="c04c3-103">They placed the order through Fabrikam's e-Commerce site.</span></span> <span data-ttu-id="c04c3-104">يجب عليك تسجيل الدخول إلى نقطة البيع وإنهاء الأمر الخاص بالعميل حتى يتمكن من استلام الحذاء الخاص به.</span><span class="sxs-lookup"><span data-stu-id="c04c3-104">You must sign in to POS and finalize the order for the customer so that they can pick up their shoes.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="c04c3-105">المتطلبات الأساسية:</span><span class="sxs-lookup"><span data-stu-id="c04c3-105">Prerequisites:</span></span> 
-   <span data-ttu-id="c04c3-106">تأكد من أن حساب Azure AD الذي تستخدمه مرتبط بالعامل الذي لديه حق الوصول إلى متجر سان فرانسيسكو.</span><span class="sxs-lookup"><span data-stu-id="c04c3-106">Ensure that the Azure AD account that you are using is linked to the worker who has access to the San Francisco store.</span></span> 
-   <span data-ttu-id="c04c3-107">يجب تنشيط CPOS.</span><span class="sxs-lookup"><span data-stu-id="c04c3-107">CPOS should be activated.</span></span>

## <a name="detailed-steps"></a><span data-ttu-id="c04c3-108">الخطوات التفصيلية</span><span class="sxs-lookup"><span data-stu-id="c04c3-108">Detailed steps</span></span>
1.  <span data-ttu-id="c04c3-109">قم بتسجيل الدخول إلى CPOS باستخدام معرف العامل الذي يرتبط به حساب Azure AD الخاص بك وكلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="c04c3-109">Sign in to CPOS by using the worker ID to which your Azure AD account is linked and the password.</span></span> 
2.  <span data-ttu-id="c04c3-110">في شاشة **الترحيب‬**، حدد **الأوامر المطلوب التقاطها**.</span><span class="sxs-lookup"><span data-stu-id="c04c3-110">On the **Welcome** screen, select **Orders to pick up**.</span></span>
3.  <span data-ttu-id="c04c3-111">حدد الأمر الذي تريد استلامه من خلال البحث عن المنتج الذي قام العميل بطلبه.</span><span class="sxs-lookup"><span data-stu-id="c04c3-111">Select the order to pick up by looking for the product that the customer has ordered.</span></span>
4.  <span data-ttu-id="c04c3-112">حدد بند الأمر الذي يحتوي على الحذاء، والذي يعرض **كمية** تبلغ **1**.</span><span class="sxs-lookup"><span data-stu-id="c04c3-112">Select the order line with the shoes, which shows a **Quantity** of **1**.</span></span>
5.  <span data-ttu-id="c04c3-113">حدد **طرق الدفع**.</span><span class="sxs-lookup"><span data-stu-id="c04c3-113">Select **Payment methods**.</span></span> 
6.  <span data-ttu-id="c04c3-114">تم إنهاء الأمر الآن، ويمكنك إعطاء العميل الحذاء الخاص به.</span><span class="sxs-lookup"><span data-stu-id="c04c3-114">The order is now finalized, and you can give the customer their shoes.</span></span>

