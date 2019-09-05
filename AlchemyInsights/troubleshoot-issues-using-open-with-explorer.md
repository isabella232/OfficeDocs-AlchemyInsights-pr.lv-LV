---
title: Novērst problēmas, izmantojot atvērt ar Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742740"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="35a6c-102">Problēmu novēršana saistībā ar atvērt ar Explorer</span><span class="sxs-lookup"><span data-stu-id="35a6c-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="35a6c-103">Kā novērst vispārējas problēmas, atverot dokumentu bibliotēku pakalpojumā SharePoint vai OneDrive, izmantojot komandu **Atvērt ar Explorer** :</span><span class="sxs-lookup"><span data-stu-id="35a6c-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="35a6c-104">Izmantojiet Internet Explorer 10 vai Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="35a6c-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="35a6c-105">**Atvērt ar Explorer** nav saderīgs ar Microsoft EDGE, Google Chrome, Firefox un citi.</span><span class="sxs-lookup"><span data-stu-id="35a6c-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="35a6c-106">**Atvērt ar Explorer** ir atspējota visās pārlūkprogrammās, izņemot Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="35a6c-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="35a6c-107">**Atvērt ar Explorer** nav pieejama mūsdienu pieredze SharePoint bibliotēkās.</span><span class="sxs-lookup"><span data-stu-id="35a6c-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="35a6c-108">Tā vietā izmantojiet **skatu failu pārlūkā** .</span><span class="sxs-lookup"><span data-stu-id="35a6c-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="35a6c-109">Atlasiet **Skatīt opcijas** \> **Skatīt failu pārlūkā**.</span><span class="sxs-lookup"><span data-stu-id="35a6c-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="35a6c-110">Skatīt File Explorer nav saderīgs ar Microsoft EDGE, Google Chrome, Firefox un citi.</span><span class="sxs-lookup"><span data-stu-id="35a6c-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="35a6c-111">**Skatīt failu pārlūkā** , kas pieejams tikai programmā Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="35a6c-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="35a6c-112">Pārliecinieties, vai WebClient pakalpojums darbojas.</span><span class="sxs-lookup"><span data-stu-id="35a6c-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="35a6c-113">Windows meklēšanas lodziņā ierakstiet palaist, atlasiet palaist datora programmu, ierakstiet Services. msc un pēc tam nospiediet taustiņu ENTER.</span><span class="sxs-lookup"><span data-stu-id="35a6c-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="35a6c-114">Ritiniet uz leju līdz WebClient pakalpojumam un pārliecinieties, vai **statusa** slejā tiek rādīts "Running".</span><span class="sxs-lookup"><span data-stu-id="35a6c-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="35a6c-115">Ja tā nenotiek, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **Sāktun**pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="35a6c-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="35a6c-116">(Iespējams, vispirms būs jāiespējo pakalpojums, lodziņā **startēšanas tips** atlasot **Manuāls** vai **Automātisks** .)</span><span class="sxs-lookup"><span data-stu-id="35a6c-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="35a6c-117">Bibliotēkas atvēršana failu pārlūkā ir noderīga, ja vienu reizi nepieciešams kopēt vai pārvietot vairākus failus un mapes, bet, ja vēlaties regulāri strādāt bibliotēkā, ieteicams to sinhronizēt.</span><span class="sxs-lookup"><span data-stu-id="35a6c-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="35a6c-118">Lai novērstu problēmas, atverot failu pārlūkā, skatiet [Atvērt programmā Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="35a6c-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="35a6c-119">Informāciju par sinhronizēšanas iestatīšanu skatiet sadaļā [SharePoint failu sinhronizēšana ar jauno OneDrive sinhronizācijas klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="35a6c-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="35a6c-120">Lūdzu, skatiet rakstā [kā izmantot komandu "atvērt ar Explorer" novērst problēmas saistībā ar SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="35a6c-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

