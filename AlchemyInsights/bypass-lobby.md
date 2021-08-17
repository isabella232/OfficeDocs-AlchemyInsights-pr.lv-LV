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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059603"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Vestibila iestatījumu un dalības līmeņa Teams

Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmiem lietotājiem, apiet vestibilu, izmantojiet PowerShell, lai veiktu šo uzdevumu. Šeit ir savas organizācijas globālās sapulces politikas modificēšanas piemērs.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šai cmdlet pašlaik ir nepieciešams Skype darbam PowerShell. Lai iestatītu šī cmdlet izmantošanu, skatiet rakstā Politiku [pārvaldība, izmantojot PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Kad politika ir iestatīta, tā ir jālieto lietotājiem; vai, ja esat modificējis globālo politiku, tā tiek automātiski lietota lietotājiem. Lai politikas izmaiņas stāsies spēkā, ir jāgaida vismaz 4 stundas līdz **24** stundām. 

Noteikti pārskatiet tālāk esošo dokumentāciju, pirms veicat šīs izmaiņas, lai saprastu, ko tas atļauj.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Informācija Teams vestibila politikas vadīklām

Šie iestatījumi nosaka, kuriem sapulces dalībniekiem jāgaida vestibilā, pirms viņi var piedalīties sapulcē, kā arī norādīts, kādā līmenī dalībnieki var piedalīties sapulcē. Varat izmantot PowerShell, lai atjauninātu sapulces politikas iestatījumus, kas vēl nav ieviesti (apzīmēti kā "drīzumā") Teams centrā. Tālāk skatiet Piemēru PowerShell cmdlet, kas sniedz iespēju visiem lietotājiem apiet vestibilu.

- [Automātiski ielaist personas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir rīkotāja politika, kas nosaka, vai personas pievienosies sapulcei tieši vai gaidīs vestibilā, līdz viņi var uzņemt autentificētu lietotāju.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Atļaut sākt sapulci anonīmām personām ir rīkotāja politika, kas nosaka, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez organizācijas dalības autentificēta lietotāja.

- Atļaut [iezvanes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) lietotājiem apiet vestibilu **(drīzumā**) ir organizatora politika, kas nosaka, vai personas, kuras veic iezvani pa tālruni, sapulcei pievienojas tieši vai gaida vestibilā neatkarīgi no iestatījuma Automātiski ielaist **personas.**

- Atļaut organizatoriem ignorēt vestibila iestatījumus (drīzumā ) ir rīkotāja politika, kas nosaka, vai  sapulces rīkotājs  var ignorēt vestibila iestatījumus, ko administrators ir iestatījis sadaļā Automātiski ielaist personas un Atļaut [iezvanes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) lietotājiem apiet vestibilu, ieplānojot jaunu sapulci.

**Piezīme.** Pilnīgu [pārskatu par sapulču politikām Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) lasiet rakstu sapulču Microsoft Teams pārvaldība programmā Microsoft.
