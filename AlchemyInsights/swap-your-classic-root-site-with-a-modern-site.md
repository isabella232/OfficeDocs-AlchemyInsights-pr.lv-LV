---
title: Swap jūsu klasisko saknes vietne ar modernu vietu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741551"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="dc1ca-102">Swap jūsu klasisko saknes vietne ar modernu vietu</span><span class="sxs-lookup"><span data-stu-id="dc1ca-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="dc1ca-103">Ja vide ir iestatīta pirms 2019. aprīlī, saknes vietni var mainīt uz mūsdienīgu vietni, izmantojot programmu Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="dc1ca-104">Ja jums ir citā vietā, kuru vēlaties izmantot kā savu saknes vietni, jūs varat nomainīt [(mijmaiņas) saknes vietnē](https://docs.microsoft.com/sharepoint/modern-root-site) ar to.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="dc1ca-105">Izmantojiet [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apmainīt vietu vietā ar citu vietu, kamēr arhivējot sākotnējā vietā.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="dc1ca-106">Pieejams gan grupas vietne (nav savienota ar grupu), gan saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="dc1ca-107">Drīzumā tiks ieviestas papildu iespējas, kas ļaus jums turpināt izmantot vietnes saturu, bet pārvērst esošo vietni par saziņas vietni.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="dc1ca-108">Šīs iespējas tiks izveltnē pakāpeniski.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="dc1ca-109">Turpiniet pārbaudīt, vai ziņojumu centrā nav atjauninājumu.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="dc1ca-110">Zināmās problēmas, kas saistītas ar vietņu pārnešana</span><span class="sxs-lookup"><span data-stu-id="dc1ca-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="dc1ca-111">Mērķa vietā var atgriezt "nav atrasts" (HTTP 404) kļūda īsā laika periodā.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="dc1ca-112">Saturs būs nepieciešams, lai atjauninātu meklēšanas indeksu.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="dc1ca-113">Nav manuālo soli nepieciešams-tas tiks izdarīts automātiski.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="dc1ca-114">Kaut kas atkarīgs no "statiskā" saites (piemēram, failu sinhronizācija un OneNote faili) būs nepieciešams manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="dc1ca-115">Ja avota vietne ir organizatoriska ziņu vietne, atjauniniet vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="dc1ca-116">Iegūstiet visu uzņēmuma ziņu vietņu sarakstu.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="dc1ca-117">Project Server vietnes var būt nepieciešams validēt, lai pārliecinātos, ka tie joprojām ir saistīti pareizi.</span><span class="sxs-lookup"><span data-stu-id="dc1ca-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
