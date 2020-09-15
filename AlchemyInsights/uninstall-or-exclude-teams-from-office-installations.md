---
title: Darba grupu atinstalēšana vai izslēgšana no Office instalācijām
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658228"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="30d54-102">Grupu atinstalēšana vai izslēgšana no jaunajām vai esošajām Office instalācijām</span><span class="sxs-lookup"><span data-stu-id="30d54-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="30d54-103">Microsoft Teams ir iekļautas Microsoft 365 lietojumprogrammās, kas paredzētas uzņēmumiem, Microsoft 365 lietojumprogrammām darbam un Office for Mac.</span><span class="sxs-lookup"><span data-stu-id="30d54-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="30d54-104">Izmantojiet [Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , lai izslēgtu komandas no jaunām Office instalācijām.</span><span class="sxs-lookup"><span data-stu-id="30d54-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="30d54-105">Lai *atinstalētu* komandas no ierīces, kurā darbojas operētājsistēma Windows, skatiet rakstu [Microsoft Teams atinstalēšana](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="30d54-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="30d54-106">Lai iztīrītu Microsoft Teams no vairākiem Target datoriem vai lietotājiem, skatiet rakstu [Microsoft Teams izvietošanas tīrīšana](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="30d54-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="30d54-107">Izmantojiet [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) opciju, lai neļautu programmai Microsoft Teams automātiski instalēt Office.</span><span class="sxs-lookup"><span data-stu-id="30d54-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="30d54-108">Izmantojiet [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) opciju, *pirms darba grupas ir instalētas*, lai neļautu Microsoft Teams automātiski startēties pēc instalēšanas.</span><span class="sxs-lookup"><span data-stu-id="30d54-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="30d54-109">Ja izmantojat Office darbam ar Mac, skatiet rakstu [Microsoft Teams instalācijas Mac datorā](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="30d54-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>