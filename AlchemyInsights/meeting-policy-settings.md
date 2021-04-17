---
title: Sapulces politikas iestatījumi
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825450"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="931e9-102">Sapulču politiku pārvaldība darbvietā Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="931e9-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="931e9-103">**Piezīme. Var paiet līdz pat 24 stundām, līdz politikas izmaiņas stājas spēkā lietotājiem.**</span><span class="sxs-lookup"><span data-stu-id="931e9-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="931e9-104">Iespējams, uzreiz nevarēsit veikt izmaiņas jaunizveidotajā politikā. uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt jaunizveidotu politiku.</span><span class="sxs-lookup"><span data-stu-id="931e9-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="931e9-105">Sapulču politikas tiek izmantotas, lai kontrolētu līdzekļus, kas pieejami sapulces dalībniekiem sapulcēm, kuras ir ieplānojis lietotājs jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="931e9-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="931e9-106">Daži sapulču politiku līdzekļi, iespējams, vēl netiks ieviesti Teams administrēšanas centrā (dokumentācijā tie apzīmēti ar "drīzumā").</span><span class="sxs-lookup"><span data-stu-id="931e9-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="931e9-107">Šajā gadījumā vai, ja saņemat kļūdas ziņojumu, piemēram, "Mēs pašlaik nevaram atjaunināt politiku, bet vēlāk to mēģināt vēlreiz" Microsoft Teams administrēšanas centrā, mēs iesakām izmantot PowerShell, lai izveidotu vai modificētu Teams sapulču politikas.</span><span class="sxs-lookup"><span data-stu-id="931e9-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="931e9-108">Papildinformāciju par sapulču politikām skatiet šādos resursos:</span><span class="sxs-lookup"><span data-stu-id="931e9-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="931e9-109">Informāciju par to, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājus politikai, skatiet rakstā [Sapulču politiku pārvaldība programmā Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="931e9-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="931e9-110">Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet [rakstu Teams PowerShell pārskats.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="931e9-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="931e9-111">Jums ir jāizmanto [Skype darbam PowerShell modulis Teams](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) sapulču politikām.</span><span class="sxs-lookup"><span data-stu-id="931e9-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="931e9-112">[Papildinformāciju skatiet \*-CsTeamsMeetingPolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentācijā.</span><span class="sxs-lookup"><span data-stu-id="931e9-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

