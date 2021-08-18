---
title: Iestatiet ClientAccessServerEnabled vērtību kā True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320363"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Iestatiet ClientAccessServerEnabled vērtību kā True

Ja nevarat atvērt šifrētu e-pasta ziņojumu un tā vietā skatīt **rpmsg** pielikumu, veiciet šādas darbības:

1. Savienošana uz Exchange Online PowerShell.

    **Piezīme.** Lai izveidotu savienojumu Exchange Online ar PowerShell, pierakstieties, izmantojot globālā administratora vai Exchange kontu.

   a. Atveriet Windows PowerShell un pēc tam izpildiet šādu komandu:`$UserCredential = Get-Credential`
   b. Dialoglodziņā **akreditācijas Windows PowerShell** ievadiet savu darba vai mācību iestādes kontu un paroli, c. Noklikšķiniet uz **Labi**. 

2. Lai izveidotu jaunu sesiju, izpildiet šādu komandu:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Palaidiet šādu komandu:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Komanda `Get-IRMConfiguration` Izpildīt

4. Pārbaudiet **clientAccessServerEnabled** iestatījumu. 

    a. Ja **ClientAccessServerEnabled iestatījums** ir **False**, izpildiet šo cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Padoms.** Vienmēr aizveriet savu Powershell sesiju ar šādu komandu: `Remove-PSSession $Session`

Papildinformāciju skatiet rakstā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

