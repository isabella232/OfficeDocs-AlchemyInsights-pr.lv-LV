---
title: Atvērt, izmantojot Internet Explorer nedarbojas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906811"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c607d-102">Atvērt, izmantojot Internet Explorer nedarbojas</span><span class="sxs-lookup"><span data-stu-id="c607d-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c607d-p101">**Atvērt, izmantojot Internet Explorer** vai **View File Explorer** nedarbojas pārliecinieties, WebClient pakalpojums ir noteikta, lai **darbojas** , izpildot tālāk norādītos soļus. Piemēram, var paiet ilgs laiks, lai atvērtu bibliotēku SharePoint vai OneDrive, kad pakalpojums nedarbojas.</span><span class="sxs-lookup"><span data-stu-id="c607d-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c607d-105">Windows meklēšanas lodziņā ierakstiet palaist, atlasiet palaist darbvirsmas app, ierakstiet Services. msc un pēc tam atlasiet **Enter**.</span><span class="sxs-lookup"><span data-stu-id="c607d-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c607d-p102">Ritiniet uz leju, lai WebClient pakalpojumu un pārbaudiet **statusa** kolonnā. Ja WebClient pakalpojuma statuss nav **palaists**, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **Sākt**un pēc tam noklikšķiniet uz **Labi**. Jāiespējo pakalpojums, ja nepieciešams, atlasot **manuālu** vai **automātisku** **startēšanas tips** lodziņā.</span><span class="sxs-lookup"><span data-stu-id="c607d-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c607d-p103">Novērst problēmas, atverot failu Explorer, skatiet [Atvērt programmā Internet Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Izpētīt ācijas labāka alternatīva: [sinhronizācijas SharePoint faili ar jauno OneDrive sinhronizācijas klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c607d-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

