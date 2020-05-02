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
# <a name="private-channels-in-microsoft-teams"></a>Privāti kanāli Microsoft Teams

Privātie kanāli ir jauns Microsoft Teams līdzeklis. Ņemiet vērā, ka privātos kanālus nevar pārveidot no standarta kanāliem vai otrādi.

Plašāku informāciju par privātiem kanāliem, piemēram, informāciju par [privātā kanāla izveidi un dalību](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) un [privātā kanāla SharePoint vietnēm](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)skatiet sadaļā [privātie kanāli Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Piezīme:** Tā kā konfigurācija privāto kanālu ziņojumu saglabāšanai vēl netiek atbalstīta, nomniekiem ar iespējotu saglabāšanas politiku nav privātu kanālu, kas ir aktivizēti pēc noklusējuma. Privātos kanālus var iespējot komandu administrēšanas centrā. Ņemiet arī vērā, ka privātā kanāla ziņojumu saglabāšana netiek atbalstīta, tiek atbalstīta failu, kas kopīgoti privātos kanālos, saglabāšana.

**Nepieciešams jauns komandas īpašnieks?**

Ja jūsu privātā kanāla īpašnieks atstāj, varat pievienot jaunu komandas īpašnieku, izmantojot komandu PowerShell.


- Dodieties [šeit](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , lai instalētu komandu PowerShell.

Šeit ir cmdlet jums būs nepieciešams:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Lai iegūtu papildinformāciju par komandu PowerShell, skatiet [darba grupas PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
