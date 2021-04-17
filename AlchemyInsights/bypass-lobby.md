---
title: Vestibila apiešanu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820041"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Vestibila iestatījumu un dalības līmeņa vadība programmā Teams

Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmiem lietotājiem, apiet vestibilu, izmantojiet PowerShell, lai veiktu šo uzdevumu. Šeit ir savas organizācijas globālās sapulces politikas modificēšanas piemērs.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šai cmdlet pašlaik ir nepieciešams Skype darbam PowerShell modulis. Lai iestatītu šī cmdlet izmantošanu, skatiet rakstā Politiku [pārvaldība, izmantojot PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Kad politika ir iestatīta, tā ir jālieto lietotājiem; vai, ja esat modificējis globālo politiku, tā tiek automātiski lietota lietotājiem. Lai politikas izmaiņas stāsies spēkā, ir jāgaida vismaz 4 stundas līdz **24** stundām. 

Noteikti pārskatiet tālāk esošo dokumentāciju, pirms veicat šīs izmaiņas, lai saprastu, ko tas atļauj.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Par Teams sapulču vestibila politikas vadīklām

Šie iestatījumi nosaka, kuriem sapulces dalībniekiem jāgaida vestibilā, pirms viņi var piedalīties sapulcē, kā arī norādīts, kādā līmenī dalībnieki var piedalīties sapulcē. Varat izmantot PowerShell, lai atjauninātu sapulces politikas iestatījumus, kas vēl nav ieviesti (apzīmēti kā "drīzumā") Teams administrēšanas centrā. Tālāk skatiet Piemēru PowerShell cmdlet, kas sniedz iespēju visiem lietotājiem apiet vestibilu.

- [Automātiski ielaist personas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir rīkotāja politika, kas nosaka, vai personas pievienosies sapulcei tieši vai gaidīs vestibilā, līdz viņi var uzņemt autentificētu lietotāju.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Atļaut sākt sapulci anonīmām personām ir rīkotāja politika, kas nosaka, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez organizācijas dalības autentificēta lietotāja.

- Atļaut [iezvanes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) lietotājiem apiet vestibilu **(drīzumā**) ir organizatora politika, kas nosaka, vai personas, kuras veic iezvani pa tālruni, sapulcei pievienojas tieši vai gaida vestibilā neatkarīgi no iestatījuma Automātiski ielaist **personas.**

- Atļaut organizatoriem ignorēt vestibila iestatījumus (drīzumā ) ir rīkotāja politika, kas nosaka, vai  sapulces rīkotājs  var ignorēt vestibila iestatījumus, ko administrators ir iestatījis sadaļā Automātiski ielaist personas un Atļaut [iezvanes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) lietotājiem apiet vestibilu, ieplānojot jaunu sapulci.

**Piezīme.** Lai iegūtu pilnu pārskatu par Microsoft Teams sapulču politikām, izlasiet rakstu Sapulču politiku pārvaldība programmā [Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)
