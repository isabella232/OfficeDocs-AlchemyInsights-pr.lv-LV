---
title: Swap jūsu klasisko saknes vietne ar modernu vietu
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749267"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap jūsu klasisko saknes vietne ar modernu vietu

Ja vide ir iestatīta pirms 2019. aprīlī, saknes vietni var mainīt uz mūsdienīgu vietni, izmantojot programmu Microsoft PowerShell.

- Ja jums ir citā vietā, kuru vēlaties izmantot kā savu saknes vietni, jūs varat nomainīt [(mijmaiņas) saknes vietnē](https://docs.microsoft.com/sharepoint/modern-root-site) ar to. 
    - Izmantojiet [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apmainīt vietu vietā ar citu vietu, kamēr arhivējot sākotnējā vietā. Pieejams gan grupas vietne (nav savienota ar grupu), gan saziņas vietne. 

- Drīzumā tiks ieviestas papildu iespējas, kas ļaus jums turpināt izmantot vietnes saturu, bet pārvērst esošo vietni par saziņas vietni. 
>[!Important]
>Šīs iespējas tiks izveltnē pakāpeniski. Turpiniet pārbaudīt Office 365 ziņojumu centrs atjauninājumus. 

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas, kas saistītas ar vietņu pārnešana

- Mērķa vietā var atgriezt "nav atrasts" (HTTP 404) kļūda īsā laika periodā.
- Saturs būs nepieciešams, lai atjauninātu meklēšanas indeksu. Nav manuālo soli nepieciešams-tas tiks izdarīts automātiski.
- Kaut kas atkarīgs no "statiskā" saites (piemēram, failu sinhronizācija un OneNote faili) būs nepieciešams manuāli jālabo.
- Ja avota vietne ir organizatoriska ziņu vietne, atjauniniet vietrādi URL.Iegūstiet visu uzņēmuma ziņu vietņu sarakstu.
- Project Server vietnes var būt nepieciešams validēt, lai pārliecinātos, ka tie joprojām ir saistīti pareizi.





