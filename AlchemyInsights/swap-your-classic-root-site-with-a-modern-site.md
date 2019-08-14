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
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270751"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="0db9a-102">Apmainiet savu klasisko saknes vietni ar mūsdienu vietā</span><span class="sxs-lookup"><span data-stu-id="0db9a-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="0db9a-103">Vidē bija uzslieta aprīlī 2019, saknes vietni mūsdienu vietu var mainīt, izmantojot Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0db9a-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="0db9a-104">Ja lietojat citu vietni, kuru vēlaties izmantot kā saknes vietni, (mijmaiņas) saknes vietni var aizstāt ar to.</span><span class="sxs-lookup"><span data-stu-id="0db9a-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="0db9a-105">Izmantot [Izsaukums SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap atrašanās vietu ar citu vietā vienlaikus arhivē sākotnējā vietā.</span><span class="sxs-lookup"><span data-stu-id="0db9a-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="0db9a-106">Pieejama gan darba grupas vietni (nav pievienots grupai) un saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="0db9a-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="0db9a-107">Tiks ieviesti papildu iespējas drīz, kas ļaus jums paturēt lietojot satura vietnē, bet pārvērst esošo vietni ir saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="0db9a-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="0db9a-108">Šīs iespējas tiek izveltnē pakāpeniski.</span><span class="sxs-lookup"><span data-stu-id="0db9a-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="0db9a-109">Turpina pārbaudīt atjauninājumus Office 365 ziņu centru.</span><span class="sxs-lookup"><span data-stu-id="0db9a-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="0db9a-110">Zināmas problēmas ar apmainīšana vietām</span><span class="sxs-lookup"><span data-stu-id="0db9a-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="0db9a-111">Mērķa vietnes var atgriezt "nav atrasts" kļūda (HTTP 404) uz neilgu laika periodu.</span><span class="sxs-lookup"><span data-stu-id="0db9a-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="0db9a-112">Saturs būs nepieciešams recrawled atjaunināt meklēšanas indeksā.</span><span class="sxs-lookup"><span data-stu-id="0db9a-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="0db9a-113">Nav nepieciešama manuāla soļu - tas tiks veikts automātiski.</span><span class="sxs-lookup"><span data-stu-id="0db9a-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="0db9a-114">Viss atkarīgs no "statisku" saites (piemēram, failu sinhronizēšana un OneNote failus) vajadzēs manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="0db9a-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="0db9a-115">Ja avota vietnes organizatoriskie jaunumi vietā, atjaunināt URL.</span><span class="sxs-lookup"><span data-stu-id="0db9a-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="0db9a-116">Parādīts saraksts ar visu organizatorisko ziņu portālos.</span><span class="sxs-lookup"><span data-stu-id="0db9a-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="0db9a-117">Project Server vietņu, iespējams, tiks pārbaudīti, vai tie ir joprojām saistīts pareizi.</span><span class="sxs-lookup"><span data-stu-id="0db9a-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>




