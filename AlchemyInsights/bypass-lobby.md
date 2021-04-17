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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="86036-102">Vestibila iestatījumu un dalības līmeņa vadība programmā Teams</span><span class="sxs-lookup"><span data-stu-id="86036-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="86036-103">Ja vēlaties atļaut visiem, tostarp iezvanes, ārējiem un anonīmiem lietotājiem, apiet vestibilu, izmantojiet PowerShell, lai veiktu šo uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="86036-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="86036-104">Šeit ir savas organizācijas globālās sapulces politikas modificēšanas piemērs.</span><span class="sxs-lookup"><span data-stu-id="86036-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="86036-105">Šai cmdlet pašlaik ir nepieciešams Skype darbam PowerShell modulis.</span><span class="sxs-lookup"><span data-stu-id="86036-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="86036-106">Lai iestatītu šī cmdlet izmantošanu, skatiet rakstā Politiku [pārvaldība, izmantojot PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="86036-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="86036-107">Kad politika ir iestatīta, tā ir jālieto lietotājiem; vai, ja esat modificējis globālo politiku, tā tiek automātiski lietota lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="86036-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="86036-108">Lai politikas izmaiņas stāsies spēkā, ir jāgaida vismaz 4 stundas līdz **24** stundām.</span><span class="sxs-lookup"><span data-stu-id="86036-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="86036-109">Noteikti pārskatiet tālāk esošo dokumentāciju, pirms veicat šīs izmaiņas, lai saprastu, ko tas atļauj.</span><span class="sxs-lookup"><span data-stu-id="86036-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="86036-110">Par Teams sapulču vestibila politikas vadīklām</span><span class="sxs-lookup"><span data-stu-id="86036-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="86036-111">Šie iestatījumi nosaka, kuriem sapulces dalībniekiem jāgaida vestibilā, pirms viņi var piedalīties sapulcē, kā arī norādīts, kādā līmenī dalībnieki var piedalīties sapulcē.</span><span class="sxs-lookup"><span data-stu-id="86036-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="86036-112">Varat izmantot PowerShell, lai atjauninātu sapulces politikas iestatījumus, kas vēl nav ieviesti (apzīmēti kā "drīzumā") Teams administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="86036-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="86036-113">Tālāk skatiet Piemēru PowerShell cmdlet, kas sniedz iespēju visiem lietotājiem apiet vestibilu.</span><span class="sxs-lookup"><span data-stu-id="86036-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="86036-114">[Automātiski ielaist personas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ir rīkotāja politika, kas nosaka, vai personas pievienosies sapulcei tieši vai gaidīs vestibilā, līdz viņi var uzņemt autentificētu lietotāju.</span><span class="sxs-lookup"><span data-stu-id="86036-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="86036-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Atļaut sākt sapulci anonīmām personām ir rīkotāja politika, kas nosaka, vai anonīmas personas, tostarp B2B un federatīvie lietotāji, var pievienoties lietotāja sapulcei bez organizācijas dalības autentificēta lietotāja.</span><span class="sxs-lookup"><span data-stu-id="86036-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="86036-116">Atļaut [iezvanes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) lietotājiem apiet vestibilu **(drīzumā**) ir organizatora politika, kas nosaka, vai personas, kuras veic iezvani pa tālruni, sapulcei pievienojas tieši vai gaida vestibilā neatkarīgi no iestatījuma Automātiski ielaist **personas.**</span><span class="sxs-lookup"><span data-stu-id="86036-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="86036-117">Atļaut organizatoriem ignorēt vestibila iestatījumus (drīzumā ) ir rīkotāja politika, kas nosaka, vai  sapulces rīkotājs  var ignorēt vestibila iestatījumus, ko administrators ir iestatījis sadaļā Automātiski ielaist personas un Atļaut [iezvanes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) lietotājiem apiet vestibilu, ieplānojot jaunu sapulci.</span><span class="sxs-lookup"><span data-stu-id="86036-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="86036-118">**Piezīme.** Lai iegūtu pilnu pārskatu par Microsoft Teams sapulču politikām, izlasiet rakstu Sapulču politiku pārvaldība programmā [Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="86036-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
