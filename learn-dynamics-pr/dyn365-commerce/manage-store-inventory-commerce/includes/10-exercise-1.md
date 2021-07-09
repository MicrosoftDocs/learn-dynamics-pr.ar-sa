---
ms.openlocfilehash: f9785f5580bb4763ae604e3012aa8f92a3e76299
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070309"
---
## <a name="before-you-begin"></a><span data-ttu-id="37eaf-101">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="37eaf-101">Before you begin</span></span>

<span data-ttu-id="37eaf-102">بالنسبة للتدريبات الخاصة بهذه الوحدة النمطية، يجب استخدام بيانات العرض التوضيحي في **USRT**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-102">For the exercises in this module, you should use the demo data in the **USRT** company.</span></span>
<span data-ttu-id="37eaf-103">تأكد من تكوين عمليات **الوارد** و **الصادر** و **عدد المخزون** في تخطيطات شاشة نقطة البيع لكل من متاجر **سان فرانسيسكو** و **هيوستن**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-103">Ensure that the **Inbound**, **Outbound**, and **Stock count** operations have been configured in your POS screen layouts for both **SANFRANCIS** and **HOUSTON** stores.</span></span>


## <a name="scenario"></a><span data-ttu-id="37eaf-104">السيناريو</span><span class="sxs-lookup"><span data-stu-id="37eaf-104">Scenario</span></span>

<span data-ttu-id="37eaf-105">في هذا التدريب، ستقوم بإنشاء طلب نقل 30 قطعة من المنتج **91001** و10 أجزاء من المنتج **93024** (الحجم 4) من متجر **هيوستن** إلى متجر **سان فرانسيسكو** الحالي.</span><span class="sxs-lookup"><span data-stu-id="37eaf-105">In this exercise, you will create a transfer request for 30 pieces of product **91001** and 10 pieces of product **93024** (size 4) from the **HOUSTON** store to your current store **SANFRANCIS**.</span></span>

1. <span data-ttu-id="37eaf-106">سجّل الدخول إلى متجر **سان فرانسيسكو** باستخدام سجل **SANFRAN-1** من تطبيق نقطة البيع باستخدام معرّف المعامل **000713**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-106">Sign in to the **SANFRANCIS** store by using the **SANFRAN-1** register from the POS application by using operator ID **000713**.</span></span>
2. <span data-ttu-id="37eaf-107">من الصفحة الرئيسية، قم بالتمرير لتحديد موقع قسم **المخزون**، ثم حدد عملية **المخزون الداخلي**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-107">From the home page, scroll to locate the **Inventory** section, and then select the **Inbound inventory** operation.</span></span>
3. <span data-ttu-id="37eaf-108">ضمن شريط التطبيقات، حدد **جديد** لإنشاء طلب مخزون وارد جديد للمتجر.</span><span class="sxs-lookup"><span data-stu-id="37eaf-108">On the app bar, select **New** to create a new inbound inventory request for your store.</span></span>
4. <span data-ttu-id="37eaf-109">عند المطالبة، حدد **اختيار المتجر**، ثم حدد **هيوستن** كالمتجر **المحول منه**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-109">When prompted, select **Choose store**, and then select **HOUSTON** as the **Transfer from** store.</span></span>
5. <span data-ttu-id="37eaf-110">حدد **إنشاء**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-110">Select **Create**.</span></span>
6. <span data-ttu-id="37eaf-111">حدد **إضافة منتج‬**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-111">Select **Add Product**.</span></span>
7. <span data-ttu-id="37eaf-112">أدخِل المنتج **91001** عند المطالبة بذلك.</span><span class="sxs-lookup"><span data-stu-id="37eaf-112">When prompted, enter product **91001**.</span></span>
8. <span data-ttu-id="37eaf-113">أدخِل الكمية **30** عند المطالبة بذلك.</span><span class="sxs-lookup"><span data-stu-id="37eaf-113">When prompted, enter quantity **30**.</span></span>
9. <span data-ttu-id="37eaf-114">أدخِل المنتج **93024** عند المطالبة بذلك.</span><span class="sxs-lookup"><span data-stu-id="37eaf-114">When prompted, enter product **93024**.</span></span>
10. <span data-ttu-id="37eaf-115">عند المطالبة، حدد الحجم **4**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-115">When prompted, select size **4**.</span></span>
11. <span data-ttu-id="37eaf-116">أدخِل الكمية **10** عند المطالبة بذلك.</span><span class="sxs-lookup"><span data-stu-id="37eaf-116">When prompted, enter quantity **10**.</span></span>
12. <span data-ttu-id="37eaf-117">أغلق مربع حوار **إضافة منتج** عن طريق تحديد الرمز **X** في مربع الحوار.</span><span class="sxs-lookup"><span data-stu-id="37eaf-117">Close the **Add a product** dialog box by selecting the **X** on the dialog box.</span></span>
13. <span data-ttu-id="37eaf-118">لإكمال العملية، حدد **إرسال الطلب**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-118">Select **Submit request** to complete the process.</span></span>
14. <span data-ttu-id="37eaf-119">عند المطالبة، حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-119">When prompted, select **Submit**.</span></span>
15. <span data-ttu-id="37eaf-120">قم بإغلاق مربع حوار التأكيد بتحديد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="37eaf-120">Close the confirmation dialog box by selecting **OK**.</span></span>

