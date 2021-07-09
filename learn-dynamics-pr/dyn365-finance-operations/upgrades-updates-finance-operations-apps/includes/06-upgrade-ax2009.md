---
ms.openlocfilehash: a63741276f77ec870c92981235d971d322c055a2
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071303"
---
<span data-ttu-id="3ed2c-101">باستخدام أداة ترحيل يمكنك تثبيتها في AX ‏2009، يمكنك ترحيل البيانات من AX ‏2009 دون ترقية كاملة للبيانات.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-101">By using a migration tool that you can install in AX 2009, you can migrate data from AX 2009 without doing a full data upgrade.</span></span> <span data-ttu-id="3ed2c-102">وتتيح لك هذه الأداة تصدير البيانات من AX ‏2009 بالتنسيق الخاص بـ Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-102">This tool allows you to export data from AX 2009 in the format for Finance and Operations.</span></span> 

<span data-ttu-id="3ed2c-103">وتتمثل الخطوات الرئيسية لترحيل AX ‏2009 في:</span><span class="sxs-lookup"><span data-stu-id="3ed2c-103">The main steps for the AX 2009 migration are:</span></span> 

1.  <span data-ttu-id="3ed2c-104">إنشاء مخطط في Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-104">Create a schema in Finance and Operations.</span></span>
2.  <span data-ttu-id="3ed2c-105">تثبيت أداة الترحيل في AX ‏2009.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-105">Install the migration tool in AX 2009.</span></span> 
3.  <span data-ttu-id="3ed2c-106">التكوين في AX ‏2009.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-106">Configure in AX 2009.</span></span>
4.  <span data-ttu-id="3ed2c-107">تصدير البيانات من AX ‏2009.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-107">Export data from AX 2009.</span></span>
5.  <span data-ttu-id="3ed2c-108">استيراد البيانات إلى Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-108">Import data to Finance and Operations.</span></span>
6.  <span data-ttu-id="3ed2c-109">المعالجة في Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-109">Process in Finance and Operations.</span></span>

