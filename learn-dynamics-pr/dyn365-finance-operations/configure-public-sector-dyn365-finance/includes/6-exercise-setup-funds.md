---
ms.openlocfilehash: 717605dad41f9b38b8b3957bd9f60b881bffe868
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070613"
---
> [!NOTE]
>  <span data-ttu-id="00e42-101">يجب تنفيذ المعامل في هذه الوحدة النمطية بالتسلسل في نفس بيئة Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="00e42-101">The labs in this module should be performed in sequence in the same Dynamics 365 Finance environment.</span></span>


## <a name="scenario"></a><span data-ttu-id="00e42-102">السيناريو</span><span class="sxs-lookup"><span data-stu-id="00e42-102">Scenario</span></span>

<span data-ttu-id="00e42-103">يجب إنشاء أنواع الأموال قبل إعداد الصناديق.</span><span class="sxs-lookup"><span data-stu-id="00e42-103">Fund types must be created before you set up funds.</span></span> <span data-ttu-id="00e42-104">يجب أن يكون لكل صندوق اسم ورقم فريد ويجب عليك تعيين نوع الصندوق وفئة الصندوق.</span><span class="sxs-lookup"><span data-stu-id="00e42-104">Each fund must have a name and a unique number and must be assigned a fund type and fund class.</span></span>

## <a name="set-up-a-fund-type"></a><span data-ttu-id="00e42-105">إعداد نوع الصندوق</span><span class="sxs-lookup"><span data-stu-id="00e42-105">Set up a fund type</span></span>

1.  <span data-ttu-id="00e42-106">في شركة **USMF‎**، انتقل إلى **دفتر الأستاذ العام > دليل الحسابات > الصناديق > أنواع الصناديق**.</span><span class="sxs-lookup"><span data-stu-id="00e42-106">In the company **USMF**, go to **General ledger > Chart of accounts > Funds > Fund types**.</span></span>
2.  <span data-ttu-id="00e42-107">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="00e42-107">Select **New**.</span></span>
3.  <span data-ttu-id="00e42-108">في الحقل **نوع الصندوق**، اكتب **DEBT SERV**.</span><span class="sxs-lookup"><span data-stu-id="00e42-108">In the **Fund type** field, type **DEBT SERV**.</span></span>
4.  <span data-ttu-id="00e42-109">في حقل **الوصف**، اكتب **خدمات قروض Foreclosure**.</span><span class="sxs-lookup"><span data-stu-id="00e42-109">In the **Description** field, type **Foreclosure Loan Services**.</span></span>
5.  <span data-ttu-id="00e42-110">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="00e42-110">Select **Save**.</span></span>
6.  <span data-ttu-id="00e42-111">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="00e42-111">Select **Close**.</span></span>

## <a name="set-up-a-fund"></a><span data-ttu-id="00e42-112">إعداد صندوق</span><span class="sxs-lookup"><span data-stu-id="00e42-112">Set up a fund</span></span>

1.  <span data-ttu-id="00e42-113">انتقل إلى **دفتر الأستاذ العام > مخطط الحسابات > الصناديق > الصناديق**.</span><span class="sxs-lookup"><span data-stu-id="00e42-113">Go to **General ledger > Chart of accounts > Funds > Funds**.</span></span>
2.  <span data-ttu-id="00e42-114">حدد **جديد‏‎**.</span><span class="sxs-lookup"><span data-stu-id="00e42-114">Select **New**.</span></span>
3.  <span data-ttu-id="00e42-115">في الحقل **رقم الصندوق**، اكتب **1050**.</span><span class="sxs-lookup"><span data-stu-id="00e42-115">In the **Fund number** field, type **1050**.</span></span>
4.  <span data-ttu-id="00e42-116">في الحقل **اسم الصندوق**، اكتب **صندوق قروض Foreclosure**.</span><span class="sxs-lookup"><span data-stu-id="00e42-116">In the **Fund name** field, type **Foreclosure Loans Fund**.</span></span>
5.  <span data-ttu-id="00e42-117">في الحقل **نوع الصندوق**، حدد زر القائمة المنسدلة لفتح البحث.</span><span class="sxs-lookup"><span data-stu-id="00e42-117">In the **Fund type** field, select the drop-down button to open the lookup.</span></span>
6.  <span data-ttu-id="00e42-118">في القائمة، حدد نوع الصندوق **DEBT SERV**.</span><span class="sxs-lookup"><span data-stu-id="00e42-118">In the list, select the fund type **DEBT SERV**.</span></span>
7.  <span data-ttu-id="00e42-119">في الحقل **فئة الصندوق**، حدد **ائتماني**.</span><span class="sxs-lookup"><span data-stu-id="00e42-119">In the **Fund class** field, select **Fiduciary**.</span></span>
8.  <span data-ttu-id="00e42-120">قم بتعيين خيار **صندوق غير مستخدم في إعداد التقارير** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="00e42-120">Set the **Non-reporting fund** option to **No**.</span></span>
9.  <span data-ttu-id="00e42-121">قم بتعيين خيار **الصندوق الرئيسي** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="00e42-121">Set the **Major fund** option to **No**.</span></span>
10. <span data-ttu-id="00e42-122">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="00e42-122">Select **Save**.</span></span>
11. <span data-ttu-id="00e42-123">حدد **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="00e42-123">Select **Close**.</span></span>
