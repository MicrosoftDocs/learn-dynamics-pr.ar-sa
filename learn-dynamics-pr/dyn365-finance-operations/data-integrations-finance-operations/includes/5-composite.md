---
ms.openlocfilehash: 80cb187d55d0ce5c5e5895280278698dd6b5b013
ms.sourcegitcommit: 82ed9ded42c47064c90ab6fe717893447cd48796
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/19/2020
ms.locfileid: "6071549"
---
<span data-ttu-id="ea7af-101">الكيان المركب هو مفهوم يسمح لك بإنشاء كيان واحد باستخدام كيانات متعددة ترتبط ببعضها.</span><span class="sxs-lookup"><span data-stu-id="ea7af-101">A composite entity is a concept that allows you to build a single entity by using multiple entities that are related to each other.</span></span> <span data-ttu-id="ea7af-102">ويُستخدم المفهوم عادة في السيناريوهات التي يمكن فيها تمثيل أحد الكيانات كمستند واحد، مثلاً كرأس أمر مبيعات، وسطر أمر مبيعات ورأس فاتورة وسطر فاتورة وكتالوج مورّد.</span><span class="sxs-lookup"><span data-stu-id="ea7af-102">The concept is usually used in scenarios where an entity can be represented as a single document, such as a sales order header, sales order line, invoice header, invoice line, and vendor catalog.</span></span>

<span data-ttu-id="ea7af-103">يمكن تطبيق الكيان المركب في سيناريوهات التكامل غير المتزامنة وليس سيناريوهات OData المتزامنة.</span><span class="sxs-lookup"><span data-stu-id="ea7af-103">A composite entity is applicable in asynchronous integration scenarios rather than synchronous OData scenarios.</span></span> <span data-ttu-id="ea7af-104">لا تتوفر واجهة برمجية للكيانات المركبة بلغة X++‎، وهي معتمدة فقط لنظام أساسي لإدارة البيانات يعد جزءاً من عمليات الاستيراد و/أو التصدير المستندة إلى ملف XML.</span><span class="sxs-lookup"><span data-stu-id="ea7af-104">A programmatic interface isn't available for composite entities in X++, and is only supported for a data management platform that is part of XML file-based imports and/or exports.</span></span>

<span data-ttu-id="ea7af-105">يعد استيراد وتصدير الكيانات المركبة عملية سريعة وبسيطة داخل مساحة عمل **إدارة البيانات** في تطبيقات Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="ea7af-105">Importing and exporting composite entities is a quick and simple process within the **Data management** workspace in Finance and Operations apps.</span></span>

<span data-ttu-id="ea7af-106">لاستيراد كيان بيانات مركب أو تصديره، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ea7af-106">To import or export a composite data entity, follow these steps:</span></span>

1.  <span data-ttu-id="ea7af-107">حدد لوحة **استيراد/تصدير** في مساحة عمل **إدارة البيانات**.</span><span class="sxs-lookup"><span data-stu-id="ea7af-107">Select the **Import/Export** tile in the **Data management** Workspace.</span></span>
2.  <span data-ttu-id="ea7af-108">أدخل اسماً في حقل **الاسم**.</span><span class="sxs-lookup"><span data-stu-id="ea7af-108">Enter a name into the **Name** field.</span></span>
3.  <span data-ttu-id="ea7af-109">حدد تنسيق مصدر البيانات لعمليات الاستيراد، أو أضِف الكيان المراد تصديره.</span><span class="sxs-lookup"><span data-stu-id="ea7af-109">Select the data source format for imports or add the entity to export.</span></span>
4.  <span data-ttu-id="ea7af-110">حدد **استيراد** لعمليات الاستيراد، أو حدد **تنزيل حزمة** لإجراء عملية تصدير.</span><span class="sxs-lookup"><span data-stu-id="ea7af-110">Select **Import** for imports or select **Download package** to perform an export.</span></span> 
