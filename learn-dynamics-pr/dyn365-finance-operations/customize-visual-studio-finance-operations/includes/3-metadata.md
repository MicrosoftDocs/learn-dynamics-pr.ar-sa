---
ms.openlocfilehash: 95f52a082bb7dd3803d53c148a7347987683e990
ms.sourcegitcommit: 376bcfca0ae39f70ac627a080fe4b4c3db34e466
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "6072266"
---
<span data-ttu-id="15aab-101">تتوفر بيانات التعريف في النماذج الحالية في "مستكشف التطبيقات".</span><span class="sxs-lookup"><span data-stu-id="15aab-101">Metadata in existing models is available in the Application Explorer.</span></span>
<span data-ttu-id="15aab-102">يحتوي مستكشف التطبيقات على شجرة مكونات البرنامج (AOT)، التي تحتوي طريقتي عرض: طريقة عرض النموذج وطريقة العرض الكلاسيكية.</span><span class="sxs-lookup"><span data-stu-id="15aab-102">The Application Explorer contains the Application Object Tree (AOT), which has two views: the model view and the classic view.</span></span>

<span data-ttu-id="15aab-103">[![رسم متحرك لطرق عرض شجرة مكونات البرنامج.](../media/aot-view.gif)](../media/aot-view.gif#lightbox)</span><span class="sxs-lookup"><span data-stu-id="15aab-103">[![Animation of the Application Object Tree views.](../media/aot-view.gif)](../media/aot-view.gif#lightbox)</span></span>


-   <span data-ttu-id="15aab-104">تنظم طريقة عرض النموذج بيانات التعريف حسب النموذج الذي يحتوي عليها، وهو أمر مفيد عندما تتصفح العناصر ذات الصلة بميزات نموذج معين.</span><span class="sxs-lookup"><span data-stu-id="15aab-104">The model view organizes metadata by the model that contains it, which is useful when you are browsing for elements that are related to a certain model's features.</span></span>
-   <span data-ttu-id="15aab-105">تجمع طريقة العرض الكلاسيكية عناصر البيانات الوصفية حسب نوعها، وهو أمر أكثر فائدة عندما تعرف نوع العنصر الذي تحتاجه وليس الوحدة النمطية التي تحتوي عليه.</span><span class="sxs-lookup"><span data-stu-id="15aab-105">The classic view groups metadata elements by their type, which is more helpful when you know what kind of element that you need but not which module contains it.</span></span>
 
<span data-ttu-id="15aab-106">تتضمن أنواع بيانات التعريف:</span><span class="sxs-lookup"><span data-stu-id="15aab-106">The metadata types include:</span></span>

-   <span data-ttu-id="15aab-107">**أنواع البيانات الموسعة (EDT)** إذا كنت قد قمت بالبرمجة من قبل، فقد تفكر في هذه الأنواع على أنها أنواع أولية: القيمة المنطقية والسلسلة وحقيقية والعدد الصحيح والمعرف الفريد العمومي (GUID) والحاوية والوقت والتاريخ والتعداد.</span><span class="sxs-lookup"><span data-stu-id="15aab-107">**Extended Data Types (EDTs)** If you have programmed before, you might think of these as primitive types: Boolean, String, Real, Integer, Globally Unique Identifier (GUID), Container, Time, Date, and Enum.</span></span>
-   <span data-ttu-id="15aab-108">**التعدادات** نوع ذو قيمة يتم اختيارها من قائمة محددة مسبقاً.</span><span class="sxs-lookup"><span data-stu-id="15aab-108">**Enums** A type with a value that is chosen from a predefined list.</span></span> <span data-ttu-id="15aab-109">قد يكون أحد الأمثلة هو يوم من أيام الأسبوع، والذي يجب أن يكون يوم الاثنين أو الثلاثاء أو الأربعاء أو الخميس أو الجمعة أو السبت أو الأحد.</span><span class="sxs-lookup"><span data-stu-id="15aab-109">One example might be a weekday, which must be one of Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, or Sunday.</span></span> <span data-ttu-id="15aab-110">يحتوي التعداد قيمة كبيرة لأنه يتم تخزين قيم التعداد كقيم تعداد في قاعدة البيانات، بدلاً من قيمة السلسلة الكاملة.</span><span class="sxs-lookup"><span data-stu-id="15aab-110">An enum has great value because the enum values are stored as enum values in the database, rather than the full string value.</span></span> 
-   <span data-ttu-id="15aab-111">**الجداول** تنظم البيانات في صفوف وأعمدة.</span><span class="sxs-lookup"><span data-stu-id="15aab-111">**Tables** Organize data into rows and columns.</span></span>
-   <span data-ttu-id="15aab-112">**النماذج** عناصر واجهة المستخدم التي تحصل على صفحتها الخاصة في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="15aab-112">**Forms** User interface elements that get their own page in Finance and Operations apps.</span></span>
-   <span data-ttu-id="15aab-113">**كيانات البيانات** هي عبارة عن ملخص لجداول قاعدة البيانات المستخدمة في عمليات التكامل واستيراد/تصدير البيانات والمزيد.</span><span class="sxs-lookup"><span data-stu-id="15aab-113">**Data entities** are an abstraction of database tables that are used for integrations, data import/export, and more.</span></span> 

<span data-ttu-id="15aab-114">إذا لم تكن طرق العرض هذه كافية لمساعدتك في العثور على العناصر التي تحتاجها، فيمكنك أيضاً تصفية AOT عن طريق إدخال اسم الحقل، متبوعاً بنقطتين ومسافة، ثم متبوعاً بقيمة.</span><span class="sxs-lookup"><span data-stu-id="15aab-114">If these views are not sufficient to help you find the elements that you need, you can also filter the AOT by entering the field name, followed by a colon and a space, and then followed by a value.</span></span> <span data-ttu-id="15aab-115">إذا كنت تبحث عن عنصر تم إنشاؤه مؤخراً، ولكن لا يمكنك العثور على ما تحتاجه، فحاول استخدام الزر **تحديث** للتأكد من أن AOT تحتوي على أحدث البيانات.</span><span class="sxs-lookup"><span data-stu-id="15aab-115">If you are looking for a recently created element, but cannot find what you need, try using the **Refresh** button to make sure that the AOT has the latest data.</span></span> 

<span data-ttu-id="15aab-116">لعرض أنواع عوامل التصفية التي يمكنك استخدامها في AOT، حدد حقل **البحث** وابدأ الكتابة في مستكشف التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="15aab-116">To view the types of filters you can use in the AOT, select the **Search** field and begin typing in the Application explorer.</span></span> <span data-ttu-id="15aab-117">ستظهر قائمة بعوامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="15aab-117">The list of filters will appear.</span></span> 

<span data-ttu-id="15aab-118">[![رسم متحرك لعامل تصفية شجرة مكونات البرنامج.](../media/aot-filter.gif)](../media/aot-filter.gif#lightbox)</span><span class="sxs-lookup"><span data-stu-id="15aab-118">[![Animation of the Application Object Tree filter.](../media/aot-filter.gif)](../media/aot-filter.gif#lightbox)</span></span>

