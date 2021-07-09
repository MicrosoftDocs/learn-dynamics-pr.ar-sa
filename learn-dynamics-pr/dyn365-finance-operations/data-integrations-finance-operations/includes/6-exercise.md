---
ms.openlocfilehash: 2daa05a951b832ca1f6522526bcba42dfa8ee09b
ms.sourcegitcommit: 0484f01637a384540476f9c6e45ba64bd86526a8
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/19/2021
ms.locfileid: "6072126"
---
<span data-ttu-id="3d630-101">تمت مطالبتك بإنشاء مشروع بيانات جديد يقوم باستيراد بيانات على أساس متكرر، لشركة Fleet Management لتصدير أوامر المبيعات الخاصة بها شهرياً.</span><span class="sxs-lookup"><span data-stu-id="3d630-101">You have been asked to create a new data project that will import data on a recurring basis, for the Fleet Management company to export its sales orders monthly.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="3d630-102">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="3d630-102">Before you begin</span></span> 

<span data-ttu-id="3d630-103">للحصول على أقصى استفادة من هذا التدريب، نوصيك بأن يكون متوفر لديك بيانات العينة القياسية المتوفرة في تطبيقات Finance and Operations والتي يتم تثبيتها باستخدام Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="3d630-103">To get the most benefit from this exercise, we recommend that you have the standard sample data available in Finance and Operations apps installed by using Lifecycle Services (LCS).</span></span> <span data-ttu-id="3d630-104">ستحتاج أيضاً إلى بيئة اختبار معزولة للمطورين وترخيص تجريبي أو دائم باستخدام Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="3d630-104">You will also need a developer sandbox environment and a trial or permanent license for using Visual Studio.</span></span>

## <a name="create-a-recurring-data-job"></a><span data-ttu-id="3d630-105">إنشاء وظيفة بيانات متكررة</span><span class="sxs-lookup"><span data-stu-id="3d630-105">Create a recurring data job</span></span> 

1.  <span data-ttu-id="3d630-106">في البيئة الخاصة بك، افتح "مستكشف الملفات".</span><span class="sxs-lookup"><span data-stu-id="3d630-106">In your environment, open File Explorer.</span></span> 
2.  <span data-ttu-id="3d630-107">انتقل إلى c:\temp.</span><span class="sxs-lookup"><span data-stu-id="3d630-107">Navigate to c:\temp.</span></span>
3.  <span data-ttu-id="3d630-108">أضف مجلداً باسم "dixf".</span><span class="sxs-lookup"><span data-stu-id="3d630-108">Add a folder named “dixf”.</span></span>
4.  <span data-ttu-id="3d630-109">افتح التطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="3d630-109">Open Finance and Operations apps.</span></span>
2.  <span data-ttu-id="3d630-110">انتقل إلى **مساحات العمل > إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="3d630-110">Go to **Workspaces > Data management**.</span></span>
3.  <span data-ttu-id="3d630-111">حدد لوحة **الاستيراد** أو **التصدير** لإنشاء مشروع بيانات جديد.</span><span class="sxs-lookup"><span data-stu-id="3d630-111">Select the **Import** or **Export** tile to create a new data project.</span></span>
4.  <span data-ttu-id="3d630-112">أدخل **مبيعات الأساطيل** لاسم وظيفة صالح.</span><span class="sxs-lookup"><span data-stu-id="3d630-112">Enter **Fleet sales** for a valid job name.</span></span>
5.  <span data-ttu-id="3d630-113">حدد **Excel** لتنسيق البيانات الهدف.</span><span class="sxs-lookup"><span data-stu-id="3d630-113">Select **Excel** for the target data format.</span></span>
6.  <span data-ttu-id="3d630-114">أدخل **رؤوس أوامر المبيعات** لاسم الكيان.</span><span class="sxs-lookup"><span data-stu-id="3d630-114">Enter **Sales order headers V2** for the entity name.</span></span>
7.  <span data-ttu-id="3d630-115">حدد **إضافة كيان**.</span><span class="sxs-lookup"><span data-stu-id="3d630-115">Select **Add Entity**.</span></span>
8.  <span data-ttu-id="3d630-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3d630-116">Select **Save**.</span></span>
9.  <span data-ttu-id="3d630-117">من الصفحة **مشروع بيانات مبيعات الأساطيل**، حدد **إنشاء وظيفة بيانات متكررة**.</span><span class="sxs-lookup"><span data-stu-id="3d630-117">On the **Fleet sales Data project** page, select **Create recurring data job**.</span></span>
10. <span data-ttu-id="3d630-118">أدخل **تصدير مبيعات الأساطيل** لاسم صالح لوظيفة البيانات المتكررة.</span><span class="sxs-lookup"><span data-stu-id="3d630-118">Enter **Fleet sales export** for a valid name for the recurring data job.</span></span>
11. <span data-ttu-id="3d630-119">في علامة التبويب **إعداد سياسة التخويل**، أدخل معرف التطبيق الذي تم إنشاؤه للتطبيق الخاص بك، وحدده باعتبار أن تم تمكينه.</span><span class="sxs-lookup"><span data-stu-id="3d630-119">On the **Set up authorization policy** tab, enter the application ID that was generated for your application, and select it as enabled.</span></span>
12. <span data-ttu-id="3d630-120">حدد **تعيين تكرار المعالجة**.</span><span class="sxs-lookup"><span data-stu-id="3d630-120">Select **Set processing recurrence**.</span></span>
13. <span data-ttu-id="3d630-121">في مربع الحوار **تحديد التكرار**، قم بإعداد تكرار صالح لوظيفة البيانات الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="3d630-121">In the **Define recurrence** dialog box, set up a valid recurrence for your data job.</span></span>
14. <span data-ttu-id="3d630-122">حدد نمط التكرار **أشهر** والعدد إلى **1**.</span><span class="sxs-lookup"><span data-stu-id="3d630-122">Select the recurrence pattern of **Months** and the count to **1**.</span></span>
15. <span data-ttu-id="3d630-123">اختياري: حدد **تعيين تكرار المراقبة** وقم بإعداد تكرار مراقبة.</span><span class="sxs-lookup"><span data-stu-id="3d630-123">Optional: Select **Set monitoring recurrence** and set up a monitoring recurrence.</span></span> 
