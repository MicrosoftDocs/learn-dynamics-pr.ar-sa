---
ms.openlocfilehash: 6f937b8daf1b47e63da5b12e671833ca66701293
ms.sourcegitcommit: 0af0a6f1739b0e2a5ec60989ffbf8aa131de41c3
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/08/2021
ms.locfileid: "6072234"
---
<span data-ttu-id="a606e-101">لعرض محتوى على صفحة في واجهة المستخدم، يجب إضافة مصدر بيانات إلى نموذج في نافذة مصمم النماذج لـ Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="a606e-101">To display content on a page in the  user interface, a data source must be added to a form in the form designer window of Visual Studio.</span></span> <span data-ttu-id="a606e-102">يمكنك تحديد وسحب جدول أو استعلام من مشروعك في نافذة **مستكشف الحلول** أو سحب جدول نظام من نافذة **مستكشف التطبيقات**.</span><span class="sxs-lookup"><span data-stu-id="a606e-102">You can select and drag a table or query from your project in the **Solution Explorer** window or drag a system table from the **Application Explorer** window.</span></span> <span data-ttu-id="a606e-103">يمكنك اختيار استخدام جدول واحد أو عدة جداول، بناءً على عدد الحقول التي ستستخدمها في النموذج الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a606e-103">You can choose to use one table or many tables, depending on the number of fields that you will use for your form.</span></span> 

<span data-ttu-id="a606e-104">[![لقطة شاشة لنافذة مصمم نماذج Visual Studio مع تمييز خيارت مصادر البيانات.](../media/data-source.png)](../media/data-source.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="a606e-104">[![Screenshsot of the Visual Studio Form designer window highlighting Data Sources options.](../media/data-source.png)](../media/data-source.png#lightbox)</span></span>

<span data-ttu-id="a606e-105">اتبع هذه الخطوات لإضافة مصدر بيانات من شجرة مكونات البرنامج (AOT) إلى النموذج باستخدام عملية التحديد والسحب:</span><span class="sxs-lookup"><span data-stu-id="a606e-105">Follow these steps to add a data source from the Application Object Tree (AOT) to your form by using a select and drag process:</span></span>

1.  <span data-ttu-id="a606e-106">تأكد من أن النموذج الخاص بك مفتوح في نافذة مصمم النماذج في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="a606e-106">Ensure that your form is open in the form designer window in Visual    Studio.</span></span>
2.  <span data-ttu-id="a606e-107">في نافذة **مستكشف التطبيقات**، قم بتوسيع عقدة **AOT**.</span><span class="sxs-lookup"><span data-stu-id="a606e-107">In the **Application Explorer** window, expand the **AOT** node.</span></span>
3.  <span data-ttu-id="a606e-108">قم بتوسيع عقدة **نموذج البيانات**.</span><span class="sxs-lookup"><span data-stu-id="a606e-108">Expand the **Data Model** node.</span></span>
4.  <span data-ttu-id="a606e-109">قم بتوسيع عقدة **الجداول** أو **ملحقات الجداول**، حسب نوع مصدر البيانات الذي تقوم بإضافته.</span><span class="sxs-lookup"><span data-stu-id="a606e-109">Expand the **Tables** or **Table Extensions** node, depending on the    type of data source that you are adding.</span></span>
5.  <span data-ttu-id="a606e-110">حدد الجدول المطلوب واسحبه من عقدة **AOT** إلى عقدة **مصادر البيانات** في الجزء الأيمن من إطار مصمم النماذج.</span><span class="sxs-lookup"><span data-stu-id="a606e-110">Select and drag your desired table from the **AOT** node to the **Data Sources** node in the left pane of the form designer window.</span></span>

<span data-ttu-id="a606e-111">وبدلاً من ذلك، يمكنك إضافة مصدر بيانات إلى النموذج الخاص بك باستخدام عقدة **مصادر البيانات** في في مصمم النماذج.</span><span class="sxs-lookup"><span data-stu-id="a606e-111">Alternatively, you can add a data source to your form by using the **Data Sources** node in the form designer.</span></span>

<span data-ttu-id="a606e-112">اتبع الخطوات التالية لإضافة مصدر بيانات من المشروع:</span><span class="sxs-lookup"><span data-stu-id="a606e-112">Follow these steps to add a data source from your project:</span></span>

1.  <span data-ttu-id="a606e-113">تأكد من أن النموذج الخاص بك مفتوح في نافذة مصمم النماذج في Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="a606e-113">Ensure that your form is open in the form designer window in Visual     Studio.</span></span>
2.  <span data-ttu-id="a606e-114">في الجزء الأيمن من المصمم، انقر بزر الماوس الأيمن فوق عقدة **مصادر البيانات** وحدد **مصدر بيانات جديد**.</span><span class="sxs-lookup"><span data-stu-id="a606e-114">In the left pane of the designer, right-click the **Data Sources**    node and select **New Data Source**.</span></span>
3.  <span data-ttu-id="a606e-115">حدد **DataSource1** ضمن عُقدة **مصادر البيانات** وانتقل إلى نافذة **الخصائص**.</span><span class="sxs-lookup"><span data-stu-id="a606e-115">Select **DataSource1** under the **Data Sources** node and go to the **Properties** window.</span></span>
4.  <span data-ttu-id="a606e-116">حدد جدولك في القائمة المنسدلة لخاصية **الجدول**.</span><span class="sxs-lookup"><span data-stu-id="a606e-116">Select your table in the **Table** property drop-down menu.</span></span> <span data-ttu-id="a606e-117">يمكنك أيضاً تحديد أي جدول من عقدة **AOT** في هذه القائمة.</span><span class="sxs-lookup"><span data-stu-id="a606e-117">You can    also select any table from the **AOT** node in this menu.</span></span>
