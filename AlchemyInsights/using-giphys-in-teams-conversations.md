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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104315"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphys izmantošana Teams sarunās

Giphys piekļuve tērzēšanā Teams iespējota pēc noklusējuma. Kā administrators jūs varat kontrolēt, vai lietotājam [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ir pieejami Giphy, iestatot ziņojumapmaiņas politiku un nodrošinot, ka Use **Giphys in conversations** is **On**.

Ja GIF faili nedarbojas, kā paredzēts, Teams sarunās, pārbaudiet:

Ziņojumapmaiņas [politikai ir](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ļautu Giphys. Lai to pārbaudītu, izmantojot PowerShell cmdlet:

- Pārliecinieties, vai [varat pārvaldīt Teams, izmantojot PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Izpildiet PowerShell komandu [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) un pārbaudiet, vai **AllowGiphy** ir iestatīts uz **TRUE**.
- Ja **allowGiphy** ir iestatīts kā **FALSE**, palaidiet tālāk norādīto PowerShell komandu [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Lai atļautu piekļuvi](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) Giphy vietrādim URL, ir jāiespējo papildu saistītie pieredzē.

> [!NOTE]
> Ja jūsu nomniekam ir konfigurētas vairākas Teams ziņojumapmaiņas politikas, varat noteikt ietekmētā lietotājam piešķirtās politikas identitāti, izmantojot PowerShell komandu [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Atlasiet TeamsMessagingPolicy.
