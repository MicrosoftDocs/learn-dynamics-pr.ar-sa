---
ms.openlocfilehash: 8168b17c8b485ebf4ce6aab957571abb8c71b9d3
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070931"
---
## <a name="scenario"></a><span data-ttu-id="dae1c-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="dae1c-101">Scenario</span></span>

<span data-ttu-id="dae1c-102">يرغب مدير الحسابات في تضمين قيمة **النسبة الحالية** على تقرير KPI للقدرة على المدى القصير.</span><span class="sxs-lookup"><span data-stu-id="dae1c-102">The Accounting manager wants to include the **Current ratio** value on the Short-term solvency KPI report.</span></span> <span data-ttu-id="dae1c-103">يتم حساب النسبة الحالية عن طريق تقسيم الأصول الحالية للشركة بواسطة التزامات الحالية.</span><span class="sxs-lookup"><span data-stu-id="dae1c-103">Current ratio is calculated by dividing a company’s current assets by current liabilities.</span></span> <span data-ttu-id="dae1c-104">تتكون الأصول الحالية عادة من النقد والأوراق النقدية السائلة وحسابات المقبوضات والمخزون والأوراق المالية القابلة للتسويق.</span><span class="sxs-lookup"><span data-stu-id="dae1c-104">Current assets typically consist of cash, cash equivalents, accounts receivable, inventory, and marketable securities.</span></span> <span data-ttu-id="dae1c-105">تتكون التزامات الحالية من أية التزامات مستحقة الدفع خلال سنة واحدة.</span><span class="sxs-lookup"><span data-stu-id="dae1c-105">Current liabilities consist of any liabilities that are payable within one year.</span></span>

<span data-ttu-id="dae1c-106">لاشتقاق قيمة الأصل الحالية، يجب أن يقوم مدير الحسابات بجمع قيم النقد والحسابات المدينة وحسابات المخزون.</span><span class="sxs-lookup"><span data-stu-id="dae1c-106">To derive the current asset value, the Accounting manager must sum the values of the cash, accounts receivable, and inventory accounts.</span></span> <span data-ttu-id="dae1c-107">ولا تعتبر الأصول الثابتة أصولاً حالية.</span><span class="sxs-lookup"><span data-stu-id="dae1c-107">Fixed assets are not considered current assets.</span></span> <span data-ttu-id="dae1c-108">لإجراء هذه العملية الحسابية، استخدم الحقل **فئة الحساب الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-108">To perform this calculation, they use the **Main account category** field.</span></span> <span data-ttu-id="dae1c-109">ستستخدم الحسابات الرئيسية التي تتم إضافتها إلى دليل الحسابات فيما بعد **فئة الحساب الرئيسي** التي سيتم تضمينها في الحسابات الموجودة.</span><span class="sxs-lookup"><span data-stu-id="dae1c-109">Main accounts that are added to the chart of accounts later will also use the **Main account category** to be included in existing calculations.</span></span>


## <a name="instructions"></a><span data-ttu-id="dae1c-110">الإرشادات</span><span class="sxs-lookup"><span data-stu-id="dae1c-110">Instructions</span></span>

<span data-ttu-id="dae1c-111">قم بإجراء الخطوات التالية لإنشاء فئة الحساب الرئيسي **دفتر الأستاذ العام**:</span><span class="sxs-lookup"><span data-stu-id="dae1c-111">Perform the following steps to create a **General ledger** Main account category:</span></span>

1.  <span data-ttu-id="dae1c-112">للوصول إلى الصفحة **فئات الحساب الرئيسي**، انتقل إلى **دفتر الأستاذ العام > دليل الحسابات > الحسابات > فئات الحساب الرئيسي**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-112">To access the **Main account categories** page, go to **General Ledger > Chart of accounts > Accounts > Main account categories**.</span></span>  
2.  <span data-ttu-id="dae1c-113">حدد الزر **جديد** لإنشاء سجل جديد.</span><span class="sxs-lookup"><span data-stu-id="dae1c-113">Select the **New** button to create a new record.</span></span>  
3.  <span data-ttu-id="dae1c-114">أدخل اسماً فريداً **لفئة الحساب الرئيسي** و **وصفاً**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-114">Enter a unique name for the **Main account category** and a **Description**.</span></span>  
4.  <span data-ttu-id="dae1c-115">حدد **نوع الحساب الرئيسي** لإقرانه بفئة الحساب.</span><span class="sxs-lookup"><span data-stu-id="dae1c-115">Select a **Main account type** to associate with the account category.</span></span> <span data-ttu-id="dae1c-116">والغرض من تحديد **نوع الحساب الرئيسي** هو تقليل البحث عن **فئات الحساب الرئيسي** المتاحة عند إنشاء حساب رئيسي جديد من الصفحة **دليل الحسابات**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-116">The purpose of selecting a **Main account type** is to reduce the lookup of available **Main account categories** when you create a new Main account from the **Chart of accounts** page.</span></span>  
5.  <span data-ttu-id="dae1c-117">لربط فئة حساب بحساب رئيسي، انقر على الزر **ربط الحسابات الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-117">To link an account category to a main account, click the **Link main accounts** button.</span></span> <span data-ttu-id="dae1c-118">أو قم بربط **فئة حساب رئيسي** بحساب من الصفحة **تفاصيل الحساب الرئيسية**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-118">Or, link a **Main account category** to an account from the **Main account details** page.</span></span> 
6.  <span data-ttu-id="dae1c-119">حدد **موافق** ثم **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="dae1c-119">Select **OK** and then **Close**.</span></span>

## <a name="go-to-the-next-lab-instructions-from-the-lab-environment"></a><span data-ttu-id="dae1c-120">الانتقال إلى إرشادات المعمل التالية من بيئة المعمل</span><span class="sxs-lookup"><span data-stu-id="dae1c-120">Go to the next lab instructions from the lab environment</span></span>
 
<span data-ttu-id="dae1c-121">حدد الزر **التالي** في الركن الأيسر السفلي من الشريط الجانبي.</span><span class="sxs-lookup"><span data-stu-id="dae1c-121">Select the **Next** button in the bottom-right corner of the side bar.</span></span> 

