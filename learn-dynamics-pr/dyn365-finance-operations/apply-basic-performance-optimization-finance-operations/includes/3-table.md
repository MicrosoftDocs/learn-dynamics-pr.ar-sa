---
ms.openlocfilehash: 52d011e81aad3fe54ccd734dd337526b2fad91f0
ms.sourcegitcommit: 0af0a6f1739b0e2a5ec60989ffbf8aa131de41c3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/08/2021
ms.locfileid: "6072246"
---

<span data-ttu-id="d5d38-101">تشرح هذه الوحدة الجداول المؤقتة، والأنواع المختلفة للجداول المؤقتة، ومتى يجب استخدامها.</span><span class="sxs-lookup"><span data-stu-id="d5d38-101">This unit explains temporary tables, the different types of temporary tables, and when they should be used.</span></span>

<span data-ttu-id="d5d38-102">تسمح لك الجداول المؤقتة بإنشاء البيانات المؤقتة وتنظيفها بكفاءة.</span><span class="sxs-lookup"><span data-stu-id="d5d38-102">Temporary tables allow you to efficiently create and clean up temporary data.</span></span> <span data-ttu-id="d5d38-103">نوعا الجداول المؤقتة هما:</span><span class="sxs-lookup"><span data-stu-id="d5d38-103">The two types of temporary tables are:</span></span>

-   `InMemory`
-   `TempDB` 

<span data-ttu-id="d5d38-104">يمكن تحديد نوع الجدول في خاصية `TableType` بالجدول.</span><span class="sxs-lookup"><span data-stu-id="d5d38-104">The table type can be determined on the table's `TableType` property.</span></span>

