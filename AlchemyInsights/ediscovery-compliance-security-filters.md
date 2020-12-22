---
title: Satura meklēšanas/eksportēšanas laikā netiek atgriezti rezultāti
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727230"
---
# <a name="no-results-returned-during-content-searchexport"></a>Satura meklēšanas/eksportēšanas laikā netiek atgriezti rezultāti

Ja rodas problēmas ar šādiem e-datu atklāšanas scenārijiem:

- Satura meklēšana/eksportēšana neatgriež datus vai negaidītus datus
- e-datu atklāšanas meklēšana vai eksportēšana nav sekmīga

To var izraisīt daži atbilstības drošības filtri, ko iestatīja konkrēts administrators un kas nav paziņoti visiem administratoriem.

Lai atrisinātu šo problēmu, pārbaudiet, vai pastāv atbilstības drošības filtri, kas var izraisīt šādas problēmas:

1. Savienojuma izveide ar drošības un atbilstības centra PowerShell
2. Palaidiet šādu commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Papildu informāciju par atbilstības drošības filtriem skatiet rakstā [atļauju filtrēšana satura meklēšanai](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
