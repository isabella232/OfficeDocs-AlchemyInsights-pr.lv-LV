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
# <a name="troubleshoot-content-search-errors"></a>Satura meklēšanas kļūdu novēršana

Vai rodas problēmas ar satura meklēšanu vai neveiksmēm, kad eksportējat meklēšanas rezultātus?

Piemēram, ja izlaižat meklēšanu, tiek parādīts tālāk norādītās darbības.

- CS008 vai CS012 kļūdas

- Servera aizņemts/taimauta kļūdas

- Radās lietojumprogrammas kļūda

Vai, meklējot vai eksportējot rezultātus no liela pastkastu skaita (virs 100 000 pastkastēm), tiek iegūtas eksportēšanas kļūdas?

Lai iegūtu šāda veida kļūdas, vēlreiz mēģiniet meklēt neveiksmīgās satura atrašanās vietas. Lai iegūtu papildinformāciju, skatiet  [šo rakstu](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Ja eksportējat vairāk nekā 100K pastkastes, ir jāizmanto tālāk norādītā PowerShell, lai lejupielādētu eksportēšanas rezultātus:  [Eksportējot rezultātus no vairāk nekā 100k pastkastēm](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
