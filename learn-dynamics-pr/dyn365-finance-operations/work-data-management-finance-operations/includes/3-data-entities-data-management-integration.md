---
ms.openlocfilehash: 7783eaf93ee82259e30fec5558eebf54200510bf
ms.sourcegitcommit: e0a1238596690b3b6eedd86c2ac14099948a5e25
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "6072546"
---
<span data-ttu-id="c18bd-101">توفر كيانات البيانات تجريداً مفاهيمياً وتغليفاً (طريقة عرض غير طبيعية) لمخطط الجدول الأساسي الذي يمثل مفاهيم البيانات ووظائفها.</span><span class="sxs-lookup"><span data-stu-id="c18bd-101">Data entities provide conceptual abstraction and encapsulation (de-normalized view) of underlying table schema that represent data concepts and functionalities.</span></span> 

<span data-ttu-id="c18bd-102">بعد إنشاء كيانات البيانات، يجب أن تكون قادراً على إعادة استخدامها لوظائف Excel الإضافية أو الاستيراد والتصدير أو سيناريوهات التكامل.</span><span class="sxs-lookup"><span data-stu-id="c18bd-102">After data entities are created, you should be able to reuse them for Excel add-ins, import and export, or integration scenarios.</span></span> <span data-ttu-id="c18bd-103">كيان البيانات هو تجريد من التنفيذ المادي لجداول قاعدة البيانات.</span><span class="sxs-lookup"><span data-stu-id="c18bd-103">A data entity is an abstraction from the physical implementation of database tables.</span></span> 

<span data-ttu-id="c18bd-104">تقدم هذه الصورة سيناريوهات تكامل كيان البيانات.</span><span class="sxs-lookup"><span data-stu-id="c18bd-104">This image presents data entity integration scenarios.</span></span>

![رسم تخطيطي لسيناريوهات تكامل كيان البيانات.](../media/data-entity.png)

<span data-ttu-id="c18bd-106">على سبيل المثال، في الجداول الموحدة، قد يتم تخزين الكثير من البيانات لكل عميل في جدول عميل، ومن ثم قد يتم توزيع الباقي عبر مجموعة صغيرة من الجداول ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-106">For example, in normalized tables, a lot of the data for each customer might be stored in a customer table, and then the rest might be spread across a small set of related tables.</span></span> <span data-ttu-id="c18bd-107">في هذه الحالة، يظهر كيان البيانات لمفهوم العميل كعرض واحد غير عادي، حيث يحتوي كل صف على جميع البيانات من جدول العميل والجداول المرتبطة به.</span><span class="sxs-lookup"><span data-stu-id="c18bd-107">In this case, the data entity for the customer concept appears as one de-normalized view, in which each row contains all the data from the customer table and its related tables.</span></span> 

<span data-ttu-id="c18bd-108">يقوم كيان البيانات بتغليف مفهوم الأعمال في تنسيق يجعل التطوير والتكامل أسهل.</span><span class="sxs-lookup"><span data-stu-id="c18bd-108">A data entity encapsulates a business concept into a format that makes development and integration easier.</span></span> <span data-ttu-id="c18bd-109">يمكن أن تبسط الطبيعة المجردة لكيان البيانات تطوير التطبيقات وتخصيصها.</span><span class="sxs-lookup"><span data-stu-id="c18bd-109">The abstracted nature of a data entity can simplify application development and customization.</span></span> <span data-ttu-id="c18bd-110">في وقت لاحق، يقوم التجريد أيضاً بعزل كود التطبيق من الاضطراب الحتمي للجداول المادية بين الإصدارات.</span><span class="sxs-lookup"><span data-stu-id="c18bd-110">Later, the abstraction also insulates application code from the inevitable churn of the physical tables between versions.</span></span> 

<span data-ttu-id="c18bd-111">كيان البيانات لديه القدرات التالية:</span><span class="sxs-lookup"><span data-stu-id="c18bd-111">A data entity has the following capabilities:</span></span>

