---
ms.openlocfilehash: e810f1f20ad0179706a7c66d6a164d7cfaf8150c
ms.sourcegitcommit: 7e7463b82916b5b36a89d2c4f45e6f1bd95c1792
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/22/2021
ms.locfileid: "7945698"
---
يعمل تكامل Microsoft Power Platform على إزالة العوائق التي تحول دون دخول العملاء للاستفادة بشكل كامل من مكدس Microsoft Power Platform مع كل بيئة من بيئاتهم في Finance and Operations. تتحوّل ميزات مثل الكتابة المزدوجة إلى تجربة تحتاج إلى نقرة واحدة لإعدادها. تكون الوظائف الإضافية غير مؤمنة لبيئة تستخدم تكامل Microsoft Power Platform. ويتم أيضاً توفير الكيانات الظاهرية بشكل افتراضي في البيئة. تتكامل أيضاً أحداث الأعمال وأحداث الإنشاء/التحديث/الحذف (CUD) في تطبيقات Finance and Operations مع Microsoft Dataverse. 

> [!Note]
> ستصبح أحداث CUD متاحة فقط مع تكامل Microsoft Power Platform.

عند استخدام تجربة جديدة في كل بيئة في Lifecycle Services، بإمكان المستخدم إكمال الجزء الأول من إعداد تكامل Microsoft Power Platform. وسيؤدي ذلك إلى إنشاء بيئة من نفس النوع (بيئة تشغيل أو بيئة اختبار معزولة) في مركز مسؤولي Power Platform. ستحمل هذه البيئة الجديدة نفس اسم البيئة الموجودة في Lifecycle Services وسيتم تشغيلها بواسطة Microsoft Dataverse، وسيتم ملء عنوان URL لتطبيق Finance and Operations في هذه البيئة في مركز المسؤولين. 

عند اكتمال الإعداد، سيتم تمكين إعداد الكتابة المزدوجة وبإمكان العملاء الذين يرغبون في استخدام الكتابة المزدوجة القيام بذلك من Lifecycle Services. بعد ذلك، يمكنهم تحديد خرائط الكيانات المراد مزامنتها من تطبيق Finance and Operations. يتم أيضاً تثبيت الكيانات الظاهرية في البيئة باستخدام تكامل Microsoft Power Platform، ومن غير الضروري إعداد اتصالات يدوية لأن البيئات تكون متصلة بشكل مسبق.

مع تمكين تكامل Microsoft Power Platform، سيُضاف مستخدمو Finance and Operations بشكل تلقائي إلى Dataverse عندما ينتقل المستخدمون إلى الكيانات الظاهرية من Microsoft Power Apps. 

هناك ميزة أخرى لتمكين تكامل Microsoft Power Platform وهي أن أحداث الأعمال في Finance and Operations ستتقارب مع أحداث الأعمال في Dataverse. سيتلقى المستخدمون الذين يشتركون في أحداث أعمال Finance and Operations هذا الحدث من Dataverse. علاوةً على ذلك، سيمكّن تنفيذ المكونات الإضافية C# في Dataverse لسيناريوهات Finance and Operations التي يتم تنفيذها بسبب أحداث الأعمال. 

مع التكامل، تتوفر أيضاً أحداث CUD في كيانات البيانات التي تم تمكينها لـ OData في Finance and Operations. بإمكان عملية CUD في تطبيق Finance and Operations أن تحدث عبر واجهة مستخدم Finance and Operations أو واجهات API لـ OData في Finance and Operations أو من Power Apps/‏Power Portal، باستخدام كيانات ظاهرية. سيقوم حدث CUD بتشغيل الكيان. علاوةً على ذلك، إنه يمكّن تنفيذ المكونات الإضافية C# في Dataverse لسيناريوهات Finance and Operations التي يتم تنفيذها كاستجابة لأحداث CUD. 

ستقوم أداة تسجيل المكون الإضافي بتمكين تسجيل أحداث الأعمال وCUD للمكونات الإضافية C# التي تأتي من تطبيقات Finance and Operations. بإمكان المطورين استكشاف بيئات Dataverse وكتابة المكونات الإضافية C# وتسجيلها ونشرها في Visual Studio باستخدام ملحق Visual Studio لـ Microsoft Power Platform. بالنسبة للمطورين، مثل مطوري Finance and Operations، الذين يعملون في Visual Studio، يؤدي ذلك إلى توفير مساحة عمل (Visual Studio) واحدة لتأليف تخصيصاتهم عبر تطبيقات Dynamics 365 في تطبيقات Finance and Operations وDataverse. 

راجع [تكامل Microsoft Power Platform مع تطبيقات Finance and Operations](/dynamics365/fin-ops-core/dev-itpro/power-platform/overview/?azure-portal=true) لمعرفة المزيد. 
