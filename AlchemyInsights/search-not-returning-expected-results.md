---
title: 1491 — meklēšana — netiek atgriezti — sagaidāmie rezultāti
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740481"
---
# <a name="content-search-not-returning-expected-results"></a>Satura meklēšana neatgriež gaidītos rezultātus

Kad notiek satura meklēšana no Microsoft 365 drošības & atbilstības centra, iespējams, saņemsit negaidītus meklēšanas rezultātus. Apsveriet tālāk norādītās darbības, kas var ietekmēt meklēšanas rezultātus.

- **Satura atrašanās vietas un meklēšanas nosacījumi**: Pārliecinieties, vai esat atlasījis atbilstošas satura atrašanās vietas un meklēšanas nosacījumus. Ja esat izpildījis lielu meklēšanu (ar daudzām atrašanās vietām), apsveriet iespēju to sadalīt vairākos meklējumos.

- **Daļēji indeksētie vienumi**: aprēķinātajos meklēšanas rezultātos tiek iekļauti  [daļēji indeksētie vienumi](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) no pastkastēm. Tomēr meklēšanas aplēsē nav iekļauta daļēji indeksētie vienumi no SharePoint un OneDrive vietnēm.

- **Meklēšanas kļūmes**: Ja meklējat lielu skaitu pastkastu (vairāk par 100 000 pastkastēm), varat saņemt meklēšanas kļūdas ar kļūdu kodiem, piemēram, CS008-009 un CS012-002). Šajā gadījumā atkārtoti mēģiniet meklēt tikai neveiksmīgajām satura atrašanās vietām. Lai iegūtu papildinformāciju, skatiet  [šo rakstu](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
