---
ms.openlocfilehash: 138bd258b44f5c2a452efe5583c7f99b63a46356
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070327"
---
<span data-ttu-id="4eb81-101">في هذا التدريب، ستقوم بإنشاء رمز معلومات جديد عندما يتم إلغاء منتج في نظام نقطة البيع (POS).</span><span class="sxs-lookup"><span data-stu-id="4eb81-101">In this exercise, you will create a new info code for when a product is voided in the point of sale (POS) system.</span></span> 

1. <span data-ttu-id="4eb81-102">في شركة **USRT**، انتقل إلى **Retail وCommerce> إعداد القناة > رموز المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-102">In the **USRT** company, go to **Retail and Commerce > Channel setup > Info codes**.</span></span>
2. <span data-ttu-id="4eb81-103">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-103">Select **New**.</span></span>
3. <span data-ttu-id="4eb81-104">في حقل **رقم رمز المعلومات**، أدخِل **صنف ملغٍ**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-104">In the **Info code number** field, enter **VoidItem**.</span></span>
4. <span data-ttu-id="4eb81-105">في حقل **الوصف**، أدخِل **مطالبه المستخدم بسبب الإلغاء**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-105">In the **Description** field, enter **Prompt the user for a void reason**.</span></span>
5. <span data-ttu-id="4eb81-106">في حقل **المطالبة**، أدخِل **سبب إلغاء الصنف**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-106">In the **Prompt** field, enter **Void Item Reason**.</span></span>
6. <span data-ttu-id="4eb81-107">في حقل **نوع الإدخال**، حدد **قائمة الرمز الفرعي**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-107">In the **Input type** field, select **Subcode list**.</span></span>
7. <span data-ttu-id="4eb81-108">ضمن المجموعة **عام**، قم بتعيين الحقل **الإدخال مطلوب** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-108">Under the **General** group, set the **Input required** field to **Yes**.</span></span>
8. <span data-ttu-id="4eb81-109">حدد **الرموز الفرعية** في جزء الإجراء.</span><span class="sxs-lookup"><span data-stu-id="4eb81-109">Select **Subcodes** in the Action Pane.</span></span>
9. <span data-ttu-id="4eb81-110">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-110">Select **New**.</span></span>
10. <span data-ttu-id="4eb81-111">في حقل **رقم الرمز الفرعي**، أدخِل **1**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-111">In the **Subcode number** field, enter **1**.</span></span>
11. <span data-ttu-id="4eb81-112">في حقل **الوصف**، أدخِل **منتج خاطئ**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-112">In the **Description** field, enter **Wrong product**.</span></span>
12. <span data-ttu-id="4eb81-113">في حقل **رقم الرمز الفرعي**، أدخِل **2**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-113">In the **Subcode number** field, enter **2**.</span></span>
13. <span data-ttu-id="4eb81-114">في حقل **الوصف**، أدخِل **ليس مطلوباً**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-114">In the **Description** field, enter **No longer needed**.</span></span>
14. <span data-ttu-id="4eb81-115">في حقل **رقم الرمز الفرعي**، أدخِل **3**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-115">In the **Subcode number** field, enter **3**.</span></span>
15. <span data-ttu-id="4eb81-116">في حقل **الوصف**، أدخِل **‏‫غير ذلك‬**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-116">In the **Description** field, enter **Other**.</span></span>
16. <span data-ttu-id="4eb81-117">انتقل إلى **Retail وCommerce > إعداد القناة > إعداد نقطة البيع > ملفات تعريف نقاط البيع > ملفات تعريف الوظائف**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-117">Go to **Retail and Commerce > Channel setup > POS Setup > POS Profiles > Functionality profiles**.</span></span>
17. <span data-ttu-id="4eb81-118">في القائمة، حدد **FN001**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-118">In the list, select **FN001**.</span></span>
18. <span data-ttu-id="4eb81-119">حدد **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-119">Select **Edit**.</span></span>
19. <span data-ttu-id="4eb81-120">في حقل **منتج ملغٍ**، ضمن مجموعة **رموز المعلومات**، حدد رمز معلومات **الصنف الملغي** الذي قمت بإنشائه مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="4eb81-120">In the **Void product** field, in the **Info codes** group, select the **VoidItem** info code that you previously created.</span></span> 
20. <span data-ttu-id="4eb81-121">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="4eb81-121">Select **Save**.</span></span>


