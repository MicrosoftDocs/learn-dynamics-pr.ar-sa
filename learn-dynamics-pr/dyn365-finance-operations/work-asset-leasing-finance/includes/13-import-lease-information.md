---
ms.openlocfilehash: 564528f54bd93cac4216d216aae209787590adb2
ms.sourcegitcommit: 3b7930e46f1a732939d8d75f99df7bf1f7ccc2ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "6072361"
---
<span data-ttu-id="31c06-101">يسمح لك إطار عمل استيراد الإيجار ضبط عدة تأجيرات في خطوة واحدة، وتوفير الوقت وتقليل فرص حدوث الخطأ البشري.</span><span class="sxs-lookup"><span data-stu-id="31c06-101">The Lease import framework allows you to adjust multiple leases in one step, saving time and reducing the chance of human error.</span></span> <span data-ttu-id="31c06-102">يمكن لهذه القدرة توصيل Finance بوحدات بيانات خارجية للمساعدة في تحميل البيانات بكفاءة.</span><span class="sxs-lookup"><span data-stu-id="31c06-102">This capability can connect Finance with external data entities to help efficiently upload data.</span></span> <span data-ttu-id="31c06-103">يمكنك استخدام عملية الاستيراد لتسوية الإيجار أو تحديث المعلومات غير المالية أو إضافة تأجيرات جديدة.</span><span class="sxs-lookup"><span data-stu-id="31c06-103">You can use the import process to adjust a lease, update non-financial information, or add new leases.</span></span> <span data-ttu-id="31c06-104">يمكنك عرض بيانات الإيجار وتحريرها قبل استيرادها.</span><span class="sxs-lookup"><span data-stu-id="31c06-104">You can view and edit the leasing data before you import it.</span></span>
## <a name="lease-import-setup"></a><span data-ttu-id="31c06-105">إعداد استيراد الإيجار</span><span class="sxs-lookup"><span data-stu-id="31c06-105">Lease import setup</span></span>
<span data-ttu-id="31c06-106">اتبع الخطوات التالية لإنشاء الاستيراد:</span><span class="sxs-lookup"><span data-stu-id="31c06-106">Follow these steps to create the import:</span></span>

1.  <span data-ttu-id="31c06-107">قم بإنشاء قالب للاستيراد باستخدام مساحة عمل **إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="31c06-107">Create a template for the import by using the **Data management** workspace.</span></span>
2.  <span data-ttu-id="31c06-108">في مساحة عمل **إدارة البيانات**، قم بتصدير كيانات البيانات **التقسيم المرحلي للتأجير والتقسيم المرحلي لعقد الدفع** و **التقسيم المرحلي للعقد التنفيذي** وقم بإجراء التحديثات للقالب.</span><span class="sxs-lookup"><span data-stu-id="31c06-108">In the **Data Management** workspace, export the **Lease staging, Payment contract staging**, and **Executory contract staging** data entities and make the updates to the template.</span></span>
3.  <span data-ttu-id="31c06-109">انتقل إلى **تأجير الأصل > إطار عمل استيراد عقد الإيجار > رأس الاستيراد**.</span><span class="sxs-lookup"><span data-stu-id="31c06-109">Go to **Asset leasing > Lease import framework > Import header**.</span></span> 

    <span data-ttu-id="31c06-110">ستسرد هذه الصفحة كيانات البيانات الثلاثة.</span><span class="sxs-lookup"><span data-stu-id="31c06-110">This page will list the three data entities.</span></span>

