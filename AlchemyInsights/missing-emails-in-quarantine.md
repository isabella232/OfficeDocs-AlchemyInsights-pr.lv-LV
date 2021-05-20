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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539831"
---
# <a name="missing-emails-in-quarantine"></a>Missing emails in quarantine"

Administratori [var skatīt, izlaist vai dzēst šos ziņojumus.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Lai atvērtu drošības & centru, dodieties uz [https://protection.office.com](https://protection.office.com/) . Lai tieši atvērtu lapu Karantīnā, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Varat meklēt pēc šādām vērtībām:  

- **Ziņojuma ID:** ziņojuma globāli unikāls identifikators. Ja sarakstā atlasāt ziņojumu, izlidošanas rūtī  Detalizēti tiek rādīta vērtība Ziņojuma **ID.** Administratori var izmantot ziņojumu [izsekošanu,](/microsoft-365/security/office-365-security/message-trace-scc) lai atrastu ziņojumus un to atbilstošās vērtības Ziņojuma ID.
- **Sūtītāja e-pasta** adrese: viena sūtītāja e-pasta adrese.
- **Adresāta e-pasta** adrese: viena adresāta e-pasta adrese.
- **Tēma:** izmantojiet visu ziņojuma tēmu. Meklēšana nav reģistrjutīga.

Kad esat ievadījis meklēšanas kritērijus, noklikšķiniet uz ![ Atsvaidzināt pogas ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atsvaidzināt,** lai filtrētu rezultātus.

Cmdlet, kuras izmantojat ziņojumu un failu skatīšanai un pārvaldīšanai karantīnā, ir:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Ņemiet vērā, ka šī cmdlet ir pieejama tikai ziņojumiem, nevis ļaunprogrammatūras failiem no programmatūras Microsoft Defender Office 365 SharePoint Online, OneDrive darbam vai Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)