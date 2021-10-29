---
ms.openlocfilehash: bf292b6db2776b22dff5f492ac002a0ba9e4e8b0fca9c2db92734802b1f36d0a
ms.sourcegitcommit: 511a76b204f93d23cf9f7a70059525f79170f6bb
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "7457341"
---
من الضروري من حين لآخر أن تقوم بعرض نافذة منبثقة لمستخدم تطبيقك. يكتشف Power Apps component framework عن واجهة API منبثقة تتيح لك تحقيق هذا المطلب. سيوضح المثال التالي كيفية إنشاء نافذة منبثقة تعرض رسم محمّل. يمكن أن تساعدك هذه الطريقة في تحقيق تجربة مستخدم مرضية حيث يتم حظر واجهة المستخدم الأساسية من إجراء العمليات في العمليات طويلة المدى.

### <a name="initialize-your-components-project"></a>تهيئة مشروع المكون الخاص بك
لتهيئة مشروع المكون الخاص بك، اتبع الخطوات التالية:

1.  قم بتهيئة المشروع عن طريق تشغيل الأمر التالي:

    ```azurepowershell
    pac pcf init --namespace SampleNamespace --name PopupComponent --template field
    ```

2.  قم بتشغيل npm install لتحميل مكتبات مستقلة في المشروع.

### <a name="implement-your-code-components-logic"></a>قم بتنفيذ منطق مكون الأكواد الخاص بك
لتنفيذ منطق مكون الأكواد، اتبع الخطوات التالية:

1.  افتح ملف البيان الخاص بمكون الأكواد (ControlManifest.Input.xml) واستبدله بالمنطق التالي:

    ```xml
    <?xml version="1.0" encoding="utf-8" ?>
    <manifest>
      <control namespace="SampleNamespace" constructor="PopupComponent" version="0.0.1" display-name-key="PopupComponent_Display_Key" description-key="PopupComponent_Desc_Key" control-type="standard">
        <!-- property node identifies a specific, configurable piece of data that the control expects from CDS -->
        <property name="sampleProperty" display-name-key="Property_Display_Key" description-key="Property_Desc_Key" of-type="SingleLine.Text" usage="bound" required="true" /> 
        <resources>
          <code path="index.ts" order="1"/>
          <css path="css/loader.css" order="1" />
        </resources>
      </control>
    </manifest>
    ```

    ستقوم بإضافة ملفات الدعم الموجودة في هذا البيان لاحقًا.

2.  قم بفتح ملف index.ts.

3.  فوق الأسلوب *constructor*، أدخل طريقة الواجهة التالية بحيث يمكنك كشف بعض الأساليب الإضافية التي توفرها واجهة برمجة التطبيقات المنبثقة (popupStyle وshadowStyle):

    ```csharp
        interface Popup extends ComponentFramework.FactoryApi.Popup.Popup {
        popupStyle: object;
        shadowStyle: object;
    }
    ```

4.  أضف المنطق التالي إلى الأسلوب *init* التابع للمكون الخاص بك:

    ```csharp
    this._container = document.createElement('div');
            //============ content of our popup =============
            let popUpContent = document.createElement('div');
            popUpContent.setAttribute("class", "loader");
            
            
            //============ our Popup object =============
            let popUpOptions: Popup = {
                closeOnOutsideClick: true,
                content: popUpContent,
                name: 'loaderPopup', // unique popup name
                type: 1, // Root popup
                popupStyle: {
                    "width": "100%",
                    "height": "100%",
                    "overflow": "hidden",
                    "backgroundColor": "transparent",
                    "display": "flex",
                    "flexDirection": "column",
                    "position": "absolute",
                    "margin-top": 28 + "px"
                },
                shadowStyle:{
                    position: "absolute",
                    width: "100%",
                    height: "100%"
                }
            };
            
            this._popUpService = context.factory.getPopupService();
    
            this._popUpService.createPopup(popUpOptions);
            
            container.appendChild(this._container);
            this._popUpService.openPopup('loaderPopup');
    ```

### <a name="add-styling-to-your-code-component"></a>إضافة تصميم إلى مكون الأكواد
لإضافة تصميم إلى مكون الأكواد، اتبع الخطوات الآتية:

1.  أنشئ مجلداً فرعياً CSS جديداً تحت المجلد PopupComponent.

2.  أنشئ ملف loader.css جديدًا داخل المجلد الفرعي CSS.

3.  أضف محتوى النمط التالي إلى ملف loader.css:

    ```xml
    .loader {
        border: 16px solid #f3f3f3; /* Light grey */
        border-top: 16px solid #3498db; /* Blue */
        border-radius: 50%;
        position: fixed;
        width: 120px;
        height: 120px;
        top:40%;
        left:50%;
        animation: spin 2s linear infinite;
      }
      
      @keyframes spin {
        0% { transform: rotate(0deg); }
        100% { transform: rotate(360deg); }
      }
    ```

4.  احفظ ملف loader.css.

### <a name="build-and-run-your-component"></a>إنشاء المكون وتشغيله
لإنشاء المكون وتشغيله، اتبع الخطوات التالية:

1.  قم بإنشاء الحل عن طريق تشغيل npm run build.

2.  وبناء على إنشاء ناجح، يمكنك اختبار مكون واجهة برمجة التطبيقات للتنسيق الجديد عن طريق تشغيل npm start. مكون المحمّل هذا مرتبط بحقل نصي. لاستخدام المكون في تطبيق يستند إلى نموذج، قد يكون من المفيد لك وضع علامة على هذا الحقل على أنه مخفي إذا كنت تريد استخدامه في نموذج. للحصول على مزيد من التفاصيل حول كيفية نشر مكونات Power Apps، راجع "تضمين مكون الاكواد" في وحدة *كتابة مكون Power Apps مخصص*.

