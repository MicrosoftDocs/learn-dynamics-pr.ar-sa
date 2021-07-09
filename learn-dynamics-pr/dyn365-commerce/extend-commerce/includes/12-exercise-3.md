---
ms.openlocfilehash: 2cd3ba490a2db249f9fed72d19b94403a7ce911b
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6070077"
---
<span data-ttu-id="081de-101">كمطور تجارة إلكترونية لشركة Fabrikam، تمت مطالبتك بإنشاء وحدة نمطية جديدة.</span><span class="sxs-lookup"><span data-stu-id="081de-101">As an e-Commerce developer for the Fabrikam company, you have been asked to create a new module.</span></span> <span data-ttu-id="081de-102">وترغب الشركة في أن يطلق عليها وحدة نمطية بسيطة ستسمى **ميزة المنتج**.</span><span class="sxs-lookup"><span data-stu-id="081de-102">The company wants a simple module that will be named **Product-feature**.</span></span>

<span data-ttu-id="081de-103">ستقوم بتنفيذ المهام التالية في هذا التدريب:</span><span class="sxs-lookup"><span data-stu-id="081de-103">In this exercise, you will perform the following tasks:</span></span>

1. <span data-ttu-id="081de-104">العمل باستخدام رمز Visual Studio لإنشاء وحدة نمطية جديدة.</span><span class="sxs-lookup"><span data-stu-id="081de-104">Work in Visual Studio Code to create a new module.</span></span>
2. <span data-ttu-id="081de-105">تحديث محتوى الوحدة النمطية.</span><span class="sxs-lookup"><span data-stu-id="081de-105">Update the content in the module.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="081de-106">قبل البدء</span><span class="sxs-lookup"><span data-stu-id="081de-106">Before you begin</span></span>

<span data-ttu-id="081de-107">ستحتاج بيئة مع أدوات التطوير وتثبيت SDK ورمز Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="081de-107">You will need to have an environment with the development tools and SDK installed and Visual Studio Code.</span></span> 

## <a name="create-a-new-module"></a><span data-ttu-id="081de-108">إنشاء وحدة جديدة</span><span class="sxs-lookup"><span data-stu-id="081de-108">Create a new module</span></span> 

<span data-ttu-id="081de-109">لإنشاء وحدة جديدة، اتبع هذه الخطوات:</span><span class="sxs-lookup"><span data-stu-id="081de-109">To create a new module, follow these steps:</span></span>

1. <span data-ttu-id="081de-110">نسخ الأمر CLI</span><span class="sxs-lookup"><span data-stu-id="081de-110">Copy the CLI command</span></span> 

    ```Console 
    yarn msdyn365 add-module product-feature 
    ```

2. <span data-ttu-id="081de-111">افتح **رمز Visual Studio** وحدد نافذة **الوحدة الطرفية > وحدة طرفية جديدة** (تأكد من أن هذه النافذة موجه أوامر وليست PowerShell).</span><span class="sxs-lookup"><span data-stu-id="081de-111">Open **Visual Studio Code** and select **Terminal > New Terminal** window (ensure that this window is a Command Prompt and not a PowerShell).</span></span>
3. <span data-ttu-id="081de-112">في النافذة **وحدة طرفية جديدة**، قم بلصق الأمر الذي قمت بنسخه، ثم حدد **إدخال** لتشغيل الأمر.</span><span class="sxs-lookup"><span data-stu-id="081de-112">In the **New terminal** window, paste the command that you copied, and then select **Enter** to run the command.</span></span> 
4. <span data-ttu-id="081de-113">في نفس النافذة، قم بتشغيل خادم العقدة مع الأمر `yarn start`.</span><span class="sxs-lookup"><span data-stu-id="081de-113">In the same window, run the Node Server with the command `yarn start`.</span></span>
5. <span data-ttu-id="081de-114">من بيئة الاختبار المعزولة (`https://localhost:4000/_sdk/allmodules`)، حدد **ميزة الوحدة**، التي ستعرض المحتوى المحدد الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="081de-114">From the sandbox environment (`https://localhost:4000/_sdk/allmodules`), select the **Product feature** module, which will display the default defined content.</span></span>
6. <span data-ttu-id="081de-115">لتحديث المحتوى، ارجع إلى الملف **الرمز المقابل > الوحدات النمطية > ميزة المنتج > عرض ميزة المنتج.tsx**.</span><span class="sxs-lookup"><span data-stu-id="081de-115">To update the content, return to the **VS Code>Modules>product-feature>product-feature.view.tsx** file.</span></span>
7. <span data-ttu-id="081de-116">افتح الملف وقم بتحديث المحتوى في علامات **<h2\>** من التنسيق HTML.</span><span class="sxs-lookup"><span data-stu-id="081de-116">Open the file and update the content in the **<h2\>** tags from the HTML format.</span></span> <span data-ttu-id="081de-117">أدخل **مرحباً** قبل **قيمة التكوين** ثم أدخل **العالم** قبل **قيمة المورد**.</span><span class="sxs-lookup"><span data-stu-id="081de-117">Enter **Hello** before **Config Value** and then enter **World** before **Resource Value**.</span></span>  
8. <span data-ttu-id="081de-118">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="081de-118">Select **Save**.</span></span> 
9. <span data-ttu-id="081de-119">قم بتحديث الصفحة.</span><span class="sxs-lookup"><span data-stu-id="081de-119">Refresh the page.</span></span> <span data-ttu-id="081de-120">يجب أن يُظهر أول صفين **مرحباً من العالم** قبل النص الآخر.</span><span class="sxs-lookup"><span data-stu-id="081de-120">The first two rows should show **Hello World** before the other text.</span></span> 


