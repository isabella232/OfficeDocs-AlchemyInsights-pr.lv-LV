---
title: Modernā vietne kā saknes vietne
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327609"
---
# <a name="modern-site-as-root-site"></a>Mūsdienīga vietne kā saknes vietne

Mēs sākām izvēršam jaunu līdzekli, ar kuru varat samainīt klasisko vietnes [saknes vietni ar mūsdienīgu vietni.](https://docs.microsoft.com/sharepoint/modern-root-site) Izmantojiet [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) lai vietnes atrašanās vietu samainītu ar citu vietni, vienlaikus arhivējot sākotnējo vietni. Pieejama gan grupas vietnei (nav savienota ar grupu), gan saziņas vietnei.

**Svarīgi!** Lai izveidotu mūsdienīgu saziņas vietni, neizdzēsiet klasisko saknes vietni. Microsoft to neatbalsta. Dzēšot saknes vietni, SharePoint visas organizācijas vietnes nepieejamas visiem lietotājiem, līdz atjaunosit vietni vai izveidosit jaunu vietni ar vienu un to pašu vietrādi URL. Mēs sazināsimies ar šo līdzekli, izmantojot ziņojumu centru. Drīzumā paredzams, ka šis līdzeklis tiks ieslēgts jūsu nomniekā.

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas ar vietņu samainīšanu
- Mērķa vietne īsu laika periodu var atgriezt kļūdu "nav atrasta" (HTTP 404).
- Lai atjauninātu meklēšanas indeksu, ir jābūt ievilktam saturam. Šeit nav jāveic manuāla darbība, tā tiks veikta automātiski.
- Viss, kas atkarīgs no "statiskām" saitēm (piemēram, failu sinhronizēšana OneNote failiem), būs jāizlabo manuāli.
- Project Servera vietnes var būt jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi. 
