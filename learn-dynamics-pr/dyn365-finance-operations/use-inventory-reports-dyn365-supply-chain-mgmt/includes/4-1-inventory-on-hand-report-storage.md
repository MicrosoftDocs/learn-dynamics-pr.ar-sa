---
ms.openlocfilehash: 3945f1485e2ce2999de52ca048cbcd5bf5d8c643
ms.sourcegitcommit: 3222998e8b78a03b9e1ee526c0b3c970f92c86d2
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/11/2021
ms.locfileid: "6073639"
---
<span data-ttu-id="a04da-101">يُعد خيار إنشاء تقرير المخزون المتاح مفيداً في الحالات التي تحتوي فيها المخرجات على عدد كبير من بنود المخزون.</span><span class="sxs-lookup"><span data-stu-id="a04da-101">The option of generating an on-hand inventory report is beneficial in cases where the output contains many inventory lines.</span></span> 

<span data-ttu-id="a04da-102">على سبيل المثال، قد يؤدي طلب المخزون المتاح حسب الصنف والموقع والمستودع في سيناريو يتضمن 50,000 صنف و300 متجر إلى الحصول على تقرير طويل، مما يجعل مراجعة البيانات صعبة.</span><span class="sxs-lookup"><span data-stu-id="a04da-102">For example, requesting the on-hand inventory by item, site, and warehouse in a scenario for 50,000 items and 300 stores would yield a long report, making the data difficult to review.</span></span> <span data-ttu-id="a04da-103">تؤدي القدرة على فرز النتائج وتصفيتها في التطبيق أو تصدير النتائج إلى نظام خارجي إلى جعل التنقل في تقرير المخزون المتاح أسرع وأسهل.</span><span class="sxs-lookup"><span data-stu-id="a04da-103">The ability to sort and filter the results in the application or export the results to an external system makes the on-hand inventory report faster and easier to navigate.</span></span>

## <a name="define-report-parameters"></a><span data-ttu-id="a04da-104">تعريف معلمات التقرير</span><span class="sxs-lookup"><span data-stu-id="a04da-104">Define report parameters</span></span>
<span data-ttu-id="a04da-105">عندما تنشئ تقريراً باستخدام ميزة تخزين تقارير المخزون المتاح، ستتم مطالبتك بتحديد اسم فريد للتقرير، ثم يتم تخزين التقرير الذي أنشأته بهذا الاسم.</span><span class="sxs-lookup"><span data-stu-id="a04da-105">When you generate a report using the Inventory on-hand report storage feature, you'll be asked to specify a unique name for the report, and then the generated report is stored under this name.</span></span> <span data-ttu-id="a04da-106">يمكنك أيضاً تعريف الحقول التي ترغب في عرضها في التقرير.</span><span class="sxs-lookup"><span data-stu-id="a04da-106">You can also define the fields that you want to be displayed on the report.</span></span>

<span data-ttu-id="a04da-107">لإنشاء تقرير حول تخزين تقارير المخزون المتاح، نفّذ الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="a04da-107">To create an Inventory on-hand report storage report, perform the following steps.</span></span>

1.  <span data-ttu-id="a04da-108">في **إدارة المخزون > الاستعلامات والتقارير > التقارير المتاحة > تخزين تقارير المخزون المتاح**، حدد **جديد**.</span><span class="sxs-lookup"><span data-stu-id="a04da-108">In **Inventory management > Inquiries and reports > On-hand reports > Inventory on-hand report storage**, select **New**.</span></span>
2.  <span data-ttu-id="a04da-109">على علامة التبويب السريعة **المعلمات**، في قسم **معرف العملية**، أدخل اسماً فريداً للتقرير في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="a04da-109">In the **Parameters** FastTab in the **Process identifier** section, give the report a unique name in the **Name** field.</span></span>
3.  <span data-ttu-id="a04da-110">في القسم **عرض**، بدّل جميع الحقول التي تريد عرضها على التقرير إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="a04da-110">In the **View** section, toggle all fields you want to display on the report to **Yes**.</span></span>
4.  <span data-ttu-id="a04da-111">على علامة التبويب السريعة **السجلات المطلوب تضمينها**، يمكنك إضافة المزيد من معايير البحث عن طريق تحديد أيقونة **عامل التصفية**.</span><span class="sxs-lookup"><span data-stu-id="a04da-111">In the **Records to include** FastTab, you can add more search criteria by selecting the **Filter** icon.</span></span>
5.  <span data-ttu-id="a04da-112">حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a04da-112">Select **OK**.</span></span>

    ![لقطة شاشة تُظهر معلمات التقرير حول تخزين تقارير المخزون المتاح.](../media/inventory-on-hand-report-storage-parameters-ss.png)
 
6.  <span data-ttu-id="a04da-114">تظهر رسالة تشير إلى إضافة التقرير إلى قائمة انتظار الدُفعات، مما يعني أن التقرير يعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="a04da-114">A message appears stating that the report is added to the batch queue, which means that the report runs in the background.</span></span>
 
    ![لقطة شاشة تُظهر رسالة قائمة انتظار الدُفعات.](../media/batch-queue-message-ss.png)

7.  <span data-ttu-id="a04da-116">عند انتهاء الوظيفة الدفعية، سترى التقرير في صفحة **تخزين تقارير المخزون المتاح**، مع خيار تحديد **عرض تفاصيل التقرير**.</span><span class="sxs-lookup"><span data-stu-id="a04da-116">When the batch job is finished, you see the report on the **Inventory on-hand report storage** page, with the option to select **View details of the report**.</span></span>

<span data-ttu-id="a04da-117">تساعد ميزة تخزين تقارير المخزون المتاح على إزالة الحاجة إلى تشغيل تقارير متعددة للمخزون المتاح للفترة نفسها.</span><span class="sxs-lookup"><span data-stu-id="a04da-117">The Inventory on-hand report storage feature eliminates the need for running multiple on-hand inventory reports for the same period.</span></span> <span data-ttu-id="a04da-118">يتم تخزين التقارير حول تخزين تقارير المخزون المتاح في كيان بيانات جديد، مما يسمح لك بتصدير مخرجات أي تقرير مخزون متاح معين مسمى إلى أي تنسيق تدعمه إدارة البيانات.</span><span class="sxs-lookup"><span data-stu-id="a04da-118">The Inventory on-hand report storage reports are stored in a new data entity, enabling you to export the output of any specific, named inventory on-hand report to any format supported by data management.</span></span>

