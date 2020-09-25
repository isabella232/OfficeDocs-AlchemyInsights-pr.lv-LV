---
title: 1490 — e-datu atklāšanas neveiksmes
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277825"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="77fe3-102">Satura meklēšanas kļūdu novēršana</span><span class="sxs-lookup"><span data-stu-id="77fe3-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="77fe3-103">Vai rodas problēmas ar satura meklēšanu vai neveiksmēm, kad eksportējat meklēšanas rezultātus?</span><span class="sxs-lookup"><span data-stu-id="77fe3-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="77fe3-104">Piemēram, ja izlaižat meklēšanu, tiek parādīts tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="77fe3-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="77fe3-105">CS008 vai CS012 kļūdas</span><span class="sxs-lookup"><span data-stu-id="77fe3-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="77fe3-106">Servera aizņemts/taimauta kļūdas</span><span class="sxs-lookup"><span data-stu-id="77fe3-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="77fe3-107">Radās lietojumprogrammas kļūda</span><span class="sxs-lookup"><span data-stu-id="77fe3-107">Application error occurred</span></span>

<span data-ttu-id="77fe3-108">Vai, meklējot vai eksportējot rezultātus no liela pastkastu skaita (virs 100 000 pastkastēm), tiek iegūtas eksportēšanas kļūdas?</span><span class="sxs-lookup"><span data-stu-id="77fe3-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="77fe3-109">Lai iegūtu šāda veida kļūdas, vēlreiz mēģiniet meklēt neveiksmīgās satura atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="77fe3-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="77fe3-110">Lai iegūtu papildinformāciju, skatiet  [šo rakstu](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="77fe3-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="77fe3-111">Ja eksportējat vairāk nekā 100K pastkastes, ir jāizmanto tālāk norādītā PowerShell, lai lejupielādētu eksportēšanas rezultātus:  [Eksportējot rezultātus no vairāk nekā 100k pastkastēm](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="77fe3-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
