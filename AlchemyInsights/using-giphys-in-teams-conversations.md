---
title: Giphy izmantošana grupu sarunās
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982505"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphy izmantošana grupu sarunās

Giphy piekļuve Teams tērzēšanā ir iespējota pēc noklusējuma. Kā administrators varat kontrolēt, vai **giphy ir pieejami** lietotājiem, [iestatot ziņojumapmaiņas politiku](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) un nodrošinot, ka **sarunas izmanto giphy** .

Ja GIFs nedarbojas, kā paredzēts, grupu sarunās, pārbaudiet:

[Ziņojumapmaiņas politikai](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ir jāatļauj giphy. Lai pārbaudītu, izmantojot PowerShell cmdlet:

- Pārbaudiet, vai varat [pārvaldīt grupas, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Palaidiet PowerShell komandu [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) un pārbaudiet, vai **AllowGiphy** ir iestatīts kā **patiess**.
- Ja **AllowGiphy** ir iestatīts kā **aplams** , izpildiet tālāk norādītās PowerShell komandu [kopas-CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Neobligātās saistītās pieredzes](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) ir jāiespējo, lai atļautu piekļuvi Giphy vietrādim URL.

> [!NOTE]
> Ja jūsu nomniekam ir konfigurētas vairākas grupu ziņojumapmaiņas politikas, varat noteikt, kāda ir lietotāja piešķiramās politikas identitāte, izmantojot PowerShell komandu [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Atlasiet TeamsMessagingPolicy.
