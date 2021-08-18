---
title: Trūkstoši e-pasta ziņojumi karantīnā
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
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329669"
---
# <a name="missing-emails-in-quarantine"></a>Trūkstoši e-pasta ziņojumi karantīnā

Administratori [var skatīt, izlaist vai dzēst šos ziņojumus](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

E-Microsoft 365 Defender portālā <https://security.microsoft.com> dodieties uz Pārskatīt **karantīnu** \> . Vai arī, lai dotos tieši uz lapu **Karantīnā,** izmantojiet <https://security.microsoft.com/quarantine> pakalpojumu .  

Papildinformāciju par meklēšanas/filtrēšanas vērtībām, ko varat izmantot, skatiet rakstā Karantīnā ievietoto ziņojumu un [failu pārvaldība EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)administratora veidā.

Cmdlet, kuras izmantojat ziņojumu un failu skatīšanai un pārvaldīšanai karantīnā, ir:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Ņemiet vērā, ka šī cmdlet ir pieejama tikai ziņojumiem, nevis failiem no Seifs SharePoint, OneDrive vai Microsoft Teams pielikumiem.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
