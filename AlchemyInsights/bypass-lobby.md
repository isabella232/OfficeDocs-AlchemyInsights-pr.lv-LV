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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376729"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrolēt vestibila iestatījumus un dalības līmeni

Šie iestatījumi nosaka, kuri sapulces dalībnieki gaida vestibilā, pirms tie tiek uzņemti sapulcē, un līdzdalības līmenis, kas ir atļauts sapulcē. Varat izmantot PowerShell atjaunināt sapulču politikas iestatījumus, kas vēl nav ieviesti (ar nosaukumu "drīzumā") komandu administrēšanas centrs.  Skatiet tālāk piemēru PowerShell cmdlet, kas ļauj visiem lietotājiem apiet vestibilā.  

- [Automātiski uzņemt cilvēki](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir per-organizators politika, kas kontrolē to, vai cilvēki pievienoties sapulcei tieši vai gaidīt vestibilā līdz tos atzīst autentificēts lietotājs.

- [Atļaut anonīmajiem cilvēkiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir katra kārtotāja politika, kas kontrolē to, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez autentificēta lietotāja no organizācijas apmeklētības.

- [Atļaut iezvanes lietotājiem apiet vestibilu](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(drīzumā**) ir per-Organizer politika, kas kontrolē, vai cilvēki, kuri iezvanās pa tālruni, pievienojas sapulcei tieši vai gaida vestibilā neatkarīgi no **automātiski uzņemt personas** iestatījumu.

- [Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir katra kārtotāja politika, kas kontrolē, vai sapulces organizators var ignorēt vestibila iestatījumus, ko administrators ir iestatījis, lai **automātiski uzņemtu cilvēkus** un **atļautu iezvanes lietotājiem apiet vestibilā** , plānojot jaunu sapulci.

**Piezīme:** Izlasiet [komandu pārvaldīt sapulču politiku komandā](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām. 


**PowerShell piemērs**

Ja vēlaties atļaut visiem, tostarp ārējiem vai anonīmiem lietotājiem, apiet vestibilu, varat arī izmantot PowerShell, lai veiktu šo uzdevumu.  Tālāk ir piemērs, kā modificēt organizācijas globālo sapulču politiku.   

(Noteikti pārskatiet iepriekš minēto dokumentāciju, pirms veicat šīs izmaiņas, lai saprastu, ko tieši tas ļauj.)

Set-CsTeamsMeetingPolicy-identitātes globālās-Autouzņemšanuusers "ikvienam"-AllowPSTNUsersToBypassLobby $True

Lai iegūtu papildinformāciju, skatiet [Set CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
