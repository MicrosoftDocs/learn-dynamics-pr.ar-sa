---
ms.openlocfilehash: c687b6a6f71630f1d2e534c19761efb0dc683822
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070629"
---
<span data-ttu-id="378a9-101">يوفر Dynamics 365 Finance وظائف شاملة لإعداد العديد من خيارات دفع المورد.</span><span class="sxs-lookup"><span data-stu-id="378a9-101">Dynamics 365 Finance offers extensive functionality for setting up various vendor payment options.</span></span>
 
<span data-ttu-id="378a9-102">يتم إعداد خيارات الدفع هذه واستخدامها في الوحدات النمطية للحسابات الدائنة والحسابات المدينة:</span><span class="sxs-lookup"><span data-stu-id="378a9-102">These payment options are set up and used in the Accounts payable and Accounts receivable modules:</span></span>

- <span data-ttu-id="378a9-103">جداول عمليات الدفع</span><span class="sxs-lookup"><span data-stu-id="378a9-103">Payment schedules</span></span>
- <span data-ttu-id="378a9-104">أيام الدفع</span><span class="sxs-lookup"><span data-stu-id="378a9-104">Payment days</span></span>
- <span data-ttu-id="378a9-105">شروط الدفع</span><span class="sxs-lookup"><span data-stu-id="378a9-105">Terms of payment</span></span>
- <span data-ttu-id="378a9-106">الخصومات النقدية</span><span class="sxs-lookup"><span data-stu-id="378a9-106">Cash discounts</span></span>
- <span data-ttu-id="378a9-107">طرق الدفع</span><span class="sxs-lookup"><span data-stu-id="378a9-107">Methods of payment</span></span>
- <span data-ttu-id="378a9-108">رسوم الدفع</span><span class="sxs-lookup"><span data-stu-id="378a9-108">Payment fees</span></span>

<span data-ttu-id="378a9-109">وتوضح هذه الوحدة النمطية الإعداد الأساسي للحسابات الدائنة وإعداد المورد لإدارة حركات الموردين والموردين بكفاءة في Finance.</span><span class="sxs-lookup"><span data-stu-id="378a9-109">This module explains the basic setup of accounts payable and the vendor setup for efficient management of vendors and vendor transactions in Finance.</span></span>

<span data-ttu-id="378a9-110">سوف تتعرف في هذه الوحدة على كيفية:</span><span class="sxs-lookup"><span data-stu-id="378a9-110">In this module, you will learn how to:</span></span>

- <span data-ttu-id="378a9-111">تكوين مكونات الحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="378a9-111">Configure accounts payable components.</span></span>
- <span data-ttu-id="378a9-112">إنشاء مورد وصيانته.</span><span class="sxs-lookup"><span data-stu-id="378a9-112">Create and maintain a vendor.</span></span> 
- <span data-ttu-id="378a9-113">تكوين مدفوعات الموردين.</span><span class="sxs-lookup"><span data-stu-id="378a9-113">Configure vendor payments.</span></span>
- <span data-ttu-id="378a9-114">إعداد ملفات تعريف ترحيل المورد.</span><span class="sxs-lookup"><span data-stu-id="378a9-114">Set up vendor posting profiles.</span></span>
- <span data-ttu-id="378a9-115">تكوين رسوم الحسابات الدائنة.</span><span class="sxs-lookup"><span data-stu-id="378a9-115">Configure accounts payable charges.</span></span>

## <a name="prerequisites-for-accounts-payable-setup"></a><span data-ttu-id="378a9-116">إعداد المتطلبات الأساسية لإعداد الحسابات الدائنة</span><span class="sxs-lookup"><span data-stu-id="378a9-116">Prerequisites for Accounts payable setup</span></span> 

<span data-ttu-id="378a9-117">قبل أن تتمكن من إعداد الحسابات الدائنة، يجب أن تقوم بإكمال إعداد دفتر الأستاذ العام والوحدات النمطية لإدارة البنك والنقد.</span><span class="sxs-lookup"><span data-stu-id="378a9-117">Before you can set up Accounts payable, you must have completed the setup of the General ledger and Cash and bank management modules.</span></span> 

<span data-ttu-id="378a9-118">على سبيل المثال، يجب إنشاء دفاتر يومية لعملية الدفع.</span><span class="sxs-lookup"><span data-stu-id="378a9-118">For example, you must create payment journals.</span></span> <span data-ttu-id="378a9-119">يمكنك استخدام دفاتر يومية المدفوعات لدفع فواتير المورّد.</span><span class="sxs-lookup"><span data-stu-id="378a9-119">You use payment journals to pay the vendor invoices.</span></span> <span data-ttu-id="378a9-120">لتشغيل تعديلات سعر الصرف، يجب إعداد:</span><span class="sxs-lookup"><span data-stu-id="378a9-120">To run exchange rate adjustments, you need to set up:</span></span>

- <span data-ttu-id="378a9-121">أكواد العملة في صفحة **دفتر الأستاذ العام > العملات > العملات**.</span><span class="sxs-lookup"><span data-stu-id="378a9-121">Currency codes on the **General ledger > Currencies > Currencies** page.</span></span>
- <span data-ttu-id="378a9-122">أنواع سعر الصرف في الصفحة **دفتر الأستاذ العام > العملات > أنواع سعر الصرف**.</span><span class="sxs-lookup"><span data-stu-id="378a9-122">Exchange rate types on the **General ledger > Currencies > Exchange rate types** page.</span></span>
- <span data-ttu-id="378a9-123">أسعار صرف العملة في الصفحة **دفتر الأستاذ العام > العملات > أسعار صرف العملات**.</span><span class="sxs-lookup"><span data-stu-id="378a9-123">Currency exchange rates on the **General ledger > Currencies > Currency exchange rates** page.</span></span>

<span data-ttu-id="378a9-124">وأخيراً، يجب التأكد من أعداد الحسابات البنكية لاستخدام البنوك مع طرق الدفع.</span><span class="sxs-lookup"><span data-stu-id="378a9-124">Finally, you need to ensure that the bank accounts have been set up to use the banks with methods of payment.</span></span>

<span data-ttu-id="378a9-125">لمزيد من المعلومات، راجع [تكوين العملات في Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/configure-currencies-dyn365-finance/?azure-portal=true) و[تكوين إدارة البنك والنقد في Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/configure-cash-bank-management-dyn365-finance/?azure-portal=true).</span><span class="sxs-lookup"><span data-stu-id="378a9-125">For more information, see [Configure currencies in Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/configure-currencies-dyn365-finance/?azure-portal=true) and [Configure cash and bank management in Dynamics 365 Finance](https://docs.microsoft.com/learn/modules/configure-cash-bank-management-dyn365-finance/?azure-portal=true).</span></span>
