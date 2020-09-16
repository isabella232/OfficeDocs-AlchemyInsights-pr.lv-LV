---
title: Sapulču politikas iestatījumi
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794341"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="f9de1-102">Sapulču politikas pārvaldība pakalpojumā Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f9de1-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="f9de1-103">**Piezīme. lai politikas izmaiņas stātos spēkā lietotājiem, var paiet līdz pat 24 stundām.**</span><span class="sxs-lookup"><span data-stu-id="f9de1-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="f9de1-104">Jūs, iespējams, nevarēsit tūlīt veikt izmaiņas jaunizveidotās politikās; uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt jaunizveidoto politiku.</span><span class="sxs-lookup"><span data-stu-id="f9de1-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="f9de1-105">Sapulču politikas tiek lietotas, lai kontrolētu dalībniekiem pieejamos līdzekļus sapulcēm, ko ieplānojuši lietotāji jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="f9de1-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="f9de1-106">Daži sapulču politiku līdzekļi, iespējams, vēl nav implementēti grupu administrēšanas centrā (šeit ir atzīmēti "drīzumā").</span><span class="sxs-lookup"><span data-stu-id="f9de1-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="f9de1-107">Šajā gadījumā, vai, ja saņemat kļūdas ziņojumu, kas līdzīgs "pašlaik nevar atjaunināt politiku, bet vēlāk mēģiniet vēlreiz" Microsoft Teams administrēšanas centrā, iesakām izmantot PowerShell, lai izveidotu vai modificētu grupu sapulču politikas.</span><span class="sxs-lookup"><span data-stu-id="f9de1-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="f9de1-108">Papildinformāciju par sapulču politikām skatiet šajos resursos:</span><span class="sxs-lookup"><span data-stu-id="f9de1-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="f9de1-109">Lai uzzinātu, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājus politikai, skatiet rakstu [Sapulču politiku pārvaldība pakalpojumā Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="f9de1-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="f9de1-110">Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet rakstu [Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="f9de1-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="f9de1-111">Jums ir jāizmanto [Skype darbam PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) grupu sapulču politikām.</span><span class="sxs-lookup"><span data-stu-id="f9de1-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="f9de1-112">Lai iegūtu papildinformāciju, pārskatiet [\*-CsTeamsMeetingPolicy cmdlet dokumentāciju](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="f9de1-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

