---
title: Lietojumprogrammas semināra reģistrācijas pārvaldība
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793915"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="8c77b-102">Lietojumprogrammas semināra reģistrācijas pārvaldība</span><span class="sxs-lookup"><span data-stu-id="8c77b-102">Manage webinar registration</span></span>

<span data-ttu-id="8c77b-103">Izmantojot Powershell komandas, varat Teams, lai pārvaldītu, Teams jūsu webinars.</span><span class="sxs-lookup"><span data-stu-id="8c77b-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="8c77b-104">Lai instalētu Teams Powershell, skatiet [rakstu Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="8c77b-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="8c77b-105">Pēc noklusējuma *WhoCanRegister ir* iespējots un iestatīts uz **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="8c77b-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="8c77b-106">Lai atļautu visiem, tostarp anonīmiem lietotājiem, reģistrēties, sapulces politika ir jāiestata kā **Ikviens,** izmantojot Powershell komandu:</span><span class="sxs-lookup"><span data-stu-id="8c77b-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="8c77b-107">**Piezīme.** Ja sapulces iestatījumos ir izslēgta anonīma pievienošanās, anonīmi lietotāji nevar pievienoties tīmekļa semināriem.</span><span class="sxs-lookup"><span data-stu-id="8c77b-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="8c77b-108">Papildinformāciju un šī iestatījuma iespējošanu skatiet [rakstā Sapulces iestatījumu pārvaldība programmā Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="8c77b-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="8c77b-109">Ja vēlaties izslēgt sapulces reģistrāciju, iestatiet *AllowMeetingRegistration* vērtību **False**.</span><span class="sxs-lookup"><span data-stu-id="8c77b-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="8c77b-110">Papildinformāciju par to, kā konfigurēt, kuras personas var reģistrēties tīmeklim, skatiet rakstā To personu konfigurēšana, [kas var reģistrēties tīmekļa semināriem.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="8c77b-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="8c77b-111">Papildinformāciju par Microsoft sarakstu iestatījumiem skatiet rakstā [Microsoft sarakstu vadības iestatījumi.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="8c77b-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
