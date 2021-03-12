---
title: ClientAccessServerEnabled iestatīšana uz patiess
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746412"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled iestatīšana uz patiess

Ja nevarat atvērt šifrētu e-pasta ziņojumu un tā vietā skatīt **rpmsg** pielikumu, veiciet tālāk norādītās darbības.

1. Savienojuma izveide ar Exchange Online PowerShell.

> [!NOTE]
> Lai izveidotu savienojumu ar Exchange Online PowerShell, jums ir jāpierakstās, izmantojot globālo administratoru vai Exchange administratora kontu.

   izveide. Atveriet programmu Windows PowerShell un pēc tam izpildiet šādu komandu: `$UserCredential = Get-Credential`
b. Dialoglodziņā **Windows PowerShell akreditācijas datu pieprasījums** ievadiet savu darba vai mācību iestādes kontu un paroli c. Noklikšķiniet uz **Labi**. 

2. Lai izveidotu jaunu sesiju, izpildiet šādu komandu:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    izveide. Palaidiet šādu komandu:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Komanda Palaist.

4. Pārbaudiet iestatījumu **ClientAccessServerEnabled** . 

    izveide. Ja **ClientAccessServerEnabled** iestatījums ir **FALSE**, izpildiet šo cmdlet komandu: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Vienmēr izvērsiet PowerShell sesiju ar šādu komandu: `Remove-PSSession $Session`

Papildinformāciju skatiet rakstā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