- <span data-ttu-id="c18bd-112">إنه يوفر مكدساً واحداً لالتقاط منطق الأعمال، وتمكين السيناريوهات مثل الاستيراد والتصدير، والتكامل، ودعم المنطق الإضافي عن طريق إضافة رمز للمطور.</span><span class="sxs-lookup"><span data-stu-id="c18bd-112">It provides a single stack to capture business logic, enable scenarios such as import and export, and integration, and support additional logics by a developer adding code.</span></span>
- <span data-ttu-id="c18bd-113">تصبح الآلية الأساسية لتصدير واستيراد حزم البيانات لإدارة دورة حياة التطبيق (ALM) وسيناريوهات البيانات التجريبية.</span><span class="sxs-lookup"><span data-stu-id="c18bd-113">It becomes the primary mechanism for exporting and importing data packages for Application Lifecycle Management (ALM) and demo data scenarios.</span></span>
- <span data-ttu-id="c18bd-114">يمكن الكشف عنها كخدمات OData، ثم استخدامها في سيناريوهات التكامل المتزامن الجدولية وتكاملات Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="c18bd-114">It can be exposed as OData services, and then used in tabular-style synchronous integration scenarios and Microsoft Office integrations.</span></span>

## <a name="entity-example"></a><span data-ttu-id="c18bd-115">مثال على الكيان</span><span class="sxs-lookup"><span data-stu-id="c18bd-115">Entity example</span></span> 

<span data-ttu-id="c18bd-116">يريد المستهلك الوصول إلى البيانات المتعلقة بكائن العميل، ولكن هذه البيانات مبعثرة حالياً عبر عدة جداول موحدة، مثل **DirParty، وCustTable، وLogisticsPostalAddress**، و **LogisticsElectronicAddress**.</span><span class="sxs-lookup"><span data-stu-id="c18bd-116">A consumer wants to access data that is related to a customer object, but this data is currently scattered across multiple normalized tables, such as **DirParty, CustTable, LogisticsPostalAddress**, and **LogisticsElectronicAddress**.</span></span> 

<span data-ttu-id="c18bd-117">لذلك، فإن عملية قراءة وكتابة بيانات العميل مملة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-117">Therefore, the process of reading and writing customer data is tedious.</span></span> <span data-ttu-id="c18bd-118">بدلاً من ذلك، يمكن تصميم كيان العميل التالي لتغليف المخطط المادي الأساسي بأكمله في عرض واحد غير عادي.</span><span class="sxs-lookup"><span data-stu-id="c18bd-118">Instead, the following customer entity can be designed to encapsulate the entire underlying physical schema into a single de-normalized view.</span></span> <span data-ttu-id="c18bd-119">يتيح ذلك عمليات قراءة وكتابة أبسط، كما يتيح تجريد أي تفاعل داخلي بين الجداول.</span><span class="sxs-lookup"><span data-stu-id="c18bd-119">This enables simpler read and write operations, and enables abstraction of any internal interaction between the tables.</span></span>

## <a name="categories-of-entities"></a><span data-ttu-id="c18bd-120">فئات الكيانات</span><span class="sxs-lookup"><span data-stu-id="c18bd-120">Categories of entities</span></span> 

<span data-ttu-id="c18bd-121">يتم تصنيف الكيانات بناءً على وظائفها ونوع البيانات التي تخدمها.</span><span class="sxs-lookup"><span data-stu-id="c18bd-121">Entities are categorized based on their functions and the type of data that they serve.</span></span> <span data-ttu-id="c18bd-122">فيما يلي خمس فئات لكيانات البيانات:</span><span class="sxs-lookup"><span data-stu-id="c18bd-122">The following are five categories for data entities:</span></span>

- <span data-ttu-id="c18bd-123">المعلمات‬</span><span class="sxs-lookup"><span data-stu-id="c18bd-123">Parameters</span></span>
- <span data-ttu-id="c18bd-124">المرجع</span><span class="sxs-lookup"><span data-stu-id="c18bd-124">Reference</span></span>
- <span data-ttu-id="c18bd-125">رئيسي</span><span class="sxs-lookup"><span data-stu-id="c18bd-125">Master</span></span>
- <span data-ttu-id="c18bd-126">المستند</span><span class="sxs-lookup"><span data-stu-id="c18bd-126">Document</span></span>
- <span data-ttu-id="c18bd-127">الحركات</span><span class="sxs-lookup"><span data-stu-id="c18bd-127">Transactions</span></span>

