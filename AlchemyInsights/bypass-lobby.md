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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="50f57-102">Vadības vestibila iestatījumi un dalības līmenis komandās</span><span class="sxs-lookup"><span data-stu-id="50f57-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="50f57-103">Ja vēlaties atļaut visiem lietotājiem, ieskaitot iezvanes, ārējos un anonīmos lietotājus, **apiet vestibilu**, izmantojiet PowerShell, lai izpildītu šo uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="50f57-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="50f57-104">Tālāk ir parādīts piemērs, kā modificēt globālās sapulces politiku savai organizācijai.</span><span class="sxs-lookup"><span data-stu-id="50f57-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="50f57-105">Šajā cmdlet pašlaik ir jāizmanto Skype darbam PowerShell modulis.</span><span class="sxs-lookup"><span data-stu-id="50f57-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="50f57-106">Lai iestatītu šī cmdlet lietošanu, skatiet rakstu [politiku pārvaldība, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="50f57-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="50f57-107">Kad būsit iestatījis politiku, tā ir jālieto lietotājiem. Ja esat modificējis globālo politiku, tā tiks automātiski lietota lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="50f57-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="50f57-108">Lai veiktu jebkādas politikas izmaiņas, ir jāgaida vismaz **4 stundas līdz 24 stundām** , lai politikas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="50f57-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="50f57-109">Pirms izmaiņu veikšanas noteikti pārskatiet tālāk esošo dokumentāciju.</span><span class="sxs-lookup"><span data-stu-id="50f57-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="50f57-110">Izpratne par Teams sapulču Lobby politikas vadīklām</span><span class="sxs-lookup"><span data-stu-id="50f57-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="50f57-111">Šie iestatījumi nosaka, kuras sapulces dalībnieki gaida vestibilā, pirms tie tiek uzņemti sapulcē un dalības līmenis ir atļauts sapulcē.</span><span class="sxs-lookup"><span data-stu-id="50f57-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="50f57-112">Varat izmantot PowerShell, lai atjauninātu sapulču politikas iestatījumus, kas vēl nav ieviesti (ar atzīmi "būs pieejams drīzumā") grupu administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="50f57-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="50f57-113">Skatiet tālāk norādīto PowerShell cmdlet piemēru, kas ļauj visiem lietotājiem apiet vestibilu.</span><span class="sxs-lookup"><span data-stu-id="50f57-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="50f57-114">[Automātiska personu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) uzņemšana ir viena organizatora politika, kas nosaka, vai lietotāji pievienojas sapulcei tieši vai nogaida vestibilā, līdz tos uzņem autentificēts lietotājs.</span><span class="sxs-lookup"><span data-stu-id="50f57-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="50f57-115">[Atļaut anonīmiem lietotājiem sākt sapulci](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ir viena organizatora politika, kas kontrolē, vai anonīmi lietotāji, tostarp B2B un integrētās lietotāji, var pievienoties lietotāja sapulcei, neizmantojot autentificētu lietotāju no klātesošajām organizācijām.</span><span class="sxs-lookup"><span data-stu-id="50f57-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="50f57-116">[Atļaut iezvanes lietotājus apiet vestibilu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**drīzumā**) ir viena organizatora politika, kas nosaka, vai personas, kas iezvanās pa tālruni, pievienojas sapulcei tieši vai nogaida vestibilā neatkarīgi no tā, vai tiek iestatīts **Automātiskais personu** iestatījums.</span><span class="sxs-lookup"><span data-stu-id="50f57-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="50f57-117">[Atļaut organizatoriem ignorēt vestibila iestatījumus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**drīzumā**) ir viena organizatora politika, kas nosaka, vai sapulces rīkotājs var ignorēt vestibila iestatījumus, ko administrators ir iestatījis **automātiski uzņemt** , un **Atļaut iezvanes lietotājiem apiet vestibilu** , kad viņi plāno jaunu sapulci.</span><span class="sxs-lookup"><span data-stu-id="50f57-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="50f57-118">**Piezīme:** Izlasiet rakstu [Sapulču politiku pārvaldība pakalpojumā Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , lai iegūtu pilnīgu pārskatu par Microsoft Teams sapulču politikām.</span><span class="sxs-lookup"><span data-stu-id="50f57-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
