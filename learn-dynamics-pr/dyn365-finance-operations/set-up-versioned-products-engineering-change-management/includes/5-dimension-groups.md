---
ms.openlocfilehash: 7ce99b0e9982e1383775249d4609f5930ca6f87a
ms.sourcegitcommit: 567643c6f57edb821768e02042f3f8f2455383f5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "6075030"
---
<span data-ttu-id="ea242-101">يحتاج العديد من الشركات إلى تعقب إصدار المنتج في جميع الحركات التي تتضمن هذا المنتج.</span><span class="sxs-lookup"><span data-stu-id="ea242-101">Many companies need to track the product version in all transactions that involve that product.</span></span> <span data-ttu-id="ea242-102">على سبيل المثال، قد ترغب في تعقب الإصدار الموجود في أمر مبيعات.</span><span class="sxs-lookup"><span data-stu-id="ea242-102">For example, they might want to track the version on a sales order.</span></span> <span data-ttu-id="ea242-103">وبدون هذا التتبع، سيقوم أمر المبيعات دائماً بتسجيل أحدث إصدار يتم بيعه.</span><span class="sxs-lookup"><span data-stu-id="ea242-103">Without that tracking, the sales order would always record the latest version as being sold.</span></span>

<span data-ttu-id="ea242-104">إذا كنت ترغب في تتبع الإصدار في إدارة التغييرات الهندسية، فيمكنك إضافته **كبُعد منتج**.</span><span class="sxs-lookup"><span data-stu-id="ea242-104">If you want to track the version in engineering change management, you can add it as a **Product dimension**.</span></span> <span data-ttu-id="ea242-105">ونتيجة لذلك، سيتم إعداد المنتج **كأصل المنتج**.</span><span class="sxs-lookup"><span data-stu-id="ea242-105">As a result, the product will be set up as a **Product master**.</span></span> <span data-ttu-id="ea242-106">بالإضافة إلى ذلك، يمكنك إضافة الإصدار مع **التكوين** و **الحجم** و **اللون** و **النمط** كأبعاد منتج محتملة.</span><span class="sxs-lookup"><span data-stu-id="ea242-106">Additionally, you can add the version along with **Configuration**, **Size**, **Color**, and **Style** as possible product dimensions.</span></span>

<span data-ttu-id="ea242-107">لإنشاء بُعد منتج الإصدار، اتبع الخطوات الآتية:</span><span class="sxs-lookup"><span data-stu-id="ea242-107">To create the version product dimension, follow these steps:</span></span>

1. <span data-ttu-id="ea242-108">قم بتمكين **إصدار بُعد المنتج** في مساحة عمل **إدارة الميزات**.</span><span class="sxs-lookup"><span data-stu-id="ea242-108">Enable the **Product dimension version** in the **Feature management** workspace.</span></span>

1. <span data-ttu-id="ea242-109">للانتقال إلى الأمام، يجب وضع الشركة في وضع **صيانة**.</span><span class="sxs-lookup"><span data-stu-id="ea242-109">To move forward, you need to put the company into **Maintenance** mode.</span></span> <span data-ttu-id="ea242-110">لمزيد من المعلومات، راجع [وضع الصيانة](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/maintenance-mode/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="ea242-110">For more information, see [Maintenance mode](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/maintenance-mode/?azure-portal=true).</span></span>

1. <span data-ttu-id="ea242-111">انتقل إلى **إدارة النظام > الإعداد > تكوين الترخيص**، انتقل إلى مجموعة **التجارة**، ثم حدد **بُعد المنتج - الإصدار** وقم بتنشيطه.</span><span class="sxs-lookup"><span data-stu-id="ea242-111">Go to **System administration > Setup > License configuration**, go to the **Trade** group, and then select and activate **Product dimension - Version**.</span></span>

    > [!div class="mx-imgBorder"]
    > <span data-ttu-id="ea242-112">[![لقطة شاشة لصفحة تكوين الترخيص، في علامة التبويب مفاتيح التكوين، مع تمييز خيار بُعد المنتج - الإصدار.](../media/product-dimension-version-license.png)](../media/product-dimension-version-license.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ea242-112">[![Screenshot of the License configuration page, on the Configuration keys tab, with the Product dimension - Version option highlighted.](../media/product-dimension-version-license.png)](../media/product-dimension-version-license.png#lightbox)</span></span>


<span data-ttu-id="ea242-113">عند تمكين البُعد واستخدامه على المنتجات، سيتم استخدامه بعدئذٍ في قوائم مكونات الصنف والمسارات.</span><span class="sxs-lookup"><span data-stu-id="ea242-113">When enabled and used on products, the dimension will then be used on BOMs and routes.</span></span> <span data-ttu-id="ea242-114">إذا لم تكن تستخدم بُعد الإصدار في أحد المنتجات، فلن تتم إضافة الإصدار إلى قوائم مكونات الصنف والمسارات، ولن تحدث أي اختلافات في الإصدارات المتتالية.</span><span class="sxs-lookup"><span data-stu-id="ea242-114">If you aren't using the version dimension on a product, the version won't be added to BOMs and routes, and no differences will occur in consecutive versions.</span></span>
