---
ms.openlocfilehash: d648c2e725c415e3173e6ce01bdaba64ebcd4fbf
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071878"
---

<span data-ttu-id="8377c-101">لاستهلاك خدمات الويب الخارجية داخل تطبيقات Finance and Operations، يمكنك استخدام فئات برنامج التضمين.</span><span class="sxs-lookup"><span data-stu-id="8377c-101">To consume external web services within Finance and Operations apps, you can use wrapper classes.</span></span> <span data-ttu-id="8377c-102">يمكنك تضمين المنطق حول الطرق المحددة في الفئة الأساسية التي تقوم بزيادتها.</span><span class="sxs-lookup"><span data-stu-id="8377c-102">You can wrap logic around methods that are defined in the base class that you're augmenting.</span></span> 

<span data-ttu-id="8377c-103">ويعني ذلك أنه يمكنك توسيع الكود لكل من الأساليب العامة والمحمية دون الاضطرار إلى استخدام معالجات الأحداث.</span><span class="sxs-lookup"><span data-stu-id="8377c-103">This means that you can extend the code of both public and protected methods without having to use event handlers.</span></span> <span data-ttu-id="8377c-104">عندما تقوم بتضمين أسلوب لجدول أو نموذج أو كيان بيانات أو كائن آخر، عليك استخدام فئة ملحق.</span><span class="sxs-lookup"><span data-stu-id="8377c-104">When you wrap a method for a table, form, data entity, or other object, you must use an extension class.</span></span> <span data-ttu-id="8377c-105">قبل معرفة كيفية استخدام فئات برنامج التضمين للاتصال بخدمات الويب الخارجية، خذ بعين الاعتبار المثال التالي من فئة برنامج التضمين.</span><span class="sxs-lookup"><span data-stu-id="8377c-105">Before learning about how to use wrapper classes to connect to external web services, consider the following example of a wrapper class.</span></span>

```xpp
[ExtensionOf(tableStr(FMCustomer))]
final class MyFleet_Extension
{
    public void salute(str message)
    {
        // ...
    }
}
```
<span data-ttu-id="8377c-106">في نموذج الكود السابق، يتم تطبيق السمة `ExtensionOf` على الفئة، ويتم توسيع فئة جدول **FMCustomer**.</span><span class="sxs-lookup"><span data-stu-id="8377c-106">In the previous code sample, the `ExtensionOf` attribute is applied to the class, and the **FMCustomer** table class is extended.</span></span> <span data-ttu-id="8377c-107">نظراً لأن الفئة هي فئة ملحق، فيجب أن تكون `public`و`final`.</span><span class="sxs-lookup"><span data-stu-id="8377c-107">Because the class is an extension class, it must be `public` and `final`.</span></span> <span data-ttu-id="8377c-108">لا يتضمن أسلوب `salute` القيمة الافتراضية لمحدد الرسالة.</span><span class="sxs-lookup"><span data-stu-id="8377c-108">The `salute` method doesn't include the default value of the message parameter.</span></span>

<span data-ttu-id="8377c-109">يمكنك إنشاء فئات برنامج التضمين للاتصال بخدمات الويب الخارجية.</span><span class="sxs-lookup"><span data-stu-id="8377c-109">You can create wrapper classes to connect to external web services.</span></span> <span data-ttu-id="8377c-110">يمكنك القيام بذلك من خلال تضمين نقطة نهاية خدمة في Visual Studio ثم إضافة المرجع في مشروعك.</span><span class="sxs-lookup"><span data-stu-id="8377c-110">You can do this by wrapping a service endpoint in Visual Studio and then adding the reference in your project.</span></span>

> [!NOTE]
> <span data-ttu-id="8377c-111">تتوفر هذه الميزة في تحديث النظام الأساسي رقم 9 أو أحدث من تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="8377c-111">This functionality is available in Finance and Operations apps Platform update 9 or later.</span></span> <span data-ttu-id="8377c-112">لا تحتوي الأساليب التي يتم تحويلها برمجياً باستخدام إصدارات سابقة على البنية الأساسية لدعم التضمين.</span><span class="sxs-lookup"><span data-stu-id="8377c-112">Methods that are compiled by using earlier versions don't have the infrastructure to support wrapping.</span></span>
