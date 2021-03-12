---
title: Exchange Online PowerShell izmantošana, lai iespējotu DKIM noteiktam domēnam
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746283"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Exchange Online PowerShell izmantošana, lai iespējotu DKIM noteiktam domēnam

Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrā, mēģiniet izmantot Exchange Online PowerShell. 

Lai izveidotu DKIM DNS ierakstu, izmantojot Exchange Online PowerShell, veiciet tālāk norādītās darbības.

1. Atveriet Windows PowerShell kā administrators un izpildiet tālāk norādītās komandas aprakstītajā secībā:

    izveide. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ja rodas problēmas, veidojot savienojumu ar Exchange Online PowerShell, skatiet rakstu [savienojuma izveide ar Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Kad ir izveidots savienojums ar Exchange Online PowerShell, izpildiet šādu komandu:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kad iepriekšminētā komanda ir veiksmīgi izpildīta, izpildiet šo komandu, lai beigtu Exchange Online PowerShell sesiju:

    `Remove-PSSession $Session` 



