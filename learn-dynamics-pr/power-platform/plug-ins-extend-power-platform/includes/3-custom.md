---
ms.openlocfilehash: 3c3b2a1531ebf2aab9a31e1cad459be7dff5b09a
ms.sourcegitcommit: 638bab9b0642ad3d3698e559bdfe044fb14354f7
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2022
ms.locfileid: "8548312"
---
تُعد ملحقات سير العمل إحدى مشتقات المكونات الإضافية التي تمكِّن المطورين من كتابة أنشطة مخصصة لا تتوفر داخل أنشطة العملية الافتراضية الموجودة داخل مصمم سير العمل. 

وتتطور Power Automate سريعاً لدعم وفرة من العمليات التي لا تتوفر في مهام سير العمل Microsoft Dataverse وينبغي اعتبارها بديلاً كلما أمكن ذلك. 

وكما هو الحال مع المكونات الإضافية، يتمثل أحد السيناريوهات الشائعة التي قد تكون فيها تجميعات سير العمل Dataverse مناسبة بشكل أكبر فيما إذا كان منطق العمل الذي تقوم بإنشائه يجب تشغيله بشكل متزامن. وفي الوقت الحالي، إذا كنت بحاجة إلى منطق متزامن لتشغيله داخل بيئة Dataverse لديك، فيجب عليك تكوين سير العمل حسب الطلب أو المكون الإضافي المتزامن لتحقيق هذا المطلب. 

## <a name="custom-workflow-extension-assemblies"></a>تجميعات ملحقات سير العمل المخصصة

بدلاً من تنفيذ واجهة IPlugin على النحو الذي نُفذت به المكونات الإضافية، ترث ملحقات سير العمل المخصصة فئة CodeActivity. وتكشف هذه الفئة عن طريقة Execute التي توفر معلمة CodeActivityContext.

### <a name="input-and-output-arguments"></a>وسيطات الإدخال والإخراج

تسمح لك ملحقات سير العمل المخصصة بتعريف المعلمات التي يمكن تمريرها إلى ملحق سير العمل ومنه باستخدام كائنات InArgument وOutArgument بالتزامن مع تزيين هذه الكائنات باستخدام سمات الإدخال والإخراج.

على سبيل المثال، لتكوين وسيطة إدخال، يمكنك استخدام النمط الآتي باستخدام [سمات ‎.NET](/dotnet/standard/attributes/index/?azure-portal=true):

```csharp
[Input("Integer input")]

public InArgument<int> IntInput { get; set; }
```

لتكوين وسيطة إخراج، استخدم بناء الجملة الآتي:

```csharp
[Output("Integer output")]

public OutArgument<int> IntOutput { get; set; }
```

كما يمكنك استخدام الخاصية نفسها كوسيطة إدخال وإخراج بتضمين كلتا السمتين:

```csharp
[Input("Int input")]

[Output("Int output")]

public InOutArgument<int> IntParameter { get; set; }
```

بعد ذلك، يمكن للكود الموجود داخل الأسلوب Execute الحصول على هذه المعلمات أو تعيينها من خلال الطريقتين "Get" و"Set" المتوفرة. على سبيل المثال، يقوم ملحق سير العمل الآتي بزيادة معلمة الإدخال بمقدار 10 وإرجاعها إلى معلمة الإخراج المطابقة. ولأن العمليات الرياضية لا يتم توفيرها من خلال مصمم سير العمل، فهذا يُعد سيناريو شائع قد يكون ملحق سير العمل المخصص مطلوباً فيه (ورغم ذلك، تجب مراعاة Power Automate في هذه الحالة كذلك).

```csharp
using Microsoft.Xrm.Sdk.Workflow;

using System.Activities;

public class IncrementByTen : CodeActivity

{

[RequiredArgument]

[Input("Decimal input")]

public InArgument<decimal> DecInput { get; set; }

[Output("Decimal output")]

public OutArgument<decimal> DecOutput { get; set; }

protected override void Execute(CodeActivityContext context)

{

decimal input = DecInput.Get(context);

DecOutput.Set(context, input + 10);

}

}
```

### <a name="other-property-attributes"></a>سمات خصائص أخرى

تعرض ملحقات سير العمل أيضاً سمات ‎.NET الآتية التي يمكن استخدامها بواسطة معلمات الإدخال والإخراج.

| [RequiredArgument]                             | تُستخدم لإنشاء وسيطة إدخال مطلوبة.                                                                                                                                         |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Default(“DefaultValue”)]                      | تُستخدم لتحديد القيم الافتراضية لوسيطة إدخال أو إخراج إذا لم يتم تعيين قيمة بالفعل.                                                                         |
| [ReferenceTarget(“entityname”)]                | مطلوبة عند تحديد خاصية لمعلمة EntityReference. لمزيد من المعلومات، راجع [معلمات EntityReference](/power-apps/developer/common-data-service/workflow/workflow-extensions#entityreference-parameters).                                                        |
| [AttributeTarget(“entityname”,”optionsetname”) | نظراً لاستخدامها بواسطة معلمات OptionSetValue، فإنها تحدد الكيان والسمة التي تحتوي على مجموعة صالحة من القيم للمعلمة. لمزيد من المعلومات، راجع [معلمات OptionSetValue](/power-apps/developer/common-data-service/workflow/workflow-extensions#optionsetvalue-parameters). |
 
