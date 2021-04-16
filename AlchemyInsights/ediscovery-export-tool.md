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
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Vai nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku?

Ja nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku, lai lejupielādētu meklēšanas rezultātus, pārbaudiet šādus datus:
  
- Jūsu dators atbilst šiem priekšnosacījiem priekšnosacīniem:

  - Windows 7 vai jaunāka 32 vai 64 bitu versija

  - Microsoft .NET Framework 4.7

  - Atbalstīta pārlūkprogramma:

  - Microsoft Edge

    Vai

  - Internet Explorer 10 un jaunākas versijas

    Citas pārlūkprogrammas, piemēram, Google Chrome un Mozilla Firefox, netiek atbalstītas.

- Jūsu organizācija var izveidot savienojumu ar Azure galapunktu **\* .blob.core.windows.net** (aizstājējzīme apzīmē eksportēšanas darba unikālo identifikatoru).

- Microsoft 365 drošības atbilstības centrā jums ir piešķirta &amp; eksportēšanas loma. Pēc noklusējuma šī loma ir piešķirta tikai e-datu atklāšanas pārvaldnieka lomu grupai. Skatiet [rakstu E-datu atklāšanas atļauju piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Papildinformāciju skatiet rakstā [Satura meklēšanas rezultātu eksportēšana.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Ja eksportējat vairāk nekā 100K pastkastes, izmantojiet šādu Powershell, lai lejupielādētu eksportēšanas rezultātus: rezultātu eksportēšana no vairāk nekā [100K pastkastēm.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)