<span data-ttu-id="d5d38-105">[![لقطة شاشة لصفحة جدول الخصائص تُبرز خاصية نوع الجدول.](../media/tables-1.png)](../media/tables-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d5d38-105">[![Screenshot of the Properties table page highlighting the Table Type property.](../media/tables-1.png)](../media/tables-1.png#lightbox)</span></span>


<span data-ttu-id="d5d38-106">تستخدم جداول `InMemory` ملف أسلوب الوصول التسلسلي المفهرس (ISAM) الموجود في طبقة العميل أو طبقة AOS.</span><span class="sxs-lookup"><span data-stu-id="d5d38-106">`InMemory` tables use an indexed sequential access method (ISAM) file that exists on the client tier or the AOS tier.</span></span> <span data-ttu-id="d5d38-107">لا يحتوي Microsoft SQL Server على اتصال بملف ISAM.</span><span class="sxs-lookup"><span data-stu-id="d5d38-107">Microsoft SQL Server has no connection to the ISAM file.</span></span> <span data-ttu-id="d5d38-108">يتم تخزين البيانات في الذاكرة حتى تصل إلى 128 كيلوبايت، ثم تتم كتابة مجموعة البيانات في ملف قرص على طبقة الخادم.</span><span class="sxs-lookup"><span data-stu-id="d5d38-108">The data is stored in memory until it reaches 128 KB, and then the dataset is written to a disk file on the server tier.</span></span> <span data-ttu-id="d5d38-109">يتم إنشاء مثيلات جداول `InMemory` عند إدراج السجل الأول.</span><span class="sxs-lookup"><span data-stu-id="d5d38-109">`InMemory` tables are instantiated when the first record is inserted.</span></span> <span data-ttu-id="d5d38-110">الجدول موجود والذاكرة مخصصة فقط للجدول أثناء وجود مخزن مؤقت للسجل.</span><span class="sxs-lookup"><span data-stu-id="d5d38-110">The table exists and memory is only allocated to the table while a record buffer exists.</span></span> 

<span data-ttu-id="d5d38-111">يمكن استخدام جدول `InMemory` عندما تحتاج إلى تخزين البيانات واستردادها دون كتابة البيانات في قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="d5d38-111">An `InMemory` table might be used when you need to store and retrieve data without writing data to the database.</span></span> <span data-ttu-id="d5d38-112">يشبه هذا الحاوية، ولكن تتيح لك جداول `InMemory` استخدام الفهارس لتسريع استرداد البيانات.</span><span class="sxs-lookup"><span data-stu-id="d5d38-112">This is like a container, but `InMemory` tables allow you to use indexes to speed up data retrieval.</span></span> <span data-ttu-id="d5d38-113">إذا كنت تستخدم عدداً قليلاً من السجلات، فيجب عليك استخدام حاوية، وليس جدول `InMemory`.</span><span class="sxs-lookup"><span data-stu-id="d5d38-113">If you are only using a few records, you should use a container, not an `InMemory` table.</span></span> <span data-ttu-id="d5d38-114">يمكنك استخدام بنية X++ SQL للانضمام إلى جدول `InMemory`، ومع ذلك، عادةً ما تكون عمليات الربط وعمليات SQL غير فعالة.</span><span class="sxs-lookup"><span data-stu-id="d5d38-114">You can use X++ SQL syntax to join an `InMemory` table, however, joins and SQL operations are usually inefficient.</span></span>

<span data-ttu-id="d5d38-115">جداول `TempDB` تستخدم قاعدة بيانات `TempDB` لـ SQL Server.</span><span class="sxs-lookup"><span data-stu-id="d5d38-115">`TempDB` tables use the `TempDB` database of the SQL Server.</span></span> <span data-ttu-id="d5d38-116">يتسبب هذا النوع من الجدول في إزالة البيانات عند عدم استخدامها بواسطة الطريقة الحالية أو عند إعادة تشغيل النظام.</span><span class="sxs-lookup"><span data-stu-id="d5d38-116">This type of table causes the data to be removed when it is no longer used by the current method or when the system is restarted.</span></span> <span data-ttu-id="d5d38-117">يتم تحويل الجداول العادية تلقائياً إلى جداول `TempDB` عن طريق تعطيل مفتاح التكوين للجدول، مما يسمح للمراجع إلى الجدول المعطل في النظام بالاستمرار في التجميع والتشغيل.</span><span class="sxs-lookup"><span data-stu-id="d5d38-117">Regular tables are automatically turned into `TempDB` tables by disabling the configuration key for the table, which allows references to the disabled table in the system to continue to compile and run.</span></span>
<span data-ttu-id="d5d38-118">بالإضافة إلى ذلك، تُستخدم جداول `TempDB` بشكل شائع في التقارير لمعالجة البيانات.</span><span class="sxs-lookup"><span data-stu-id="d5d38-118">Additionally, `TempDB` tables are commonly used on reports to manipulate data.</span></span>

<span data-ttu-id="d5d38-119">تتضمن إمكانات جداول `TempDB` ما يلي:</span><span class="sxs-lookup"><span data-stu-id="d5d38-119">The capabilities of `TempDB` tables include the following:</span></span>

-   <span data-ttu-id="d5d38-120">الانضمام إلى الجداول العادية.</span><span class="sxs-lookup"><span data-stu-id="d5d38-120">Joining to regular tables.</span></span>
-   <span data-ttu-id="d5d38-121">استخدام المفاتيح الخارجية.</span><span class="sxs-lookup"><span data-stu-id="d5d38-121">Using foreign keys.</span></span>
-   <span data-ttu-id="d5d38-122">أن تكون لكل شركة أو عالمية.</span><span class="sxs-lookup"><span data-stu-id="d5d38-122">Being per company or global.</span></span>
-   <span data-ttu-id="d5d38-123">الاحتواء على الفهارس.</span><span class="sxs-lookup"><span data-stu-id="d5d38-123">Having indexes.</span></span>
-   <span data-ttu-id="d5d38-124">وجود الأساليب ولكن مع عدم القدرة على تجاوز الأساليب.</span><span class="sxs-lookup"><span data-stu-id="d5d38-124">Having methods but an inability to override the methods.</span></span>
-   <span data-ttu-id="d5d38-125">إنشاء مثيل من العميل أو مستوى الخادم.</span><span class="sxs-lookup"><span data-stu-id="d5d38-125">Instantiating from the client or server tier.</span></span>
-   <span data-ttu-id="d5d38-126">قيد الاستخدام كاستعلام.</span><span class="sxs-lookup"><span data-stu-id="d5d38-126">Being used as a query.</span></span>
-   <span data-ttu-id="d5d38-127">عدم وجود متطلبات لمفتاح التكوين.</span><span class="sxs-lookup"><span data-stu-id="d5d38-127">Having no requirements for a configuration key.</span></span>

<span data-ttu-id="d5d38-128">تحتوي جداول `TempDB` على القيود التالية أيضاً:</span><span class="sxs-lookup"><span data-stu-id="d5d38-128">`TempDB` tables also have the following limitations:</span></span>

-   <span data-ttu-id="d5d38-129">عدم القدرة على إدارة بيانات التاريخ الفعلي.</span><span class="sxs-lookup"><span data-stu-id="d5d38-129">Inability to manage date-effective data.</span></span>
-   <span data-ttu-id="d5d38-130">لا تحتوي على إجراءات حذف.</span><span class="sxs-lookup"><span data-stu-id="d5d38-130">They do not contain delete actions.</span></span>
-   <span data-ttu-id="d5d38-131">لا يتم تطبيق أمان مستوى السجل.</span><span class="sxs-lookup"><span data-stu-id="d5d38-131">Record Level Security does not apply.</span></span>
-   <span data-ttu-id="d5d38-132">لا يمكنك استخدامها في طرق العرض.</span><span class="sxs-lookup"><span data-stu-id="d5d38-132">You cannot use them in views.</span></span>
