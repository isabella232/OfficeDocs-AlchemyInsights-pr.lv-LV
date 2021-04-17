---
title: Microsoft Edge izmantošana, pamatojoties uz Chromium pārlūkprogrammām Ediscovery eksportēšanai
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834378"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="a1057-102">Microsoft Edge izmantošana, pamatojoties uz Chromium pārlūkprogrammām Ediscovery eksportēšanai</span><span class="sxs-lookup"><span data-stu-id="a1057-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="a1057-103">Neseno izmaiņu dēļ Microsoft Edge pārlūkprogrammās vairs nebūs iespējots ClickOnce atbalsts pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="a1057-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="a1057-104">Lai turpinātu izmantot Microsoft 365 e-datu atklāšanas eksportēšanas rīku, ir jāizmanto Microsoft Internet Explorer vai jāiespējo ClickOnce atbalsts pārlūkprogrammā Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a1057-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="a1057-105">Lai iespējotu ClickOnce atbalstu microsoft Edge, pamatojoties uz Chromium:</span><span class="sxs-lookup"><span data-stu-id="a1057-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="a1057-106">Pārlūkprogrammā Microsoft Edge apmeklējiet vietni edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="a1057-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="a1057-107">Opcijai ClickOnce atbalsts mainiet vērtību no Noklusējums **vai Atspējots** uz  **Iespējots.**</span><span class="sxs-lookup"><span data-stu-id="a1057-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="a1057-108">Pārlūkprogrammas loga lejasdaļā atlasiet **Restartēt**.</span><span class="sxs-lookup"><span data-stu-id="a1057-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="a1057-109">Izmaiņas stāsies spēkā pēc Microsoft Edge restartēšanas.</span><span class="sxs-lookup"><span data-stu-id="a1057-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="a1057-110">Informāciju par šo informāciju un eksportēšanas rīka instalēšanas darbībām skatiet rakstā: [Satura meklēšanas rezultātu eksportēšana.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="a1057-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>