---
title: 1491-Search-not-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355884"
---
# <a name="content-search-not-returning-expected-results"></a>Satura meklēšana nav atgriešanās gaidāmie rezultāti

Braucot satura meklēšanu no & biroja 365 drošības ievērošanu centrs var saņemt negaidītu meklēšanas rezultātus. Apsveriet šādas lietas, kas var ietekmēt meklēšanas rezultātus:

- **Satura atrašanās vietu un meklēšanas nosacījumus**: Pārliecinieties, vai esat izvēlējies atbilstošu satura atrašanās vietu un meklēšanas nosacījumiem. Ja jūs vadīja lielu meklēšanas (ar daudzām vietām), uzskata, sadalot to vairākās meklēšanas.

- **Daļēji indeksē vienumus**: [daļēji indeksē vienumus](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) no pastkastes paredzamo meklēšanas rezultātos tiek iekļautas. Tomēr daļēji indeksē vienumus no vietas savā SharePoint un OneDrive netiek iekļauti meklēšanas budžetu.

- **Meklēšanas kļūmes**: meklējot lielu skaitu pastkastītes (vairāk nekā 100000 pastkastes), jūs varat saņemt meklēšanas kļūdas, kļūdas kodus, piem., CS008-009 un CS012-002). Šādā gadījumā mēģiniet vēlreiz tikai meklēt neizdevās satura atrašanās vietu. Skatiet [šajā rakstā](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) plašāku informāciju.
