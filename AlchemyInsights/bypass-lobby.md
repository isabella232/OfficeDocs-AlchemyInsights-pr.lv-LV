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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768447"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrolēt vestibila iestatījumus un dalības līmeni

Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmajiem lietotājiem apiet vestibilā Microsoft Teams, varat izmantot PowerShell, lai to izdarītu. Tālāk ir piemērs, kā modificēt organizācijas globālo sapulču politiku.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šī cmdlet pašlaik ir nepieciešams izmantot Skype biznesa PowerShell modulis. Lai iegūtu setup izmantot šo cmdlet, izbraukšana [pārvaldības politiku, izmantojot PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Varat iestatīt jaunu politiku, kas pēc tam ir jālieto lietotājiem. Ja modificēsit globālo politiku, tā automātiski tiks piemērota lietotājiem. Visām politikas izmaiņām jums ir jāgaida vismaz 4 stundas un līdz 24 stundām, lai politikas stātos spēkā.

Noteikti pārskatīt dokumentāciju, pirms veikt šīs izmaiņas, lai saprastu, ko tieši tas ļauj.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Izpratne komandas sanāksme Lobby politikas kontrole

- [Automātiski uzņemt cilvēki](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir per-organizators politika, kas kontrolē to, vai cilvēki pievienoties sapulcei tieši vai gaidīt vestibilā līdz tos atzīst autentificēts lietotājs.

- [Atļaut anonīmajiem cilvēkiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir katra kārtotāja politika, kas kontrolē to, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez autentificēta lietotāja no organizācijas apmeklētības.

- [Atļaut iezvanes lietotājiem apiet vestibilu](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(drīzumā**) ir per-Organizer politika, kas kontrolē, vai cilvēki, kuri iezvanās pa tālruni, pievienojas sapulcei tieši vai gaida vestibilā neatkarīgi no **automātiski uzņemt personas** iestatījumu.

- [Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir katra kārtotāja politika, kas kontrolē, vai sapulces organizators var ignorēt vestibila iestatījumus, ko administrators ir iestatījis, lai **automātiski uzņemtu** lietotājus un **ļautu iezvanes lietotājiem apiet vestibilu** , plānojot jaunu sapulci.

**Piezīme:** Izlasiet [komandu pārvaldīt sapulču politiku komandā](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.