### <a name="parameters"></a><span data-ttu-id="c18bd-128">المعلمات‬</span><span class="sxs-lookup"><span data-stu-id="c18bd-128">Parameters</span></span> 

- <span data-ttu-id="c18bd-129">المعلمات الوظيفية أو السلوكية.</span><span class="sxs-lookup"><span data-stu-id="c18bd-129">Functional or behavioral parameters.</span></span>
- <span data-ttu-id="c18bd-130">مطلوب لإعداد نشر أو وحدة توزيع لإنشاء أو عميل معين.</span><span class="sxs-lookup"><span data-stu-id="c18bd-130">Required to set up a deployment or a module for a specific build or customer.</span></span>
- <span data-ttu-id="c18bd-131">يمكن أن تتضمن بيانات خاصة بصناعة أو أعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-131">Can include data that is specific to an industry or business.</span></span> <span data-ttu-id="c18bd-132">يمكن أن تنطبق البيانات أيضاً على مجموعة أوسع من العملاء.</span><span class="sxs-lookup"><span data-stu-id="c18bd-132">The data can also apply to a broader set of customers.</span></span>
- <span data-ttu-id="c18bd-133">الجداول التي تحتوي على سجل واحد فقط، حيث تكون الأعمدة عبارة عن قيم للإعدادات.</span><span class="sxs-lookup"><span data-stu-id="c18bd-133">Tables that contain only one record, where the columns are values for settings.</span></span> <span data-ttu-id="c18bd-134">توجد أمثلة على هذه الجداول للحسابات الدائنة (AP) ودفتر الأستاذ العام (GL) وخيارات أداء العميل ومهام سير العمل وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="c18bd-134">Examples of such tables exist for Accounts payable (AP), General ledger (GL), client performance options, workflows, and so on.</span></span>

### <a name="reference"></a><span data-ttu-id="c18bd-135">المرجع</span><span class="sxs-lookup"><span data-stu-id="c18bd-135">Reference</span></span> 

- <span data-ttu-id="c18bd-136">بيانات مرجعية بسيطة، بكميات صغيرة، مطلوبة لتشغيل عملية أعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-136">Simple reference data, of small quantity, that is required to operate a business process.</span></span>
- <span data-ttu-id="c18bd-137">البيانات الخاصة بصناعة أو عملية أعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-137">Data that is specific to an industry or a business process.</span></span>
- <span data-ttu-id="c18bd-138">تشمل الأمثلة الوحدات والأبعاد ورموز الضرائب.</span><span class="sxs-lookup"><span data-stu-id="c18bd-138">Examples include units, dimensions, and tax codes.</span></span>


### <a name="master"></a><span data-ttu-id="c18bd-139">رئيسي</span><span class="sxs-lookup"><span data-stu-id="c18bd-139">Master</span></span> 

- <span data-ttu-id="c18bd-140">أصول البيانات الخاصة بالأعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-140">Data assets of the business.</span></span> <span data-ttu-id="c18bd-141">بشكل عام، هذه هي "أسماء" الاعمال، والتي تقع عادةً في فئات مثل الأشخاص والأماكن والمفاهيم.</span><span class="sxs-lookup"><span data-stu-id="c18bd-141">Generally, these are the "nouns" of the business, which typically fall into categories such as people, places, and concepts.</span></span>
- <span data-ttu-id="c18bd-142">بيانات مرجعية معقدة بكميات كبيرة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-142">Complex reference data, of large quantity.</span></span> <span data-ttu-id="c18bd-143">تشمل الأمثلة العملاء والموردين والمشاريع.</span><span class="sxs-lookup"><span data-stu-id="c18bd-143">Examples include customers, vendors, and projects.</span></span>

