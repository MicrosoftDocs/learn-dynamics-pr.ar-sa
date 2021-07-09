---
ms.openlocfilehash: 7905b82fd4914134c0d25f3089a2384cc4b6a20f
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071999"
---
<span data-ttu-id="5f342-101">غالباً ما يكون لدى البلدان والمناطق المختلفة متطلبات قانونية فيما يتعلق بتنسيق المستندات الإلكترونية الواردة والصادرة.</span><span class="sxs-lookup"><span data-stu-id="5f342-101">Often, different countries and regions have legal requirements regarding the format for incoming and outgoing electronic documents.</span></span> <span data-ttu-id="5f342-102">تقوم وظيفة التقارير الإلكترونية (ER) بإدارة تلك التنسيقات خلال دورة حياتها.</span><span class="sxs-lookup"><span data-stu-id="5f342-102">The Electronic reporting (ER) functionality manages those formats during their life cycle.</span></span> <span data-ttu-id="5f342-103">بالإضافة إلى ذلك، فإن التغييرات العادية المحتملة في المتطلبات من قبل الهيئات الحكومية أو البنوك تعني أنه يجب تحديث مستندات العمل وفقاً لذلك.</span><span class="sxs-lookup"><span data-stu-id="5f342-103">Additionally, potential regular requirement changes by government bodies or banks mean that business documents must be updated accordingly.</span></span>

<span data-ttu-id="5f342-104">وظيفة إعداد التقارير الإلكترونية مخصصة لمستخدمي الأعمال المتقدمين لأنها مسألة تكوين وليست رمزاً للحفاظ على تنسيقات المستندات الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="5f342-104">The ER reporting functionality is intended for advanced business users because it is a matter of configuration and not code to maintain formats for electronic documents.</span></span>

<span data-ttu-id="5f342-105">يوضح القسم التالي محرك التقارير الإلكترونية من مستوى عالٍ.</span><span class="sxs-lookup"><span data-stu-id="5f342-105">The following section explains the ER engine from a high level.</span></span>

## <a name="capabilities"></a><span data-ttu-id="5f342-106">القدرات</span><span class="sxs-lookup"><span data-stu-id="5f342-106">Capabilities</span></span>

<span data-ttu-id="5f342-107">توفر وظيفة التقارير الإلكترونية الإمكانات التالية:</span><span class="sxs-lookup"><span data-stu-id="5f342-107">ER functionality provides the following capabilities:</span></span>

- <span data-ttu-id="5f342-108">إنها أداة واحدة للتقارير الإلكترونية وهي مصدر واحد لما كان سابقاً 20 محركاً مختلفاً كان يقوم بإعداد التقارير الإلكترونية.</span><span class="sxs-lookup"><span data-stu-id="5f342-108">It is a single tool for electronic reporting and is a single source for what was previously 20 different engines that performed electronic reporting.</span></span>
- <span data-ttu-id="5f342-109">ينطبق التنسيق على إصدارات مختلفة.</span><span class="sxs-lookup"><span data-stu-id="5f342-109">The format is applicable for different versions.</span></span>
- <span data-ttu-id="5f342-110">يمكن إنشاء تنسيق مخصص يستند إلى تنسيق آخر.</span><span class="sxs-lookup"><span data-stu-id="5f342-110">A custom format can be created that is based on another format.</span></span> <span data-ttu-id="5f342-111">ستقوم وظيفة التقارير الإلكترونية بترقية التنسيق المخصص تلقائياً عند تغيير التنسيق الأصلي.</span><span class="sxs-lookup"><span data-stu-id="5f342-111">ER functionality will automatically upgrade the custom format when the original one is changed.</span></span>
- <span data-ttu-id="5f342-112">إنها الأداة القياسية الأساسية لدعم الترجمة.</span><span class="sxs-lookup"><span data-stu-id="5f342-112">It is the primary standard tool to support localization.</span></span>
- <span data-ttu-id="5f342-113">يمكن توزيع التنسيقات من خلال Microsoft Dynamics Lifecycle Services (LCS)‎.</span><span class="sxs-lookup"><span data-stu-id="5f342-113">Formats can be distributed through Microsoft Dynamics Lifecycle Services (LCS).</span></span>

<span data-ttu-id="5f342-114">لمزيد من المعلومات الفنية حول مواضيع التقارير الإلكترونية التالية، انتقل إلى [نظرة عامة على التقارير الإلكترونية (ER)](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/analytics/general-electronic-reporting?toc=/dynamics365/commerce/toc.json/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="5f342-114">For more technical information on the following electronic reporting topics, go to [Electronic reporting (ER) overview](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/analytics/general-electronic-reporting?toc=/dynamics365/commerce/toc.json/?azure-portal=true).</span></span>

- <span data-ttu-id="5f342-115">نماذج البيانات ومكونات تعيين النماذج</span><span class="sxs-lookup"><span data-stu-id="5f342-115">Data models and model-mapping components</span></span>
- <span data-ttu-id="5f342-116">مكونات التنسيق للمستندات الإلكترونية الصادرة</span><span class="sxs-lookup"><span data-stu-id="5f342-116">Format components for outgoing electronic documents</span></span>
- <span data-ttu-id="5f342-117">مكونات التنسيق للمستندات الإلكترونية الواردة</span><span class="sxs-lookup"><span data-stu-id="5f342-117">Format components for incoming electronic documents</span></span>
- <span data-ttu-id="5f342-118">إصدار المكونات</span><span class="sxs-lookup"><span data-stu-id="5f342-118">Component versioning</span></span>
- <span data-ttu-id="5f342-119">فعالية تاريخ المكون</span><span class="sxs-lookup"><span data-stu-id="5f342-119">Component date effectivity</span></span>
- <span data-ttu-id="5f342-120">الوصول إلى المكون</span><span class="sxs-lookup"><span data-stu-id="5f342-120">Component access</span></span>
- <span data-ttu-id="5f342-121">التكوين</span><span class="sxs-lookup"><span data-stu-id="5f342-121">Configuration</span></span>
- <span data-ttu-id="5f342-122">الموفر</span><span class="sxs-lookup"><span data-stu-id="5f342-122">Provider</span></span>
- <span data-ttu-id="5f342-123">المستودع</span><span class="sxs-lookup"><span data-stu-id="5f342-123">Repository</span></span>
- <span data-ttu-id="5f342-124">السيناريوهات المدعومة</span><span class="sxs-lookup"><span data-stu-id="5f342-124">Supported scenarios</span></span>
- <span data-ttu-id="5f342-125">معالجة مكونات التقارير الإلكترونية</span><span class="sxs-lookup"><span data-stu-id="5f342-125">Handling ER components</span></span>
- <span data-ttu-id="5f342-126">قائمة تكوينات التقارير الإلكترونية التي تم تسليمها في تطبيق Finance</span><span class="sxs-lookup"><span data-stu-id="5f342-126">List of ER configurations that are delivered in the Finance application</span></span>