---
ms.openlocfilehash: d3449fc44b3e5c02b9d3aabc99fd1867e051b6c5
ms.sourcegitcommit: 24d9968aa50d817923b7ffaef674b71d2c06238a
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/16/2022
ms.locfileid: "9021543"
---
يوفر نموذج تطبيق التاجر Microsoft Dynamics 365 Fraud Protection مثالاً على كيفية استدعاء [واجهات API لـ Dynamics 365 Fraud Protection](/dynamics365/fraud-protection/). قد يكون نموذج التطبيق هذا مفيداً إذا كنت تتكامل مع واجهات API لـ Fraud Protection أو إذا كنت تريد معرفة كيفية دمج نقاط نهاية/ميزات API الجديدة عند توفر إصدارات جديدة من API. 

يعتمد معظم نموذج الرمز على تطبيق [eShopOnWeb](https://github.com/dotnet-architecture/eShopOnWeb/?azure-portal=true). لذلك، قبل تشغيل الحل، تأكد من تثبيت NET Core SDK. الإصدار 3.1 أو إصدار أحدث على جهازك. 

لتسريع التطوير المحلي، يمكنك بدء تشغيل/تصحيح أخطاء التطبيق محلياً. يستخدم التطبيق قاعدة بيانات في الذاكرة تستمر لجلسة التشغيل/التصحيح الفردية. بخلاف ذلك، اتبع الخطوات المذكورة في [نماذج Dynamics 365 Fraud Protection](https://github.com/microsoft/Dynamics-365-Fraud-Protection-Samples/tree/master/src/?azure-portal=true) لاستخدام قاعدة البيانات الخاصة بك، ثم تشغيل/تصحيح التطبيق.


