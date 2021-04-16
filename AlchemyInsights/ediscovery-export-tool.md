---
title: E-datu atklāšanas eksportēšanas rīks
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814595"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="2d9ed-102">Vai nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku?</span><span class="sxs-lookup"><span data-stu-id="2d9ed-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="2d9ed-103">Ja nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku, lai lejupielādētu meklēšanas rezultātus, pārbaudiet šādus datus:</span><span class="sxs-lookup"><span data-stu-id="2d9ed-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="2d9ed-104">Jūsu dators atbilst šiem priekšnosacījiem priekšnosacīniem:</span><span class="sxs-lookup"><span data-stu-id="2d9ed-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="2d9ed-105">Windows 7 vai jaunāka 32 vai 64 bitu versija</span><span class="sxs-lookup"><span data-stu-id="2d9ed-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="2d9ed-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="2d9ed-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="2d9ed-107">Atbalstīta pārlūkprogramma:</span><span class="sxs-lookup"><span data-stu-id="2d9ed-107">A supported browser:</span></span>

  - <span data-ttu-id="2d9ed-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2d9ed-108">Microsoft Edge</span></span>

    <span data-ttu-id="2d9ed-109">Vai</span><span class="sxs-lookup"><span data-stu-id="2d9ed-109">Or</span></span>

  - <span data-ttu-id="2d9ed-110">Internet Explorer 10 un jaunākas versijas</span><span class="sxs-lookup"><span data-stu-id="2d9ed-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="2d9ed-111">Citas pārlūkprogrammas, piemēram, Google Chrome un Mozilla Firefox, netiek atbalstītas.</span><span class="sxs-lookup"><span data-stu-id="2d9ed-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="2d9ed-112">Jūsu organizācija var izveidot savienojumu ar Azure galapunktu **\* .blob.core.windows.net** (aizstājējzīme apzīmē eksportēšanas darba unikālo identifikatoru).</span><span class="sxs-lookup"><span data-stu-id="2d9ed-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="2d9ed-113">Microsoft 365 drošības atbilstības centrā jums ir piešķirta &amp; eksportēšanas loma.</span><span class="sxs-lookup"><span data-stu-id="2d9ed-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="2d9ed-114">Pēc noklusējuma šī loma ir piešķirta tikai e-datu atklāšanas pārvaldnieka lomu grupai.</span><span class="sxs-lookup"><span data-stu-id="2d9ed-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="2d9ed-115">Skatiet [rakstu E-datu atklāšanas atļauju piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="2d9ed-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="2d9ed-116">Papildinformāciju skatiet rakstā [Satura meklēšanas rezultātu eksportēšana.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="2d9ed-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="2d9ed-117">Ja eksportējat vairāk nekā 100K pastkastes, izmantojiet šādu Powershell, lai lejupielādētu eksportēšanas rezultātus: rezultātu eksportēšana no vairāk nekā [100K pastkastēm.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="2d9ed-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>