### <a name="document"></a><span data-ttu-id="c18bd-144">المستند</span><span class="sxs-lookup"><span data-stu-id="c18bd-144">Document</span></span> 

- <span data-ttu-id="c18bd-145">بيانات ورقة العمل التي يتم تحويلها إلى معاملات لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="c18bd-145">Worksheet data that is converted into transactions later.</span></span>
- <span data-ttu-id="c18bd-146">المستندات التي تحتوي على هياكل معقدة، مثل عدة عناصر لكل سجل رأس.</span><span class="sxs-lookup"><span data-stu-id="c18bd-146">Documents that have complex structures, such as several line items for each header record.</span></span> <span data-ttu-id="c18bd-147">تتضمن الأمثلة أوامر المبيعات وأوامر الشراء والأرصدة المفتوحة ودفاتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="c18bd-147">Examples include sales orders, purchase orders, open balances, and journals.</span></span>
- <span data-ttu-id="c18bd-148">البيانات التشغيلية للأعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-148">The operational data of the business.</span></span>

### <a name="transactions"></a><span data-ttu-id="c18bd-149">الحركات</span><span class="sxs-lookup"><span data-stu-id="c18bd-149">Transactions</span></span> 
- <span data-ttu-id="c18bd-150">بيانات الحركات التشغيلية للأعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-150">The operational transaction data of the business.</span></span>
- <span data-ttu-id="c18bd-151">الحركات المُرحّلة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-151">Posted transactions.</span></span> <span data-ttu-id="c18bd-152">هذه عناصر غير ثابتة مثل الفواتير والأرصدة التي تم ترحيلها.</span><span class="sxs-lookup"><span data-stu-id="c18bd-152">These are non-idempotent items such as posted invoices and balances.</span></span> <span data-ttu-id="c18bd-153">عادةً، يتم استبعاد هذه العناصر أثناء نسخ مجموعة البيانات الكاملة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-153">Typically, these items are excluded during a full dataset copy.</span></span>
- <span data-ttu-id="c18bd-154">تشمل الأمثلة الفواتير المعلقة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-154">Examples include pending invoices.</span></span>

## <a name="configuration-keys-and-data-entities"></a><span data-ttu-id="c18bd-155">مفاتيح التكوين وكيانات البيانات</span><span class="sxs-lookup"><span data-stu-id="c18bd-155">Configuration keys and data entities</span></span> 

<span data-ttu-id="c18bd-156">قبل استخدام كيانات البيانات لاستيراد البيانات أو تصديرها، نوصيك أولاً بتحديد تأثير مفاتيح التكوين على كيانات البيانات التي تخطط لاستخدامها.</span><span class="sxs-lookup"><span data-stu-id="c18bd-156">Before you use data entities to import or export data, we recommended that you first determine the impact of configuration keys on the data entities that you are planning to use.</span></span>

