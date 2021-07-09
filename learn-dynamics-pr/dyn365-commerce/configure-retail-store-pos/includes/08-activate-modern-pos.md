---
ms.openlocfilehash: 0150ace4e553e35615b61a15185414fa780d2a7b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070179"
---
<span data-ttu-id="f3027-101">تحتوي نقطة البيع الحديثة (MPOS) على إطار عمل ذاتي الخدمة يسمح للموارد غير الفنية بتثبيت السجلات جديدة وتنشيطها.</span><span class="sxs-lookup"><span data-stu-id="f3027-101">The MPOS has a self-service framework that lets non-technical resources install and activate new registers.</span></span> 

<span data-ttu-id="f3027-102">يحدد تسجيل الجهاز للسجل، الموجود ضمن **البيع بالتجزئة والتجارة > إعداد القنوات> إعداد نقطة البيع > الأجهزة**، ما إذا كان السجل هو جهاز MPOS أو CPOS.</span><span class="sxs-lookup"><span data-stu-id="f3027-102">The device record for a register, which is found under **Retail and Commerce > Channels setup > POS setup > Devices**, specifies if the register is an MPOS or CPOS device.</span></span> <span data-ttu-id="f3027-103">إذا كان نوع التطبيق هو **Retail Modern POS**، يعرض جزء الإجراءات الزر **تنزيل** الذي يمكنك تحديده لتنزيل **حزمة السجل** المحددة في التسجيل.</span><span class="sxs-lookup"><span data-stu-id="f3027-103">If the application type is **Retail Modern POS**, the Action Pane will display a **Download** button that you can select to download the **Register package** that is specified in the record.</span></span>  
  
<span data-ttu-id="f3027-104">[ ![لقطه شاشة لوظيفة التنزيل في صفحة الأجهزة](../media/download-ssm.jpg) ](../media/download-ssm.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="f3027-104">[ ![Screenshot of the download function on the  Devices page](../media/download-ssm.jpg) ](../media/download-ssm.jpg#lightbox)</span></span>


<span data-ttu-id="f3027-105">عند تنزيل تطبيق MPOS، يتطلب التطبيق وصولاً إدارياً لتثبيته على الجهاز.</span><span class="sxs-lookup"><span data-stu-id="f3027-105">When downloaded, the MPOS application requires administrative access to install it on the device.</span></span> <span data-ttu-id="f3027-106">سيحتاج العامل حينئذ إلى التحقق من إمكانية الوصول إلى Commerce Scale Unit من الوحدة الطرفية لنقطة البيع.</span><span class="sxs-lookup"><span data-stu-id="f3027-106">The worker will then need to validate that the Commerce Scale Unit from the POS terminal is accessible.</span></span> 

<span data-ttu-id="f3027-107">قد تكون هناك حاجة إلى مهام إضافية، مثل تمكين التحميل الجانبي للتطبيقات التي قد تتطلب مساعدة فنية، إذا لم يتم تمكينها بالفعل في إعداد سياسة عمومية على مستوى الشركة.</span><span class="sxs-lookup"><span data-stu-id="f3027-107">Additional tasks might be required, such as enabling the side loading of applications that might require technical assistance, if they are not already enabled in a company-wide global policy setting.</span></span> 

<span data-ttu-id="f3027-108">ويشبه تثبيت برنامج MPOS أي برنامج آخر بالامتداد ‎.exe على Microsoft Windows.</span><span class="sxs-lookup"><span data-stu-id="f3027-108">The installation of the MPOS software is like any other .exe program on Microsoft Windows.</span></span> <span data-ttu-id="f3027-109">بالنسبة إلى الأنظمة الأساسية للأجهزة المحمولة، فهي التجربة ذاتها لتثبيت أي جهاز محمول آخر لهذا النظام الأساسي دون استخدام تطبيق متجر التطبيق.</span><span class="sxs-lookup"><span data-stu-id="f3027-109">For mobile device platforms, it’s the same experience as installing any other mobile device for that platform without using the application’s store app.</span></span> 

<span data-ttu-id="f3027-110">عند تثبيت MPOS، يمكن للمستخدم تحديد **تنشيط** في التطبيق MPOS.</span><span class="sxs-lookup"><span data-stu-id="f3027-110">When MPOS is installed, the user can select **Activate** in the MPOS application.</span></span> <span data-ttu-id="f3027-111">سيُطلب من المستخدم معلومات تسجيل الدخول Azure AD (المجموعة أو المحلية) التي تم تعيينها للمستخدم لهويته الخارجية.</span><span class="sxs-lookup"><span data-stu-id="f3027-111">The user will be prompted for the Azure AD (cloud or on-premises) sign-in information that was mapped to the user for their external identity.</span></span>  

<span data-ttu-id="f3027-112">إذا كانت **حالة التنشيط** الخاصة بالجهاز معلقة، وكان لدى العامل هوية خارجية مرتبطة بالمستخدم وتم تعيين أمان **أذونات المدير** على **نعم** في **مجموعات أذونات نقطة البيع**، يمكن تنشيط الجهاز.</span><span class="sxs-lookup"><span data-stu-id="f3027-112">If the device's **Activation status** is pending, and the worker has an external identity associated with their user and has the **Manager permissions** security set to **Yes** in the **POS permissions groups**, the device can be activated.</span></span> 

<span data-ttu-id="f3027-113">سيسمح تطبيق المركز الرئيسي (HQ) لـ Commerce أيضاً بإيقاف تشغيل السجلات من موقع مركزي.</span><span class="sxs-lookup"><span data-stu-id="f3027-113">The Commerce Headquarters (HQ) application will also allow for the decommissioning of the registers from a centralized location.</span></span> 

