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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="f5f22-102">Exchange Online PowerShell izmantošana, lai iespējotu DKIM noteiktam domēnam</span><span class="sxs-lookup"><span data-stu-id="f5f22-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="f5f22-103">Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrā, mēģiniet izmantot Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5f22-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="f5f22-104">Lai izveidotu DKIM DNS ierakstu, izmantojot Exchange Online PowerShell, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="f5f22-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="f5f22-105">Atveriet Windows PowerShell kā administrators un izpildiet tālāk norādītās komandas aprakstītajā secībā:</span><span class="sxs-lookup"><span data-stu-id="f5f22-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="f5f22-106">izveide.</span><span class="sxs-lookup"><span data-stu-id="f5f22-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="f5f22-107">b.</span><span class="sxs-lookup"><span data-stu-id="f5f22-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="f5f22-108">c.</span><span class="sxs-lookup"><span data-stu-id="f5f22-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="f5f22-109">Ja rodas problēmas, veidojot savienojumu ar Exchange Online PowerShell, skatiet rakstu [savienojuma izveide ar Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="f5f22-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="f5f22-110">Kad ir izveidots savienojums ar Exchange Online PowerShell, izpildiet šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="f5f22-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="f5f22-111">Kad iepriekšminētā komanda ir veiksmīgi izpildīta, izpildiet šo komandu, lai beigtu Exchange Online PowerShell sesiju:</span><span class="sxs-lookup"><span data-stu-id="f5f22-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



