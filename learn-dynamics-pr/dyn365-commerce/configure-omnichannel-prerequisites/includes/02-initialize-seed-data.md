---
ms.openlocfilehash: 3da941ddf90f0543063f398b9cdef7aca7d71fce
ms.sourcegitcommit: 606a7a063fe820fd318a57c61cae555d91de8c51
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "6070412"
---
<span data-ttu-id="90a40-101">تعتبر مجموعة بيانات التكوين الافتراضية مطلوبة لكل عمليات التنفيذ كنقطه بداية.</span><span class="sxs-lookup"><span data-stu-id="90a40-101">A set of default configuration data is required for all implementations as a starting point.</span></span> <span data-ttu-id="90a40-102">بدلاً من إعادة إنشاء هذه البيانات يدويا، يمكنك بدء البيانات الأولية في **البيع بالتجزئة وCommerce > إعداد المراكز الرئيسية > المعلمات > معلمات Commerce > عام**.</span><span class="sxs-lookup"><span data-stu-id="90a40-102">Rather than re-create this data manually, you can initiate the seed data in **Retail and Commerce > Headquarters setup > Parameters > Commerce parameters > General**.</span></span> <span data-ttu-id="90a40-103">عند تحديد الزر **تهيئة**، سيقوم الحل Commerce بتشغيل برنامج نصي يقوم بملء أي بيانات موجودة واستبدالها والتي قد يتم تكوينها في مجموعة من الجداول.</span><span class="sxs-lookup"><span data-stu-id="90a40-103">When the **Initialize** button is selected, Commerce runs a script that populates and replaces any existing data that might be configured in a set of tables.</span></span>  

<span data-ttu-id="90a40-104">عادةً ما يتم تشغيل هذه العملية في بداية أي عملية تنفيذ ولكن يمكن تشغيلها أيضا عند تطبيق التحديثات.</span><span class="sxs-lookup"><span data-stu-id="90a40-104">This process is typically run at the beginning of an implementation but can also be run when updates are applied.</span></span> <span data-ttu-id="90a40-105">وباستخدام هذه الميزة بعد تغيير البيانات وتكوينها لتنفيذ ما يجب القيام به بحذر نظراً لأنه يمكن أن تخاطر بتغيير البيانات الخاصة بالتطبيق التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="90a40-105">Using this feature after data has been changed and configured for an implementation should be done with caution because you could risk changing implementation-specific data that is configured.</span></span> 
 
 
<span data-ttu-id="90a40-106">[ ![لقطة شاشة لصفحة Dynamics 365 Commerce المعلمات.](../media/commerce-parameters-page-02-ss.jpg) ](../media/commerce-parameters-page-02-ss.jpg#lightbox)</span><span class="sxs-lookup"><span data-stu-id="90a40-106">[ ![Screenshot of Dynamics 365 Commerce parameters page.](../media/commerce-parameters-page-02-ss.jpg) ](../media/commerce-parameters-page-02-ss.jpg#lightbox)</span></span>


<span data-ttu-id="90a40-107">تقوم التهيئة بإنشاء بيانات التكوين الافتراضية التالية:</span><span class="sxs-lookup"><span data-stu-id="90a40-107">Initialization creates the following default configuration data:</span></span>

-   <span data-ttu-id="90a40-108">المهام والمهام الفرعية في مجدول Commerce</span><span class="sxs-lookup"><span data-stu-id="90a40-108">Commerce scheduler jobs and sub jobs</span></span>
-   <span data-ttu-id="90a40-109">مخطط قناة Commerce</span><span class="sxs-lookup"><span data-stu-id="90a40-109">Commerce channel schema</span></span>
-   <span data-ttu-id="90a40-110">جداول التوزيع في Commerce</span><span class="sxs-lookup"><span data-stu-id="90a40-110">Commerce distribution schedules</span></span>
-   <span data-ttu-id="90a40-111">تخطيطات الشاشة الافتراضية التي تتضمن شبكات الأزرار والصور والسمات</span><span class="sxs-lookup"><span data-stu-id="90a40-111">Default screen layouts that include button grids, images, and themes</span></span>
-   <span data-ttu-id="90a40-112">معلومات المنطقة الزمنية</span><span class="sxs-lookup"><span data-stu-id="90a40-112">Time zone information</span></span>
-   <span data-ttu-id="90a40-113">عمليات نقطة البيع (POS)</span><span class="sxs-lookup"><span data-stu-id="90a40-113">Point-of-sale (POS) operations</span></span>
-   <span data-ttu-id="90a40-114">أذونات نقطة البيع</span><span class="sxs-lookup"><span data-stu-id="90a40-114">POS permissions</span></span>
-   <span data-ttu-id="90a40-115">تقارير القناة</span><span class="sxs-lookup"><span data-stu-id="90a40-115">Channel reports</span></span>
-   <span data-ttu-id="90a40-116">بيانات تعريف السمة</span><span class="sxs-lookup"><span data-stu-id="90a40-116">Attribute metadata</span></span>
-   <span data-ttu-id="90a40-117">قوالب التحقق من صحة الكيان</span><span class="sxs-lookup"><span data-stu-id="90a40-117">Entity validation templates</span></span>
-   <span data-ttu-id="90a40-118">مهمة الدفعات لإزالة سجل جلسة Commerce Data Exchange</span><span class="sxs-lookup"><span data-stu-id="90a40-118">Batch job to purge Commerce Data Exchange session history</span></span>
-   <span data-ttu-id="90a40-119">تمكين تسجيل الدخول إلى صناعة بطاقة الدفع (PCI)</span><span class="sxs-lookup"><span data-stu-id="90a40-119">Enabling of Payment card industry (PCI) logging</span></span>

<span data-ttu-id="90a40-120">قبل تشغيل عملية **التهيئة**، يجب إعداد بيانات اللغة والعنوان البريدي للكيان القانوني لأن البيانات التي يتم تكوينها تعتمد على هذه المتغيرات للتكوين الصحيح للبيانات.</span><span class="sxs-lookup"><span data-stu-id="90a40-120">Before you run the **Initialize** process, the language and postal address data must be set up for the legal entity because the data that is being configured relies on those variables for correct data configuration.</span></span> 