<span data-ttu-id="c18bd-157">لمعرفه المزيد حول مفاتيح التكوين في تطبيقات Finance and Operations، راجع [تقرير أكواد الترخيص ومفاتيح التكوين](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/license-codes-configuration-keys-report/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="c18bd-157">To learn more about configuration keys in Finance and Operations apps, refer to the [License codes and configuration keys report](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/license-codes-configuration-keys-report/?azure-portal=true).</span></span>

### <a name="configuration-key-assignments"></a><span data-ttu-id="c18bd-158">تعيينات مفاتيح التكوين</span><span class="sxs-lookup"><span data-stu-id="c18bd-158">Configuration key assignments</span></span> 

<span data-ttu-id="c18bd-159">يمكن تعيين مفاتيح التكوين لواحد أو كل العناصر التالية.</span><span class="sxs-lookup"><span data-stu-id="c18bd-159">Configuration keys can be assigned to one or all of the following artifacts.</span></span>

- <span data-ttu-id="c18bd-160">كيانات البيانات</span><span class="sxs-lookup"><span data-stu-id="c18bd-160">Data entities</span></span>
- <span data-ttu-id="c18bd-161">الجداول المستخدمة كمصادر بيانات</span><span class="sxs-lookup"><span data-stu-id="c18bd-161">Tables used as data sources</span></span>
- <span data-ttu-id="c18bd-162">حقول الجدول</span><span class="sxs-lookup"><span data-stu-id="c18bd-162">Table fields</span></span>
- <span data-ttu-id="c18bd-163">حقول كيانات البيانات</span><span class="sxs-lookup"><span data-stu-id="c18bd-163">Data entity fields</span></span>

## <a name="supported-integrations"></a><span data-ttu-id="c18bd-164">التكاملات المدعومة</span><span class="sxs-lookup"><span data-stu-id="c18bd-164">Supported integrations</span></span> ##

<span data-ttu-id="c18bd-165">يمكن أن تدعم إدارة البيانات باستخدام كيانات البيانات عمليات التكامل التالية:</span><span class="sxs-lookup"><span data-stu-id="c18bd-165">Data management by using data entities can support the following integrations:</span></span>

- <span data-ttu-id="c18bd-166">**الخدمة المتزامنة (OData)** – تعمل كيانات البيانات على تمكين واجهات برمجة التطبيقات العامة (API) على الكيانات ليتم كشفها، مما يتيح الخدمات المتزامنة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-166">**Synchronous service (OData)** – Data entities enable public application programming interfaces (APIs) on entities to be exposed, which enables synchronous services.</span></span> <span data-ttu-id="c18bd-167">تُستخدم هذه الطريقة لتكامل Office وتكاملات تطبيقات الأجهزة المحمولة التابعة لجهات خارجية</span><span class="sxs-lookup"><span data-stu-id="c18bd-167">This method is used for Office integration and third-party mobile app integrations</span></span>
- <span data-ttu-id="c18bd-168">**التكامل غير المتزامن** – تدعم كيانات البيانات أيضاً التكامل غير المتزامن من خلال مسار إدارة البيانات.</span><span class="sxs-lookup"><span data-stu-id="c18bd-168">**Asynchronous integration** – Data entities also support asynchronous integration through a data management pipeline.</span></span> <span data-ttu-id="c18bd-169">يتيح ذلك سيناريوهات إدخال واستخراج البيانات غير المتزامنة وعالية الأداء.</span><span class="sxs-lookup"><span data-stu-id="c18bd-169">This enables asynchronous and high-performing data insertion and extraction scenarios.</span></span> <span data-ttu-id="c18bd-170">تُستخدم هذه الطريقة للاستيراد/التصدير التفاعلي المستند إلى الملف والتكاملات المتكررة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-170">This method is used for interactive file-based import/export and recurring integrations.</span></span>
- <span data-ttu-id="c18bd-171">**ذكاء الأعمال** – باستخدام القياسات الإجمالية المتاحة في تطبيقات Finance and Operations، وعناصر التحكم المضمنة مثل المخططات والتكامل مع Power Platform، يقدم تقارير لتقديم رؤى لبيانات الأعمال.</span><span class="sxs-lookup"><span data-stu-id="c18bd-171">**Business intelligence** – By using the aggregate measures available in Finance and Operations apps, built-in controls such as charts and integration with Power Platform, provides reports to offer insights to business data.</span></span>

## <a name="data-migration-from-legacy-or-external-systems"></a><span data-ttu-id="c18bd-172">ترحيل البيانات من الأنظمة القديمة أو الخارجية</span><span class="sxs-lookup"><span data-stu-id="c18bd-172">Data migration from legacy or external systems</span></span> 

<span data-ttu-id="c18bd-173">بعد أن يبدأ التوزيع الأولي وتشغيله، سيقوم منفذ النظام بترحيل أصول البيانات الحالية للعميل إلى تطبيقات Finance and Operations، مثل:</span><span class="sxs-lookup"><span data-stu-id="c18bd-173">After the initial deployment is up and running, the system implementer will migrate existing data assets of the customer into Finance and Operations apps, such as:</span></span>

- <span data-ttu-id="c18bd-174">البيانات الرئيسية (على سبيل المثال، العملاء والموردون)</span><span class="sxs-lookup"><span data-stu-id="c18bd-174">Master data (for example, customers and vendors)</span></span>
- <span data-ttu-id="c18bd-175">مجموعات فرعية من المستندات (على سبيل المثال، أوامر المبيعات)</span><span class="sxs-lookup"><span data-stu-id="c18bd-175">Subsets of documents (for example, sales orders)</span></span>

<span data-ttu-id="c18bd-176">يمكنك استخدام إطار عمل إدارة البيانات لنسخ التكوينات بين الشركات أو البيئات، وتكوين العمليات أو الوحدات النمطية باستخدام Lifecycle Services ‏(LCS).</span><span class="sxs-lookup"><span data-stu-id="c18bd-176">You can use the data management framework to copy configurations between companies or environments, and configure processes or modules by using Lifecycle Services (LCS).</span></span>

<span data-ttu-id="c18bd-177">يهدف نسخ التكوينات إلى تسهيل بدء تنفيذ جديد، حتى إذا كان فريقك لا يفهم بعمق بنية البيانات التي يجب إدخالها، أو تبعيات البيانات، أو التسلسل لإضافة البيانات إلى التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="c18bd-177">Copying configurations is intended to make it easier to start a new implementation, even if your team doesn't deeply understand the structure of data that needs to be entered, data dependencies, or which sequence to add data to an implementation.</span></span>

<span data-ttu-id="c18bd-178">يتيح لك إطار عمل إدارة البيانات:</span><span class="sxs-lookup"><span data-stu-id="c18bd-178">The data management framework allows you to:</span></span>

<span data-ttu-id="c18bd-179">نقل البيانات بين نظامين متشابهين.</span><span class="sxs-lookup"><span data-stu-id="c18bd-179">Move data between two similar systems.</span></span>
- <span data-ttu-id="c18bd-180">اكتشف الكيانات والتبعيات بين الكيانات لعملية أعمال أو وحدة معينة.</span><span class="sxs-lookup"><span data-stu-id="c18bd-180">Discover entities and dependencies between entities for a given business process or module.</span></span>
- <span data-ttu-id="c18bd-181">الاحتفاظ بمكتبة قابلة لإعادة الاستخدام من قوالب البيانات ومجموعات البيانات.</span><span class="sxs-lookup"><span data-stu-id="c18bd-181">Maintain a reusable library of data templates and datasets.</span></span>
- <span data-ttu-id="c18bd-182">استخدم حزم البيانات لإنشاء كيانات البيانات التزايدية.</span><span class="sxs-lookup"><span data-stu-id="c18bd-182">Use data packages to create incremental data entities.</span></span> <span data-ttu-id="c18bd-183">يمكن ترتيب كيانات البيانات داخل الحزم.</span><span class="sxs-lookup"><span data-stu-id="c18bd-183">Data entities can be sequenced inside the packages.</span></span> <span data-ttu-id="c18bd-184">يمكنك تسمية حزم البيانات، والتي يمكن التعرف عليها بسهولة أثناء الاستيراد أو التصدير.</span><span class="sxs-lookup"><span data-stu-id="c18bd-184">You can name data packages, which can be easily identifiable during import or export.</span></span> <span data-ttu-id="c18bd-185">عند إنشاء حزم البيانات، يمكن تعيين كيانات البيانات إلى جداول مرحلية في شبكات أو باستخدام أداة رسم الخرائط المرئية.</span><span class="sxs-lookup"><span data-stu-id="c18bd-185">When building data packages, data entities can be mapped to staging tables in grids or by using a visual mapping tool.</span></span> <span data-ttu-id="c18bd-186">يمكنك أيضاً سحب الأعمدة وإفلاتها يدوياً.</span><span class="sxs-lookup"><span data-stu-id="c18bd-186">You can also drag-and-drop columns manually.</span></span>
- <span data-ttu-id="c18bd-187">اعرض البيانات أثناء عمليات الاستيراد، حتى تتمكن من مقارنة البيانات والتأكد من صحتها.</span><span class="sxs-lookup"><span data-stu-id="c18bd-187">View data during imports, so you can compare data and ensure that it is valid.</span></span>

