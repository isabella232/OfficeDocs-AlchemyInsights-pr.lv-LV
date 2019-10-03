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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="6dd2d-102">Kontrolēt vestibila iestatījumus un dalības līmeni</span><span class="sxs-lookup"><span data-stu-id="6dd2d-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="6dd2d-103">Šie iestatījumi nosaka, kuri sapulces dalībnieki gaida vestibilā, pirms tie tiek uzņemti sapulcē, un līdzdalības līmenis, kas ir atļauts sapulcē.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="6dd2d-104">Varat izmantot PowerShell atjaunināt sapulču politikas iestatījumus, kas vēl nav ieviesti (ar nosaukumu "drīzumā") komandu administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="6dd2d-105">Skatiet tālāk piemēru PowerShell cmdlet, kas ļauj visiem lietotājiem apiet vestibilā.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="6dd2d-106">[Automātiski uzņemt cilvēki](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir per-organizators politika, kas kontrolē to, vai cilvēki pievienoties sapulcei tieši vai gaidīt vestibilā līdz tos atzīst autentificēts lietotājs.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="6dd2d-107">[Atļaut anonīmajiem cilvēkiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir katra kārtotāja politika, kas kontrolē to, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez autentificēta lietotāja no organizācijas apmeklētības.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="6dd2d-108">[Atļaut iezvanes lietotājiem apiet vestibilu](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(drīzumā**) ir per-Organizer politika, kas kontrolē, vai cilvēki, kuri iezvanās pa tālruni, pievienojas sapulcei tieši vai gaida vestibilā neatkarīgi no **automātiski uzņemt personas** iestatījumu.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="6dd2d-109">[Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir katra kārtotāja politika, kas kontrolē, vai sapulces organizators var ignorēt vestibila iestatījumus, ko administrators ir iestatījis, lai **automātiski uzņemtu cilvēkus** un **atļautu iezvanes lietotājiem apiet vestibilā** , plānojot jaunu sapulci.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="6dd2d-110">**Piezīme:** Izlasiet [komandu pārvaldīt sapulču politiku komandā](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="6dd2d-111">**PowerShell piemērs**</span><span class="sxs-lookup"><span data-stu-id="6dd2d-111">**PowerShell example**</span></span>

<span data-ttu-id="6dd2d-112">Ja vēlaties atļaut visiem, tostarp ārējiem vai anonīmiem lietotājiem, apiet vestibilu, varat arī izmantot PowerShell, lai veiktu šo uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="6dd2d-113">Tālāk ir piemērs, kā modificēt organizācijas globālo sapulču politiku.</span><span class="sxs-lookup"><span data-stu-id="6dd2d-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="6dd2d-114">(Noteikti pārskatiet iepriekš minēto dokumentāciju, pirms veicat šīs izmaiņas, lai saprastu, ko tieši tas ļauj.)</span><span class="sxs-lookup"><span data-stu-id="6dd2d-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="6dd2d-115">Set-CsTeamsMeetingPolicy-identitātes globālās-Autouzņemšanuusers "ikvienam"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="6dd2d-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="6dd2d-116">Lai iegūtu papildinformāciju, skatiet [Set CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="6dd2d-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
