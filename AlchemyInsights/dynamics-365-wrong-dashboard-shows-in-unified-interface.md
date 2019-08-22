---
title: Dynamics 365 - nepareizi informācijas panelis parāda Dynamics 365 vienotu interfeisu
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528558"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="df2ad-102">Nepareizi informācijas panelis parāda Dynamics 365 vienotu interfeisu</span><span class="sxs-lookup"><span data-stu-id="df2ad-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="df2ad-103">Ir vairāki iemesli, kāpēc var redzēt dažādu paneļa, nevis to, kas jūs sagaida:</span><span class="sxs-lookup"><span data-stu-id="df2ad-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="df2ad-104">Lietotājs ir iestatījis noklusēto paneļa lietotāja</span><span class="sxs-lookup"><span data-stu-id="df2ad-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="df2ad-105">Parasti lietotājs var noteikt noklusēto paneļa ir iestatīts, ja **Iestatīts kā noklusējuma** poga nav redzama paneļa darbību joslā.</span><span class="sxs-lookup"><span data-stu-id="df2ad-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="df2ad-106">Lietotāja noklusēto paneļa ignorē citu noklusējuma paneļus, pat ja lietotāja noklusēto paneļa neatrodas pašreizējā app.</span><span class="sxs-lookup"><span data-stu-id="df2ad-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="df2ad-107">Izmantot šādu profilakse, lai atiestatītu savu noklusēto paneļa.</span><span class="sxs-lookup"><span data-stu-id="df2ad-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="df2ad-108">Izveidot jaunas personiskās informācijas paneli.</span><span class="sxs-lookup"><span data-stu-id="df2ad-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="df2ad-109">Noteikts, ka jaunā paneļa lietotāja noklusējums.</span><span class="sxs-lookup"><span data-stu-id="df2ad-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="df2ad-110">Dzēst šo vadības paneli.</span><span class="sxs-lookup"><span data-stu-id="df2ad-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="df2ad-111">Informācijas panelis ir iestatīts sitemap</span><span class="sxs-lookup"><span data-stu-id="df2ad-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="df2ad-112">Jums var noteikt organizācijas noklusēto paneļa izvēloties informācijas panelī un izvēloties 'iestatīt kā noklusējuma"saskaņā ar"Pielāgot sistēmu".</span><span class="sxs-lookup"><span data-stu-id="df2ad-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="df2ad-113">Bet noteikts sitemap dizainers dashboard tiks ņem virsroku pār paneļa, ja lietotājam ir piekļuve.</span><span class="sxs-lookup"><span data-stu-id="df2ad-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="df2ad-114">Lai apskatītu paneļa iestatāt kā noklusējuma organizācijas lietotājiem, jūs varat:</span><span class="sxs-lookup"><span data-stu-id="df2ad-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="df2ad-115">Noteikts, ka dashboard sitemap</span><span class="sxs-lookup"><span data-stu-id="df2ad-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="df2ad-116">Atspējot piekļuvi sitemap noteikti paneļa tiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="df2ad-116">Remove access to the sitemap defined dashboard for those users</span></span>
