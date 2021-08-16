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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000399"
---
# <a name="modern-site-as-root-site"></a>Mūsdienīga vietne kā saknes vietne

Mēs esam sākuši izmantot jaunu līdzekli, ar kuru varat samainīt klasisko vietnes [saknes vietni ar mūsdienīgu vietni.](https://docs.microsoft.com/sharepoint/modern-root-site) Izmantojiet [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) lai vietnes atrašanās vietu samainītu ar citu vietni, vienlaikus arhivējot sākotnējo vietni. Pieejama gan grupas vietnei (nav savienota ar grupu), gan saziņas vietnei.

>[!Important]
> Lai izveidotu mūsdienīgu saziņas vietni, neizdzēsiet klasisko saknes vietni. Microsoft to neatbalsta. Dzēšot saknes vietni, visas SharePoint visas vietnes jūsu organizācijā nevarēs piekļūt visiem lietotājiem, līdz atjaunosit vietni vai izveidosit jaunu vietni ar tādu pašu vietrādi URL. Mēs sazināsimies ar šo līdzekli, izmantojot ziņojumu centru. Drīzumā paredzams, ka šis līdzeklis tiks ieslēgts jūsu nomniekā.

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas ar vietņu samainīšanu
- Mērķa vietne īsu laika periodu var atgriezt kļūdu "nav atrasta" (HTTP 404).
- Lai atjauninātu meklēšanas indeksu, ir jābūt ievilktam saturam. Šeit nav jāveic manuāla darbība, tā tiks veikta automātiski.
- Viss, kas atkarīgs no "statiskām" saitēm (piemēram, failu sinhronizēšana OneNote failiem), būs jāizlabo manuāli.
- Project Iespējams, servera vietnes ir jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi. 
