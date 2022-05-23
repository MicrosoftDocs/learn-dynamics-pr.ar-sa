---
ms.openlocfilehash: 3d621ab131a614b00345b6b3957a40791e22d65d
ms.sourcegitcommit: d923ddcaa6b0e6740cbcf77535cb6de781dc6b19
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/03/2022
ms.locfileid: "8666776"
---
من الضروري أن تقوم في بعض الأحيان بعرض نافذة منبثقة لمستخدم تطبيقك. يكتشف Power Apps component framework عن واجهة API منبثقة تتيح لك تحقيق هذا المطلب. سيوضح المثال التالي كيفية إنشاء نافذة منبثقة تعرض رسم محمّل. يمكن أن تساعدك هذه الطريقة في تحقيق تجربة مستخدم مرضية حيث يتم حظر واجهة المستخدم الأساسية من إجراء العمليات في العمليات طويلة المدى.

### <a name="initialize-your-components-project"></a>تهيئة مشروع المكون الخاص بك
لتهيئة مشروع المكون الخاص بك، اتبع الخطوات التالية:

1.  ابدأ تشغيل Visual Studio Code.
2.  حدد "وحدة طرفية"، ثم حدد "وحدة طرفية جديدة".
3.  شغّل الأمر التالي لإنشاء دليل جديد يسمى Popup-Component.

    ```
    md Popup-Component
    ```

4.  شغّل الأمر التالي للتبديل إلى الدليل الجديد.
   
    ```
    cd Popup-Component
    ```
5.  تهيئة المشروع عن طريق تشغيل الأمر التالي:

    ```
    pac pcf init --namespace SampleNamespace --name PopupComponent --template field
    ```

6.  قم بتشغيل npm install لتحميل مكتبات مستقلة في المشروع.
   
    ```
    npm install
    ```

7. افتح المشروع في Visual Studio Code عن طريق تشغيل الأمر التالي:

    ```
    code -a .
    ```

### <a name="implement-your-code-components-logic"></a>تنفيذ منطق مكون التعليمات البرمجية
لتنفيذ منطق مكون التعليمات البرمجية، اتبع الخطوات التالية:

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

    ستقوم بإضافة ملفات الدعم الموجودة في هذا البيان لاحقاً.

2.  افتح الملف index.ts.

3.  فوق الأسلوب *export class*، أدخل طريقة الواجهة التالية بحيث يمكنك كشف بعض الأساليب الأخرى التي توفرها واجهة برمجة التطبيقات (API) المنبثقة (popupStyle وshadowStyle):

    ```csharp
        interface Popup extends ComponentFramework.FactoryApi.Popup.Popup {
        popupStyle: object;
        shadowStyle: object;
    }
    ```

4.  أضف المتغير التالي فوق الأسلوب *constructor*.
   
    ```csharp
    private _container: HTMLDivElement;
    private _popUpService: ComponentFramework.FactoryApi.Popup.PopupService;
    ```

5.  أضف المنطق التالي إلى الأسلوب *init* التابع للمكون الخاص بك:

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

### <a name="add-styling-to-your-code-component"></a>إضافة تصميم إلى مكون التعليمات البرمجية‬
لإضافة تصميم إلى مكون التعليمات البرمجية‬، اتبع الخطوات الآتية:

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

1.  أنشئ حلك عن طريق تشغيل الأمر التالي.
   
    ```
    npm run build
    ```

2.  وبناء على إنشاء ناجح، يمكنك اختبار مكون واجهة برمجة التطبيقات (API) للتنسيق الجديد عن طريق تشغيل npm start. مكون المحمّل هذا مرتبط بحقل نصي. لاستخدام المكون في تطبيق يستند إلى نموذج، قد يكون من المفيد لك وضع علامة على هذا الحقل على أنه مخفي إذا كنت تريد استخدامه في نموذج. للحصول على المزيد من المعلومات حول كيفية نشر مكونات Power Apps، راجع "حزم مكون التعليمات البرمجية" في الوحدة النمطية *كتابة مكون Power Apps مخصص*.
   
    ```
    npm start
    ```

