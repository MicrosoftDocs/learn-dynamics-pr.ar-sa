---
ms.openlocfilehash: 820173f007558d06a1f112220c78f7e2e36ed779
ms.sourcegitcommit: 3f08118ff49b5a2079aa627c8b1d967564a68fc9
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/13/2021
ms.locfileid: "6071060"
---
<span data-ttu-id="9b3e9-101">يؤدي التحقق من صحة رقم الحساب المصرفي الدولي (IBAN) إلى زيادة مقدار التحقق من الصحة الذي يتم إجراؤه عند إضافة رقم IBAN إلى حساب بنكي.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-101">International Bank Account Number (IBAN) validation increases the amount of validation that is done when you add an IBAN to a bank account.</span></span>

<span data-ttu-id="9b3e9-102">يتم تخزين معلومات حول بنية IBAN في المالية.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-102">Information about IBAN structure is stored in Finance.</span></span> 

<span data-ttu-id="9b3e9-103">يتم تحميل هذه المعلومات تلقائياً عند استخدام IBAN في الحسابات البنكية لأول مرة.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-103">That information is automatically loaded when you first use the IBAN on bank accounts.</span></span> <span data-ttu-id="9b3e9-104">وهي تشمل طول رقم IBAN، ورقم الحساب البنكي ومواضع البداية لرقم المسار، وطول رقم الحساب البنكي ورقم المسار.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-104">It contains the length of the IBAN, the bank account number and routing number starting positions, and the length of the bank account number and routing number.</span></span>

<span data-ttu-id="9b3e9-105">في حالة الانتقال إلى **إدارة النقد والبنوك > الإعداد > بنى IBAN**، لاحظ أن بنى IBAN لكل بلد أو منطقة يتم إعدادها تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-105">If you go to **Cash and bank management > Setup > IBAN structures**, notice that the IBAN structures for each country or region have been set up automatically.</span></span> <span data-ttu-id="9b3e9-106">وإذا كنت ترغب في تخصيص البنى لبلد أو منطقة معينين، فيمكنك تحريرها.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-106">If you want to customize the structures for a specific country or region, you can edit them.</span></span>
 
![لقطة شاشة لصفحة بنى IBAN في Finance and Operations.](../media/iban-structures.png)


<span data-ttu-id="9b3e9-108">ستكون تعريفات البنى جزءاً من كل إصدار جديد.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-108">The structure definitions will be a part of each new release.</span></span> <span data-ttu-id="9b3e9-109">يمكنك استخدام قائمة **إعادة تعيين البنى** لتحميل أحدث التعريفات بعد كل تحديث.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-109">You can use the **Reset structures** menu to load the latest definitions after each update.</span></span>

<span data-ttu-id="9b3e9-110">وإذا لم يتطابق طول IBAN مع الطول الذي تم تعريفه لكل بلد أو منطقة، فستتلقى رسالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-110">If the length of the IBAN doesn't match the length that is defined for each country or region, you will receive an error message.</span></span> <span data-ttu-id="9b3e9-111">لا يمكنك المتابعة إذا لم يتطابق طول IBAN مع الطول المحدد في بنية IBAN.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-111">You can't continue if the length of the IBAN doesn't match the length specified in the IBAN structure.</span></span>

<span data-ttu-id="9b3e9-112">يؤدي التحقق من الصحة أيضاً إلى التحقق من أن رقم الحساب البنكي يطابق جزء IBAN الذي يمثل رقم الحساب البنكي.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-112">The validation also verifies that the bank account number matches the part of the IBAN that represents the bank account number.</span></span> <span data-ttu-id="9b3e9-113">وفي حالة عدم تطابق رقم الحساب البنكي، ستتلقى رسالة تحذير.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-113">If the bank account number doesn't match, you will receive a warning message.</span></span> <span data-ttu-id="9b3e9-114">وهذه الرسالة تحذيرية فقط.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-114">This message is only a warning.</span></span> <span data-ttu-id="9b3e9-115">حيث يمكنك المتابعة حتى إذا لم يكن رقم الحساب البنكي مطابقاً.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-115">You can continue even if the bank account number doesn't match.</span></span>

<span data-ttu-id="9b3e9-116">كما يؤدي التحقق من الصحة أيضاً إلى التحقق من أن رقم التوجيه البنكي يطابق جزء IBAN الذي يمثل رقم التوجيه البنكي.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-116">The validation also verifies that the bank routing number matches the part of the IBAN that represents the bank routing number.</span></span> <span data-ttu-id="9b3e9-117">ويتضمن رقم التوجيه رقماً بنكياً وغالباً فرع بنك إضافياً.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-117">The routing number includes a bank number and often an additional bank branch.</span></span> <span data-ttu-id="9b3e9-118">وفي حالة عدم مطابقة رقم التوجيه البنكي، ستتلقى رسالة تحذير.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-118">If the bank routing number doesn't match, you will receive a warning message.</span></span> <span data-ttu-id="9b3e9-119">وهذه الرسالة تحذيرية فقط.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-119">This message is only a warning.</span></span> <span data-ttu-id="9b3e9-120">ويمكنك المتابعة حتى إذا لم يكن رقم التوجيه البنكي مطابقاً.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-120">You can continue even if the bank routing number doesn't match.</span></span>

<span data-ttu-id="9b3e9-121">يمكنك إضافة و/أو إعادة تعيين بنى IBAN في الصفحة نفسها بتحديد **جديد** في جزء الإجراءات.</span><span class="sxs-lookup"><span data-stu-id="9b3e9-121">You can add and/or reset IBAN structures on this same page by selecting **New** in the Action Pane.</span></span>



