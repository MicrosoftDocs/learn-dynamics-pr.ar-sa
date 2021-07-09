---
ms.openlocfilehash: 75387301fdcec56fca00dfd813672c576ffbb510
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071232"
---
<span data-ttu-id="4fd91-101">يمكنك استخدام `GetExecutionSummaryStatus` لكل من مهام الاستيراد والتصدير.</span><span class="sxs-lookup"><span data-stu-id="4fd91-101">You can use `GetExecutionSummaryStatus` for both import and export jobs.</span></span> <span data-ttu-id="4fd91-102">يستخدم هذا للتحقق من حالة وظيفة تشغيل مشروع البيانات.</span><span class="sxs-lookup"><span data-stu-id="4fd91-102">This is used to check the status of a data project run job.</span></span> <span data-ttu-id="4fd91-103">واجهة برمجة التطبيقات (API) هذه قابلة للتطبيق على عمليات النشر السحابية وعمليات النشر المحلية.</span><span class="sxs-lookup"><span data-stu-id="4fd91-103">This API is applicable to cloud deployments and on-premises deployments.</span></span> <span data-ttu-id="4fd91-104">ضع في اعتبارك أن الملف سيبقى في مساحة تخزين الكائنات الثنائية كبيرة الحجم لمدة سبعة أيام، وبعد ذلك سيتم حذفه تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="4fd91-104">Keep in mind that the file will remain in the Blob storage for seven days, and then it will be automatically deleted.</span></span>

<span data-ttu-id="4fd91-105">للتحقق من حالة واجهة برمجة التطبيقات (API)، استخدم `GetExecutionSummaryStatus` ثم حدد معرف التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="4fd91-105">To check the status of the API, use `GetExecutionSummaryStatus` and then specify the executionId.</span></span>

<span data-ttu-id="4fd91-106">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="4fd91-106">For example:</span></span>

```csharp
POST /data/DataManagementDefinitionGroups/Microsoft.Dynamics.DataEntities.GetExecutionSummaryStatus
BODY
{"executionId":"<executionId>"}
```
<span data-ttu-id="4fd91-107">سيتم إرسال رسالة رد JSON بنجاح وسيتم عرض حالة التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="4fd91-107">A JSON successful response message will be sent and the execution status will be displayed.</span></span> <span data-ttu-id="4fd91-108">هناك العديد من المخرجات التي قد تتلقاها في هذه الرسالة:</span><span class="sxs-lookup"><span data-stu-id="4fd91-108">There are several outputs you might receive in this message:</span></span>

-   <span data-ttu-id="4fd91-109">غير معروف</span><span class="sxs-lookup"><span data-stu-id="4fd91-109">Unknown</span></span>
-   <span data-ttu-id="4fd91-110">‏‫ليس قيد التشغيل‬</span><span class="sxs-lookup"><span data-stu-id="4fd91-110">NotRun</span></span>
-   <span data-ttu-id="4fd91-111">جارٍ التنفيذ</span><span class="sxs-lookup"><span data-stu-id="4fd91-111">Executing</span></span>
-   <span data-ttu-id="4fd91-112">ناجح</span><span class="sxs-lookup"><span data-stu-id="4fd91-112">Succeeded</span></span>
-   <span data-ttu-id="4fd91-113">نجح جزئياً</span><span class="sxs-lookup"><span data-stu-id="4fd91-113">PartiallySucceeded</span></span>
-   <span data-ttu-id="4fd91-114">فشل</span><span class="sxs-lookup"><span data-stu-id="4fd91-114">Failed</span></span>
-   <span data-ttu-id="4fd91-115">‏‫تم الإلغاء‬</span><span class="sxs-lookup"><span data-stu-id="4fd91-115">Canceled</span></span>
 