---
ms.openlocfilehash: 2806a1fd82ef993f1477fe2a791ba0701f053cbe
ms.sourcegitcommit: 221c56e4fce366780f005ef07d331b5011a9c0e1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "6072445"
---
<span data-ttu-id="e3d00-101">يمكنك استخدام Microsoft Dataverse لتمكين تدفق البيانات بين تطبيقات Finance and Operations وDynamics 365 Sales باستخدام وظيفة الكتابة المزدوجة.</span><span class="sxs-lookup"><span data-stu-id="e3d00-101">You can use Microsoft Dataverse to enable the flow of data between Finance and Operations apps and Dynamics 365 Sales by using the dual-write functionality.</span></span> 

<span data-ttu-id="e3d00-102">على سبيل المثال، يمكن أن تتدفق معلومات العميل في قسم المبيعات إلى Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="e3d00-102">For example, customer information in Sales can flow to Finance and Operations.</span></span> <span data-ttu-id="e3d00-103">لا يتعين عليك نقل البيانات يدوياً أو استخدام أداة تكامل بيانات تابعة لجهة خارجية.</span><span class="sxs-lookup"><span data-stu-id="e3d00-103">You don’t have to manually move the data or use a third-party data integration tool.</span></span>

<span data-ttu-id="e3d00-104">لفهم استخدام Dataverse بشكل أفضل، ضع في اعتبارك سيناريو النقد المحتمل.</span><span class="sxs-lookup"><span data-stu-id="e3d00-104">To better understand using Dataverse, consider the prospect to cash scenario.</span></span> <span data-ttu-id="e3d00-105">يوفر حل العميل المتوقع إلى النقدية مزامنة مباشرة عبر تطبيقات Finance and Operations وSales.</span><span class="sxs-lookup"><span data-stu-id="e3d00-105">The Prospect to cash solution provides direct synchronization across Finance and Operations apps and Sales.</span></span> 

<span data-ttu-id="e3d00-106">يمكنك تنزيل حل **العميل المتوقع إلى النقدية في Dynamics 365** من [AppSource](https://appsource.microsoft.com/?azure-portal=true)</span><span class="sxs-lookup"><span data-stu-id="e3d00-106">You can download the **Dynamics 365, Prospect to Cash** solution from [AppSource](https://appsource.microsoft.com/?azure-portal=true)</span></span>

<span data-ttu-id="e3d00-107">تتيح قوالب العميل المتوقع إلى النقدية المتوفرة مع ميزة تكامل البيانات تدفق البيانات للحسابات وجهات الاتصال والمنتجات وعروض أسعار المبيعات وأوامر المبيعات وفواتير المبيعات بين تطبيقات Finance and Operations وSales.</span><span class="sxs-lookup"><span data-stu-id="e3d00-107">The Prospect to cash templates that are available with the data integration feature enable the flow of data for accounts, contacts, products, sales quotations, sales orders, and sales invoices between Finance and Operations apps and Sales.</span></span> 

<span data-ttu-id="e3d00-108">بينما يتم تدفق البيانات بين Finance and Operations وSales، يمكنك تنفيذ أنشطة المبيعات والتسويق في المبيعات، ويمكنك التعامل مع تنفيذ الطلبات باستخدام إدارة المخزون في Dynamics 365 Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="e3d00-108">While data is flowing between Finance and Operations and Sales, you can perform sales and marketing activities in Sales, and you can handle order fulfillment by using inventory management in Dynamics 365 Supply Chain Management.</span></span>

<span data-ttu-id="e3d00-109">لمزيد من المعلومات حول كيفية استخدام كيانات البيانات وتجهيزها لتكامل البيانات باستخدام Dataverse، راجع [التعامل مع إدارة البيانات في تطبيقات Finance and Operations ](https://docs.microsoft.com/learn/modules/work-data-management-finance-operations/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="e3d00-109">For more information on how to use data entities and prepare them for data integration using Dataverse see  [Work with data management in Finance and Operations apps](https://docs.microsoft.com/learn/modules/work-data-management-finance-operations/?azure-portal=true).</span></span> 


## <a name="dual-write"></a><span data-ttu-id="e3d00-110">الكتابة المزدوجة</span><span class="sxs-lookup"><span data-stu-id="e3d00-110">Dual-write</span></span>
<span data-ttu-id="e3d00-111">إذا كنت ترغب في تكامل تطبيقات Finance and Operations مع تطبيقات Dynamics 365 الأخرى مثل Dynamics 365 Sales، يمكنك استخدام الكتابة المزدوجة.</span><span class="sxs-lookup"><span data-stu-id="e3d00-111">If you want to seamlessly integrate Finance and Operations apps with other Dynamics 365 applications such as Dynamics 365 Sales, you can use dual-write.</span></span> 

<span data-ttu-id="e3d00-112">ببضع نقرات، ستتمكن من ربط Finance and Operations بـ Dataverse لإرسال البيانات من تطبيق إلى آخر.</span><span class="sxs-lookup"><span data-stu-id="e3d00-112">With just a few clicks, you will be able to connect Finance and Operations with the Dataverse to send data from one application to another.</span></span> <span data-ttu-id="e3d00-113">اختيارياً، يمكن لمسؤولي Finance and Operations استخدام إصدار متقدم من الإعداد، حيث يمكنهم تخصيص الكيانات وتعيينات الحقول وأيضاً إجراء تصفية وتحويل لبيانات المصدر.</span><span class="sxs-lookup"><span data-stu-id="e3d00-113">Optionally, Finance and Operations admins can use an advanced version of the setup, in which they can customize entities and field mappings and also do source data filtering and transformation.</span></span>

<span data-ttu-id="e3d00-114">لإعداد الكتابة المزدوجة، ستحتاج إلى استخدام مساحة العمل **إدارة البيانات** وتحديد الإطار المتجانب **الكتابة المزدوجة** في قسم **الملخص**.</span><span class="sxs-lookup"><span data-stu-id="e3d00-114">To set up dual-write, you will need to use the **Data management** workspace and select the **Dual write** tile in the **Summary** section.</span></span>

![لقطة شاشة لمساحة عمل إدارة البيانات تُبرز مربع الكتابة المزدوجة.](../media/data-management.png)
