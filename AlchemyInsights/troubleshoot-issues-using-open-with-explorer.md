---
title: Novērst problēmas, kas saistītas ar Internet Explorer, izmantojot Open
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390614"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="cae0b-102">Novērst problēmas ar atvērtu ar Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="cae0b-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="cae0b-103">Novērst bieži sastopamas problēmas atverot dokumentu bibliotēkā SharePoint vai OneDrive, izmantojot komandu **Atvērt, izmantojot Internet Explorer** :</span><span class="sxs-lookup"><span data-stu-id="cae0b-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="cae0b-104">Izmantojiet Internet Explorer 10 vai Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="cae0b-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="cae0b-105">**Atvērt ar Internet Explorer** nav saderīgs ar Microsoft Edge, Google Chrome, Firefox un citi.</span><span class="sxs-lookup"><span data-stu-id="cae0b-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="cae0b-106">**Atvērt ar Explorer** ir atspējota visās pārlūkprogrammās, izņemot Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="cae0b-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="cae0b-107">**Atvērt ar Internet Explorer** nav pieejams SharePoint bibliotēkas mūsdienu pieredzi.</span><span class="sxs-lookup"><span data-stu-id="cae0b-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="cae0b-108">Izmantojiet **failu Explorer skats** .</span><span class="sxs-lookup"><span data-stu-id="cae0b-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="cae0b-109">Izvēlieties **skata opcijas** \> **failu Explorer skats**.</span><span class="sxs-lookup"><span data-stu-id="cae0b-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="cae0b-110">Failu Explorer skats nav saderīgs ar Microsoft Edge, Google Chrome, Firefox un citi.</span><span class="sxs-lookup"><span data-stu-id="cae0b-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="cae0b-111">**Failu Explorer skats** ir pieejams tikai programmā Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="cae0b-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="cae0b-112">Pārliecinieties, vai WebClient pakalpojumu darbojas.</span><span class="sxs-lookup"><span data-stu-id="cae0b-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="cae0b-113">Windows meklēšanas lodziņā ierakstiet palaist, izvēlieties palaist darbvirsmas app, ierakstiet Services. msc un pēc tam nospiediet taustiņu Enter.</span><span class="sxs-lookup"><span data-stu-id="cae0b-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="cae0b-114">Ritiniet uz leju, lai WebClient pakalpojumu un pārliecinieties, vai kolonnā **statuss** tiek parādīts, "Gaitas".</span><span class="sxs-lookup"><span data-stu-id="cae0b-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="cae0b-115">Ja tā nav, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **Sākt**un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="cae0b-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="cae0b-116">(Iespējams, ka vispirms ir jāiespējo pakalpojuma **startēšanas tips** lodziņā, atlasot **manuālo** vai **automātisko** .)</span><span class="sxs-lookup"><span data-stu-id="cae0b-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="cae0b-117">Atvērt bibliotēkas failu pārlūks ir ērts, ja jums ir nepieciešams, lai kopētu vai pārvietotu vairākus failus un mapes pēc, bet, ja jūs vēlaties regulāri strādāt bibliotēkā, mēs iesakām to sinhronizāciju.</span><span class="sxs-lookup"><span data-stu-id="cae0b-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="cae0b-118">Novērst problēmas, atverot failu Explorer, skatiet [Atvērt programmā Internet Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="cae0b-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="cae0b-119">Info par sinhronizēšanas iestatīšanu, skatiet [sinhronizācijas SharePoint faili ar jauno OneDrive sinhronizācijas klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="cae0b-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="cae0b-120">Lūdzu, skatiet rakstu [kā izmantot "Open ar Explorer" komandu, lai problēmu novēršana programmā SharePoint tiešsaistē](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="cae0b-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

