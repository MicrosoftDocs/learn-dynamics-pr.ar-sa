---
ms.openlocfilehash: 04a2bebd851301a28a83a583b1dc7c67426f0328
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070358"
---
<span data-ttu-id="1b54c-101">لا يتطلب تنشيط نقطة بيع المجموعة (CPOS) سوى إدخال عنوان URL في مستعرض مدعوم على جهاز نقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="1b54c-101">CPOS activation only requires that a URL is entered into a supported browser on the POS device.</span></span> <span data-ttu-id="1b54c-102">ويتم العثور على عنوان URL هذا في الحقل **عنوان URL لنقطة بيع المجموعة** في صفحة **البيع بالتجزئة والتجارة > إعداد القناة > إعداد نقطة البيع > الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="1b54c-102">This URL is found in the **Cloud POS URL** field on the **Retail and Commerce > Channel setup > POS setup > Devices** page.</span></span> <span data-ttu-id="1b54c-103">يتم ملء هذا الحقل تلقائياً عندما تقوم بتعيين الجهاز على أنه **نوع التطبيق** من **Retail Cloud POS**.</span><span class="sxs-lookup"><span data-stu-id="1b54c-103">This field is automatically populated when you designate the device as an **Application type** of **Retail Cloud POS**.</span></span>
 
<span data-ttu-id="1b54c-104">يتوفر تطبيق موجه.</span><span class="sxs-lookup"><span data-stu-id="1b54c-104">A guided application is available.</span></span>

![ <span data-ttu-id="1b54c-105">لقطة شاشة لصفحة بدء تنشيط Retail Cloud POS</span><span class="sxs-lookup"><span data-stu-id="1b54c-105">Screenshot of the Activate Retail Cloud POS start page</span></span>](../media/cpos-activate-ss.jpg)

<span data-ttu-id="1b54c-106">شاهد مقطع الفيديو التالي لتتعلم كيفية تنشيط نقطة بيع المجموعة.</span><span class="sxs-lookup"><span data-stu-id="1b54c-106">Watch the following video to learn how to activate CPOS.</span></span>

 > [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4AmL7]

<span data-ttu-id="1b54c-107">يجب إدخال **عنوان URL للخادم** و **معرف الجهاز** و **رقم السجل** في صفحة **التنشيط**.</span><span class="sxs-lookup"><span data-stu-id="1b54c-107">The **Server URL**, **Device ID**, and **Register number** must be entered on the **Activation** page.</span></span> <span data-ttu-id="1b54c-108">تُظهر لقطة الشاشة التالية مثالاً من صفحة **البيع بالتجزئة والتجارة > إعداد القناة> إعداد نقطة البيع > الأجهزة** ومن **عنوان URL لـ HOUSTON CPOS** لسجل **HOUSTON-14**.</span><span class="sxs-lookup"><span data-stu-id="1b54c-108">The following screenshot shows an example from the **Retail and Commerce > Channel setup > POS setup > Devices** page and from the **HOUSTON CPOS URL** for **HOUSTON-14** register.</span></span>
 
<span data-ttu-id="1b54c-109">[ ![لقطه شاشة لصفحة "الأجهزة" وارتباطات للبيانات في شاشة التنشيط](../media/cpos-activation-data-ssm.jpg) ](../media/cpos-activation-data-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="1b54c-109">[ ![Screenshot of the Devices page and links to data in the activation screen](../media/cpos-activation-data-ssm.jpg) ](../media/cpos-activation-data-ssm.jpg#lightbox)</span></span>

<span data-ttu-id="1b54c-110">بعد إدخال هذه المعلومات، ستتم مطالبة العامل مرة أخرى ببيانات اعتماد Azure AD (المجموعة أو المحلية) الخاصة بالهوية الخارجية المقترنة بها.</span><span class="sxs-lookup"><span data-stu-id="1b54c-110">After this information is entered, the worker will again be prompted for their Azure AD (cloud or on-premises) credentials of the external identity that is associated to them.</span></span> 

<span data-ttu-id="1b54c-111">ربما تم تنشيط السجل بالفعل على جهاز آخر ثم تم إلغاء تنشيطه.</span><span class="sxs-lookup"><span data-stu-id="1b54c-111">The register might have already been activated on another device and then deactivated.</span></span> <span data-ttu-id="1b54c-112">في هذه الحالة، ستظهر الشاشة التالية التي تفيد بأن الجهاز الآخر لن يعود صالحاً لهذا التسجيل.</span><span class="sxs-lookup"><span data-stu-id="1b54c-112">In that case, the following screen will appear, stating that the other device will no longer be valid for this register.</span></span> <span data-ttu-id="1b54c-113">تم إقران المعلومات المتعلقة بالجهاز مع السجل، وسيؤدي تحديد **متابعة** إلى تجاوز المعلومات القديمة.</span><span class="sxs-lookup"><span data-stu-id="1b54c-113">The information about the device is paired with the register and selecting **Continue** will override the old information.</span></span> 

![ <span data-ttu-id="1b54c-114">لقطة شاشة لصفحة إلغاء تنشيط السجل على جهاز آخر</span><span class="sxs-lookup"><span data-stu-id="1b54c-114">Screenshot of the page for deactivating the register on another device</span></span>](../media/deactivate-register-ss.jpg)

<span data-ttu-id="1b54c-115">ستمر نقطة البيع بعد ذلك خلال خطوات التنشيط مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="1b54c-115">The POS will then go through the activation steps again.</span></span> <span data-ttu-id="1b54c-116">عند اكتمال التنشيط، سيتم إحضار المستخدم إلى شاشة **تسجيل الدخول** الخاصة بنقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="1b54c-116">When the activation is complete, the user will be brought to the **Sign-in** screen of the POS.</span></span>
 
![ <span data-ttu-id="1b54c-117">لقطة شاشة لصفحة تسجيل الدخول في متجر Houston</span><span class="sxs-lookup"><span data-stu-id="1b54c-117">Screenshot of the Houston store sign-in page</span></span>](../media/houston-sign-in-ss.jpg)


