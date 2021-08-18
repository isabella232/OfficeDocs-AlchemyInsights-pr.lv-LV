---
title: Klasiskās saknes vietnes maiņa ar modernu vietni
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
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316147"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasiskās saknes vietnes maiņa ar modernu vietni

Ja vide tika iestatīta pirms 2019. gada aprīļa, varat nomainīt savu saknes vietni uz mūsdienīgu vietni, izmantojot Microsoft PowerShell:

- Ja jums ir cita vietne, kuru vēlaties izmantot kā savu saknes vietni, varat to aizstāt [(samainīt)](https://docs.microsoft.com/sharepoint/modern-root-site) ar to. 
    - Izmantojiet [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) lai vietnes atrašanās vietu samainītu ar citu vietni, vienlaikus arhivējot sākotnējo vietni. Pieejama gan grupas vietnei (nav savienota ar grupu), gan saziņas vietnei. 

- Drīzumā tiks ieviestas papildu iespējas, kas ļauj turpināt lietot vietnes saturu, bet esošo vietni konvertēt par saziņas vietni. 

**Svarīgi!** Šīs iespējas tiks ieviestas pakāpeniski. Turpiniet pārbaudīt, vai ziņojumu centrā nav atjauninājumu. 

## <a name="known-issues-with-swapping-sites"></a>Zināmās problēmas ar vietņu samainīšanu

- Mērķa vietne īsu laika periodu var atgriezt kļūdu "nav atrasta" (HTTP 404).
- Lai atjauninātu meklēšanas indeksu, ir jābūt ievilktam saturam. Nav jāveic manuāla darbība — tas tiks paveikts automātiski.
- Viss, kas atkarīgs no "statiskām" saitēm (piemēram, failu sinhronizēšana OneNote failiem), būs jāizlabo manuāli.
- Ja avota vietne ir organizācijas ziņu vietne, atjauniniet vietrādi URL. Iegūstiet sarakstu ar visām organizācijas ziņu vietnēm.
- Project Servera vietnes var būt jāvalidē, lai pārliecinātos, vai tās joprojām ir saistītas pareizi.
