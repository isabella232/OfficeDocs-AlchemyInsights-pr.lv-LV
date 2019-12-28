---
title: Apvedceļš Lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889089"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrolējiet vestibila iestatījumus un dalības līmeni darba grupās

Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmajiem lietotājiem, **apiet vestibilā**, izmantojiet PowerShell, lai veiktu šo uzdevumu. Tālāk ir piemērs, kā modificēt organizācijas globālo sapulču politiku.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šī cmdlet pašlaik ir nepieciešams izmantot Skype biznesa PowerShell modulis. Lai iegūtu, kas izveidota, lai izmantotu šo cmdlet, izbraukšana [pārvaldības politiku, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kad esat iestatījis politiku, jums tā ir jāpiemēro lietotājiem; vai, ja modificējat globālo politiku, tā automātiski tiks piemērota lietotājiem. Visām politikas izmaiņām ir jāgaida vismaz **4 stundas līdz 24 stundām** , lai politikas stātos spēkā. 

Noteikti pārskatīt dokumentāciju, pirms veikt šīs izmaiņas, lai saprastu, ko tieši tas ļauj.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Izpratne komandas sanāksme Lobby politikas kontrole

Šie iestatījumi nosaka, kuri sapulces dalībnieki gaida vestibilā, pirms tie tiek uzņemti sapulcē, un līdzdalības līmenis, kas ir atļauts sapulcē. Varat izmantot PowerShell atjaunināt sapulču politikas iestatījumus, kas vēl nav ieviesti (ar nosaukumu "drīzumā") komandu administrēšanas centrs. Skatiet tālāk piemēru PowerShell cmdlet, kas ļauj visiem lietotājiem apiet vestibilā.

- [Automātiski uzņemt cilvēki](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir per-organizators politika, kas kontrolē to, vai cilvēki pievienoties sapulcei tieši vai gaidīt vestibilā līdz tos atzīst autentificēts lietotājs.

- [Atļaut anonīmajiem cilvēkiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir katra kārtotāja politika, kas kontrolē to, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez autentificēta lietotāja no organizācijas apmeklētības.

- [Atļaut iezvanes lietotājiem apiet vestibilu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(drīzumā**) ir per-Organizer politika, kas kontrolē, vai cilvēki, kuri iezvanās pa tālruni, pievienojas sapulcei tieši vai gaida vestibilā neatkarīgi no **automātiski uzņemt personas** iestatījumu.

- [Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir katra kārtotāja politika, kas kontrolē, vai sapulces organizators var ignorēt vestibila iestatījumus, ko administrators ir iestatījis, lai **automātiski uzņemtu** lietotājus un **ļautu iezvanes lietotājiem apiet vestibilu** , plānojot jaunu sapulci.

**Piezīme:** Izlasiet [komandu pārvaldīt sapulču politiku komandā](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.
