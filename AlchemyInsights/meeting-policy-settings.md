---
title: Sapulču politikas iestatījumi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376724"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="b7a3d-102">Sapulču politiku pārvaldīšana programmā Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b7a3d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="b7a3d-103">Sapulču politikas tiek izmantotas, lai kontrolētu līdzekļus, kas ir pieejami sapulces dalībniekiem sapulcēs, kuras ieplānoja lietotāji jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="b7a3d-104">Daži sapulču politikas līdzekļi, iespējams, nav ieviesti komandu administrēšanas centrā, tomēr (dokumentācijā tie ir apzīmēti ar "drīzumā").</span><span class="sxs-lookup"><span data-stu-id="b7a3d-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="b7a3d-105">Šajā gadījumā, vai, ja saņemat kļūdas, piemēram, "mēs nevaram atjaunināt politiku tūlīt, bet mēģināt vēlreiz vēlāk" Microsoft Teams administrēšanas centrs, ieteicams izmantot PowerShell, lai izveidotu vai modificētu grupas sapulču politiku.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="b7a3d-106">Lai iegūtu papildinformāciju par sapulču politiku, skatiet šādus resursus:</span><span class="sxs-lookup"><span data-stu-id="b7a3d-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="b7a3d-107">Lai uzzinātu, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājiem politiku, skatiet sadaļu [Sapulču politiku pārvaldīšana komandā](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="b7a3d-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="b7a3d-108">Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet [Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="b7a3d-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="b7a3d-109">Jums ir jāizmanto [Skype biznesa PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) grupas sapulču politiku.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="b7a3d-110">Pārskatiet [\*-csteamsmeetingpolicy cmdlet dokumentāciju](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="b7a3d-111">**Piezīme:** Politikas izmaiņām var būt nepieciešams līdz 24 stundām, lai tās stātos spēkā lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="b7a3d-112">Iespējams, nevarēsit nekavējoties veikt izmaiņas jaunizveidotajā politikā; uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt tikko izveidoto politiku.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="b7a3d-113">Ja jums joprojām ir problēmas, mēģiniet PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b7a3d-113">If you're still having problems, try PowerShell.</span></span>  