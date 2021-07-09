---
ms.openlocfilehash: 24234b442760c6232fdb85c9a12442be3f2c3e05
ms.sourcegitcommit: 013207079dac7bc5d856f987fe790e7316c48106
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/19/2021
ms.locfileid: "6072844"
---
<span data-ttu-id="6e4dd-101">يمكن إدارة العملاء المتوقعين بالاستناد إلى المشروع وتأهيلهم في Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-101">Project-based leads can be managed and qualified in Project Operations.</span></span> <span data-ttu-id="6e4dd-102">تتضمن عملية إدارة العملاء المتوقعين إنشاء عملاء متوقعين على أساس العمل ثم تأهيلهم.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-102">The process of lead management includes creating work-based leads and then qualifying those leads.</span></span>
## <a name="project-sales-leads"></a><span data-ttu-id="6e4dd-103">عملاء متوقعون لمبيعات المشروع</span><span class="sxs-lookup"><span data-stu-id="6e4dd-103">Project sales leads</span></span>
<span data-ttu-id="6e4dd-104">في قسم **المبيعات**، في جزء التنقل الأيمن، افتح صفحة قائمة **عملاء متوقعون** لعرض قائمة بكافة سجلات العملاء المتوقعين في النظام.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-104">In the **Sales** section, in the left navigation pane, open the **Leads** list page to view a list of all lead records in the system.</span></span> <span data-ttu-id="6e4dd-105">قائمة العملاء المتوقعين التي يتم عرضها تستند إلى العمل وأنواع أخرى من العملاء المتوقعين التي يمكن إنشاؤها إذا كان لديك أيضاً تطبيقات Dynamics 365 Sales أو Dynamics 365 Field Service.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-105">The list of leads that are shown are work-based and other types of leads that can be created if you also have the Dynamics 365 Sales or Dynamics 365 Field Service applications.</span></span>

<span data-ttu-id="6e4dd-106">يمكنك إنشاء طريقة عرض تمت تصفيتها لرؤية العملاء المتوقعين بالاستناد إلى المشروع فقط عن طريق إنشاء عامل تصفية على قيمة **النوع**.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-106">You can create a filtered view to see only project-based leads by creating a filter on the **Type** value.</span></span> <span data-ttu-id="6e4dd-107">على سبيل المثال، يمكنك تحديد إظهار العملاء المتوقعين استناداً إلى العمل فحسب.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-107">For example, you can select to show only work-based leads.</span></span>

## <a name="create-a-new-lead-for-a-project-based-deal"></a><span data-ttu-id="6e4dd-108">إنشاء عميل متوقع جديد لصفقة مستندة إلى مشروع</span><span class="sxs-lookup"><span data-stu-id="6e4dd-108">Create a new lead for a project-based deal</span></span>
<span data-ttu-id="6e4dd-109">عند تأهيل العميل المتوقع المستند إلى المشروع، يتم إنشاء فرصة وحساب.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-109">When a project-based lead is qualified, an opportunity and an account are created.</span></span> <span data-ttu-id="6e4dd-110">الفرصة المستندة إلى المشروع هي نقطة البداية لأنشطة متابعة المبيعات في مرحلة "الفرصة".</span><span class="sxs-lookup"><span data-stu-id="6e4dd-110">A project-based opportunity is the starting point for sales pursuit activities in the Opportunity phase.</span></span> <span data-ttu-id="6e4dd-111">تتميز الفرص المستندة إلى المشروع بقدرات فريدة مطلوبة لبيع عمل المشروع.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-111">Project-based opportunities have unique capabilities that are required for selling project work.</span></span> 

<span data-ttu-id="6e4dd-112">وتشتمل هذه القدرات على ما يلي:</span><span class="sxs-lookup"><span data-stu-id="6e4dd-112">These capabilities include:</span></span>

- <span data-ttu-id="6e4dd-113">أسلوبا الفوترة الوقت والمواد والسعر الثابت.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-113">Time and material and fixed price billing methods</span></span>
- <span data-ttu-id="6e4dd-114">قوائم أسعار بتاريخ سريان متعددة للموارد البشرية والمواد والنفقات المستحقة على المشاريع</span><span class="sxs-lookup"><span data-stu-id="6e4dd-114">Multiple date-effective price lists for human resources, material, and expenses that are incurred on projects</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6e4dd-115">بالنسبة لعميل متوقع مؤهَّل لإنشاء فرصة تلقائياً، قم بتعيين السمة **نوع الأمر** إلى **معتمد على العمل** عند إنشاء العميل المتوقع.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-115">For a qualified lead to automatically create an opportunity, set the **Order Type** attribute to **Work based** when you create the lead.</span></span> <span data-ttu-id="6e4dd-116">وإذا اخترت نوعاً مختلفاً، فلن يُنشئ العميل المتوقع فرصة مستندة إلى المشروع عندما يكون مؤهلاً.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-116">If you choose a different type, the lead won't create a project-based opportunity when it is qualified.</span></span> <span data-ttu-id="6e4dd-117">إذا لم يتم إنشاء الفرصة المستندة إلى المشروع، فلن تتوفر القدرات الخاصة بالمشروع في عمليات المبيعات في المراحل النهائية.</span><span class="sxs-lookup"><span data-stu-id="6e4dd-117">If the project-based opportunity isn't created, the project-specific capabilities won't be available in the downstream sales processes.</span></span>


![لقطة شاشة لعلامة التبويب "الملخص" في صفحة "عميل متوقع جديد".](../media/new-lead-ss.png)



