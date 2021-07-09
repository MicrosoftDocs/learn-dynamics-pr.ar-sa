---
ms.openlocfilehash: 181c25467ae82c8d1fbdf232c3c2fa6e2ef84dfd
ms.sourcegitcommit: 13594cb3c8f0b1478f14aac7e239bc20317f480c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/15/2021
ms.locfileid: "6072502"
---
<span data-ttu-id="4a218-101">كما هو الحال مع **مواقع العمل** و **طلبات الصيانة**، يكون للأصول حالات دورة حياة تحدد حالة الأصل.</span><span class="sxs-lookup"><span data-stu-id="4a218-101">As with **Functional locations** and **Maintenance requests**, assets have lifecycle states that define the status of the asset.</span></span> <span data-ttu-id="4a218-102">تتضمن بعض أمثلة **‏‫حالات دورة حياة الأصول‬** كلاً من **جديد**، و **نشط**، و **منتهٍ**.</span><span class="sxs-lookup"><span data-stu-id="4a218-102">Some examples of **Asset lifecycle states** include **New**, **Active**, and **Terminated**.</span></span> <span data-ttu-id="4a218-103">يمكنك عرض الحالة الحالية للأصل في أي وقت على صفحة **كل الأصول**.</span><span class="sxs-lookup"><span data-stu-id="4a218-103">You can view the current state of an asset at any time on the **All assets** page.</span></span> 


<span data-ttu-id="4a218-104">**إدارة الأصول > إعداد > الأصول > حالات دورة الحياة**</span><span class="sxs-lookup"><span data-stu-id="4a218-104">**Asset Management > Setup > Assets > Lifecycle states**</span></span>
 
![لقطة شاشة لصفحة حالات الأصول تعرض حالة دورة الحياة "قيد الانتظار".](../media/create-asset-lifecycle-states-ssm.png)

<span data-ttu-id="4a218-106">توضح هذه الوحدة كيفية إعداد حالات دورة حياة موقع العمل.</span><span class="sxs-lookup"><span data-stu-id="4a218-106">This unit describes how to set up functional location lifecycle states.</span></span>

1.  <span data-ttu-id="4a218-107">حدد **‎إدارة الأصول > إعداد > الأصول > حالات دورة الحياة**.</span><span class="sxs-lookup"><span data-stu-id="4a218-107">Select **Asset management > Setup > Assets > Lifecycle states**.</span></span>
2.  <span data-ttu-id="4a218-108">حدد **جديد** لإنشاء حالة دورة حياة أصل جديدة.</span><span class="sxs-lookup"><span data-stu-id="4a218-108">Select **New** to create a new asset lifecycle state.</span></span>
3.  <span data-ttu-id="4a218-109">في حقل **حالة دورة الحياة**، أدخل معرّف حالة دورة الحياة.</span><span class="sxs-lookup"><span data-stu-id="4a218-109">In the **Lifecycle state** field, enter the lifecycle state ID.</span></span> <span data-ttu-id="4a218-110">‏‫وكمثال، يمكن أن يكون هذا المعرف **نشط**، و **جديد**، و **قيد الانتظار**، و **منتهٍ**، وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="4a218-110">As an example, this ID can be **Active**, **New**, **On Hold**, **Terminated**, and so on.</span></span> <span data-ttu-id="4a218-111">بالنسبة لهذا المثال، أدخل المعرّف **قيد الإصلاح"**.</span><span class="sxs-lookup"><span data-stu-id="4a218-111">For this example, enter the ID as **In Repair**.</span></span>
4.  <span data-ttu-id="4a218-112">في حقل **الاسم**، أدخل اسماً وصفياً.</span><span class="sxs-lookup"><span data-stu-id="4a218-112">In the **Name** field, enter a descriptive name.</span></span> <span data-ttu-id="4a218-113">نظراً لأن هذا الإدخال يقوم بإنشاء عنوان فرعي لعرضه، ضع اسماً في هذا الحقل يصف حالة دورة الحياة، على سبيل المثال، **الأصل قيد الإصلاح**.</span><span class="sxs-lookup"><span data-stu-id="4a218-113">Because this entry creates a subtitle to view, put a name in this field that describes the lifecycle state, for example, **Asset is in repair**.</span></span> 
    <span data-ttu-id="4a218-114">يُظهر الحقل **‏‫نماذج دورة الحياة** عدد نماذج دورة حياة الأصل التي تقترن بها حالة دورة الحياة.</span><span class="sxs-lookup"><span data-stu-id="4a218-114">The **Lifecycle models** field shows the number of asset lifecycle models that the lifecycle state is associated to.</span></span> 
5.  <span data-ttu-id="4a218-115">قم بتعيين الخيار **نشط** إلى **نعم** لتنشيط حالة دورة الحياة.</span><span class="sxs-lookup"><span data-stu-id="4a218-115">Set the **Active** option to **Yes** to activate the lifecycle state.</span></span> <span data-ttu-id="4a218-116">في حالة التنشيط، يمكن إنشاء أوامر عمل للأصل في حالة دورة الحياة.</span><span class="sxs-lookup"><span data-stu-id="4a218-116">When active, work orders can be established for the asset in the lifecycle state.</span></span>
6.  <span data-ttu-id="4a218-117">قم بتعيين خيار **حذف بنود الجدول المفتوحة** ‎إلى **‎نعم** ‎للسماح بحذف بنود الجدول المفتوحة المقترنة بحالة دورة حياة الأصل.</span><span class="sxs-lookup"><span data-stu-id="4a218-117">Set the **Delete open schedule lines** option to **Yes** to allow open schedule lines that are associated with the asset lifecycle state to be deleted.</span></span> <span data-ttu-id="4a218-118">تكمن ميزة هذا الإعداد في أن القدرة على الاحتفاظ بجداول نظيفة وحذف الجداول لم تعد قابلة للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="4a218-118">The benefit of this setting is that the ability to maintain clean schedules and delete schedules is no longer applicable.</span></span>
7.  <span data-ttu-id="4a218-119">يجب عليك **‏‫حفظ** حالة الأصل الجديدة.</span><span class="sxs-lookup"><span data-stu-id="4a218-119">**Save** your new asset state.</span></span>


> [!NOTE]
> <span data-ttu-id="4a218-120">كما قد تتذكر، عند إعداد حالات دورة حياة موقع العمل، يمكنك تكوين النظام لتحديث حالات دورة حياة الأصل تلقائياً عند تغيير حالة دورة حياة موقع العمل.</span><span class="sxs-lookup"><span data-stu-id="4a218-120">As you might recall, when setting up the Functional location lifecycle states, you can configure the system to automatically update asset lifecycle states when the functional lifecycle state changes.</span></span>  

<span data-ttu-id="4a218-121">**إدارة الأصول > إعداد > مواقع العمل > حالات دورة الحياة**</span><span class="sxs-lookup"><span data-stu-id="4a218-121">**Asset Management > Setup > Functional locations > Lifecycle states**</span></span>

![لقطة شاشة لصفحة حالات الأصول تعرض حالة دورة الحياة "نشط".](../media/asset-lifecycle-states-functional-ssm.png)


