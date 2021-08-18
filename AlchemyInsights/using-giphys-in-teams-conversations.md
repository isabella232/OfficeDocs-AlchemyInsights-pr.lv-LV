---
title: Giphys izmantošana Teams sarunās
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323527"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphys izmantošana Teams sarunās

Giphys piekļuve tērzēšanā Teams iespējota pēc noklusējuma. Kā administrators jūs varat kontrolēt, vai lietotājam [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ir pieejami Giphy, iestatot ziņojumapmaiņas politiku un nodrošinot, ka Use **Giphys in conversations** is **On**.

Ja GIF faili nedarbojas, kā paredzēts, Teams, pārbaudiet:

Ziņojumapmaiņas [politikai ir](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ļautu Giphys. Lai to pārbaudītu, izmantojot PowerShell cmdlet:

- Pārliecinieties, vai [varat pārvaldīt Teams, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Izpildiet PowerShell komandu [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) un pārbaudiet, vai **AllowGiphy** ir iestatīts uz **TRUE**.
- Ja **allowGiphy** ir iestatīts kā **FALSE**, palaidiet tālāk norādīto PowerShell komandu [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Neobligātie pievienotie](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) pieredzē ir jāiespējo, lai atļautu piekļuvi Giphy vietrādim URL.

**Piezīme.** Ja jūsu nomniekam ir konfigurētas vairākas Teams ziņojumapmaiņas politikas, varat noteikt ietekmētā lietotājam piešķirtās politikas identitāti, izmantojot PowerShell komandu [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Atlasiet TeamsMessagingPolicy.
