---
title: Trūkst e-pasta karantīnā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569233"
---
# <a name="missing-emails-in-quarantine"></a>Trūkst e-pasta ziņojumu karantīnā "

Administratori var [Skatīt, izlaist vai dzēst šos ziņojumus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Lai atvērtu drošības & atbilstības centru, dodieties uz [https://protection.office.com](https://protection.office.com/) . Lai tieši atvērtu karantīnas lapu, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Jūs varat meklēt pēc šādām vērtībām:  

- **Ziņojuma ID**: ziņojuma vispārēji unikālais identifikators. Ja sarakstā atlasāt ziņojumu, **ziņojuma ID** vērtība tiek parādīta **informācijas** izlidošanas rūtī, kas tiek parādīta. Administratori var izmantot [ziņojumu trasēšanas](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) atrast ziņojumus un to atbilstošo ziņojumu ID vērtības.
- **Sūtītāja e-pasta adrese**: viena sūtītāja e-pasta adrese.
- **Adresāta e-pasta adrese**: viena adresāta e-pasta adrese.
- **Tēma**: izmantojiet visu ziņojuma tēmu. Meklēšana nav reģistrjutīga.

Pēc meklēšanas kritēriju ievadīšanas noklikšķiniet uz ![ Atsvaidzināt atsvaidzināšanas pogas, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** lai filtrētu rezultātus.  

Cmdlet, ko izmanto, lai skatītu un pārvaldīt ziņojumus un failus karantīnā, ir šādi:
- [Izdzēst-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksports-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Priekšapskate-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Ņemiet vērā, ka šī cmdlet ir tikai ziņojumi, nevis Malware failus no ATP SharePoint Online, OneDrive uzņēmumiem vai darba grupas.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)