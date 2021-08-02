---
ms.openlocfilehash: 3d74842add40aed5b4805ab1522a0d6b54f47c82
ms.sourcegitcommit: fde44a19a7497a0d50347583f4126b3e9c0a842c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/27/2021
ms.locfileid: "6112099"
---
لتنفيذ حدث عمل جديد، تحتاج إلى إنشاء عقد، وإنشاء الحدث، ثم إضافة رمز لإرسال الحدث.

يتم تنفيذ فئتين لحدث جديد: فئة حدث الأعمال وفئة عقد أحداث الأعمال. تعمل فئة حدث الأعمال على توسيع فئة `BusinessEventsBase` وتدعم إنشاء حدث الأعمال وبناء الحمولة وإرسال حدث الأعمال.
يجب أن يشتمل الاسم على الاسم أو العبارة التي تتوافق مع الحدث، متبوعةً بلاحقة `BusinessEvent`، مثل `CustomerInvoicePostedBusinessEvent`.

بعد إنشاء الفئة، استخدم الإجراء التالي لإضافة أساليب إلى الفئة الخاصة بك. تحدد أمثلة التعليمات البرمجية حدث `SalesInvoicePostedBusinessEvent`.

1. أضف أسلوب `newFrom<my_buffer>` ثابتاً، مع ملء جزء `my_buffer` مع المخزن المؤقت للجدول الذي يتم استخدامه لتهيئة عقد حدث الأعمال.


    ```xpp
    static public SalesInvoicePostedBusinessEvent
    newFromCustInvoiceJour(CustInvoiceJour _custInvoiceJour)
    {
        SalesInvoicePostedBusinessEvent businessEvent = new
        SalesInvoicePostedBusinessEvent();
        businessEvent.parmCustInvoiceJour(_custInvoiceJour);
        return businessEvent;
    }
    ```
2. قم بتوسيع فئة `BusinessEventsBase`. يجب تحديد التسميات لوسائط الاسم والوصف، ولكن يجب ترك الرمز "@" لتجنب تخزين البيانات المترجمة. توفر سمة `BusinessEvents` إطار أحداث الأعمال مع معلومات حول عقد حدث الأعمال واسمه ووصفه.

    ```xpp
    [BusinessEvents(classStr(SalesInvoicePostedBusinessEventContract)),
    "AccountsReceivable:SalesOrderInvoicePostedBusinessEventName","AccountsReceivable:SalesOrderInvoicePostedBusinessEventDescription",ModuleAxapta::SalesOrder)]
        public class SalesInvoicePostedBusinessEvent extends BusinessEventsBase
    ```
    
3. أضف أساليب `private parm` للحفاظ على الحالة الداخلية للفئة.

    ```xpp
    private CustInvoiceJour parmCustInvoiceJour(CustInvoiceJour_custInvoiceJour = custInvoiceJour)
    {
        custInvoiceJour = _custInvoiceJour;
        return custInvoiceJour;
    }
    ```
    
4. أضف أسلوب `buildContract`. يجب تزيين الأسلوب باستخدام السمتين `Wrappable(true)` و`Replaceable(true)`، وسيتم استدعاؤه فقط عند تمكين حدث أعمال لإحدى الشركات.

    ```xpp
   [Wrappable(true)], [Replaceable(true)]
   public BusinessEventsContract buildContract()
   {
      return
      SalesInvoicePostedBusinessEventContract::newFromCustInvoiceJour(custInvoiceJour);
   }
   ```

تقوم فئة عقد أحداث الأعمال بتوسيع فئة `BusinessEventsContract`. إنها تحدد حمولة حدث الأعمال وتسمح بملء العقد في وقت التشغيل.

استخدم الخطوات التالية لتوسيع فئة `BusinessEventContract` وإضافة الأساليب إلى الفئة. تحدد أمثلة التعليمات البرمجية حدث `SalesInvoicePostedBusinessEventContract`.

1. قم بتوسيع فئة `BusinessEventContract`، مع التأكد من تزيينها بالسمة `DataContract`.

    ```xpp
    [DataContract]
    public final class SalesInvoicePostedBusinessEventContract extends
    BusinessEventsContract
    ```

2. أضف متغيرات `private` للاحتفاظ بحالة العقد.

    ```xpp
    private CustInvoiceAccount      invoiceAccount;
    private CustInvoiceId           invoiceId;
    private SalesIdBase             salesId;
    private TransDate               invoiceDate;
    private DueDate                 invoiceDueDate;
    private AmountMST               invoiceAmount;
    private TaxAmount               invoiceTaxAmount;
    private LegalEntityDataAreaId   legalEntity;
    ```

3. أضف أسلوب تهيئة `private` باستخدام اسم `initialize`. تحدد هذه الطريقة الحالة الخاصة لفئة عقد حدث الأعمال، استناداً إلى البيانات التي يتم توفيرها من خلال أسلوب منشئ `static`.

    ```xpp
    private void initialize(CustInvoiceJour _custInvoiceJour)
    {
        invoiceAccount = _custInvoiceJour.InvoiceAccount;
        invoiceId = _custInvoiceJour.InvoiceId;
        salesId = _custInvoiceJour.SalesId;
        invoiceDate = _custInvoiceJour.InvoiceDate;
        invoiceDueDate = _custInvoiceJour.DueDate;
        invoiceAmount = _custInvoiceJour.InvoiceAmountMST;
        invoiceTaxAmount = _custInvoiceJour.SumTaxMST;
        legalEntity = _custInvoiceJour.DataAreaId;
    }
    ```

4. أضف أسلوب منشئ `static`.

    ```xpp
    public static SalesInvoicePostedBusinessEventContract
    newFromCustInvoiceJour(CustInvoiceJour _custInvoiceJour)
    {
        var contract = new SalesInvoicePostedBusinessEventContract();
        contract.initialize(_custInvoiceJour);
        return contract;
    }
    ```
    
5. أضف أساليب `parm` للوصول إلى حالة العقد. ويجب تزيين هذه الطرق باستخدام السمتين `DataMember('')` و`BusinessEventsDataMember('')`. لملء الحالة الداخلية لعقد البيانات، قد تحتاج إلى أساليب استرداد إضافية يجب أن تظهر على أنها `private` ويتم استدعاؤها من أسلوب `initialize`.

    ```xpp
    [DataMember('InvoiceAccount'),
    BusinessEventsDataMember("@AccountsReceivable:InvoiceAccount")]
    public CustInvoiceAccount parmInvoiceAccount(CustInvoiceAccount_invoiceAccount = invoiceAccount)
    {
        invoiceAccount = _invoiceAccount;
        return invoiceAccount;
    }
    ```
