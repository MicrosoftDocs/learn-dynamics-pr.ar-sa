---
ms.openlocfilehash: 782482a06421ac83328bdb25a995d28ddf0f15b8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073459"
---
<span data-ttu-id="acd80-101">يمكن تعريف المنتج بتركيزه على مكون نشط.</span><span class="sxs-lookup"><span data-stu-id="acd80-101">A product can be defined by its concentration of an active ingredient.</span></span>
<span data-ttu-id="acd80-102">يتم تصميم المكون النشط للمنتج باستخدام سمة دفعية خاصة بالمنتج ذات قيمة دنيا وقيمة قصوى ومستوى هدف.</span><span class="sxs-lookup"><span data-stu-id="acd80-102">The active ingredient of a product is modeled by using a product-specific batch attribute that has a minimum value, a maximum value, and a target level.</span></span>

<span data-ttu-id="acd80-103">يمثل المستوى المستهدف لسمة الدُفعة النسبة المئوية المقدرة لمكون نشط في منتج.</span><span class="sxs-lookup"><span data-stu-id="acd80-103">The target level of a batch attribute represents the estimated percentage of an active ingredient in a product.</span></span> <span data-ttu-id="acd80-104">تمثل القيم الدنيا والقصوى الانحراف المقبول من المستوى المستهدف.</span><span class="sxs-lookup"><span data-stu-id="acd80-104">The minimum and maximum values represent the accepted deviation from the target level.</span></span> <span data-ttu-id="acd80-105">على سبيل المثال، يمكن استخدام هذه القيم كتفاوت مقبول للدفعات عند استلام المنتج.</span><span class="sxs-lookup"><span data-stu-id="acd80-105">For example, these values can be used as an accepted tolerance for batches at product receipt.</span></span>

<span data-ttu-id="acd80-106">يمكن أن يكون للمنتج مكون نشط واحد فقط.</span><span class="sxs-lookup"><span data-stu-id="acd80-106">A product can have only one active ingredient.</span></span> <span data-ttu-id="acd80-107">لتحديد العنصر النشط لمنتج ما، يجب أولاً تعريف سمة دفعية خاصة بالمنتج.</span><span class="sxs-lookup"><span data-stu-id="acd80-107">To specify the active ingredient of a product, you must first define a product-specific batch attribute.</span></span> <span data-ttu-id="acd80-108">ثم يمكنك إقران السمة كسمة أساسية للمنتج.</span><span class="sxs-lookup"><span data-stu-id="acd80-108">Then, you can associate the attribute as a base attribute of the product.</span></span>

<span data-ttu-id="acd80-109">على مستوى المنتج، يجب أيضاً تحديد كيفية تسجيل مستوى المكون النشط لمجموعة من المنتج: كجزء من عملية استلام الشراء أو كجزء من عملية أمر الجودة.</span><span class="sxs-lookup"><span data-stu-id="acd80-109">On the product level, you must also specify how the level of the active ingredient for a batch of the product should be recorded: as part of the purchase receipt process or as part of a quality order process.</span></span>

<span data-ttu-id="acd80-110">لإقران سمة أساسية بمنتج، يكون الإعداد التالي مطلوباً:</span><span class="sxs-lookup"><span data-stu-id="acd80-110">To associate a base attribute with a product, the following setup is required:</span></span>

-   <span data-ttu-id="acd80-111">يجب أن يتم التحكم في المنتج من خلال الدُفعة.</span><span class="sxs-lookup"><span data-stu-id="acd80-111">The product must be batch-controlled.</span></span> <span data-ttu-id="acd80-112">لإجراء التحكم في دُفعة المنتجات، يجب تعيين مجموعة أبعاد تعقب للمنتج الذي يحتوي على بُعد دُفعة نشط.</span><span class="sxs-lookup"><span data-stu-id="acd80-112">To make a product batch-controlled, you must assign a tracking dimension group to the product that has an active Batch dimension.</span></span>

-   <span data-ttu-id="acd80-113">يجب تحديد السمة التي تشير إلى مستويات المكونات كسمة دفعية خاصة بالمنتج.</span><span class="sxs-lookup"><span data-stu-id="acd80-113">The attribute that indicates the ingredient levels must be defined as a product-specific batch attribute for the product.</span></span>

<span data-ttu-id="acd80-114">يمكنك البحث عن القيمة الفعلية للمكون النشط لإحدى الدفعات في الصفحة **سمات الدُفعات للمخزون** .</span><span class="sxs-lookup"><span data-stu-id="acd80-114">You can look up and edit the actual value of the active ingredient for a batch on the **Inventory batch attributes** page.</span></span> <span data-ttu-id="acd80-115">حدد **إدارة المخزون > الاستعلامات والتقارير > أبعاد التعقب > الدُفعات > سمات الدُفعات للمخزون**.</span><span class="sxs-lookup"><span data-stu-id="acd80-115">Select **Inventory management > Inquiries and reports > Tracking dimensions > Batches > Inventory batch attributes**.</span></span>
