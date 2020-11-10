---
title: Giphy izmantošana grupu sarunās
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982505"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="261c7-102">Giphy izmantošana grupu sarunās</span><span class="sxs-lookup"><span data-stu-id="261c7-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="261c7-103">Giphy piekļuve Teams tērzēšanā ir iespējota pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="261c7-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="261c7-104">Kā administrators varat kontrolēt, vai **giphy ir pieejami** lietotājiem, [iestatot ziņojumapmaiņas politiku](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) un nodrošinot, ka **sarunas izmanto giphy** .</span><span class="sxs-lookup"><span data-stu-id="261c7-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="261c7-105">Ja GIFs nedarbojas, kā paredzēts, grupu sarunās, pārbaudiet:</span><span class="sxs-lookup"><span data-stu-id="261c7-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="261c7-106">[Ziņojumapmaiņas politikai](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ir jāatļauj giphy.</span><span class="sxs-lookup"><span data-stu-id="261c7-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="261c7-107">Lai pārbaudītu, izmantojot PowerShell cmdlet:</span><span class="sxs-lookup"><span data-stu-id="261c7-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="261c7-108">Pārbaudiet, vai varat [pārvaldīt grupas, izmantojot PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="261c7-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="261c7-109">Palaidiet PowerShell komandu [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) un pārbaudiet, vai **AllowGiphy** ir iestatīts kā **patiess**.</span><span class="sxs-lookup"><span data-stu-id="261c7-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="261c7-110">Ja **AllowGiphy** ir iestatīts kā **aplams** , izpildiet tālāk norādītās PowerShell komandu [kopas-CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="261c7-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="261c7-111">[Neobligātās saistītās pieredzes](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) ir jāiespējo, lai atļautu piekļuvi Giphy vietrādim URL.</span><span class="sxs-lookup"><span data-stu-id="261c7-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="261c7-112">Ja jūsu nomniekam ir konfigurētas vairākas grupu ziņojumapmaiņas politikas, varat noteikt, kāda ir lietotāja piešķiramās politikas identitāte, izmantojot PowerShell komandu [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Atlasiet TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="261c7-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
