---
title: Iespējot Teams webinars
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793786"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="10c10-102">Iespējot Teams webinars</span><span class="sxs-lookup"><span data-stu-id="10c10-102">Enable Teams Webinars</span></span>

<span data-ttu-id="10c10-103">Lietojumprogrammu lietojumprogrammas ir iespējotas pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="10c10-103">Webinars are enabled by default.</span></span> <span data-ttu-id="10c10-104">Izmantojot PowerShell komandas, varat Teams, lai pārvaldītu, kuras personas Teams jūsu webinars.</span><span class="sxs-lookup"><span data-stu-id="10c10-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="10c10-105">Visi lietotāji, kas var izveidot sapulci, var arī izveidot tīmekļa semināra sapulci.</span><span class="sxs-lookup"><span data-stu-id="10c10-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="10c10-106">Ja vēlaties pārvaldīt to, kuras personas var Teams Webinars, izmantojiet *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="10c10-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="10c10-107">Pēc noklusējuma *WhoCanRegister ir* iespējots un iestatīts uz **Everyone**.</span><span class="sxs-lookup"><span data-stu-id="10c10-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="10c10-108">Ja vēlaties izslēgt sapulces reģistrāciju, iestatiet *AllowMeetingRegistration* vērtību **False**.</span><span class="sxs-lookup"><span data-stu-id="10c10-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="10c10-109">Lai mainītu šos iestatījumus, ir [jāinstalē Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="10c10-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="10c10-110">Tāpat sapulču politikas ir ieviestas Teams tīmeklī.</span><span class="sxs-lookup"><span data-stu-id="10c10-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="10c10-111">Piemēram, ja sapulces iestatījumos ir izslēgta anonīma pievienošanās, anonīmi lietotāji nevar pievienoties tīmekļa semināriem.</span><span class="sxs-lookup"><span data-stu-id="10c10-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="10c10-112">Papildinformāciju par to, kā konfigurēt, kuras personas var reģistrēties tīmeklim, skatiet rakstā To personu konfigurēšana, [kas var reģistrēties tīmekļa semināriem.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="10c10-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="10c10-113">Papildinformāciju par Microsoft sarakstu iestatījumiem skatiet rakstā [Microsoft sarakstu vadības iestatījumi.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="10c10-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>