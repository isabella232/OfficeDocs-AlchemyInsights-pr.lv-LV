---
title: Atinstalējiet vai izslēdziet Teams no Office instalācijām
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/01/2019
ms.locfileid: "37344244"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="d232f-102">Atinstalējiet vai izslēdziet komandas no jaunajām vai esošajām Office instalācijām</span><span class="sxs-lookup"><span data-stu-id="d232f-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="d232f-103">Microsoft Teams tagad ir iekļauts kā daļa no Office 365 ProPlus, Office 365 Business un Office darbam ar Mac.</span><span class="sxs-lookup"><span data-stu-id="d232f-103">Microsoft Teams is now included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="d232f-104">Izmantojiet [Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) , lai neiekļautu komandas no jaunajām Office instalācijām.</span><span class="sxs-lookup"><span data-stu-id="d232f-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="d232f-105">Lai *atinstalētu* darba grupas no ierīces, kurā darbojas sistēma Windows, skatiet sadaļu [Microsoft Teams atinstalēšana](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="d232f-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="d232f-106">Lai iztīrītu Microsoft Teams no vairākām mērķa mašīnām vai lietotājiem, skatiet sadaļu [Microsoft Teams izvietošanas tīrīšana](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="d232f-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="d232f-107">Izmantojiet opciju [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , lai neļautu Microsoft komandām automātiski instalēt Office.</span><span class="sxs-lookup"><span data-stu-id="d232f-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="d232f-108">Izmantojiet opciju [Preventfirstlaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *pirms darba grupas ir instalētas*, lai neļautu Microsoft komandām automātiski startēties pēc instalēšanas.</span><span class="sxs-lookup"><span data-stu-id="d232f-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="d232f-109">Ja izmantojat Office for Mac, skatiet [Microsoft Teams instalācijas Mac datorā](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="d232f-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>