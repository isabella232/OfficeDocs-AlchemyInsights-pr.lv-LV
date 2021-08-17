---
title: 1491-meklēšana-neatgriež-sagaidāmie-rezultāti
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052717"
---
# <a name="content-search-not-returning-expected-results"></a>Satura meklēšana neatgriež gaidāmos rezultātus

Palaižot satura meklēšanu no drošības Microsoft 365 &, iespējams, tiks nodrošināti neparedzēti meklēšanas rezultāti. Apsveriet tālāk minētās darbības, kas var ietekmēt meklēšanas rezultātus.

- **Satura atrašanās vietas un meklēšanas nosacījumi:** pārliecinieties, vai esat atlasījis pareizas satura atrašanās vietas un meklēšanas nosacījumus. Ja veicām lielu meklēšanu (ar daudzām atrašanās vietām), apsveriet iespēju to sadalīt vairākās meklēšanas rezultātos.

- **Daļēji indeksēti vienumi:**  [daļēji indeksēti vienumi](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) no pastkastēm tiek iekļauti plānotajā meklēšanas rezultātos. Tomēr daļēji indeksēti vienumi no SharePoint OneDrive vietnes netiek iekļauti meklēšanas aprēķinos.

- **Meklēšanas kļūmes.** Meklējot lielā pastkastu skaitu (vairāk nekā 100 000 pastkastu), var tikt parādīts meklēšanas kļūdas ar kļūdu kodiem, piemēram, CS008-009 un CS012-002). Šādā gadījumā atkārtoti mēģiniet meklēt tikai nesekmīgo satura atrašanās vietas. [Papildinformāciju](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) skatiet šajā rakstā.
