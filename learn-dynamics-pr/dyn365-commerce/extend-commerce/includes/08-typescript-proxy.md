---
ms.openlocfilehash: 17a96bd8ed2a933963b2cb5dc65e92c24aea4cc8
ms.sourcegitcommit: 8773c31cceaa4d9a36c62c964a2b414c6e0656f3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "7328404"
---
يقوم وكيل Commerce بتجريد الواجهة بين Retail Server وCommerce runtime (CRT). 

على سبيل المثال، يمكنك إنشاء كيان جديد وبعض منطق الأعمال كعمليات طلب/استجابة في CRT، ويمكنك إضافة واجهة API جديدة لـ Retail Server لعرض هذا الكيان وعمليات الطلب/الاستجابة هذه. والآن، فإنك ترغب في الوصول إلى الكيان وعمليات الطلب/الاستجابة في نقطة البيع (POS) لإنشاء منطق العميل. 

يمكنك إنشاء جميع الكيانات وبيانات تعريف الطلب/الاستجابة في نقطة البيع يدوياً، ويمكنك الوصول إلى Retail Server باستخدام المعلمات الصحيحة. يقلل وكيل Commerce من هذا الجهد عن طريق إنشاء الوكيل تلقائياً لجميع الكيانات المخصصة وعمليات الطلب/الاستجابة التي تمت إضافتها في واجهة API لـ Retail Server. 

تقوم أداة الوكيل بإنشاء الواجهة المطلوبة وجميع بيانات التعريف المطلوبة ثم تقوم بتجريد التنفيذ الفعلي. بهذه الطريقة، يمكنك تضمين الملفات في مشروعات الملحقات والوصول إلى واجهات API لـ Retail Server والكيانات باستخدام بيانات التعريف والواجهة التي تم إنشاؤها.

لإنشاء وكيل Typescript لنقطة البيع، اتبع الخطوات التالية:

1. افتح نموذج مشروع قالب الوكيل من **\RetailSDK\Code\SampleExtensions\TypeScriptProxy\TypeScriptProxy.Extensions.StoreHoursSample\Proxies.TypeScriptProxy.Extensions.StoreHoursSample.csproj** في Visual Studio. أعد تسميته، إذا لزم الأمر.
2. أضف مشروع ملحق Retail Server كمشروع مرجعي للمشروع إلى مشروع قالب الوكيل هذا. قم بإزالة المشروع المرجعي **StoreHoursSample** الموجود.
3. انقر بزر الماوس الأيمن فوق **Proxies.TypeScriptProxy.Extensions.StoreHoursSample.csproj** ثم حدد **تحرير Proxies.TypeScriptProxy.Extensions.StoreHoursSample.csproj**.
4. ضمن العقدة **RetailServerExtensionAssemblies**، حدد اسم تجميع ملحق Retail Server. يوضح المثال التالي كيفية إضافة اسم التجميع.
  
    ```csharp
    <ItemGroup>
        <RetailServerExtensionAssemblies Include="..\..\RetailServer\Extensions.Sample\bin\$(Configuration)\net461\$(AssemblyNamePrefix).RetailServer.Extension.Sample.dll" />
    </ItemGroup>
    ```
5. ضمن العقدة **نسخ**، قم بتحديث المسار **DestinationFolder** إلى مجلد ملحق نقطة البيع حتى يتم نسخ ملفات الوكيل التي تم إنشاؤها إلى المجلد **ملحق نقطة البيع** تلقائياً. سيتم أيضاً نسخ ملفات الوكيل التي تم إنشاؤها إلى **\RetailSDK\Code\SampleExtensions\TypeScriptProxy\TypeScriptProxy.Extensions.StoreHoursSample\DataService**. يوضح المثال التالي كيفية تحديث المسار.
 
    ```csharp
    <Copy SourceFiles="@(GeneratedDataServiceContracts)" DestinationFolder="$(SdkRootPath)\POS\Extensions\Sample\DataService" SkipUnchangedFiles="true" />
    ``` 

6. بعد اكتمال التغييرات، قم بإنشاء مشروع الوكيل لإنشاء ملفات وكيل Typescript. عند اكتمال الإنشاء، ستتوفر ملفات الوكيل في المجلد **\RetailSDK\Code\SampleExtensions\TypeScriptProxy\TypeScriptProxy.Extensions.StoreHoursSample\DataService** وفي المجلد المحدد في الأمر **نسخ**. يمكن أن يختلف المسار ومسار المجلد بناءً على بنية المجلد.

لمعرفة المزيد من المعلومات، راجع [إنشاء واجهة API جديدة لملحق Retail Server](/dynamics365/commerce/dev-itpro/retail-server-icontroller-extension/?azure-portal=true).

