---
title: PowerShell Exchange Online DKIM iespējošana konkrētam domēnam
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070314"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>PowerShell Exchange Online DKIM iespējošana konkrētam domēnam

Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrā, mēģiniet izmantot Exchange Online PowerShell. 

Lai izveidotu DKIM DNS ierakstu, izmantojot Exchange Online PowerShell, veiciet šādas darbības:

1. Atveriet Windows PowerShell kā administrators un izpildiet tālāk norādītās komandas aprakstītajā secībā.

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ja rodas problēmas, veidojot savienojumu ar Exchange Online PowerShell, [skatiet rakstu Savienošana Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Kad ir izveidots savienojums ar Exchange Online PowerShell, izpildiet šādu komandu:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kad iepriekš minētā komanda ir sekmīgi izpildīta, izpildiet šādu komandu, lai pārtrauktu Exchange Online PowerShell sesiju:

    `Remove-PSSession $Session` 



