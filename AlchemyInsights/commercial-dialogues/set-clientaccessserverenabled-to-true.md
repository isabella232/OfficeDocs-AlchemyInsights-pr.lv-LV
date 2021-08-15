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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994872"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Iestatiet ClientAccessServerEnabled vērtību kā True

Ja nevarat atvērt šifrētu e-pasta ziņojumu un tā vietā skatīt **rpmsg** pielikumu, veiciet šādas darbības:

1. Savienošana uz Exchange Online PowerShell.

> [!NOTE]
> Lai izveidotu savienojumu Exchange Online PowerShell, pierakstieties, izmantojot globālā administratora vai administratora Exchange kontu.

   a. Atveriet Windows PowerShell un pēc tam izpildiet šādu komandu:`$UserCredential = Get-Credential`
b. Dialoglodziņā **Akreditācijas Windows PowerShell pieprasījums** ievadiet savu darba vai mācību iestādes kontu un paroli c. Noklikšķiniet uz **Labi**. 

2. Lai izveidotu jaunu sesiju, izpildiet šādu komandu:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Palaidiet šādu komandu:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Komanda `Get-IRMConfiguration` Izpildīt

4. Pārbaudiet **clientAccessServerEnabled** iestatījumu. 

    a. Ja **ClientAccessServerEnabled iestatījums** ir **False**, izpildiet šo cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Vienmēr aizveriet powershell sesiju ar šādu komandu: `Remove-PSSession $Session`

Papildinformāciju skatiet rakstā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

