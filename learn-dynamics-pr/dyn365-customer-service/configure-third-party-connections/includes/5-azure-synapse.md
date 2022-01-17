---
ms.openlocfilehash: de6c5e43b3495e49b49c6ae6330f0e26c0d0cfc2
ms.sourcegitcommit: c9e4fdec30906fc4b8686ea5c65b335ca5b68c26
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2021
ms.locfileid: "7933586"
---
يوفر Dynamics 365 Customer Insights ميزات وأدوات متعددة مختلفة، مثل توقعات الذكاء الاصطناعي الجاهزة التي تبسط عملية محللي الأعمال لبناء الحلول. تساعدك الموصلات التي تم إنشاؤها مسبقاً على استخدام وظائف Customer Insights بكفاءة، مثل ملفات التعريف والشرائح والقياسات والإثراء والذكاء الاصطناعي. ومع ذلك، قد تحدث حالات لا توفر فيها الميزات الجاهزة العمق اللازم أو لا تدعم حالة الاستخدام المحددة التي تريد استخدامها. على سبيل المثال، يتضمن Customer Insights نموذج خسارة العملاء الجاهز، الذي يمكنك استخدامه لإجراء توقعات تتعلق بعميل لا يجدد الاشتراك. يجب أن تتضمن البيانات المرفقة بالنموذج حقولاً وتنسيقات محددة. قد يتناسب هذا النموذج الآن مع بنية بياناتك العام. وفي هذه الحالات، قد ترغب في الحصول على القدرة على إنشاء نماذج توقع خاصة بك لتناسب احتياجاتك. وبالتالي، ستحتاج إلى استخدام تطبيقات أخرى تسمح لك ببناء حلول أكثر تعقيداً يمكنها سد الثغرات في Customer Insights وتقديم خدمات تكميلية. 

## <a name="azure-synapse-and-customer-insights"></a>Azure Synapse وCustomer Insights 

إن Microsoft Azure Synapse Analytics عبارة عن خدمة تحليلات غير محدودة تجمع بين تكامل البيانات وتخزين بيانات المؤسسة وتحليلات البيانات الكبيرة. وتمنحك هذه الخدمة حرية الاستعلام عن البيانات وفقاً لشروطك باستخدام خيارات بلا خادم أو خيارات بلا على نطاق واسع. يجمع Azure Synapse هذه العوالم جنباً إلى جنب مع تجربة موحدة لاستيعاب البيانات واستكشافها وإعدادها وتحويلها وإدارتها وتقديمها لتلبية احتياجات المعلومات المهنية والتعلم الآلي الفورية.

من خلال الفعالية المدمجة لكل من Azure Synapse Analytics وCustomer Insights، بإمكان المؤسسات توحيد بيانات عملائها. بالإضافة إلى ذلك، يمكنها إحضار مصادر بيانات أخرى، مثل بيانات العمليات والبيانات المالية والبيانات المنظمة/غير المنظمة وIoT الأشياء والبيانات الكبيرة. علاوة على ذلك، بإمكان المؤسسات تحقيق هذا الهدف في Azure Data Lake Storage نفسه في مخطط نموذج بيانات عامة. بإمكان المؤسسات الآن استخدام الرؤى الجاهزة (المتوفرة من Customer Insights) وتطوير نماذج ذكاء اصطناعي وتعلم آلي مخصصة للحصول على رؤى تنبؤية أكثر تحديداً وتخصيصاً قابلة للتنفيذ عبر المؤسسة بأكملها. 

> [!div class="mx-imgBorder"]
> [![رسم تخطيطي لـ Customer Insights مع Azure Synapse.](../media/customer-insights-azure-synapse.png)](../media/customer-insights-azure-synapse.png#lightbox)

يلتقي كل من Customer Insights وAzure Synapse Analytics في Azure Data Lake Storage لإكمال مخطط نموذج البيانات العامة. بشكل أساسي، يوحد مخطط نموذج البيانات العامة الأنواع التالية من البيانات لتقديم طريقة عرض شاملة لعميلك:

- بيانات العميل الموحدة، مثل البيانات من تطبيقات الأعمال (Salesforce وAdobe وDynamics 365) التي تأتي من Customer Insights 
- البيانات التشغيلية والبيانات الكبيرة، مثل البيانات التاريخية والبيانات غير المنظمة. 
- بيانات البث/الوقت الحقيقي (مثل Twitter) والبيانات الاجتماعية من Azure Synapse Analytics 

بالإضافة إلى ذلك، يوفر نموذج البيانات العامة وقتاً لا مثيل له للرؤى القابلة للتنفيذ عبر المؤسسة بأكملها.
 

## <a name="set-up-exports-to-azure-synapse-analytics"></a>اعداد عمليات التصدير إلى Azure Synapse Analytics

قبل أن تتمكن من تصدير البيانات من Customer Insights إلى Azure Synapse Analytics، تأكد من استيفاء جميع المتطلبات الأساسية الضرورية. لمزيد من المعلومات، راجع [المتطلبات الأساسية في Customer Insights](/dynamics365/customer-insights/audience-insights/export-azure-synapse-analytics?azure-portal=true#prerequisites-in-customer-insights). 

على غرار إمكانات التصدير الأخرى، إذا أردت استخدام بيانات Customer Insights في Azure Synapse Analytics، فأكمل الإجراءات التالية:

-   **إعداد الاتصال لـ Azure Synapse Analytics** - ضمن **الإدارة > اتصالات**، أضف اتصالاً، ثم حدد **Azure Synapse Analytics**. بعد تحديد عنوان الخادم والمصادقة، سيكون الاتصال متاحاً في المستقبل لعمليات التصدير. [اعرف كيفية إعداد اتصال بـ Azure Synapse Analytics](/dynamics365/customer-insights/audience-insights/export-azure-synapse-analytics?azure-portal=true#set-up-the-connection-and-export-to-azure-synapse).

-   **إعداد التصدير** - ضمن **البيانات > عمليات التصدير**، أضف وجهة تصدير جديدة تشير إلى اتصال Azure Synapse Analytics الذي أنشأته في وقت سابق. في التصدير، حدد المقاطع المراد تضمينها في التصدير. [اعرف كيفية إعداد تصدير إلى Azure Synapse Analytics](/dynamics365/customer-insights/audience-insights/export-azure-synapse-analytics?azure-portal=true#set-up-the-connection-and-export-to-azure-synapse).

الآن بعد أن تعلمت كيفية استخدام ملف تعريف العميل وبيانات المقطع من Customer Insights مع Dynamics 365 Marketing وDynamics 365 Sales، يمكنك معرفة كيفية عرض بيانات Customer Insights في سجلات Dynamics 365.
