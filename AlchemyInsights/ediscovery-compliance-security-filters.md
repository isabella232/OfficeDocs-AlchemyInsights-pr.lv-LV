---
title: Satura meklēšanas/eksportēšanas laikā netiek atgriezti nekādi rezultāti
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101273"
---
# <a name="no-results-returned-during-content-searchexport"></a>Satura meklēšanas/eksportēšanas laikā netiek atgriezti nekādi rezultāti

Ja rodas problēmas saistībā ar šādiem e-datu atklāšanas scenārijiem:

- Satura meklēšana/eksportēšana neatgriež datus vai neparedzētus datus
- E-datu atklāšanas meklēšana vai eksportēšana neizdodas

Tas var rasties noteiktu atbilstības drošības filtru dēļ, kurus iestata konkrēts administrators, un par to netiek paziņots visiem administratoriem.

Lai novērstu šo problēmu, pārbaudiet, vai ir kāds atbilstības drošības filtrs, kas varētu izraisīt šīs problēmas:

1. Savienošana uz drošības un atbilstības centra Powershell
2. Palaidiet šādus komandsīklietotņus:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Papildinformāciju par atbilstības drošības filtriem skatiet [rakstā Satura meklēšanas atļauju filtrēšana.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
