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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="c8d68-102">Kontrolējiet vestibila iestatījumus un dalības līmeni darba grupās</span><span class="sxs-lookup"><span data-stu-id="c8d68-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="c8d68-103">Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmajiem lietotājiem, **apiet vestibilā**, izmantojiet PowerShell, lai veiktu šo uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="c8d68-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="c8d68-104">Tālāk ir piemērs, kā modificēt organizācijas globālo sapulču politiku.</span><span class="sxs-lookup"><span data-stu-id="c8d68-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="c8d68-105">Šī cmdlet pašlaik ir nepieciešams izmantot Skype biznesa PowerShell modulis.</span><span class="sxs-lookup"><span data-stu-id="c8d68-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="c8d68-106">Lai iegūtu, kas izveidota, lai izmantotu šo cmdlet, izbraukšana [pārvaldības politiku, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="c8d68-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="c8d68-107">Kad esat iestatījis politiku, jums tā ir jāpiemēro lietotājiem; vai, ja modificējat globālo politiku, tā automātiski tiks piemērota lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="c8d68-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="c8d68-108">Visām politikas izmaiņām ir jāgaida vismaz **4 stundas līdz 24 stundām** , lai politikas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="c8d68-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="c8d68-109">Noteikti pārskatīt dokumentāciju, pirms veikt šīs izmaiņas, lai saprastu, ko tieši tas ļauj.</span><span class="sxs-lookup"><span data-stu-id="c8d68-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="c8d68-110">Izpratne komandas sanāksme Lobby politikas kontrole</span><span class="sxs-lookup"><span data-stu-id="c8d68-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="c8d68-111">Šie iestatījumi nosaka, kuri sapulces dalībnieki gaida vestibilā, pirms tie tiek uzņemti sapulcē, un līdzdalības līmenis, kas ir atļauts sapulcē.</span><span class="sxs-lookup"><span data-stu-id="c8d68-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="c8d68-112">Varat izmantot PowerShell atjaunināt sapulču politikas iestatījumus, kas vēl nav ieviesti (ar nosaukumu "drīzumā") komandu administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="c8d68-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="c8d68-113">Skatiet tālāk piemēru PowerShell cmdlet, kas ļauj visiem lietotājiem apiet vestibilā.</span><span class="sxs-lookup"><span data-stu-id="c8d68-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="c8d68-114">[Automātiski uzņemt cilvēki](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir per-organizators politika, kas kontrolē to, vai cilvēki pievienoties sapulcei tieši vai gaidīt vestibilā līdz tos atzīst autentificēts lietotājs.</span><span class="sxs-lookup"><span data-stu-id="c8d68-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c8d68-115">[Atļaut anonīmajiem cilvēkiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir katra kārtotāja politika, kas kontrolē to, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez autentificēta lietotāja no organizācijas apmeklētības.</span><span class="sxs-lookup"><span data-stu-id="c8d68-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c8d68-116">[Atļaut iezvanes lietotājiem apiet vestibilu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(drīzumā**) ir per-Organizer politika, kas kontrolē, vai cilvēki, kuri iezvanās pa tālruni, pievienojas sapulcei tieši vai gaida vestibilā neatkarīgi no **automātiski uzņemt personas** iestatījumu.</span><span class="sxs-lookup"><span data-stu-id="c8d68-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c8d68-117">[Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir katra kārtotāja politika, kas kontrolē, vai sapulces organizators var ignorēt vestibila iestatījumus, ko administrators ir iestatījis, lai **automātiski uzņemtu** lietotājus un **ļautu iezvanes lietotājiem apiet vestibilu** , plānojot jaunu sapulci.</span><span class="sxs-lookup"><span data-stu-id="c8d68-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c8d68-118">**Piezīme:** Izlasiet [komandu pārvaldīt sapulču politiku komandā](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.</span><span class="sxs-lookup"><span data-stu-id="c8d68-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
