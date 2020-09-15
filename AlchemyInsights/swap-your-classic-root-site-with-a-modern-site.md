---
title: Klasiskās saknes vietnes mainīšana ar mūsdienīgu vietni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691186"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="df12e-102">Klasiskās saknes vietnes mainīšana ar mūsdienīgu vietni</span><span class="sxs-lookup"><span data-stu-id="df12e-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="df12e-103">Ja jūsu vide ir iestatīta pirms aprīļa 2019, saknes vietni varat mainīt uz mūsdienīgu vietni, izmantojot Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="df12e-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="df12e-104">Ja jums ir cita vietne, kuru vēlaties izmantot kā saknes vietni, varat to aizstāt [(mainīt) saknes vietni](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="df12e-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="df12e-105">Izmantojiet [izsauciet-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , lai apmainītu vietnes atrašanās vietu ar citu vietni, kamēr tiek arhivēta sākotnējā vietne.</span><span class="sxs-lookup"><span data-stu-id="df12e-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="df12e-106">Pieejams gan grupas vietnei (nav savienots ar grupu), gan saziņas vietnē.</span><span class="sxs-lookup"><span data-stu-id="df12e-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="df12e-107">Drīzumā tiks ieviests papildu iespējas, kas ļaus turpināt izmantot vietnes saturu, bet esošo vietni pārvērst par saziņas vietni.</span><span class="sxs-lookup"><span data-stu-id="df12e-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="df12e-108">Šīs iespējas tiks izritinātas pakāpeniski.</span><span class="sxs-lookup"><span data-stu-id="df12e-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="df12e-109">Turpiniet, lai pārbaudītu, vai ziņojumu centrā nav atjauninājumu.</span><span class="sxs-lookup"><span data-stu-id="df12e-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="df12e-110">Zināmās problēmas ar pārnešanas vietnēm</span><span class="sxs-lookup"><span data-stu-id="df12e-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="df12e-111">Lai īsā laika periodā varētu tikt parādīta kļūda "nav atrasta" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="df12e-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="df12e-112">Lai atjauninātu meklēšanas indeksu, saturs ir jāpārmeklē.</span><span class="sxs-lookup"><span data-stu-id="df12e-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="df12e-113">Nav nepieciešama manuāla darbība — tas tiks veikts automātiski.</span><span class="sxs-lookup"><span data-stu-id="df12e-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="df12e-114">Viss, kas ir atkarīgs no nemainīgajām saitēm (piemēram, failu sinhronizācijas un OneNote failiem), būs manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="df12e-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="df12e-115">Ja avota vietne bija organizācijas ziņu vietne, atjauniniet vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="df12e-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="df12e-116">Iegūstiet sarakstu ar visām organizācijas ziņu vietnēm.</span><span class="sxs-lookup"><span data-stu-id="df12e-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="df12e-117">Project Server vietnes, iespējams, ir jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi.</span><span class="sxs-lookup"><span data-stu-id="df12e-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
