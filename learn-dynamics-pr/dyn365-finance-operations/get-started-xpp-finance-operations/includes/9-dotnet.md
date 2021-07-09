---
ms.openlocfilehash: 127833dc7d08483cbe92966cd27b22ca8cb7b918
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071898"
---
<span data-ttu-id="93f3c-101">تحتوي مشاريع تطبيقات Finance and Operations في Visual Studio على كود X++ يتفاعل بسلاسة مع التعليمات البرمجية المكتوبة بلغات .NET الأخرى.</span><span class="sxs-lookup"><span data-stu-id="93f3c-101">Finance and Operations apps projects in Visual Studio contain X++ code that interacts smoothly with code that is written in other .NET languages.</span></span>

<span data-ttu-id="93f3c-102">يمكنك إنشاء مرجع من مشروع تطبيقات Finance and Operations إلى مكتبة الفئة C#، أو إلى أي نوع من مشاريع C# التي تنشئ تجميعاً، باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="93f3c-102">You can create a reference from a Finance and Operations apps project to a C# class library, or to any type of C# project that generates an assembly, by following these steps:</span></span>

1.  <span data-ttu-id="93f3c-103">قم بعمل إصدار من مشروع C# قبل مشروع تطبيقات Finance and Operations الذي يشير إليه ويعتمد عليه.</span><span class="sxs-lookup"><span data-stu-id="93f3c-103">Perform a build of the C# project before your Finance and Operations apps project that references and depends on it.</span></span>
2.  <span data-ttu-id="93f3c-104">تحتوي تطبيقات Finance and Operations على المراجع وتضمن نشر تجميعات C# بشكل صحيح على السحابة قبل تشغيلها.</span><span class="sxs-lookup"><span data-stu-id="93f3c-104">Finance and Operations apps comprehends the references and ensures that  the C# assemblies are deployed correctly to the cloud before being run.</span></span>
3.  <span data-ttu-id="93f3c-105">قم بإضافة مشروع مكتبة فئة C# ومشروع عمليات موحدة إلى الحل الخاص بك عن طريق تحديد قائمة **ملف** في Visual Studio وتحديد **جديد > مشروع**.</span><span class="sxs-lookup"><span data-stu-id="93f3c-105">Add a C# class library project and a Unified Operations project to your solution by selecting the **File** menu in Visual Studio and  selecting **New > Project**.</span></span> <span data-ttu-id="93f3c-106">عند إنشاء مشروع العمليات المالية، يتم إنشاء مجلد **المراجع** تلقائياً بداخله.</span><span class="sxs-lookup"><span data-stu-id="93f3c-106">When a Finance Operations project is created, a **References** folder is automatically created within it.</span></span>
4.  <span data-ttu-id="93f3c-107">يمكنك إضافة مرجع إلى مشروع C# أو تجميعات .NET أخرى داخل مستكشف الحلول.</span><span class="sxs-lookup"><span data-stu-id="93f3c-107">You can add a reference to a C# project or other .NET assemblies within Solution Explorer.</span></span> <span data-ttu-id="93f3c-108">انقر بزر الماوس الأيمن فوق مجلد **المراجع** وحدد **إضافة مرجع**.</span><span class="sxs-lookup"><span data-stu-id="93f3c-108">Right-click the **References** folder and  select **Add Reference**.</span></span>
5.  <span data-ttu-id="93f3c-109">يتم بعد ذلك إضافة عنصر مرجعي إلى المشروع الخاص بك ويتم نسخ ملف .dll إلى مجلد bin الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="93f3c-109">A reference element is then added to your project and a .dll file is copied to the bin folder of your package.</span></span> 

