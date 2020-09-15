---
title: Dynamics 365 — nepareizs informācijas panelis tiek rādīts Dynamics 365 vienotajā interfeisā
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711282"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c5d65-102">Nepareizs informācijas panelis tiek rādīts Dynamics 365 vienotajā interfeisā</span><span class="sxs-lookup"><span data-stu-id="c5d65-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c5d65-103">Pastāv vairāki iemesli, kāpēc, iespējams, redzēsit citu informācijas paneli, nevis vēlamo.</span><span class="sxs-lookup"><span data-stu-id="c5d65-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c5d65-104">Lietotājs ir iestatījis lietotāja noklusējuma informācijas paneli</span><span class="sxs-lookup"><span data-stu-id="c5d65-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c5d65-105">Parasti varat noteikt, ka lietotāja noklusējuma informācijas panelis ir iestatīts, ja nav redzama poga **Iestatīt kā noklusējumu** informācijas paneļa komandjoslā.</span><span class="sxs-lookup"><span data-stu-id="c5d65-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c5d65-106">Lietotāja noklusējuma informācijas panelī tiek ignorēti visi pārējie noklusējuma informācijas paneļi pat tad, ja lietotāja noklusējuma informācijas panelis nav pašreizējā lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="c5d65-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c5d65-107">Izmantojiet tālāk norādītos risinājumus, lai atiestatītu noklusējuma informācijas paneli.</span><span class="sxs-lookup"><span data-stu-id="c5d65-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c5d65-108">Izveidojiet jaunu personisko informācijas paneli.</span><span class="sxs-lookup"><span data-stu-id="c5d65-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c5d65-109">Iestatiet šo jauno informācijas paneli kā lietotāja noklusējumu.</span><span class="sxs-lookup"><span data-stu-id="c5d65-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c5d65-110">Dzēst šo informācijas paneli</span><span class="sxs-lookup"><span data-stu-id="c5d65-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c5d65-111">Informācijas panelis ir iestatīts vietnes kartē</span><span class="sxs-lookup"><span data-stu-id="c5d65-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c5d65-112">Iespējams, esat iestatījis organizācijas noklusējuma informācijas paneli, atlasot informācijas paneli un izvēloties "iestatīt kā noklusējumu" sadaļā sistēmas pielāgošana.</span><span class="sxs-lookup"><span data-stu-id="c5d65-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c5d65-113">Taču vietnes kartes noformētājā noteiktais informācijas panelis dominēs pār šo informācijas paneli, ja lietotājam tam ir piekļuve.</span><span class="sxs-lookup"><span data-stu-id="c5d65-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c5d65-114">Lai lietotāji redzētu informācijas paneļa, ko esat iestatījis kā organizācijas noklusējumu, varat veikt kādu no tālāk norādītajām darbībām.</span><span class="sxs-lookup"><span data-stu-id="c5d65-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c5d65-115">Informācijas paneļa iestatīšana vietnes kartē</span><span class="sxs-lookup"><span data-stu-id="c5d65-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c5d65-116">Noņemt piekļuvi vietnes kartes definētam informācijas panelim šiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="c5d65-116">Remove access to the sitemap defined dashboard for those users</span></span>
