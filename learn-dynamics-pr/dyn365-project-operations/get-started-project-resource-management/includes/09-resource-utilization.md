---
ms.openlocfilehash: 309c4d2acfc7e5fcf738028704a7a524359915e1
ms.sourcegitcommit: ecd5b30834eade4258e6987fff347afcf97fbf7a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "6072899"
---
<span data-ttu-id="3ffa7-101">يمكن أن يكون للموارد استخدام قابل للفوترة مستهدف.</span><span class="sxs-lookup"><span data-stu-id="3ffa7-101">Resources can have a target billable utilization.</span></span> <span data-ttu-id="3ffa7-102">ويتم تحديد استخدام الهدف هذا كسمة في الدور الافتراضي للمَورد أو يتم تعيينه في سجل المَورد القابل للحجز الفردي.</span><span class="sxs-lookup"><span data-stu-id="3ffa7-102">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="3ffa7-103">وتعتمد العمليات الحسابية للاستخدام على الساعات الفعلية التي قامت الموارد بالإعلام عنها باستخدام قيود الوقت المعتمدة.</span><span class="sxs-lookup"><span data-stu-id="3ffa7-103">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="3ffa7-104">تستخدم المعادلات الآتية لحساب الاستخدام:</span><span class="sxs-lookup"><span data-stu-id="3ffa7-104">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="3ffa7-105">**الاستخدام القابل للفوترة** - الساعات الفعلية الخاضعة للرسوم ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="3ffa7-105">**Billable utilization** - Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="3ffa7-106">**الاستخدام غير القابل للفوترة** - الوقت الفعلي مع معرف إدخال الفوترة = غير الخاضع للرسوم أو التكميلي أو غير المتاح ÷ القدرة الإنتاجية للمورد</span><span class="sxs-lookup"><span data-stu-id="3ffa7-106">**Non-billable utilization** - Actual time with billing enter ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="3ffa7-107">**داخلي** -الوقت الفعلي من دون عقد مبيعات ÷ القدرة الإنتاجية للمورد‬</span><span class="sxs-lookup"><span data-stu-id="3ffa7-107">**Internal** - Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="3ffa7-108">**القدرة الإنتاجية للمورد‬**- ساعات عمل المَورد – ساعات العمل – أيام غير العمل</span><span class="sxs-lookup"><span data-stu-id="3ffa7-108">**Resource capacity** - Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="3ffa7-109">يمكن العثور على طريقة عرض **استخدام المَورد** في جزء **الموارد**.</span><span class="sxs-lookup"><span data-stu-id="3ffa7-109">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="3ffa7-110">كل خليه في الشبكة تمثل النسبة المئوية للاستخدام القابل للفوترة للمَورد في فترة زمنية، مثل يوم أو أسبوع أو شهر.</span><span class="sxs-lookup"><span data-stu-id="3ffa7-110">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="3ffa7-111">تستخدم المعادلات الآتية لتلوين الخلايا:</span><span class="sxs-lookup"><span data-stu-id="3ffa7-111">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="3ffa7-112">**أخضر** - استخدام قابل للفوترة > = الاستخدام المستهدف للمَورد</span><span class="sxs-lookup"><span data-stu-id="3ffa7-112">**Green** - Billable utilization >= Resource target utilization</span></span>
- <span data-ttu-id="3ffa7-113">**أصفر** - الاستخدام المستهدف – 20 < = الاستخدام القابل للفوترة < الاستخدام المستهدف</span><span class="sxs-lookup"><span data-stu-id="3ffa7-113">**Yellow** - Target utilization – 20 <= Billable utilization < Target utilization</span></span>
- <span data-ttu-id="3ffa7-114">**أحمر** - استخدام قابل للفوترة > الاستخدام المستهدف – 20</span><span class="sxs-lookup"><span data-stu-id="3ffa7-114">**Red** - Billable utilization < Target utilization – 20</span></span>

![لقطة شاشة لطريقة عرض "استخدام المَورد".](../media/resource-utilization-ss.png)
  
