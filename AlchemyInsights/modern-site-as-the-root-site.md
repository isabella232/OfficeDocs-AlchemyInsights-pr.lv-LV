---
title: Mūsdienīga vietne kā saknes vietne
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666877"
---
# <a name="modern-site-as-root-site"></a>Mūsdienīga vietne kā saknes vietne

Ir sākta jauna līdzekļa izvēršana, kas ļaus [mainīt klasisko vietnes saknes vietni ar mūsdienīgu vietni](https://docs.microsoft.com/sharepoint/modern-root-site). Izmantojiet [izsauciet-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , lai apmainītu vietnes atrašanās vietu ar citu vietni, kamēr tiek arhivēta sākotnējā vietne. Pieejams gan grupas vietnei (nav savienots ar grupu), gan saziņas vietnē.

>[!Important]
> Nedzēsiet savu klasisko saknes vietni, lai izveidotu mūsdienīgu saziņas vietni. To neatbalsta korporācija Microsoft. Dzēšot saknes vietni, visas SharePoint vietnes jūsu organizācijā kļūst nepieejamas visiem lietotājiem, līdz atjaunojat vietni vai izveidojat jaunu vietni tajā pašā vietrādī URL. Mēs sazināsimies šo līdzekli, izmantojot ziņojumu centru. Drīzumā būs nepieciešams ieslēgt līdzekli savā nomniekā.

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas ar pārnešanas vietnēm
- Lai īsā laika periodā varētu tikt parādīta kļūda "nav atrasta" (HTTP 404).
- Lai atjauninātu meklēšanas indeksu, saturs ir jāpārmeklē. Šeit nav manuālas darbības, tas tiks veikts automātiski.
- Viss, kas ir atkarīgs no nemainīgajām saitēm (piemēram, failu sinhronizācijas un OneNote failiem), būs manuāli jālabo.
- Project Server vietnes, iespējams, ir jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi. 
