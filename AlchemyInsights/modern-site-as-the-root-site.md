---
title: Mūsdienu vietni kā saknes vietni
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269383"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="35dca-102">Mūsdienu vietni kā saknes</span><span class="sxs-lookup"><span data-stu-id="35dca-102">Modern site as root site</span></span>

<span data-ttu-id="35dca-103">Mēs esam sākuši izvēršana jauns līdzeklis, kas ļaus apmainīties ar klasisko vietnes saknes vietne, ar mūsdienu vietā.</span><span class="sxs-lookup"><span data-stu-id="35dca-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="35dca-104">Izmantot [Izsaukums SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap atrašanās vietu ar citu vietā vienlaikus arhivē sākotnējā vietā.</span><span class="sxs-lookup"><span data-stu-id="35dca-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="35dca-105">Pieejama gan darba grupas vietni (nav pievienots grupai) un saziņas vietne.</span><span class="sxs-lookup"><span data-stu-id="35dca-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="35dca-106">Klasisks saknes vietne, lai izveidotu mūsdienīgu saziņas vietne nevar dzēst.</span><span class="sxs-lookup"><span data-stu-id="35dca-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="35dca-107">Šī korporācija Microsoft to neatbalsta.</span><span class="sxs-lookup"><span data-stu-id="35dca-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="35dca-108">Saknes vietnes dzēšana padarīs visas SharePoint vietnes organizācijā nepieejama visiem lietotājiem, kamēr vietā atjaunot vai izveidot jaunu vietni ar tādu pašu URL.</span><span class="sxs-lookup"><span data-stu-id="35dca-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="35dca-109">Mums būs sazināties šo iespēju, izmantojot ziņu centru.</span><span class="sxs-lookup"><span data-stu-id="35dca-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="35dca-110">Iespēja ieslēgt savu īrnieka drīzumā vajadzētu sagaidīt.</span><span class="sxs-lookup"><span data-stu-id="35dca-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="35dca-111">Zināmas problēmas ar apmainīšana vietām</span><span class="sxs-lookup"><span data-stu-id="35dca-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="35dca-112">Mērķa vietnes var atgriezt "nav atrasts" kļūda (HTTP 404) uz neilgu laika periodu.</span><span class="sxs-lookup"><span data-stu-id="35dca-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="35dca-113">Saturs būs nepieciešams recrawled atjaunināt meklēšanas indeksā.</span><span class="sxs-lookup"><span data-stu-id="35dca-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="35dca-114">Tur ir bez manuālas darbības, kāda vajadzīga šeit, tas tiks veikts automātiski.</span><span class="sxs-lookup"><span data-stu-id="35dca-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="35dca-115">Viss atkarīgs no "statisku" saites (piemēram, failu sinhronizēšana un OneNote failus) vajadzēs manuāli jālabo.</span><span class="sxs-lookup"><span data-stu-id="35dca-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="35dca-116">Project Server vietņu, iespējams, tiks pārbaudīti, vai tie ir joprojām saistīts pareizi.</span><span class="sxs-lookup"><span data-stu-id="35dca-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
