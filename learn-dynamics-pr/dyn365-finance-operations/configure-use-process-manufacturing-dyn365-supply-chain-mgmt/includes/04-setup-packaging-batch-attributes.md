---
ms.openlocfilehash: db0e5db8b7dba45fba044f024ae6de631a97808d
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073431"
---

## <a name="packaging-setup-for-bulk-and-packed-products"></a><span data-ttu-id="31094-101">إعداد التعبئة والتغليف للأصناف المجمعة والمعبأة</span><span class="sxs-lookup"><span data-stu-id="31094-101">Packaging setup for bulk and packed products</span></span>

<span data-ttu-id="31094-102">تُعرف الأصناف مثل المسامير والبراغي والترابيس والأجهزة الأخرى المستخدمة في عملية التصنيع بالأصناف المجمعة.</span><span class="sxs-lookup"><span data-stu-id="31094-102">Items such as nails, bolts, screws, and other hardware that is used in the manufacturing process are known as bulk items.</span></span>

<span data-ttu-id="31094-103">يتم إنشاء المنتجات المعبأة لتحديد وتتبع مدى توفر المواد السائبة المخزنة في أحجام عبوات مختلفة في المخزون.</span><span class="sxs-lookup"><span data-stu-id="31094-103">Packaged products are created to identify and track the availability of bulk material that is stored in different package sizes in inventory.</span></span> <span data-ttu-id="31094-104">تحتوي المعادلة للمنتج المعبأ على الصنف المجمع كمكون رئيسي مع مواد التعبئة والتصنيف.</span><span class="sxs-lookup"><span data-stu-id="31094-104">The formula for the packed product contains the bulk item as its main ingredient together with packing and labeling materials.</span></span>

<span data-ttu-id="31094-105">لإعداد وظيفة أوامر الدُفعة الموحدة (الحزم المعبأة في حاويات) لربط الطلبات السائبة مع الطلبات المعبأة، يجب عليك تحديد تحويل الصنف المجمع لجميع لأصناف مركبة معبأة.</span><span class="sxs-lookup"><span data-stu-id="31094-105">To set up the consolidated batch orders functionality (containerized packaging) to link a bulk order with packed orders, you must define the bulk item conversion for all packaged formula items.</span></span>

## <a name="batch-attributes-setup"></a><span data-ttu-id="31094-106">إعداد مواصفات التشغيلة</span><span class="sxs-lookup"><span data-stu-id="31094-106">Batch attributes setup</span></span>

<span data-ttu-id="31094-107">الهدف من مواصفات التشغيلة هو وصف خصائص المنتج ودُفعات المنتج.</span><span class="sxs-lookup"><span data-stu-id="31094-107">The purpose of batch attributes is to describe properties of the product and product batches.</span></span>

<span data-ttu-id="31094-108">بينما تختلف مواصفات التشغيلة من دُفعة إلى أخرى، بناءً على عوامل مثل الظروف البيئية أو جودة المواد الخام المستخدمة لإنتاج الدُفعة، ترتبط مواصفات التشغيلة نفسها بعدد صنف معين.</span><span class="sxs-lookup"><span data-stu-id="31094-108">While batch attributes can differ from batch to batch, depending on factors such as environmental conditions or the quality of raw materials that are used to produce the batch, the same batch attributes are associated with a specific item number.</span></span>

<span data-ttu-id="31094-109">لذلك، يتم دائماً تسجيل مواصفات التشغيلة هذه عند شراء أو إنشاء دُفعة جديدة من تلك المادة لهذا الصنف.</span><span class="sxs-lookup"><span data-stu-id="31094-109">Therefore, these batch attributes are always recorded whenever a new batch of that material is purchased or created for that item.</span></span> <span data-ttu-id="31094-110">قد تختلف أنواع مواصفات التشغيلة المستخدمة بشكل كبير من صناعة إلى أخرى.</span><span class="sxs-lookup"><span data-stu-id="31094-110">The use and types of batch attributes that are used can vary widely from one industry to another.</span></span>

<span data-ttu-id="31094-111">لمعرفة المزيد حول مواصفات التشغيلة، راجع [تحديد مواصفات التشغيلة وتكوينها لعملية التصنيع في Dynamics 365 Supply Chain Management](https://docs.microsoft.com/learn/modules/identify-configure-batch-attributes-process-manufacturing-dyn365-supply-chain-mgmt/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="31094-111">To learn more about batch attributes, see [Identify and configure batch attributes for process manufacturing in Dynamics 365 Supply Chain Management](https://docs.microsoft.com/learn/modules/identify-configure-batch-attributes-process-manufacturing-dyn365-supply-chain-mgmt/?azure-portal=true).</span></span>

### <a name="batch-number-group"></a><span data-ttu-id="31094-112">مجموعة رقم الدُفعة</span><span class="sxs-lookup"><span data-stu-id="31094-112">Batch number group</span></span>

<span data-ttu-id="31094-113">تسمح مجموعة أرقام الدُفعة لـ Supply Chain Management بإنشاء رقم دُفعة تلقائياً لأحد الأصناف استناداً إلى البيانات المحددة مثل التاريخ ومعرف التسلسل الرقمي.</span><span class="sxs-lookup"><span data-stu-id="31094-113">A batch number group allows Supply Chain Management to create a batch number automatically for an item based on specified data such as the date and number sequence ID.</span></span> <span data-ttu-id="31094-114">تكون هذه الطريقة مفيدة عند طلب رقم الدُفعة ولكن الشركة لا تريد إدخال الرقم يدوياً في حركة إيصال الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="31094-114">This method is useful when a batch number is required but a company does not want the number manually entered on a production receipt transaction.</span></span>
