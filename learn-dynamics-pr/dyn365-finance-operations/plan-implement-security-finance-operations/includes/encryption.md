---
ms.openlocfilehash: 2bdde922adbaa98654e5cf5c896f9e7b5f6f9d66
ms.sourcegitcommit: 9adc0b78e181986a042bb4a7b22fe7aae27b62ba
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/16/2022
ms.locfileid: "8454488"
---
## <a name="encryption-at-rest"></a>التشفير في حالة السكون

تستخدم Microsoft تقنية التشفير لحماية بيانات العملاء أثناء السكون في قاعدة بيانات SQL Server ومخزن Azure الخاصين بالبيئة.

تستخدم كافة المثيلات [Microsoft SQL Server تشفير البيانات الشفاف (TDE)](/sql/relational-databases/security/encryption/transparent-data-encryption?&preserve-view=sql-server-ver15/?azure-portal=true) و[تشفير تخزين Azure](/azure/storage/common/storage-service-encryption/?azure-portal=true) لإجراء تشفير في الوقت الفعلي للبيانات عند كتابتها إلى القرص في حالة السكون. 

تستخدم تطبيقات التمويل والعمليات التشفير من جانب الخادم باستخدام مفاتيح تتم إدارتها بواسطة الخدمة. تتم معالجة كافة أوجه إدارة المفاتيح مثل إصدار المفتاح والتدوير والنسخ الاحتياطي من قبل Microsoft.

بالإضافة إلى التشفير الافتراضي في حالة السكون المتوفر أعلاه، يمكنك استخدام تشفير API المتوفر في فئة X++ **العمومية**. تستخدم الأساليب **العمومية::editEncryptedField()** و **العمومية::editEncryptedStringField()** شهادة تشفير البيانات الخاصة بالبيئة لإجراء تشفير البيانات وفك تشفيرها. يمكنك استخدام هذه الطرق كطبقة إضافية للحماية بخلاف تقنية التشفير الافتراضي في حالة السكون المستخدمة لتخزين البيانات.

## <a name="encryption-in-transit"></a>التشفير أثناء النقل

يتم تشفير الاتصالات التي تم إنشاؤها بين العملاء ومراكز بيانات Microsoft، كما يتم تأمين جميع نقاط النهاية العامة باستخدام بروتوكول أمان طبقة النقل (TLS) 1.2 المتوافق مع معايير الصناعة. ينشئ بروتوكول أمان طبقة النقل (TLS) بشكل فعال متصفح محسّن أمنياً للاتصال بالخادم للمساعدة في ضمان سرية البيانات وتكاملها بين أجهزة سطح المكتب ومراكز البيانات. 

راجع [التشفير في تطبيقات التمويل والعمليات](/dynamics365/fin-ops-core/dev-itpro/sysadmin/encryption/?azure-portal=true) للحصول على معلومات حول التشفير.
