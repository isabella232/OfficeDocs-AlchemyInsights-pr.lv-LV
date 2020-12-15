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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678680"
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
