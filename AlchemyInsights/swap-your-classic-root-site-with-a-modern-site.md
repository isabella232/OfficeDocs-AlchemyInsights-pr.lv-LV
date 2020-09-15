---
title: Klasiskās saknes vietnes mainīšana ar mūsdienīgu vietni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691186"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasiskās saknes vietnes mainīšana ar mūsdienīgu vietni

Ja jūsu vide ir iestatīta pirms aprīļa 2019, saknes vietni varat mainīt uz mūsdienīgu vietni, izmantojot Microsoft PowerShell.

- Ja jums ir cita vietne, kuru vēlaties izmantot kā saknes vietni, varat to aizstāt [(mainīt) saknes vietni](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Izmantojiet [izsauciet-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , lai apmainītu vietnes atrašanās vietu ar citu vietni, kamēr tiek arhivēta sākotnējā vietne. Pieejams gan grupas vietnei (nav savienots ar grupu), gan saziņas vietnē. 

- Drīzumā tiks ieviests papildu iespējas, kas ļaus turpināt izmantot vietnes saturu, bet esošo vietni pārvērst par saziņas vietni. 
>[!Important]
>Šīs iespējas tiks izritinātas pakāpeniski. Turpiniet, lai pārbaudītu, vai ziņojumu centrā nav atjauninājumu. 

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas ar pārnešanas vietnēm

- Lai īsā laika periodā varētu tikt parādīta kļūda "nav atrasta" (HTTP 404).
- Lai atjauninātu meklēšanas indeksu, saturs ir jāpārmeklē. Nav nepieciešama manuāla darbība — tas tiks veikts automātiski.
- Viss, kas ir atkarīgs no nemainīgajām saitēm (piemēram, failu sinhronizācijas un OneNote failiem), būs manuāli jālabo.
- Ja avota vietne bija organizācijas ziņu vietne, atjauniniet vietrādi URL.Iegūstiet sarakstu ar visām organizācijas ziņu vietnēm.
- Project Server vietnes, iespējams, ir jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi.
