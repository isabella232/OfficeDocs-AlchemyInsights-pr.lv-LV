---
title: Apmainiet savu klasisko saknes vietni ar mūsdienu vietā
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501086"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="2ec9f-102">Apmainiet savu klasisko saknes vietni ar mūsdienu vietā</span><span class="sxs-lookup"><span data-stu-id="2ec9f-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="2ec9f-103">Vidē bija uzslieta aprīlī 2019, saknes vietni mūsdienu vietu var mainīt, izmantojot Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2ec9f-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="2ec9f-104">Ja lietojat citu vietni, kuru vēlaties izmantot kā saknes vietni, (mijmaiņas) saknes vietni var aizstāt ar to.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="2ec9f-105">Izmantot [Izsaukums SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap atrašanās vietu ar citu vietā vienlaikus arhivē sākotnējā vietā.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="2ec9f-106">Pieejama gan darba grupas vietni (nav pievienots grupai) un saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="2ec9f-107">Tiks ieviesti papildu iespējas drīz, kas ļaus jums paturēt lietojot satura vietnē, bet pārvērst esošo vietni ir saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="2ec9f-108">Šīs iespējas tiek izveltnē pakāpeniski.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="2ec9f-109">Turpina pārbaudīt atjauninājumus Office 365 ziņu centru.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="2ec9f-110">Zināmas problēmas ar apmainīšana vietām</span><span class="sxs-lookup"><span data-stu-id="2ec9f-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="2ec9f-111">Mērķa vietnes var atgriezt "nav atrasts" kļūda (HTTP 404) uz neilgu laika periodu.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="2ec9f-112">Saturs būs nepieciešams recrawled atjaunināt meklēšanas indeksā.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="2ec9f-113">Nav nepieciešama manuāla soļu - tas tiks veikts automātiski.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="2ec9f-114">Viss atkarīgs no "statisku" saites (piemēram, failu sinhronizēšana un OneNote failus) vajadzēs manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="2ec9f-115">Ja avota vietnes organizatoriskie jaunumi vietā, atjaunināt URL.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="2ec9f-116">Parādīts saraksts ar visu organizatorisko ziņu portālos.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="2ec9f-117">Project Server vietņu, iespējams, tiks pārbaudīti, vai tie ir joprojām saistīts pareizi.</span><span class="sxs-lookup"><span data-stu-id="2ec9f-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





