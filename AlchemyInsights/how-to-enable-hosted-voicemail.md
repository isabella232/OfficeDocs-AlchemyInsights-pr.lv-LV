---
title: Viesotā balss pasta iespējošana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677997"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="b7b0f-102">Viesotā balss pasta iespējošana</span><span class="sxs-lookup"><span data-stu-id="b7b0f-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="b7b0f-103">Lai iespējotu balss pastu, **HostedVoicemail** ir jābūt iestatītai uz $True.</span><span class="sxs-lookup"><span data-stu-id="b7b0f-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="b7b0f-104">Rekvizīts **HostedVoicemail** lietotājam, kas izmanto attālo POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="b7b0f-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="b7b0f-105">Lai iegūtu papildinformāciju par savienojuma izveidi ar RPS, skatiet rakstu [Microsoft Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) , lai iegūtu papildinformāciju par savienojuma izveidi ar RPS.</span><span class="sxs-lookup"><span data-stu-id="b7b0f-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="b7b0f-106">Teams administratoram ir jāpiesakās attālajā PowerShell darbam ar Teams.</span><span class="sxs-lookup"><span data-stu-id="b7b0f-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="b7b0f-107">No PowerShell uzvednes Teams administrators var palaist **Set-csuser user@contoso.com-HostedVoiceMail $True** , kur SIP URI ir lietotāja jautājums.</span><span class="sxs-lookup"><span data-stu-id="b7b0f-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="b7b0f-108">Politikas izmaiņas var ilgt līdz pat 24 stundām.</span><span class="sxs-lookup"><span data-stu-id="b7b0f-108">Changes to policies can take up to 24 hours to replicate.</span></span>