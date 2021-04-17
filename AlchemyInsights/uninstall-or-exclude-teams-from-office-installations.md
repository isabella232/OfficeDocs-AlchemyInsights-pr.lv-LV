---
title: Teams atinstalēšana vai izslēgšana no Office instalācijām
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
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827799"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="b68b8-102">Teams atinstalēšana vai izslēgšana no jaunām vai esošām Office instalācijām</span><span class="sxs-lookup"><span data-stu-id="b68b8-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="b68b8-103">Microsoft Teams ir iekļauta kā daļa no Microsoft 365 programmām uzņēmumiem, Microsoft 365 programmām darbam un Office darbam ar Mac.</span><span class="sxs-lookup"><span data-stu-id="b68b8-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="b68b8-104">Izmantojiet [Office izvietošanas rīku, lai](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) izslēgtu Teams no jaunām Office instalācijām.</span><span class="sxs-lookup"><span data-stu-id="b68b8-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="b68b8-105">Lai *atinstalētu* Teams ierīcē, kurā darbojas Windows, skatiet rakstu [Microsoft Teams atinstalēšana.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="b68b8-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="b68b8-106">Lai tīrīt Microsoft Teams no vairākiem mērķa datoriem vai lietotājiem, skatiet [sadaļu Microsoft Teams izvietošanas tīrīšana.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="b68b8-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="b68b8-107">[PreventTeams lietošanaInstalēšanas](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) opcija, lai neļautu Microsoft Teams automātiski instalēt ar Office.</span><span class="sxs-lookup"><span data-stu-id="b68b8-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="b68b8-108">Izmantojiet opciju [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) pirms *Teams* instalēšanas , lai neļautu Microsoft Teams automātiski sākt darbu pēc instalēšanas.</span><span class="sxs-lookup"><span data-stu-id="b68b8-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="b68b8-109">Ja izmantojat Office for Mac, skatiet rakstu [Microsoft Teams instalācijas Mac datorā.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="b68b8-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>