4.  <span data-ttu-id="31c06-111">لعرض البيانات المرحلية، قبل تشغيل العملية، حدد خيار **بيانات التشغيل المرحلي** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="31c06-111">To view the staging data, prior to the process being run, select the **Staging data** option in the Action Pane.</span></span>
5.  <span data-ttu-id="31c06-112">من صفحة **بيانات التشغيل المرحلي**، لديك خيارات للقيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="31c06-112">From the **Staging data** page, you have options to:</span></span>

    - <span data-ttu-id="31c06-113">**مراجعة الاختلافات في البيانات** - عرض الاختلافات بين الموجود حاليا في النظام وما هو موجود في جداول التشغيل المرحلي.</span><span class="sxs-lookup"><span data-stu-id="31c06-113">**See differences in data** - View the differences between what is currently in the system and what is in the staging tables.</span></span> 
    - <span data-ttu-id="31c06-114">**التحقق من صحة بيانات الاستيراد** -يقوم النظام بتشغيل العديد من عمليات التحقق للتأكد من أنه سيتم استيراد السجل بنجاح.</span><span class="sxs-lookup"><span data-stu-id="31c06-114">**Validate the import data** - The system runs several validations to ensure that the record will be successfully imported.</span></span>
    - <span data-ttu-id="31c06-115">**ترحيل سجلات عقد الإيجار** - لمعالجة عقد إيجار فردي، حدد **ترحيل سجلات عقد الإيجار** في صفحة **رأس الاستيراد**.</span><span class="sxs-lookup"><span data-stu-id="31c06-115">**Migrate lease records** - To process an individual lease, select **Migrate lease records** on the **Import header** page.</span></span> <span data-ttu-id="31c06-116">عند ترحيل عقد الإيجار، يقوم النظام بتنفيذ الإجراء المحدد في الحقل **نوع العملية**.</span><span class="sxs-lookup"><span data-stu-id="31c06-116">When a lease is migrated, the system performs the action that is specified in the **Process type** field.</span></span>
    - <span data-ttu-id="31c06-117">**تشغيل تقارير المقارنة والفرق** - لمقارنة سجل إيجار فردي، حدد عقد إيجار ثم حدد **مقارنة**.</span><span class="sxs-lookup"><span data-stu-id="31c06-117">**Run the Compare and Difference reports** - To compare an individual lease record, select a lease and then select **Compare**.</span></span> <span data-ttu-id="31c06-118">يجب عليك إكمال هذه الخطوة لإنشاء تقرير **فروق** قبل ترحيل سجلات عقد الإيجار.</span><span class="sxs-lookup"><span data-stu-id="31c06-118">You should complete this step to generate a **Differences** report before you migrate the lease records.</span></span> 

## <a name="set-up-update-fields"></a><span data-ttu-id="31c06-119">إعداد تحديث الحقول</span><span class="sxs-lookup"><span data-stu-id="31c06-119">Set up update fields</span></span>
<span data-ttu-id="31c06-120">قبل استخدام إطار عمل استيراد الإيجار لتحديث الإيجارات، تأكد من تعريف الحقول لعملية الاستيراد في القسم **تأجير الأصل > إطار عمل استيراد عقد الإيجار > الإعداد > تحديث الحقول**.</span><span class="sxs-lookup"><span data-stu-id="31c06-120">Prior to using the Lease import framework to update leases, make sure that you define fields for the import in the **Asset leasing > Lease import framework > Setup > Update fields** section.</span></span> <span data-ttu-id="31c06-121">تسمح لك هذه الصفحة بتحديد الحقل الذي ستقوم بتحديثه في الإيجار.</span><span class="sxs-lookup"><span data-stu-id="31c06-121">This page allows you to select the field that you will be updating on the lease.</span></span>
<span data-ttu-id="31c06-122">أسماء الجداول التي يمكنك تحديدها لعمليه الاستيراد هي:</span><span class="sxs-lookup"><span data-stu-id="31c06-122">The table names that you can select for the import are:</span></span>

- <span data-ttu-id="31c06-123">تفاصيل عقد الإيجار</span><span class="sxs-lookup"><span data-stu-id="31c06-123">Lease details</span></span>
- <span data-ttu-id="31c06-124">عقد جدول الدفع</span><span class="sxs-lookup"><span data-stu-id="31c06-124">Payment schedule contract</span></span>
- <span data-ttu-id="31c06-125">عقد تكلفة تنفيذ العقد</span><span class="sxs-lookup"><span data-stu-id="31c06-125">Executory cost contact</span></span>


<span data-ttu-id="31c06-126">بعد تحديد اسم الجدول الذي ستقوم بتحديثه، سيتم عرض قائمة بالحقول المراد إضافتها إلى استيراد التحديث.</span><span class="sxs-lookup"><span data-stu-id="31c06-126">After you have selected the table name that you will be updating, you will be presented with a list of fields to add to your update import.</span></span> <span data-ttu-id="31c06-127">قم بإضافة حقل من القائمة **الحقول المتوفرة**، وحدد **السهم الأيمن** لإضافتها إلى قائمة **الحقول المحددة**.</span><span class="sxs-lookup"><span data-stu-id="31c06-127">Select the field in the **Available fields** list, and then select the **right arrow** to add them to the **Selected fields** list.</span></span>

![لقطة شاشة لصفحة إعداد تحديد تحديث الإيجار.](../media/update-lease-selection-setup.png)


