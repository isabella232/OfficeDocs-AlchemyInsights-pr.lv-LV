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
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419879"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="7b554-102">Atvērt, izmantojot Internet Explorer nedarbojas</span><span class="sxs-lookup"><span data-stu-id="7b554-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="7b554-103">**Atvērt, izmantojot Internet Explorer** vai **View File Explorer** nedarbojas pārliecinieties, WebClient pakalpojums ir noteikta, lai **darbojas** , izpildot tālāk norādītos soļus.</span><span class="sxs-lookup"><span data-stu-id="7b554-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="7b554-104">Piemēram, var paiet ilgs laiks, lai atvērtu bibliotēku SharePoint vai OneDrive, kad pakalpojums nedarbojas.</span><span class="sxs-lookup"><span data-stu-id="7b554-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="7b554-105">Windows meklēšanas lodziņā ierakstiet palaist, atlasiet palaist darbvirsmas app, ierakstiet Services. msc un pēc tam atlasiet **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7b554-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="7b554-106">Ritiniet uz leju, lai WebClient pakalpojumu un pārbaudiet **statusa** kolonnā.</span><span class="sxs-lookup"><span data-stu-id="7b554-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="7b554-107">Ja WebClient pakalpojuma statuss nav **palaists**, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **Sākt**un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="7b554-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="7b554-108">Jāiespējo pakalpojums, ja nepieciešams, atlasot **manuālu** vai **automātisku** **startēšanas tips** lodziņā.</span><span class="sxs-lookup"><span data-stu-id="7b554-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="7b554-109">Novērst problēmas, atverot failu Explorer, skatiet [Atvērt programmā Internet Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="7b554-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="7b554-110">Izpētīt ācijas labāka alternatīva: [sinhronizācijas SharePoint faili ar jauno OneDrive sinhronizācijas klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="7b554-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

