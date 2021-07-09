---
ms.openlocfilehash: 576a8187216fc7cdf04127f37e3e82975474cf27
ms.sourcegitcommit: 92a606f075028b19e15ae2f9ba20912cbeb643e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "6072637"
---
## <a name="scenario"></a><span data-ttu-id="97e39-101">السيناريو</span><span class="sxs-lookup"><span data-stu-id="97e39-101">Scenario</span></span>

<span data-ttu-id="97e39-102">يتم استخدام التسلسلات الرقمية لإنشاء المعرفات الفريدة الخاصة بسجلات البيانات الرئيسية وسجلات الحركات التي تتطلبها.</span><span class="sxs-lookup"><span data-stu-id="97e39-102">Number sequences are used to generate readable, unique identifiers for master data records and transaction records that require them.</span></span> 

<span data-ttu-id="97e39-103">يوضح هذا المعمل كيفيه إعداد التسلسلات الرقمية باستخدام صفحة **التسلسلات الرقمية**.</span><span class="sxs-lookup"><span data-stu-id="97e39-103">This lab shows how to set up number sequences using the **Number sequences** page.</span></span>

1. <span data-ttu-id="97e39-104">انتقل إلى **إدارة المؤسسة** > **التسلسلات الرقمية** > **التسلسلات الرقمية**.</span><span class="sxs-lookup"><span data-stu-id="97e39-104">Go to **Organization administration** > **Number sequences** > **Number sequences**.</span></span>
2. <span data-ttu-id="97e39-105">يستخدم في تحديد **التسلسل الرقمي**، ضمن القائمة الفرعية **جديد**.</span><span class="sxs-lookup"><span data-stu-id="97e39-105">Select **Number sequence**, under the **New** sub-menu.</span></span>
3. <span data-ttu-id="97e39-106">في الحقل **كود التسلسل الرقمي**، أدخل **معادلات**.</span><span class="sxs-lookup"><span data-stu-id="97e39-106">In the **Number sequence code** field, enter **Formulas**.</span></span>
4. <span data-ttu-id="97e39-107">في حقل **الاسم**، أدخِل **معادلات**.</span><span class="sxs-lookup"><span data-stu-id="97e39-107">In the **Name** field, enter **Formulas**.</span></span>
5. <span data-ttu-id="97e39-108">قم بتوسيع القسم **معلمات النطاق**، وحدد **مشترك** كنطاق للتسلسل الرقمي.</span><span class="sxs-lookup"><span data-stu-id="97e39-108">Expand the **Scope parameters** section, and select **Shared** as the scope for the number sequence.</span></span>
6. <span data-ttu-id="97e39-109">قم بتمديد قسم **المقاطع**، حدد **إضافة** وحدد تنسيق التسلسل الرقمي كما يلي:</span><span class="sxs-lookup"><span data-stu-id="97e39-109">Expand the **Segments** section, select **Add** and define the format for the number sequence as follows:</span></span>
   - <span data-ttu-id="97e39-110">**المقطع** – ثابتة؛ **القيمة** – نموذج</span><span class="sxs-lookup"><span data-stu-id="97e39-110">**Segment** – Constant; **Value** – FORM.</span></span> <span data-ttu-id="97e39-111">ولاحظ انه تم تعيين الطول إلى 4.</span><span class="sxs-lookup"><span data-stu-id="97e39-111">Notice that the length is set to 4.</span></span>
   - <span data-ttu-id="97e39-112">**مقطع** – أبجدي رقمي؛ **القيمة** - # # # #.</span><span class="sxs-lookup"><span data-stu-id="97e39-112">**Segment** – Alphanumeric; **Value** - ####.</span></span> <span data-ttu-id="97e39-113">ولاحظ انه تم تعيين الطول إلى 4.</span><span class="sxs-lookup"><span data-stu-id="97e39-113">Notice that the length is set to 4.</span></span>
7. <span data-ttu-id="97e39-114">قم بتوسيع القسم **عام**، وحدد ما إذا كان التسلسل الرقمي يدوياً أم مستمراً أو غير مستمر.</span><span class="sxs-lookup"><span data-stu-id="97e39-114">Expand the **General** section, and specify whether the number sequence is manual, and continuous or non-continuous.</span></span>
8. <span data-ttu-id="97e39-115">ضمن **تخصيص الرقم**، قم بتعيين **الأكبر** إلى **9999**.</span><span class="sxs-lookup"><span data-stu-id="97e39-115">Under **NUMBER ALLOCATION**, set the **Largest** to **9999**.</span></span>
9. <span data-ttu-id="97e39-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="97e39-116">Select **Save**.</span></span>
 
