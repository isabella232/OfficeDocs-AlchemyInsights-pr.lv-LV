---
title: 1490 problēmu novēršana-e-datu atklāšanas kļūmes
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
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105575"
---
# <a name="troubleshoot-content-search-errors"></a>Satura meklēšanas kļūdu novēršana

Vai, eksportējot meklēšanas rezultātus, rodas ar satura meklēšanu saistītas problēmas vai rodas kļūmes?

Piemēram, vai, palaižot meklēšanas vaicājumus, tiek rādīts tālāk redzamais?

- CS008 vai CS012 kļūdas

- Servera aizņemtības/taimauta kļūdas

- Radās lietojumprogrammas kļūda

Vai, meklējot vai eksportējot rezultātus no liela pastkastu skaita (vairāk nekā 100 000 pastkastu), vai saņemat eksportēšanas kļūdas?

Šo tipu kļūdas atkārtoti mēģiniet meklēt satura atrašanās vietas, kuras nav nesekmīgas. [Papildinformāciju](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) skatiet šajā rakstā.

Ja eksportējat vairāk nekā 100K pastkastes, izmantojiet šādu Powershell, lai lejupielādētu eksportēšanas rezultātus: rezultātu eksportēšana no vairāk nekā [100K pastkastēm.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
