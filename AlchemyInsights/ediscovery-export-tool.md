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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101309"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Vai nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku?

Ja nevarat instalēt vai palaist e-datu atklāšanas eksportēšanas rīku, lai lejupielādētu meklēšanas rezultātus, pārbaudiet šādus datus:
  
- Jūsu dators atbilst šiem priekšnosacījiem priekšnosacīniem:

  - Windows 7 vai jaunākas 32 vai 64 bitu versijas

  - Microsoft .NET Framework 4.7

  - Atbalstīta pārlūkprogramma:

  - Microsoft Edge

    Vai

  - Internet Explorer 10 un jaunākas versijas

    Citas pārlūkprogrammas, piemēram, Google Chrome un Mozilla Firefox, netiek atbalstītas.

- Jūsu organizācija var izveidot savienojumu ar Azure galapunktu **\* .blob.core.windows.net** (aizstājējzīme apzīmē eksportēšanas darba unikālo identifikatoru).

- Eksportēšanas loma ir piešķirta Microsoft 365 &amp; atbilstības centrā. Pēc noklusējuma šī loma ir piešķirta tikai e-datu atklāšanas pārvaldnieka lomu grupai. Skatiet [rakstu E-datu atklāšanas atļauju piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Papildinformāciju skatiet rakstā [Satura meklēšanas rezultātu eksportēšana.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Ja eksportējat vairāk nekā 100K pastkastes, izmantojiet šādu Powershell, lai lejupielādētu eksportēšanas rezultātus: rezultātu eksportēšana no vairāk nekā [100K pastkastēm.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)