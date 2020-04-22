---
title: Atvērt ar Explorer nedarbojas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713041"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="712f6-102">Atvērt ar Explorer nedarbojas</span><span class="sxs-lookup"><span data-stu-id="712f6-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="712f6-103">Ja **Atvērt ar Explorer** vai **Skatīt failu pārlūks** nedarbojas pārliecinieties, vai webclient pakalpojums ir iestatīts uz **darbojas** , izpildot tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="712f6-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="712f6-104">Piemēram, var paiet ilgs laiks, lai atvērtu SharePoint vai OneDrive bibliotēku, kad pakalpojums nedarbojas.</span><span class="sxs-lookup"><span data-stu-id="712f6-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="712f6-105">Windows meklēšanas lodziņā ierakstiet palaist, atlasiet palaist datora programmu, ierakstiet Services. msc un pēc tam atlasiet **Enter**.</span><span class="sxs-lookup"><span data-stu-id="712f6-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="712f6-106">Ritiniet uz leju līdz WebClient pakalpojumam un pārbaudiet **statusa** sleju.</span><span class="sxs-lookup"><span data-stu-id="712f6-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="712f6-107">Ja WebClient pakalpojuma statuss nav **palaists**, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **sāktun**pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="712f6-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="712f6-108">Iespējojiet pakalpojumu, ja nepieciešams, lodziņā **startēšanas tips** atlasot **Manuāls** vai **Automātisks** .</span><span class="sxs-lookup"><span data-stu-id="712f6-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="712f6-109">Lai novērstu problēmas, atverot failu pārlūkā, skatiet [Atvērt programmā Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="712f6-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="712f6-110">Izpētiet sinhronizāciju kā labāku alternatīvu: [sinhronizējiet SharePoint failus ar jauno OneDrive sinhronizācijas klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="712f6-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

