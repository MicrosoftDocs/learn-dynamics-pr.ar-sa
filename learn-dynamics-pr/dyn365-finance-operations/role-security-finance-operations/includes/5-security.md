---
ms.openlocfilehash: f66aee77b8f1e24519de90246ccb1f125f1f8627
ms.sourcegitcommit: 7d4cc5f2048fa309552e39da447684b1d06d0772
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/13/2021
ms.locfileid: "6072489"
---
<span data-ttu-id="87c38-101">يتم تعيين المستخدمين إلى أدوار الأمان في الوحدة النمطية لإدارة النظام في تطبيقات Finance and Operations من خلال الانتقال إلى **إدارة الأمان > الأمان > تكوين الأمان.**</span><span class="sxs-lookup"><span data-stu-id="87c38-101">Users are assigned to security roles in the System administration module in Finance and Operations apps by going to **Security administration > Security > Security configuration.**</span></span>

<span data-ttu-id="87c38-102">[![لقطة شاشة لصفحة "تكوين الأمان".](../media/security-1.png)](../media/security-1.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="87c38-102">[![Screenshot of the Security configuration page.](../media/security-1.png)](../media/security-1.png#lightbox)</span></span>

<span data-ttu-id="87c38-103">يمكنك تعيين مستخدمين إلى أدوار تلقائياً باستخدام استعلامات من Visual Studio، أو يمكنك تعيين مستخدم فردي لأحد الأدوار يدوياً.</span><span class="sxs-lookup"><span data-stu-id="87c38-103">You can automatically assign users to roles by using queries from Visual Studio, or you can manually assign an individual user to a role.</span></span> <span data-ttu-id="87c38-104">بالإضافة إلى ذلك، يمكنك اختيار استبعاد مستخدم من التعيين التلقائي للدور وذلك بإعادة تعيين حالته أو حالتها.</span><span class="sxs-lookup"><span data-stu-id="87c38-104">Additionally, you can choose to have a user excluded from automatic role assignment by resetting her or his status.</span></span>

<span data-ttu-id="87c38-105">اتبع الخطوات التالية لتعيين مستخدمين إلى أدوار تلقائياً:</span><span class="sxs-lookup"><span data-stu-id="87c38-105">Follow these steps to assign users to roles automatically:</span></span>

1.  <span data-ttu-id="87c38-106">في تطبيقات Finance and Operations، افتح جزء التنقل عن طريق تحديد أيقونة القائمة في الركن العلوي الأيسر من الصفحة.</span><span class="sxs-lookup"><span data-stu-id="87c38-106">In Finance and Operations apps, open the Navigation pane by selecting the menu icon in the top-left corner of the page.</span></span>
2.  <span data-ttu-id="87c38-107">وضمن عُقدة **الوحدات النمطية**، حدد **إدارة النظام**.</span><span class="sxs-lookup"><span data-stu-id="87c38-107">Under the **Modules** node, select **System administration**.</span></span>
3.  <span data-ttu-id="87c38-108">حدد **الأمان** لتوسيع العقدة، ثم حدد **تعيين مستخدمين للأدوار**.</span><span class="sxs-lookup"><span data-stu-id="87c38-108">Select **Security** to expand the node, and then select **Assign    users to roles**.</span></span>
4.  <span data-ttu-id="87c38-109">في العمود الأيمن، حدد الدور الذي ترغب في تعيين مستخدمين إليه، مثل **موظف الحسابات الدائنة**.</span><span class="sxs-lookup"><span data-stu-id="87c38-109">In the left column, select the role that you want to assign users to, such as **Accounts payable clerk**.</span></span>
5.  <span data-ttu-id="87c38-110">في العمود الأوسط، أسفل عنوان **قواعد التعيين الديناميكي للمستخدمين إلى الأدوار**، حدد **إضافة قاعدة**.</span><span class="sxs-lookup"><span data-stu-id="87c38-110">In the middle column, beneath the **Rules for dynamically assigning    users to role** heading, select **Add rule**.</span></span>
6.  <span data-ttu-id="87c38-111">حدد اسم الاستعلام المطلوب للقاعدة، مثل **LedgerJournalPostControl**.</span><span class="sxs-lookup"><span data-stu-id="87c38-111">Select your desired query name for the rule, such as **LedgerJournalPostControl**.</span></span>
7.  <span data-ttu-id="87c38-112">لتعديل الاستعلام، مثل إزالة شركة من القاعدة أو إضافة صلة جدول، حدد **تحرير الاستعلام**.</span><span class="sxs-lookup"><span data-stu-id="87c38-112">To modify the query, such as removing a company from the rule or adding a table join, select **Edit query**.</span></span>
8.  <span data-ttu-id="87c38-113">في جزء الإجراء، حدد **التشغيل التلقائي لتعيين الدور**.</span><span class="sxs-lookup"><span data-stu-id="87c38-113">In the Action Pane, select **Run automatic role assignment**.</span></span> <span data-ttu-id="87c38-114">ستشاهد المستخدمين الذين تمت إضافتهم في العمود الأوسط ضمن **المستخدمون الذين تم تعيينهم للدور**.</span><span class="sxs-lookup"><span data-stu-id="87c38-114">You will see the users that have been added in the middle column under the **Users assigned to role** heading.</span></span> 