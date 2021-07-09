---
ms.openlocfilehash: 817efc6688c2cb48ff09f5a968bc8c6e6aa45720
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070359"
---
<span data-ttu-id="8e7ec-101">بالنسبة لهذا التمرين، والتمرينات الأخرى في هذه الوحدة، استخدم بيانات العرض التوضيحي في الكيان القانوني **USRT**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-101">For this exercise, and the other exercises in this module, use the demo data in the **USRT** company.</span></span>

## <a name="scenario"></a><span data-ttu-id="8e7ec-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="8e7ec-102">Scenario</span></span>

<span data-ttu-id="8e7ec-103">ستقوم بتكوين مهمة توزيع لدفع تغييرات بيانات البيع بالتجزئة التي حدثت في آخر 30 دقيقة إلى مجموعة من متاجر البيع بالتجزئة.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-103">You will configure a distribution job to push changes to retail data that have occurred in the last 30 minutes to a group of retail stores.</span></span>

1. <span data-ttu-id="8e7ec-104">في شركة **USRT**، انتقل إلى **البيع بالتجزئة والتجارة > تكنولوجيا معلومات البيع بالتجزئة والتجارة > جدولة التوزيع**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-104">In the **USRT** company, go to **Retail and Commerce > Retail and Commerce IT > Distribution schedule**.</span></span>
2. <span data-ttu-id="8e7ec-105">في القائمة، حدد سجل جدولة التوزيع رقم **9999**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-105">In the list, select distribution schedule record **9999**.</span></span>
3. <span data-ttu-id="8e7ec-106">حدد **إنشاء وظيفة دفعية** في جزء الإجراءات بالصفحة.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-106">Select **Create batch job** in the Action Pane of the page.</span></span>
4. <span data-ttu-id="8e7ec-107">قم بتوسيع المجموعة **تشغيل في الخلفية**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-107">Expand the **Run in the background** group.</span></span>
5. <span data-ttu-id="8e7ec-108">قم بتعيين قيمة **معالجة الدُفعات** على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-108">Set the **Batch processing** value to **Yes**.</span></span>
6. <span data-ttu-id="8e7ec-109">في الحقل **وصف المهمة**، قم بتغيير القيمة إلى **9999-30mins**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-109">In the **Task description** field, change the value to **9999-30mins**.</span></span> 

   > [!NOTE]
   > <span data-ttu-id="8e7ec-110">يمكن أن يكون هذا الوصف هو كل ما تشعر أنه ملائم ووصفي للوظيفة الدفعية.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-110">This description can be whatever you feel is relevant and descriptive for the batch job.</span></span> 

7. <span data-ttu-id="8e7ec-111">في الحقل **مجموعة الدُفعات**، قم بتعيين القيمة على **البيع بالتجزئة**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-111">In the **Batch Group** field, set the value to **Retail**.</span></span>
8. <span data-ttu-id="8e7ec-112">حدد **تكرار**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-112">Select **Recurrence**.</span></span>
9. <span data-ttu-id="8e7ec-113">اترك القيمة **الانتهاء بعد** كما هي.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-113">Leave the **End After** value as it is.</span></span> <span data-ttu-id="8e7ec-114">ومع ذلك، في بيئة التشغيل، يمكن تعيين هذه القيمة على **لا يوجد تاريخ انتهاء**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-114">However, in a production environment, this value could be set to **No end date**.</span></span> 
10. <span data-ttu-id="8e7ec-115">في الحقل **العدد**، قم بتغيير القيمة إلى **30**.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-115">In the **Count** field, change the value to **30**.</span></span>
11. <span data-ttu-id="8e7ec-116">حدد **موافق** مرتين.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-116">Select **OK** twice.</span></span>

<span data-ttu-id="8e7ec-117">سيظهر شريط إعلام أزرق أسفل جزء الإجراءات الذي يحدد أنه قد تمت إضافة المهمة 9999-30mins إلى صف الدُفعة.</span><span class="sxs-lookup"><span data-stu-id="8e7ec-117">A blue notification bar will appear below the Action Pane that states that the 9999-30mins job was added to the batch queue.</span></span> 

