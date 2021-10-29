---
ms.openlocfilehash: d402caa030bc41a27c3b3f1900d7a1adf0fb337fdfc8819bae68c7e623095e60
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7582694"
---
قبل أن تبدأ، تحقق من استيفاء المتطلبات الأساسية الثلاثة التالية:

- الوصول إلى مدخل Fraud Protection الخاص بك
- تنزيل Visual Studio
- تثبيت .NET Core SDK v3.1 

## <a name="access-to-your-fraud-protection-portal"></a>الوصول إلى مدخل Fraud Protection الخاص بك

ينشئ Fraud Protection جميع التفاصيل المطلوبة لإنشاء رمز مميز واستدعاء بيئة Fraud Protection لديك. وبالتالي، ستحتاج إلى الوصول إلى لوحة معلومات مدخل Fraud Protection لديك. ستستخدم المعلومات من لوحة المعلومات لإعداد استدعاءات واجهة برمجة التطبيقات وتهيئة نموذج التطبيق، كما هو موضح في الوحدات اللاحقة من هذه الوحدة. 

إذا كنت بحاجة إلى ترخيص لاستخدام المنتج (قد تكون مؤهلاً للحصول على ترخيص تجريبي)، فاتصل بممثل Microsoft أو أرسل بريداً إلكترونياً إلى [Dynamics 365 Fraud Protection-IADHelp@Microsoft.com](mailto:Protection-IADHelp@Microsoft.com).

## <a name="download-visual-studio"></a>تنزيل Visual Studio 

توضح لك هذه الوحدة كيفية تكوين وتشغيل تطبيق نموذجي، والذي يتكامل مع مثيل Fraud Protection، باستخدام Visual Studio. يمكنك استخدام أي بيئة تطوير متكاملة. ومع ذلك، إذا كنت ترغب في المتابعة مع الأمثلة التي تظهر في نهاية هذه الوحدة، فستحتاج إلى مثيل Visual Studio ‏(Community 2019) على جهازك. يمكنك تنزيل Visual Studio من [Visual Studio ‏IDE، محرر التعليمات البرمجية‬, Azure DevOps، مركز التطبيقات - Visual Studio ‏(microsoft.com)]( https://visualstudio.microsoft.com/?azure-portal=true).

## <a name="install-net-core-sdk-v31"></a>تثبيت .NET Core SDK v3.1 

يعتمد معظم نموذج رمز التطبيق على تطبيق [eShopOnWeb](https://github.com/dotnet-architecture/eShopOnWeb/?azure-portal=true). لذلك، قبل البدء في تكوين نموذج التطبيق، تحتاج إلى التأكد من تثبيت .NET Core SDK الإصدار 3.1 أو إصدار أحدث على جهاز الكمبيوتر الخاص بك. 

