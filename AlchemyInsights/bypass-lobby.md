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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626355"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="55f92-102">Kontrolēt vestibila iestatījumus un dalības līmeni</span><span class="sxs-lookup"><span data-stu-id="55f92-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="55f92-103">Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmajiem lietotājiem apiet vestibilā Microsoft Teams, varat izmantot PowerShell, lai to izdarītu.</span><span class="sxs-lookup"><span data-stu-id="55f92-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="55f92-104">Tālāk ir piemērs, kā modificēt organizācijas globālo sapulču politiku.</span><span class="sxs-lookup"><span data-stu-id="55f92-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="55f92-105">Šī cmdlet pašlaik ir nepieciešams izmantot Skype biznesa PowerShell modulis.</span><span class="sxs-lookup"><span data-stu-id="55f92-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="55f92-106">Lai iegūtu setup izmantot šo cmdlet, izbraukšana [pārvaldības politiku, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="55f92-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="55f92-107">Varat iestatīt jaunu politiku, kas pēc tam ir jālieto lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="55f92-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="55f92-108">Ja modificēsit globālo politiku, tā automātiski tiks piemērota lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="55f92-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="55f92-109">Visām politikas izmaiņām jums ir jāgaida vismaz 4 stundas un līdz 24 stundām, lai politikas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="55f92-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="55f92-110">Noteikti pārskatīt dokumentāciju, pirms veikt šīs izmaiņas, lai saprastu, ko tieši tas ļauj.</span><span class="sxs-lookup"><span data-stu-id="55f92-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="55f92-111">Izpratne komandas sanāksme Lobby politikas kontrole</span><span class="sxs-lookup"><span data-stu-id="55f92-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="55f92-112">[Automātiski uzņemt cilvēki](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir per-organizators politika, kas kontrolē to, vai cilvēki pievienoties sapulcei tieši vai gaidīt vestibilā līdz tos atzīst autentificēts lietotājs.</span><span class="sxs-lookup"><span data-stu-id="55f92-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="55f92-113">[Atļaut anonīmajiem cilvēkiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir katra kārtotāja politika, kas kontrolē to, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez autentificēta lietotāja no organizācijas apmeklētības.</span><span class="sxs-lookup"><span data-stu-id="55f92-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="55f92-114">[Atļaut iezvanes lietotājiem apiet vestibilu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(drīzumā**) ir per-Organizer politika, kas kontrolē, vai cilvēki, kuri iezvanās pa tālruni, pievienojas sapulcei tieši vai gaida vestibilā neatkarīgi no **automātiski uzņemt personas** iestatījumu.</span><span class="sxs-lookup"><span data-stu-id="55f92-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="55f92-115">[Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir katra kārtotāja politika, kas kontrolē, vai sapulces organizators var ignorēt vestibila iestatījumus, ko administrators ir iestatījis, lai **automātiski uzņemtu** lietotājus un **ļautu iezvanes lietotājiem apiet vestibilu** , plānojot jaunu sapulci.</span><span class="sxs-lookup"><span data-stu-id="55f92-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="55f92-116">**Piezīme:** Izlasiet [komandu pārvaldīt sapulču politiku komandā](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.</span><span class="sxs-lookup"><span data-stu-id="55f92-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
