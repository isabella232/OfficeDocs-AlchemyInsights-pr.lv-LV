---
title: Modernu vietni kā saknes vietni
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713798"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="c8fbd-102">Modern site kā root site</span><span class="sxs-lookup"><span data-stu-id="c8fbd-102">Modern site as root site</span></span>

<span data-ttu-id="c8fbd-103">Mēs esam sākuši izvēršu jaunu funkciju, kas ļaus jums [apmainīt savu klasisko vietnes saknes vietni ar modernu vietni](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="c8fbd-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="c8fbd-104">Izmantojiet [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apmainīt vietu vietā ar citu vietu, kamēr arhivējot sākotnējā vietā.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="c8fbd-105">Pieejams gan grupas vietne (nav savienota ar grupu), gan saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="c8fbd-106">Neizdzēsiet klasisko saknes vietni, lai izveidotu modernu saziņas vietni.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="c8fbd-107">Microsoft to neatbalsta.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="c8fbd-108">Dzēšot saknes vietni, visas SharePoint vietnes jūsu organizācijā nebūs pieejamas visiem lietotājiem, kamēr neatjaunosit vietni vai neizveidojat jaunu vietni ar tādu pašu vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="c8fbd-109">Mēs sazināsim šo funkciju, izmantojot ziņu centru.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="c8fbd-110">Jums vajadzētu sagaidīt līdzeklis ir ieslēgts jūsu nomnieka drīzumā.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="c8fbd-111">Zināmās problēmas, kas saistītas ar vietņu pārnešana</span><span class="sxs-lookup"><span data-stu-id="c8fbd-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="c8fbd-112">Mērķa vietā var atgriezt "nav atrasts" (HTTP 404) kļūda īsā laika periodā.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="c8fbd-113">Saturs būs nepieciešams, lai atjauninātu meklēšanas indeksu.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="c8fbd-114">Šeit nav manuālas darbības, tas tiks izdarīts automātiski.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="c8fbd-115">Kaut kas atkarīgs no "statiskā" saites (piemēram, failu sinhronizācija un OneNote faili) būs nepieciešams manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="c8fbd-116">Project Server vietnes var būt nepieciešams validēt, lai pārliecinātos, ka tie joprojām ir saistīti pareizi.</span><span class="sxs-lookup"><span data-stu-id="c8fbd-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
