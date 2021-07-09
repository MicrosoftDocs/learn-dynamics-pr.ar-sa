---
ms.openlocfilehash: 0bb0e63905dfbd561270642386aae5bc8a3bc26c
ms.sourcegitcommit: 374b549f0eda9bb2e3d14ab91f3955a9b58abf34
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/27/2020
ms.locfileid: "6072024"
---
<span data-ttu-id="5869e-101">لتنفيذ حدث عمل جديد، تحتاج إلى إنشاء عقد، وإنشاء الحدث، ثم إضافة رمز لإرسال الحدث.</span><span class="sxs-lookup"><span data-stu-id="5869e-101">To implement a new business event, you need to build a contract, build the event, and then add code to send the event.</span></span>

<span data-ttu-id="5869e-102">يتم تنفيذ فئتين لحدث جديد: فئة حدث الأعمال وفئة عقد أحداث الأعمال.</span><span class="sxs-lookup"><span data-stu-id="5869e-102">Two classes are implemented for a new event: a business event class and a business events contract class.</span></span> <span data-ttu-id="5869e-103">تعمل فئة حدث الأعمال على توسيع فئة `BusinessEventsBase` وتدعم إنشاء حدث الأعمال وبناء الحمولة وإرسال حدث الأعمال.</span><span class="sxs-lookup"><span data-stu-id="5869e-103">The business event class extends the `BusinessEventsBase` class and supports constructing the business event, building the payload, and sending the business event.</span></span>
<span data-ttu-id="5869e-104">يجب أن يشتمل الاسم على الاسم أو العبارة التي تتوافق مع الحدث، متبوعةً بلاحقة `BusinessEvent`، مثل `CustomerInvoicePostedBusinessEvent`.</span><span class="sxs-lookup"><span data-stu-id="5869e-104">The name should include the noun or phrase that corresponds with the event, followed by the `BusinessEvent` suffix, such as `CustomerInvoicePostedBusinessEvent`.</span></span>

<span data-ttu-id="5869e-105">بعد إنشاء الفئة، استخدم الإجراء التالي لإضافة أساليب إلى الفئة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="5869e-105">After the class is created, use the following procedure to add methods to your class.</span></span> <span data-ttu-id="5869e-106">تحدد أمثلة التعليمات البرمجية حدث `SalesInvoicePostedBusinessEvent`.</span><span class="sxs-lookup"><span data-stu-id="5869e-106">The code examples define the `SalesInvoicePostedBusinessEvent` event.</span></span>

1. <span data-ttu-id="5869e-107">أضف أسلوب `newFrom<my_buffer>` ثابتاً، مع ملء جزء `my_buffer` مع المخزن المؤقت للجدول الذي يتم استخدامه لتهيئة عقد حدث الأعمال.</span><span class="sxs-lookup"><span data-stu-id="5869e-107">Add a static `newFrom<my_buffer>` method, filling in the `my_buffer` piece with the table buffer that is used to initialize the business event contract.</span></span>


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
2. <span data-ttu-id="5869e-108">قم بتوسيع فئة `BusinessEventsBase`.</span><span class="sxs-lookup"><span data-stu-id="5869e-108">Extend the `BusinessEventsBase` class.</span></span> <span data-ttu-id="5869e-109">يجب تحديد التسميات لوسائط الاسم والوصف، ولكن يجب ترك الرمز "@" لتجنب تخزين البيانات المترجمة.</span><span class="sxs-lookup"><span data-stu-id="5869e-109">Labels must be defined for the name and description arguments, but the at "@" symbol should be left out to avoid storing localized data.</span></span> <span data-ttu-id="5869e-110">توفر سمة `BusinessEvents` إطار أحداث الأعمال مع معلومات حول عقد حدث الأعمال واسمه ووصفه.</span><span class="sxs-lookup"><span data-stu-id="5869e-110">The `BusinessEvents` attribute provides the business events framework with information about the business event's contract, name, and description.</span></span>

    ```xpp
    [BusinessEvents(classStr(SalesInvoicePostedBusinessEventContract)),
    "AccountsReceivable:SalesOrderInvoicePostedBusinessEventName","AccountsReceivable:SalesOrderInvoicePostedBusinessEventDescription",ModuleAxapta::SalesOrder)]
        public class SalesInvoicePostedBusinessEvent extends BusinessEventsBase
    ```
    
3. <span data-ttu-id="5869e-111">أضف أساليب `private parm` للحفاظ على الحالة الداخلية للفئة.</span><span class="sxs-lookup"><span data-stu-id="5869e-111">Add `private parm` methods to maintain the internal state of the class.</span></span>

    ```xpp
    private CustInvoiceJour parmCustInvoiceJour(CustInvoiceJour_custInvoiceJour = custInvoiceJour)
    {
        custInvoiceJour = _custInvoiceJour;
        return custInvoiceJour;
    }
    ```
    
