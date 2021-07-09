---
ms.openlocfilehash: edb29f83a6d198cd03b4f7e4104ebfb0f3b392e8
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070930"
---
## <a name="scenario"></a><span data-ttu-id="80d46-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="80d46-101">Scenario</span></span>

<span data-ttu-id="80d46-102">يقوم مدير الحسابات بإعداد مخططات الحسابات لمؤسسة Contoso.</span><span class="sxs-lookup"><span data-stu-id="80d46-102">The Accounting manager is setting up the charts of accounts for Contoso Enterprise.</span></span> <span data-ttu-id="80d46-103">بالنسبة لبعض الحسابات، ترغب المؤسسة في تتبع المعلومات الإضافية التي لم يتم التقاطها في بنيات الحساب.</span><span class="sxs-lookup"><span data-stu-id="80d46-103">For some of the accounts, the organization wants to track additional information that is not captured in the account structures.</span></span> <span data-ttu-id="80d46-104">ويجب عليهم التأكد من أن مجموعة عملاء البعد المالي **80: العملاء الآخرون** فقط يمكن استخدام أقسام معينة.</span><span class="sxs-lookup"><span data-stu-id="80d46-104">They must ensure that for the financial dimension customer group **80: Other customers** only certain departments can be used.</span></span>  

<span data-ttu-id="80d46-105">قم بإجراء الخطوات التالية لإنشاء قاعدة متقدمة:</span><span class="sxs-lookup"><span data-stu-id="80d46-105">Perform the following steps to create an advanced rule:</span></span> 

1.  <span data-ttu-id="80d46-106">انتقل إلى **دفتر الأستاذ العام > مخطط الحسابات > البنى > بنى القواعد المتقدمة**.</span><span class="sxs-lookup"><span data-stu-id="80d46-106">Go to **General ledger > Chart of accounts > Structures > Advanced rule structures**.</span></span>    
2.  <span data-ttu-id="80d46-107">حدد **جديد** لإنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="80d46-107">Select **New** to create a new record.</span></span>  
3.  <span data-ttu-id="80d46-108">أدخل معرفاً فريداً لبنية القاعدة المتقدمة، ثم أدخل وصفاً مختصراً، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="80d46-108">Enter a unique identifier for the Advanced rule structure, enter a brief description, and then select **OK**.</span></span>  
4.  <span data-ttu-id="80d46-109">حدد **إضافة شريحة** لإضافة بعد مالي إلى البنية.</span><span class="sxs-lookup"><span data-stu-id="80d46-109">Select **Add segment** to add a financial dimension to the structure.</span></span>  
5.  <span data-ttu-id="80d46-110">حدد **مركز تكلفة** البعد المالي من القائمة، ثم حدد **إضافة شريحة**.</span><span class="sxs-lookup"><span data-stu-id="80d46-110">Select the financial dimension **CostCenter** from the list and then select **Add segment**.</span></span>  
7.  <span data-ttu-id="80d46-111">تحت علامة التبويب السريعة **تفاصيل القيمة المسموح بها**، يتم تعيين القيم الافتراضية **أين** إلى **مركز  التكلفة**.</span><span class="sxs-lookup"><span data-stu-id="80d46-111">Under the **Allowed value details** FastTab, the **Where** defaults to **CostCenter**.</span></span> 
8.  <span data-ttu-id="80d46-112">حدد **عامل التشغيل** مثل **يكون**.</span><span class="sxs-lookup"><span data-stu-id="80d46-112">Define the **Operator** such as **is**.</span></span>
9.  <span data-ttu-id="80d46-113">ثم قم بتعريف **القيمة** على سبيل المثال **020**</span><span class="sxs-lookup"><span data-stu-id="80d46-113">And then define the **Value** for example **020**.</span></span> 
10. <span data-ttu-id="80d46-114">أدخل **020** في حقل **مركز التكلفة** فقط تحت علامة التبويب السريعة **القسم والقيم المسموح بها**.</span><span class="sxs-lookup"><span data-stu-id="80d46-114">Enter **020** in the **CostCenter** field just under **Segments and allowed values** FastTab.</span></span> 
11. <span data-ttu-id="80d46-115">حدد **تنشيط** في القائمة بأعلى لحفظ التغييرات وجعلها فعالة في دفتر الأستاذ.</span><span class="sxs-lookup"><span data-stu-id="80d46-115">Select **Activate** in the menu at the top to save the changes and make them effective in the ledger.</span></span>
12. <span data-ttu-id="80d46-116">حدد **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="80d46-116">Select **Activate**.</span></span>






