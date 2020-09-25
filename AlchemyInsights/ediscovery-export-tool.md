---
title: e-datu atklāšanas eksportēšanas rīks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277948"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="aae10-102">Vai nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku?</span><span class="sxs-lookup"><span data-stu-id="aae10-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="aae10-103">Ja nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku, lai lejupielādētu meklēšanas rezultātus, skatiet tālāk minētos elementus.</span><span class="sxs-lookup"><span data-stu-id="aae10-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="aae10-104">Jūsu izmantotais dators atbilst šiem priekšnosacījumiem:</span><span class="sxs-lookup"><span data-stu-id="aae10-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="aae10-105">32 vai 64 bitu versijas Windows 7 un jaunākās versijās</span><span class="sxs-lookup"><span data-stu-id="aae10-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="aae10-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="aae10-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="aae10-107">Atbalstīta pārlūkprogramma:</span><span class="sxs-lookup"><span data-stu-id="aae10-107">A supported browser:</span></span>

  - <span data-ttu-id="aae10-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="aae10-108">Microsoft Edge</span></span>

    <span data-ttu-id="aae10-109">Vai</span><span class="sxs-lookup"><span data-stu-id="aae10-109">Or</span></span>

  - <span data-ttu-id="aae10-110">Internet Explorer 10 un jaunākas versijas</span><span class="sxs-lookup"><span data-stu-id="aae10-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="aae10-111">Citas pārlūkprogrammas, piemēram, Google Chrome un Mozilla Firefox, netiek atbalstītas.</span><span class="sxs-lookup"><span data-stu-id="aae10-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="aae10-112">Jūsu organizācija var izveidot savienojumu ar Azure galapunktu, kas ir \*\* \* . BLOB.Core.Windows.NET\*\* (aizstājējzīme apzīmē jūsu eksportēšanas darba unikālo identifikatoru).</span><span class="sxs-lookup"><span data-stu-id="aae10-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="aae10-113">Jums ir piešķirta eksportēšanas loma Microsoft 365 drošības &amp; atbilstības centrā.</span><span class="sxs-lookup"><span data-stu-id="aae10-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="aae10-114">Pēc noklusējuma šī loma ir piešķirta tikai e-datu atklāšanas pārvaldnieka lomu grupai.</span><span class="sxs-lookup"><span data-stu-id="aae10-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="aae10-115">Skatiet rakstu [e-datu atklāšanas atļauju piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="aae10-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="aae10-116">Papildinformāciju skatiet rakstā [satura meklēšanas rezultātu eksportēšana](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="aae10-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="aae10-117">Ja eksportējat vairāk nekā 100K pastkastes, ir jāizmanto tālāk norādītā PowerShell, lai lejupielādētu eksportēšanas rezultātus:  [Eksportējot rezultātus no vairāk nekā 100k pastkastēm](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="aae10-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>