<span data-ttu-id="3ed2c-110">لبدء عملية الترحيل، يجب الحصول على حق الوصول إلى أداة الترحيل من خلال التسجيل في [Microsoft.qualtrics.com](https://microsoft.qualtrics.com/jfe/form/SV_brOLCioQ7mmeykB/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="3ed2c-110">To get started with the migration process, you must gain access to the migration tool by registering at [Microsoft.qualtrics.com](https://microsoft.qualtrics.com/jfe/form/SV_brOLCioQ7mmeykB/?azure-portal=true).</span></span> <span data-ttu-id="3ed2c-111">يحتوي الملف المضغوط على تغييرات X + +‎ وحزم MSI لتثبيت الخدمات.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-111">The zip file includes X++ changes and MSI packages to install services.</span></span> <span data-ttu-id="3ed2c-112">تقدم مجموعة Yammer الخاصة تعليمات فيديو حول كيفية استخدام الأداة.</span><span class="sxs-lookup"><span data-stu-id="3ed2c-112">The private Yammer group provides video instructions on how to use the tool.</span></span>

<span data-ttu-id="3ed2c-113">وتتضمن أداة الترحيل هذه الميزات الآتية:</span><span class="sxs-lookup"><span data-stu-id="3ed2c-113">This migration tool includes the following features:</span></span> 

-   <span data-ttu-id="3ed2c-114">تكوين النظام - التسلسلات الرقمية والمستخدمون ومجموعات المستخدمين والأمان وما إلى ذلك</span><span class="sxs-lookup"><span data-stu-id="3ed2c-114">System configuration - Number sequences, users, user groups, security, and so on</span></span> 
-   <span data-ttu-id="3ed2c-115">التكوين والإعداد - دفتر الأستاذ ومجموعات العملاء ومجموعات الموردين وما إلى ذلك</span><span class="sxs-lookup"><span data-stu-id="3ed2c-115">Configuration and setup - Ledger, customer groups, vendor groups, and so on</span></span> 
-   <span data-ttu-id="3ed2c-116">البيانات الرئيسية – العميل والمورد والمشاريع والحسابات وما إلى ذلك</span><span class="sxs-lookup"><span data-stu-id="3ed2c-116">Master data – Customer, vendor, projects, accounts, and so on</span></span> 
-   <span data-ttu-id="3ed2c-117">الأرصدة – أرصدة دفتر الأستاذ والمخزون والأسعار وما إلى ذلك</span><span class="sxs-lookup"><span data-stu-id="3ed2c-117">Balances – Ledger balances, stock, prices, and so on</span></span> 
-   <span data-ttu-id="3ed2c-118">فتح المستندات والفواتير المعلقة وأوامر المبيعات وأوامر الشراء وفواتير الحسابات المدينة وما إلى ذلك</span><span class="sxs-lookup"><span data-stu-id="3ed2c-118">Open documents, pending invoices, sales orders, purchase orders, AR invoices, and so on</span></span> 
-   <span data-ttu-id="3ed2c-119">أي شيء له كيان (وبشكل أمثل، ليست الحركات التاريخية)</span><span class="sxs-lookup"><span data-stu-id="3ed2c-119">Anything that has an entity (ideally not historical transactions)</span></span> 
-   <span data-ttu-id="3ed2c-120">القدرة على إنشاء حقول مخصصة في Finance and Operations لتوفيرها للترحيل</span><span class="sxs-lookup"><span data-stu-id="3ed2c-120">Ability to create custom fields in Finance and Operations to make them available for migration</span></span>
-   <span data-ttu-id="3ed2c-121">يوفر منطق AX ‏2009 التحويل للتغييرات الرئيسية مثل الأبعاد</span><span class="sxs-lookup"><span data-stu-id="3ed2c-121">AX 2009 logic provides transformation for major changes such as dimensions</span></span> 
-   <span data-ttu-id="3ed2c-122">تسمح لك المعالجة في Finance and Operations بتحويل قيم الحقل</span><span class="sxs-lookup"><span data-stu-id="3ed2c-122">Processing in Finance and Operations allows you to convert field values</span></span> 
-   <span data-ttu-id="3ed2c-123">يمكنك إعادة تشغيل عمليات التصدير والاستيراد نفسها دون تكرار البيانات (سيتم تحديث البيانات الموجودة)</span><span class="sxs-lookup"><span data-stu-id="3ed2c-123">You can re-run the same exports and imports without duplicating data (it will update existing data)</span></span> 
-   <span data-ttu-id="3ed2c-124">يمكنك إعادة تشغيل عملية Finance and Operations، والتي يمكنك تكرارها دون الرجوع إلى AX‏ 2009</span><span class="sxs-lookup"><span data-stu-id="3ed2c-124">You can re-run the Finance and Operations process, which you can iterate quickly without going back to AX 2009</span></span> 

<span data-ttu-id="3ed2c-125">تتكون عملية الترحيل من المهام الآتية:</span><span class="sxs-lookup"><span data-stu-id="3ed2c-125">The migration process consists of the following tasks:</span></span>

1.  <span data-ttu-id="3ed2c-126">**تحليل** البيانات التي يجب ترحيلها</span><span class="sxs-lookup"><span data-stu-id="3ed2c-126">**Analyze** data that needs to be migrated</span></span> 
2.  <span data-ttu-id="3ed2c-127">**المعالجة المسبقة**، توفير البيانات المفقودة والتنظيف والدمج</span><span class="sxs-lookup"><span data-stu-id="3ed2c-127">**Pre-process**, provide missing data, clean, and merge</span></span> 
3.  <span data-ttu-id="3ed2c-128">**الاستخراج** من المصدر إلى حزمة البيانات</span><span class="sxs-lookup"><span data-stu-id="3ed2c-128">**Extract** from source to data package</span></span> 
4.  <span data-ttu-id="3ed2c-129">**تحميل الحزمة** إلى المنطقة **المرحلية** في Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="3ed2c-129">**Load package** to **Staging** area in Finance and Operations</span></span> 
5.  <span data-ttu-id="3ed2c-130">**التحقق** والتنظيف والتحويل</span><span class="sxs-lookup"><span data-stu-id="3ed2c-130">**Validate**, clean, and transform</span></span> 
6.  <span data-ttu-id="3ed2c-131">**الدفع** من المرحلة إلى الهدف</span><span class="sxs-lookup"><span data-stu-id="3ed2c-131">**Push** from stage to target</span></span>
7.  <span data-ttu-id="3ed2c-132">**التحقق** من الهدف</span><span class="sxs-lookup"><span data-stu-id="3ed2c-132">**Validate** target</span></span> 



