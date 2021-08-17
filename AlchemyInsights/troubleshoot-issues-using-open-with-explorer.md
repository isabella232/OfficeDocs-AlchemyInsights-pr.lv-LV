---
title: Ar "Atvērt ar Explorer" saistīto problēmu novēršana
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048163"
---
# <a name="fix-problems-with-open-with-explorer"></a>Ar "Atvērt ar Explorer" problēmu novēršana

Novērsiet bieži sastopamas problēmas ar dokumentu bibliotēkas atvēršanu SharePoint vai OneDrive **izmantojot komandu Atvērt ar Explorer:** 
  
- Izmantojiet Internet Explorer 10 vai Internet Explorer 11. **Opcija Atvērt ar Explorer** nav saderīga ar Microsoft Edge, Google Chrome, Firefox un citām pārlūkprogrammām. **Atvēršana ar Explorer** ir atspējota visās pārlūkprogrammās, izņemot Internet Explorer. 
    
- **Atvēršana ar Explorer** mūsdienīgajās versijās nav pieejama SharePoint bibliotēkām. Tā **vietā izmantojiet skatu failu pārlūkā.** Atlasiet **Skatīt opcijas** Skatīt failu \> **pārlūkā**. Skatīšana failu pārlūkā nav saderīga ar Microsoft Edge, Google Chrome, Firefox un citām pārlūkprogrammām. **Skatīt failu pārlūkā,** kas ir pieejams tikai pārlūkprogrammā Internet Explorer. 
    
- Pārliecinieties, vai darbojas pakalpojums WebClient. Meklēšanas Windows ierakstiet palaist, atlasiet palaist datora lietojumprogrammu, ierakstiet services.msc un pēc tam nospiediet taustiņu Enter. Ritiniet uz leju līdz pakalpojumam WebClient un pārliecinieties, vai kolonnā **Statuss** tiek rādīts "Darbojas". Ja tā nenotiek, veiciet dubultklikšķi uz pakalpojuma, noklikšķiniet uz **Sākt** un pēc tam noklikšķiniet uz **Labi**. (Iespējams, pakalpojums vispirms būs jāiespējo, lodziņā **Startēšanas** **tips** atlasot Manuāli **vai** Automātiski.) 
    
> [!NOTE]
> Bibliotēkas atvēršana failu pārlūkā ir lieliska, ja vēlaties kopēt vai pārvietot vairākus failus un mapes vienreiz, bet, ja vēlaties regulāri strādāt bibliotēkā, iesakām to sinhronizēt. Lai novērstu problēmas saistībā ar atvēršanu failu pārlūkā, skatiet [rakstu Atvēršana pārlūkā.](https://go.microsoft.com/fwlink/?linkid=871665) Informāciju par sinhronizācijas iestatīšanu skatiet rakstā [Sinhronizācijas SharePoint ar jauno OneDrive sinhronizācija klientu.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Papildinformāciju [skatiet rakstā Komandas Atvērt](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) ar Explorer izmantošana, lai novērstu problēmas programmā SharePoint Online. 
  