4. <span data-ttu-id="5869e-112">أضف أسلوب `buildContract`.</span><span class="sxs-lookup"><span data-stu-id="5869e-112">Add the `buildContract` method.</span></span> <span data-ttu-id="5869e-113">يجب تزيين الأسلوب باستخدام السمتين `Wrappable(true)` و`Replaceable(true)`، وسيتم استدعاؤه فقط عند تمكين حدث أعمال لإحدى الشركات.</span><span class="sxs-lookup"><span data-stu-id="5869e-113">The method must be decorated with the `Wrappable(true)` and `Replaceable(true)` attributes, and it will only be called when a business event is enabled for a company.</span></span>

    ```xpp
   [Replaceable(true)]
   public BusinessEventsContract buildContract()
   {
      return
      SalesInvoicePostedBusinessEventContract::newFromCustInvoiceJour(custInvoiceJour);
   }
   ```

<span data-ttu-id="5869e-114">تقوم فئة عقد أحداث الأعمال بتوسيع فئة `BusinessEventsContract`.</span><span class="sxs-lookup"><span data-stu-id="5869e-114">The Business events contract class extends the `BusinessEventsContract` class.</span></span> <span data-ttu-id="5869e-115">إنها تحدد حمولة حدث الأعمال وتسمح بملء العقد في وقت التشغيل.</span><span class="sxs-lookup"><span data-stu-id="5869e-115">It defines the payload of the business event and allows the contract to be populated at runtime.</span></span>

<span data-ttu-id="5869e-116">استخدم الخطوات التالية لتوسيع فئة `BusinessEventContract` وإضافة الأساليب إلى الفئة.</span><span class="sxs-lookup"><span data-stu-id="5869e-116">Use the following steps to extend the `BusinessEventContract` class and add methods to the class.</span></span> <span data-ttu-id="5869e-117">تحدد أمثلة التعليمات البرمجية حدث `SalesInvoicePostedBusinessEventContract`.</span><span class="sxs-lookup"><span data-stu-id="5869e-117">The code examples define the `SalesInvoicePostedBusinessEventContract` event.</span></span>

1. <span data-ttu-id="5869e-118">قم بتوسيع فئة `BusinessEventContract`، مع التأكد من تزيينها بالسمة `DataContract`.</span><span class="sxs-lookup"><span data-stu-id="5869e-118">Extend the `BusinessEventContract` class, ensuring that it's  decorated with the `DataContract` attribute.</span></span>

    ```xpp
    [DataContract]
    public final class SalesInvoicePostedBusinessEventContract extends
    BusinessEventsContract
    ```

2. <span data-ttu-id="5869e-119">أضف متغيرات `private` للاحتفاظ بحالة العقد.</span><span class="sxs-lookup"><span data-stu-id="5869e-119">Add `private` variables to hold the contract state.</span></span>

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

3. <span data-ttu-id="5869e-120">أضف أسلوب تهيئة `private` باستخدام اسم `initialize`.</span><span class="sxs-lookup"><span data-stu-id="5869e-120">Add a `private` initialization method by using the `initialize` name.</span></span> <span data-ttu-id="5869e-121">تحدد هذه الطريقة الحالة الخاصة لفئة عقد حدث الأعمال، استناداً إلى البيانات التي يتم توفيرها من خلال أسلوب منشئ `static`.</span><span class="sxs-lookup"><span data-stu-id="5869e-121">This method sets the business event contract class's private state, based on data that is provided through the `static` constructor method.</span></span>

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

4. <span data-ttu-id="5869e-122">أضف أسلوب منشئ `static`.</span><span class="sxs-lookup"><span data-stu-id="5869e-122">Add a `static` constructor method.</span></span>

    ```xpp
    public static SalesInvoicePostedBusinessEventContract
    newFromCustInvoiceJour(CustInvoiceJour _custInvoiceJour)
    {
        var contract = new SalesInvoicePostedBusinessEventContract();
        contract.initialize(_custInvoiceJour);
        return contract;
    }
    ```
    
5. <span data-ttu-id="5869e-123">أضف أساليب `parm` للوصول إلى حالة العقد.</span><span class="sxs-lookup"><span data-stu-id="5869e-123">Add `parm` methods to access the contract state.</span></span> <span data-ttu-id="5869e-124">ويجب تزيين هذه الطرق باستخدام السمتين `DataMember('')` و`BusinessEventsDataMember('')`.</span><span class="sxs-lookup"><span data-stu-id="5869e-124">These methods should be decorated with the `DataMember('')` and `BusinessEventsDataMember('')` attributes.</span></span> <span data-ttu-id="5869e-125">لملء الحالة الداخلية لعقد البيانات، قد تحتاج إلى أساليب استرداد إضافية يجب أن تظهر على أنها `private` ويتم استدعاؤها من أسلوب `initialize`.</span><span class="sxs-lookup"><span data-stu-id="5869e-125">To populate the data contract's internal state, you might need additional retrieval methods, which should be shown as `private` and called from the `initialize` method.</span></span>

    ```xpp
    [DataMember('InvoiceAccount'),
    BusinessEventsDataMember("@AccountsReceivable:InvoiceAccount")]
    public CustInvoiceAccount parmInvoiceAccount(CustInvoiceAccount_invoiceAccount = invoiceAccount)
    {
        invoiceAccount = _invoiceAccount;
        return invoiceAccount;
    }
    ```
