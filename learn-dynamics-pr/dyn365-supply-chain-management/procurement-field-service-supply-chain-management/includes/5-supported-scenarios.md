---
ms.openlocfilehash: c67c7c8f48cd02ceb0d1e92ffb136d3b22563dc9
ms.sourcegitcommit: 971396efb8e68a74511ae8ca417a67c4d9cef8ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/04/2021
ms.locfileid: "7599853"
---
توضح الأقسام التالية السيناريوهات المدعومة وغير المدعومة لهذا التطبيق.

## <a name="supported-scenarios"></a>السيناريوهات المدعومة

تتضمن السيناريوهات المدعومة للتطبيق:

- يمكن لمستخدمي Dataverse إنشاء أوامر الشراء وتغييرها. ومع ذلك، تتحكم Supply Chain Management في العملية والبيانات. عند وصول التحديثات من Field Service، يتم تطبيق الحدود الخاصة بالتسويات إلى أعمده أمر الشراء في Supply Chain Management. على سبيل المثال، بعد أن يتم إنهاء أمر شراء، لا يمكن تحديثه.

- لا يمكن لمستخدم Field Service تحرير أمر شراء إلا إذا كانت حالة اعتماد Supply Chain Management عبارة عن **مسودة** إذا كان أمر الشراء منظماً بواسطة إدارة التغيير في Supply Chain Management.

- يتم الاحتفاظ بالعديد من الأعمدة بشكل حصري بواسطة Supply Chain Management ولا يمكن تغييرها بواسطة Field Service. راجع جداول التعيين الموجودة ضمن المنتج لمعرفة الأعمدة التي لا يمكن تعديلها. تكون معظم الأعمدة للقراءة فقط على صفحات Dataverse لإبقاء الأمر بسيطاً.‬

    على سبيل المثال، تتم إدارة أعمدة معلومات السعر بواسطة Supply Chain Management. إن Supply Chain Management لديها اتفاقيات تجارية والتي يمكن لـ Field Service الاستفادة منها. تأتي الأعمدة مثل **سعر الوحدة** و **الخصم** و **المبلغ الصافي** من Supply Chain Management. للتأكد من مزامنة السعر مع Field Service، يجب استخدام ميزة **المزامنة** في صفحتي **أمر الشراء** وكذلك **منتج أمر الشراء** على Dataverse عند إدخال بيانات أمر الشراء. 

- نظراً لأنه لا تتوفر إجماليات محدثة لأمر الشراء في Supply Chain Management، يكون عمود **الإجماليات‬** متاحاً فقط في Field Service. يتم اشتقاق إجماليات Supply Chain Management باستخدام معلمات متنوعة لا تتوفر في Field Service.

- يمكن فقط لـ Supply Chain Management بدء بنود أمر شراء بفئة تدبير محددة أو حيث يكون المنتج المُشار إليه هو أحد أصناف نوع منتج الخدمة أو نوع منتج Field Service. وبعد ذلك، تتم مزامنة البنود مع Dataverse وستظهر في Field Service.

- في حالة تثبيت Field Service فقط وعدم توفر Supply Chain Management، يكون عمود **المستودع** الموجود في أمر الشراء مطلوباً. تقل حدة هذه الضرورة إذا تم تثبيت Supply Chain Management حيث إنها تسمح ببنود أمر الشراء حيث لا يتم توفير مستودع في سيناريوهات معينة.

- تتم إدارة إيصالات استلام المنتجات (عمليات استلام طلبات الشراء على Dataverse) بواسطة Supply Chain Management ولا يمكن إنشاؤها من Dataverse في حالة تثبيت Supply Chain Management. تتم مزامنة إيصالات استلام المنتجات من Supply Chain Management من Supply Chain Management إلى Dataverse.

- تسمح Supply Chain Management بالتسليم بالنقص. يتضمن حل OneFSSCM الوظيفة التي تقوم بإنشاء أو تحديث صف دفاتر يومية المخزون في Dataverse عند إنتاج بند إيصال استلام المنتجات (أو منتج استلام أمر الشراء في Dataverse) أو تغييره لتعديل المبلغ المتبقي الموجود بالأمر في حالات التسليم بالنقص.

## <a name="unsupported-scenarios"></a>السيناريوهات غير المدعومة

تتضمن السيناريوهات غير المدعومة للتطبيق:

- في Supply Chain Management، تمنع Field Service إضافة البنود إلى أمر الشراء الذي تم إلغاؤه. وكحل بديل لذلك، يمكنك تعديل حالة النظام الخاصة بأمر الشراء في Field Service ثم إضافة البند الإضافي في Field Service أو Supply Chain Management.

- على الرغم من أن صفوف التدابير لها تأثير في مستويات المخزون في كلا النظامين، إلا أن هذه الواجهة لا تضمن محاذاة المخزون بين Supply Chain Management وField Service. ستقوم العمليات الأخرى في Field Service وSupply Chain Management بتحديث مستويات المخزون. لا تتم تغطية هذه الإجراءات بواسطة التدبير.
