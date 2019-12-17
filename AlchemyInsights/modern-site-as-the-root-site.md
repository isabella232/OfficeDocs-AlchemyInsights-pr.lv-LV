---
title: Modernu vietni kā saknes vietni
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054709"
---
# <a name="modern-site-as-root-site"></a>Modern site kā root site

Mēs esam sākuši izvēršu jaunu funkciju, kas ļaus jums [apmainīt savu klasisko vietnes saknes vietni ar modernu vietni](https://docs.microsoft.com/sharepoint/modern-root-site). Izmantojiet [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apmainīt vietu vietā ar citu vietu, kamēr arhivējot sākotnējā vietā. Pieejams gan grupas vietne (nav savienota ar grupu), gan saziņas vietne.

>[!Important]
> Neizdzēsiet klasisko saknes vietni, lai izveidotu modernu saziņas vietni. Microsoft to neatbalsta. Dzēšot saknes vietni, visas SharePoint vietnes jūsu organizācijā nebūs pieejamas visiem lietotājiem, kamēr neatjaunosit vietni vai neizveidojat jaunu vietni ar tādu pašu vietrādi URL. Mēs sazināsim šo funkciju, izmantojot ziņu centru. Jums vajadzētu sagaidīt līdzeklis ir ieslēgts jūsu nomnieka drīzumā.

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas, kas saistītas ar vietņu pārnešana
- Mērķa vietā var atgriezt "nav atrasts" (HTTP 404) kļūda īsā laika periodā.
- Saturs būs nepieciešams, lai atjauninātu meklēšanas indeksu. Šeit nav manuālas darbības, tas tiks izdarīts automātiski.
- Kaut kas atkarīgs no "statiskā" saites (piemēram, failu sinhronizācija un OneNote faili) būs nepieciešams manuāli jālabo.
- Project Server vietnes var būt nepieciešams validēt, lai pārliecinātos, ka tie joprojām ir saistīti pareizi. 
