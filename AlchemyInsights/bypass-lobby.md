---
title: Apvedceļa vestibils
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684957"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Vadības vestibila iestatījumi un dalības līmenis komandās

Ja vēlaties atļaut visiem lietotājiem, ieskaitot iezvanes, ārējos un anonīmos lietotājus, **apiet vestibilu**, izmantojiet PowerShell, lai izpildītu šo uzdevumu. Tālāk ir parādīts piemērs, kā modificēt globālās sapulces politiku savai organizācijai.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šajā cmdlet pašlaik ir jāizmanto Skype darbam PowerShell modulis. Lai iestatītu šī cmdlet lietošanu, skatiet rakstu [politiku pārvaldība, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kad būsit iestatījis politiku, tā ir jālieto lietotājiem. Ja esat modificējis globālo politiku, tā tiks automātiski lietota lietotājiem. Lai veiktu jebkādas politikas izmaiņas, ir jāgaida vismaz **4 stundas līdz 24 stundām** , lai politikas stātos spēkā. 

Pirms izmaiņu veikšanas noteikti pārskatiet tālāk esošo dokumentāciju.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Izpratne par Teams sapulču Lobby politikas vadīklām

Šie iestatījumi nosaka, kuras sapulces dalībnieki gaida vestibilā, pirms tie tiek uzņemti sapulcē un dalības līmenis ir atļauts sapulcē. Varat izmantot PowerShell, lai atjauninātu sapulču politikas iestatījumus, kas vēl nav ieviesti (ar atzīmi "būs pieejams drīzumā") grupu administrēšanas centrā. Skatiet tālāk norādīto PowerShell cmdlet piemēru, kas ļauj visiem lietotājiem apiet vestibilu.

- [Automātiska personu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) uzņemšana ir viena organizatora politika, kas nosaka, vai lietotāji pievienojas sapulcei tieši vai nogaida vestibilā, līdz tos uzņem autentificēts lietotājs.

- [Atļaut anonīmiem lietotājiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir viena organizatora politika, kas kontrolē, vai anonīmi lietotāji, tostarp B2B un integrētās lietotāji, var pievienoties lietotāja sapulcei, neizmantojot autentificētu lietotāju no klātesošajām organizācijām.

- [Atļaut iezvanes lietotājus apiet vestibilu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**drīzumā**) ir viena organizatora politika, kas nosaka, vai personas, kas iezvanās pa tālruni, pievienojas sapulcei tieši vai nogaida vestibilā neatkarīgi no tā, vai tiek iestatīts **Automātiskais personu** iestatījums.

- [Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir viena organizatora politika, kas nosaka, vai sapulces rīkotājs var ignorēt vestibila iestatījumus, ko administrators ir iestatījis **automātiski uzņemt** , un **Atļaut iezvanes lietotājiem apiet vestibilu** , kad viņi plāno jaunu sapulci.

**Piezīme:** Izlasiet rakstu [Sapulču politiku pārvaldība pakalpojumā Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.
