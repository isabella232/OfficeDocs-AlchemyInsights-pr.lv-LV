---
title: Trūkstošie e-pasta ziņojumi karantīnā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673721"
---
# <a name="missing-emails-in-quarantine"></a>Trūkstošie e-pasta ziņojumi karantīnā

Administratori var [Skatīt, izlaist vai izdzēst šos ziņojumus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Lai atvērtu drošības & atbilstības centru, dodieties uz [https://protection.office.com](https://protection.office.com/) . Lai tieši atvērtu karantīnas lapu, dodieties uz [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Varat meklēt pēc šādām vērtībām:  

- **Ziņojuma ID**: ziņojuma globāli unikālais identifikators. Ja sarakstā atlasāt ziņojumu,  **ziņojuma ID**  vērtība tiek rādīta rūtī  **Detalizēta informācija**  , kas tiek parādīta. Administratori var izmantot [ziņojumu izsekošanu](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) , lai atrastu ziņojumus un to atbilstošos ziņojuma ID vērtības.
- **Sūtītāja e-pasta adrese**: viena sūtītāja e-pasta adrese.
- **Adresāta e-pasta adrese**: viena adresāta e-pasta adrese.
- **Tēma**: izmantojiet visu ziņojuma tēmu. Meklēšana nav reģistrjutīga.

Pēc meklēšanas kritēriju ievadīšanas noklikšķiniet uz ![ Atsvaidzināt pogas Atsvaidzināt ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **,** lai filtrētu rezultātus.  

Cmdlet, ko izmantojat, lai skatītu un pārvaldītu ziņojumus un failus karantīnā, ir šādi:
- [Dzēst-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksportēšana — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): ievērojiet, ka šajā cmdlet ir tikai ziņojumi, nevis ļaunprogrammatūras faili no ATP pakalpojumam SharePoint Online, OneDrive darbam vai Teams.
- [Laidiens — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)