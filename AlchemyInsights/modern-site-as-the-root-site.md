---
title: Mūsdienīga vietne kā saknes vietne
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666877"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="9b8d3-102">Mūsdienīga vietne kā saknes vietne</span><span class="sxs-lookup"><span data-stu-id="9b8d3-102">Modern site as root site</span></span>

<span data-ttu-id="9b8d3-103">Ir sākta jauna līdzekļa izvēršana, kas ļaus [mainīt klasisko vietnes saknes vietni ar mūsdienīgu vietni](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="9b8d3-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="9b8d3-104">Izmantojiet [izsauciet-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , lai apmainītu vietnes atrašanās vietu ar citu vietni, kamēr tiek arhivēta sākotnējā vietne.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9b8d3-105">Pieejams gan grupas vietnei (nav savienots ar grupu), gan saziņas vietnē.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="9b8d3-106">Nedzēsiet savu klasisko saknes vietni, lai izveidotu mūsdienīgu saziņas vietni.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="9b8d3-107">To neatbalsta korporācija Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="9b8d3-108">Dzēšot saknes vietni, visas SharePoint vietnes jūsu organizācijā kļūst nepieejamas visiem lietotājiem, līdz atjaunojat vietni vai izveidojat jaunu vietni tajā pašā vietrādī URL.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="9b8d3-109">Mēs sazināsimies šo līdzekli, izmantojot ziņojumu centru.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="9b8d3-110">Drīzumā būs nepieciešams ieslēgt līdzekli savā nomniekā.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9b8d3-111">Zināmās problēmas ar pārnešanas vietnēm</span><span class="sxs-lookup"><span data-stu-id="9b8d3-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="9b8d3-112">Lai īsā laika periodā varētu tikt parādīta kļūda "nav atrasta" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="9b8d3-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9b8d3-113">Lai atjauninātu meklēšanas indeksu, saturs ir jāpārmeklē.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9b8d3-114">Šeit nav manuālas darbības, tas tiks veikts automātiski.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="9b8d3-115">Viss, kas ir atkarīgs no nemainīgajām saitēm (piemēram, failu sinhronizācijas un OneNote failiem), būs manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9b8d3-116">Project Server vietnes, iespējams, ir jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi.</span><span class="sxs-lookup"><span data-stu-id="9b8d3-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
