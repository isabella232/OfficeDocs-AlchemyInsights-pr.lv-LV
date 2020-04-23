---
title: Swap jūsu klasisko saknes vietne ar modernu vietu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741551"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap jūsu klasisko saknes vietne ar modernu vietu

Ja vide ir iestatīta pirms 2019. aprīlī, saknes vietni var mainīt uz mūsdienīgu vietni, izmantojot programmu Microsoft PowerShell.

- Ja jums ir citā vietā, kuru vēlaties izmantot kā savu saknes vietni, jūs varat nomainīt [(mijmaiņas) saknes vietnē](https://docs.microsoft.com/sharepoint/modern-root-site) ar to. 
    - Izmantojiet [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apmainīt vietu vietā ar citu vietu, kamēr arhivējot sākotnējā vietā. Pieejams gan grupas vietne (nav savienota ar grupu), gan saziņas vietne. 

- Drīzumā tiks ieviestas papildu iespējas, kas ļaus jums turpināt izmantot vietnes saturu, bet pārvērst esošo vietni par saziņas vietni. 
>[!Important]
>Šīs iespējas tiks izveltnē pakāpeniski. Turpiniet pārbaudīt, vai ziņojumu centrā nav atjauninājumu. 

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas, kas saistītas ar vietņu pārnešana

- Mērķa vietā var atgriezt "nav atrasts" (HTTP 404) kļūda īsā laika periodā.
- Saturs būs nepieciešams, lai atjauninātu meklēšanas indeksu. Nav manuālo soli nepieciešams-tas tiks izdarīts automātiski.
- Kaut kas atkarīgs no "statiskā" saites (piemēram, failu sinhronizācija un OneNote faili) būs nepieciešams manuāli jālabo.
- Ja avota vietne ir organizatoriska ziņu vietne, atjauniniet vietrādi URL.Iegūstiet visu uzņēmuma ziņu vietņu sarakstu.
- Project Server vietnes var būt nepieciešams validēt, lai pārliecinātos, ka tie joprojām ir saistīti pareizi.
