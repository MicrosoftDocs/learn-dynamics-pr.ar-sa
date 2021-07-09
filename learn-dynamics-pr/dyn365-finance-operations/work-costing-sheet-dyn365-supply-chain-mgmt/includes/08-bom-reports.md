---
ms.openlocfilehash: ad7afb58d4853b8cde6c36000158a5a99c0fb002
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6073514"
---

<span data-ttu-id="bc45d-101">تقرير **أماكن الاستخدام** هو المكان الذي يمكنك من خلاله معرفة مكان استخدام قائمة مكونات الصنف (BOM).</span><span class="sxs-lookup"><span data-stu-id="bc45d-101">The **Where-used** report is where you can find out where a BOM has been used.</span></span>

<span data-ttu-id="bc45d-102">يمكنك استخدام تقارير BOM لتوفير البيانات المطبوعة المرتبطة ببنى BOM للتأكد من مكان استخدام الأصناف ولعرض نتائج حساب BOM.</span><span class="sxs-lookup"><span data-stu-id="bc45d-102">You can use BOM reports to provide printed data that is related to BOM structures to ascertain where the items are used and to view BOM calculation results.</span></span>

<span data-ttu-id="bc45d-103">يستخدم الموظفون الذين يقومون بإنشاء قوائم BOM وتعديلها الوظائف الدفعية ووظائف التشغيل التلقائي التي تمنع الأخطاء التي يمكن أن تحدث عند إجراء تغييرات يدوية على قوائم BOM.</span><span class="sxs-lookup"><span data-stu-id="bc45d-103">Employees who create and modify BOMs use batch jobs and automated functions that prevent errors that can occur when manual changes are made to BOMs.</span></span>

<span data-ttu-id="bc45d-104">على سبيل المثال، يمكن للموظفين استخدام الوظيفة الدفعية للتحكم في التحديثات الشاملة عند تغيير مكونات BOM، ويمكنهم تشغيل فحوصات التحقق من صحة BOM للتحقق من عدم حدوث أخطاء في بنى BOM.</span><span class="sxs-lookup"><span data-stu-id="bc45d-104">For example, employees can use a batch job to control mass updates when changing BOM components, and can run BOM validation checks to verify that no errors occur in the BOM structures.</span></span>

<span data-ttu-id="bc45d-105">يمكن تصفية تقرير **أماكن الاستخدام** لسطور BOM أو إصداراتها:</span><span class="sxs-lookup"><span data-stu-id="bc45d-105">The **Where-used** report can be filtered for BOM lines or versions:</span></span>

-   <span data-ttu-id="bc45d-106">**سطور BOM** - يتم عرض رقم الصنف بقوائم BOM المرتبطة المدرجة.</span><span class="sxs-lookup"><span data-stu-id="bc45d-106">**BOM lines** - The item number is displayed with the related BOMs that are listed.</span></span> <span data-ttu-id="bc45d-107">يتضمن هذا الخيار أيضاً معلومات أخرى متعلقة بسطر BOM مثل الكميات والوحدات وأنواع السطور ومجموعات التكوين.</span><span class="sxs-lookup"><span data-stu-id="bc45d-107">This option also includes other BOM line related information such as quantities, units, line types, and configuration groups.</span></span>

-   <span data-ttu-id="bc45d-108">**الإصدارات** - يتم عرض رقم الصنف مع أرقام الأصناف المرتبطة (الإصدارات) وقوائم BOM المدرجة.</span><span class="sxs-lookup"><span data-stu-id="bc45d-108">**Versions** - The item number is displayed with the related item numbers (versions) and BOMs that are listed.</span></span> <span data-ttu-id="bc45d-109">يتضمن هذا الخيار أيضاً المعلومات المتعلقة بالإصدار مثل تواريخ صلاحية الإصدار وما إذا كان الإصدار/الإصدارات معتمدة ونشطة.</span><span class="sxs-lookup"><span data-stu-id="bc45d-109">This option also includes version-related information such as version validity dates and whether the version(s) is approved and active.</span></span>

<span data-ttu-id="bc45d-110">يساعد تقرير **أماكن الاستخدام** في تحديد موقع المكونات ومعلومات BOM ذات الصلة عندما يكون أحد مكونات BOM معيباً ويكون التغيير مطلوباً.</span><span class="sxs-lookup"><span data-stu-id="bc45d-110">The **Where-used** report helps locate components and the related BOM information when a BOM component is defective and a change is required.</span></span>

<span data-ttu-id="bc45d-111">يمكن أن يحتوي إصدار التكلفة على محتوى حول سجلات أسعار شراء الصنف.</span><span class="sxs-lookup"><span data-stu-id="bc45d-111">A costing version can contain content about item purchase price records.</span></span>
<span data-ttu-id="bc45d-112">الغرض الأساسي من السماح بمحتوى سعر الشراء هو تحديد سجلات أسعار الشراء لأصناف المكونات، والتي يمكن استخدامها بعد ذلك لحساب تكاليف الأصناف المصنعة.</span><span class="sxs-lookup"><span data-stu-id="bc45d-112">The primary purpose of allowing purchase price content is to define purchase price records for component items, which can then be used to calculate the costs of manufactured items.</span></span>

<span data-ttu-id="bc45d-113">لدعم هذا الغرض، يجب على المستخدم تحديد مجموعة حساب BOM تحتوي على نموذج سعر تكلفة لسعر شراء الصنف، وتعيين مجموعة حساب BOM للأصناف المشتراة.</span><span class="sxs-lookup"><span data-stu-id="bc45d-113">To support this purpose, the user must define a BOM calculation group that contains a cost price model of the item purchase price, and assign the BOM calculation group to purchased items.</span></span> <span data-ttu-id="bc45d-114">بعد ذلك، يجب على المستخدم تطبيق نموذج سعر التكلفة لمجموعة حساب BOM عند إجراء حسابات BOM بالتكاليف المخططة لحساب سعر مبيعات الأصناف المصنعة.</span><span class="sxs-lookup"><span data-stu-id="bc45d-114">Then, the user must apply a cost price model of BOM calculation group when performing BOM calculations with planned costs to calculate the sales price of manufactured items.</span></span>
