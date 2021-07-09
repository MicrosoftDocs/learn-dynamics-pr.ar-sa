---
ms.openlocfilehash: e4821e58afe2f284224a6ff85d4154f99f0ad9d2
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071075"
---
<span data-ttu-id="150c8-101">يمكنك استخدام قيم من سجلات رئيسية، مثل العميل والمورد، كقيم افتراضية في الأبعاد الجديدة.</span><span class="sxs-lookup"><span data-stu-id="150c8-101">You can use values from master records, such as customer and vendor, as default values in new dimensions.</span></span> <span data-ttu-id="150c8-102">عند إنشاء الأبعاد الجديدة، يتم إدخال معرف السجل الرئيسي بقيم الأبعاد الخاصة بهذه السجلات الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="150c8-102">When the new dimensions are created, the master record ID is entered in the dimension values for those master records.</span></span> <span data-ttu-id="150c8-103">على سبيل المثال، عند إنشاء عميل جديد، يتم إدخال معرف العميل في البعد الخاص بالعميل.</span><span class="sxs-lookup"><span data-stu-id="150c8-103">For example, when you create a new customer, the customer ID is entered in the customer dimension.</span></span> <span data-ttu-id="150c8-104">عند إنشاء أوامر التوريد أو الفواتير أو المستندات الأخرى التي تتطلب معرف العميل، يتم استخدام القواعد الافتراضية الموجودة، وتتم إضافة معرف العميل إلى المستند.</span><span class="sxs-lookup"><span data-stu-id="150c8-104">When you create sales orders, invoices, or other documents that require a customer ID, the existing defaulting rules are used, and the customer ID is added to the document.</span></span>

<span data-ttu-id="150c8-105">**دفتر الأستاذ العام > دليل الحسابات > الحسابات > قيم الأبعاد المالية**</span><span class="sxs-lookup"><span data-stu-id="150c8-105">**General ledger > Chart of accounts > Accounts > Financial dimension values**</span></span>
 
<span data-ttu-id="150c8-106">[![لقطة شاشة لصفحة قيم الأبعاد المالية - العميل.](../media/customer-dim-values.png)](../media/customer-dim-values.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="150c8-106">[![Screenshot of the Financial dimensions values – CUSTOMER page.](../media/customer-dim-values.png)](../media/customer-dim-values.png#lightbox)</span></span>

<span data-ttu-id="150c8-107">يتم التحكم في ميزة البعد الافتراضي هذه بواسطة إعداد في الصفحة **الأبعاد المالية**.</span><span class="sxs-lookup"><span data-stu-id="150c8-107">This default dimension feature is controlled by a setting in the **Financial dimensions** page.</span></span> <span data-ttu-id="150c8-108">يسمي هذا الإعداد **نسخ القيم إلى هذا البعد في كل اسم بعد جديد تم إنشاؤه**، حيث **اسم البعد** هو اسم البعد.</span><span class="sxs-lookup"><span data-stu-id="150c8-108">This setting is named **Copy values to this dimension on each new DimensionName created**, where **DimensionName** is the name of the dimension.</span></span> <span data-ttu-id="150c8-109">بشكل افتراضي، يتم إيقاف تشغيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="150c8-109">By default, the feature is turned off.</span></span> <span data-ttu-id="150c8-110">ومع ذلك، يمكن تشغيلها في أي وقت.</span><span class="sxs-lookup"><span data-stu-id="150c8-110">However, it can be turned on at any time.</span></span>
 

<span data-ttu-id="150c8-111">[![لقطة شاشة لصفحة الأبعاد المالية التي تم تمييز إعداد نسخ القيم فيها.](../media/copy-values.png)](../media/copy-values.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="150c8-111">[![Screenshot of the Financial dimensions  page with the Copy values setting highlighted.](../media/copy-values.png)](../media/copy-values.png#lightbox)</span></span>

<span data-ttu-id="150c8-112">إذا كانت السجلات موجودة بالفعل للبعد، سيتم تحديث السجلات الرئيسية عند تشغيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="150c8-112">If records already exist for the dimension, the master records are updated when you turn the feature on.</span></span> <span data-ttu-id="150c8-113">ومع ذلك، لا يتم تحديث المستندات والحركات الموجودة.</span><span class="sxs-lookup"><span data-stu-id="150c8-113">However, existing documents and transactions aren't updated.</span></span>



