---
title: Privātais kanāls
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005445"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="745bb-102">Privāti kanāli Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="745bb-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="745bb-103">Privātie kanāli ir jauns Microsoft Teams līdzeklis.</span><span class="sxs-lookup"><span data-stu-id="745bb-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="745bb-104">Ņemiet vērā, ka privātos kanālus nevar pārveidot no standarta kanāliem vai otrādi.</span><span class="sxs-lookup"><span data-stu-id="745bb-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="745bb-105">Plašāku informāciju par privātiem kanāliem, piemēram, informāciju par [privātā kanāla izveidi un dalību](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) un [privātā kanāla SharePoint vietnēm](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)skatiet sadaļā [privātie kanāli Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="745bb-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="745bb-106">**Piezīme:** Tā kā konfigurācija privāto kanālu ziņojumu saglabāšanai vēl netiek atbalstīta, nomniekiem ar iespējotu saglabāšanas politiku nav privātu kanālu, kas ir aktivizēti pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="745bb-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="745bb-107">Privātos kanālus var iespējot komandu administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="745bb-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="745bb-108">Ņemiet arī vērā, ka privātā kanāla ziņojumu saglabāšana netiek atbalstīta, tiek atbalstīta failu, kas kopīgoti privātos kanālos, saglabāšana.</span><span class="sxs-lookup"><span data-stu-id="745bb-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="745bb-109">**Nepieciešams jauns komandas īpašnieks?**</span><span class="sxs-lookup"><span data-stu-id="745bb-109">**Need a new team owner?**</span></span>

<span data-ttu-id="745bb-110">Ja jūsu privātā kanāla īpašnieks atstāj, varat pievienot jaunu komandas īpašnieku, izmantojot komandu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="745bb-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="745bb-111">Dodieties [šeit](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , lai instalētu komandu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="745bb-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="745bb-112">Šeit ir cmdlet jums būs nepieciešams:</span><span class="sxs-lookup"><span data-stu-id="745bb-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="745bb-113">Lai iegūtu papildinformāciju par komandu PowerShell, skatiet [darba grupas PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="745bb-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
