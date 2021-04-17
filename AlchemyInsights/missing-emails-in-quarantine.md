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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831741"
---
# <a name="missing-emails-in-quarantine"></a>Missing emails in quarantine"

Administratori [var skatīt, izlaist vai dzēst šos ziņojumus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Lai atvērtu drošības & centru, dodieties uz [https://protection.office.com](https://protection.office.com/) . Lai tieši atvērtu lapu Karantīnā, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Varat meklēt pēc šādām vērtībām:  

- **Ziņojuma ID:** ziņojuma globāli unikāls identifikators. Ja sarakstā atlasāt ziņojumu, izlidošanas rūtī  Detalizēti tiek rādīta vērtība Ziņojuma **ID.** Administratori var izmantot ziņojumu [izsekošanu,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) lai atrastu ziņojumus un to atbilstošās vērtības Ziņojuma ID.
- **Sūtītāja e-pasta** adrese: viena sūtītāja e-pasta adrese.
- **Adresāta e-pasta** adrese: viena adresāta e-pasta adrese.
- **Tēma:** izmantojiet visu ziņojuma tēmu. Meklēšana nav reģistrjutīga.

Kad esat ievadījis meklēšanas kritērijus, noklikšķiniet uz ![ Atsvaidzināt pogas ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atsvaidzināt,** lai filtrētu rezultātus.  

Cmdlet, kuras izmantojat ziņojumu un failu skatīšanai un pārvaldīšanai karantīnā, ir:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Ņemiet vērā, ka šī cmdlet ir pieejama tikai ziņojumiem, nevis ļaunprogrammatūras failiem no ATP pakalpojumā SharePoint Online, OneDrive darbam vai Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)