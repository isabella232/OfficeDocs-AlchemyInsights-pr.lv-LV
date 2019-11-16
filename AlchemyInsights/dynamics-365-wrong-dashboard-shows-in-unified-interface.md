---
title: Dynamics 365-nepareiza informācijas paneļa parāda Dynamics 365 vienotā interfeisā
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528558"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="95ddd-102">Nepareizs informācijas panelis parāda Dynamics 365 vienotā interfeisā</span><span class="sxs-lookup"><span data-stu-id="95ddd-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="95ddd-103">Ir vairāki iemesli, kāpēc var tikt parādīts cits informācijas panelis, nekā paredzēts:</span><span class="sxs-lookup"><span data-stu-id="95ddd-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="95ddd-104">Lietotājs ir iestatījis lietotāja noklusējuma informācijas paneli</span><span class="sxs-lookup"><span data-stu-id="95ddd-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="95ddd-105">Parasti var identificēt lietotāja noklusējuma informācijas paneli ir iestatīts, ja poga **Iestatīt kā noklusējumu** informācijas paneļa komandu joslā netiek rādīta.</span><span class="sxs-lookup"><span data-stu-id="95ddd-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="95ddd-106">Lietotāja noklusējuma informācijas panelis ignorē visus pārējos noklusējuma informācijas paneļus, pat ja lietotāja noklusējuma informācijas panelis nav pašreizējā programmā.</span><span class="sxs-lookup"><span data-stu-id="95ddd-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="95ddd-107">Lai unset noklusējuma informācijas paneli, izmantojiet tālāk minēto metodi.</span><span class="sxs-lookup"><span data-stu-id="95ddd-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="95ddd-108">Izveidojiet jaunu personisko informācijas paneli.</span><span class="sxs-lookup"><span data-stu-id="95ddd-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="95ddd-109">Iestatiet jauno informācijas paneli kā lietotāja noklusējumu.</span><span class="sxs-lookup"><span data-stu-id="95ddd-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="95ddd-110">Dzēsiet šo informācijas paneli.</span><span class="sxs-lookup"><span data-stu-id="95ddd-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="95ddd-111">Informācijas panelis ir iestatīts vietnes kartē</span><span class="sxs-lookup"><span data-stu-id="95ddd-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="95ddd-112">Iespējams, esat iestatījis organizācijas noklusējuma informācijas paneli, atlasot informācijas paneli un izvēloties "iestatīt kā noklusējumu" sadaļā "sistēmas pielāgošana".</span><span class="sxs-lookup"><span data-stu-id="95ddd-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="95ddd-113">Bet informācijas panelis noteikts sitemap dizainers būs priekšroka pār šo informācijas paneli, ja lietotājs var piekļūt.</span><span class="sxs-lookup"><span data-stu-id="95ddd-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="95ddd-114">Lai lietotāji redzētu informācijas paneli, kuru esat iestatījis kā organizācijas noklusējumu, varat:</span><span class="sxs-lookup"><span data-stu-id="95ddd-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="95ddd-115">Iestatīt šo informācijas paneli vietnes kartē</span><span class="sxs-lookup"><span data-stu-id="95ddd-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="95ddd-116">Noņemt piekļuvi vietnes karte definēts informācijas panelis tiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="95ddd-116">Remove access to the sitemap defined dashboard for those users</span></span>
