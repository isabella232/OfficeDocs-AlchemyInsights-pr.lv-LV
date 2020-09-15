---
title: Problēmu novēršana, izmantojot atvērt ar Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659065"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="bf52b-102">Problēmu novēršana saistībā ar programmu open with Explorer</span><span class="sxs-lookup"><span data-stu-id="bf52b-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="bf52b-103">Bieži sastopamu problēmu novēršana saistībā ar dokumentu bibliotēkas atvēršanu pakalpojumā SharePoint vai OneDrive, izmantojot komandu **Atvērt ar Explorer** :</span><span class="sxs-lookup"><span data-stu-id="bf52b-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="bf52b-104">Izmantojiet Internet Explorer 10 vai Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="bf52b-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="bf52b-105">**Atvērt ar Explorer** nav saderīga ar Microsoft Edge, Google Chrome, Firefox un citiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="bf52b-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="bf52b-106">**Atvērt ar Explorer** ir atspējota visās pārlūkprogrammās, izņemot Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="bf52b-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="bf52b-107">**Atvērt ar Explorer** nav pieejama mūsdienīgai pieredzei SharePoint bibliotēkās.</span><span class="sxs-lookup"><span data-stu-id="bf52b-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="bf52b-108">Tā vietā izmantojiet **skatu failu pārlūkā** .</span><span class="sxs-lookup"><span data-stu-id="bf52b-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="bf52b-109">**View options** \> **Failu pārlūkā**atlasiet skata opciju skats.</span><span class="sxs-lookup"><span data-stu-id="bf52b-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="bf52b-110">Skats failu pārlūkā nav saderīgs ar Microsoft Edge, Google Chrome, Firefox un citiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="bf52b-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="bf52b-111">**Skatīšana failu pārlūkā** ir pieejama tikai pārlūkprogrammā Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="bf52b-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="bf52b-112">Pārliecinieties, vai darbojas klienta pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="bf52b-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="bf52b-113">Windows meklēšanas lodziņā ierakstiet palaist, atlasiet datora programmu palaist, ierakstiet Services. msc un pēc tam nospiediet taustiņu ENTER.</span><span class="sxs-lookup"><span data-stu-id="bf52b-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="bf52b-114">Ritiniet uz leju līdz klienta pakalpojumam un pārliecinieties, vai kolonnā **statuss** tiek rādīts "darbojas".</span><span class="sxs-lookup"><span data-stu-id="bf52b-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="bf52b-115">Ja tā nav, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **Sākt**un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="bf52b-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="bf52b-116">(Iespējams, vispirms ir jāiespējo pakalpojums, lodziņā **startēšanas tips** atlasot **manuāli** vai **automātiski** .)</span><span class="sxs-lookup"><span data-stu-id="bf52b-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="bf52b-117">Bibliotēkas atvēršana failu pārlūkā ir noderīga, ja vēlaties kopēt vai pārvietot vairākus failus un mapes vienreiz, bet, ja vēlaties regulāri strādāt bibliotēkā, iesakām to sinhronizēt.</span><span class="sxs-lookup"><span data-stu-id="bf52b-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="bf52b-118">Lai novērstu problēmas, kas rodas, atverot failu pārlūku, skatiet rakstu [atvēršana pārlūkprogrammā Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="bf52b-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="bf52b-119">Informāciju par sinhronizācijas iestatīšanu skatiet rakstā [SharePoint failu sinhronizēšana ar jauno OneDrive sinhronizācijas klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="bf52b-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="bf52b-120">Lai iegūtu papildinformāciju, skatiet rakstu [kā izmantot komandu atvērt ar Explorer, lai novērstu problēmas pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="bf52b-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

