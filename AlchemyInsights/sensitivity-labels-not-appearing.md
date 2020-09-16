---
title: Jutīguma etiķetes netiek rādītas
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801191"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="4955c-102">Jutīguma etiķetes netiek rādītas</span><span class="sxs-lookup"><span data-stu-id="4955c-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="4955c-103">Jutīguma etiķetes ļauj klasificēt un palīdzēt aizsargāt sensitīvu saturu.</span><span class="sxs-lookup"><span data-stu-id="4955c-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="4955c-104">Tās var izveidot Microsoft 365 atbilstības centrā, Microsoft 365 drošības centrā vai Microsoft 365 drošības & atbilstības centrā sadaļā klasifikācija > jutīguma etiķetes.</span><span class="sxs-lookup"><span data-stu-id="4955c-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="4955c-105">Papildinformāciju par šo līdzekli skatiet rakstā [jutīguma etiķešu pārskats](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="4955c-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="4955c-106">Ja esat konfigurējis jutīguma etiķetes, bet tās netiek rādītas Microsoft 365 lietojumprogrammās, skatiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="4955c-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="4955c-107">Apstipriniet, ka jutīguma uzlīme ir [publicēta](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) nepieciešamajiem lietotājiem un grupām.</span><span class="sxs-lookup"><span data-stu-id="4955c-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="4955c-108">Pārliecinieties, vai lietotājs izmanto lietojumprogrammu, kas atbalsta jutīguma etiķetes — skatiet sadaļu [jutīguma etiķetes dokumentā](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="4955c-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="4955c-109">Ja [migrējat Azure informācijas aizsardzības uzlīmes](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ņemiet vērā [šeit](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)norādītos apsvērumus.</span><span class="sxs-lookup"><span data-stu-id="4955c-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="4955c-110">Atbalsts datu zuduma novēršanai (DLP): pašlaik tikai saglabāšanas etiķetes var izmantot kā nosacījumu DLP politikās.</span><span class="sxs-lookup"><span data-stu-id="4955c-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="4955c-111">Datu jutības etiķešu atbalsts DLP politikā vēl nav pieejams, bet mēs strādājam pie tā.</span><span class="sxs-lookup"><span data-stu-id="4955c-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="4955c-112">Ja jutības etiķetē ir iespējota šifrēšana, varat izvēlēties kādu no šīm darbībām:</span><span class="sxs-lookup"><span data-stu-id="4955c-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="4955c-113">Atļauju piešķiršana tūlīt</span><span class="sxs-lookup"><span data-stu-id="4955c-113">Assign permissions now</span></span>
    - <span data-ttu-id="4955c-114">Atļauju piešķiršana lietotājiem</span><span class="sxs-lookup"><span data-stu-id="4955c-114">Let users assign permissions</span></span>


<span data-ttu-id="4955c-115">Lai iegūtu papildinformāciju par iespējamajām problēmām, skatiet rakstu [zināmās problēmas ar jutības etiķetēm](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="4955c-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>