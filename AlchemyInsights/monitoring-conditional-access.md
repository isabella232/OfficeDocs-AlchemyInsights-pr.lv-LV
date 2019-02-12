---
title: Ierobežotas piekļuves kontroli
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902360"
---
# <a name="monitoring-conditional-access"></a>Ierobežotas piekļuves kontroli

Lietotāju mērķauditorija ar ierobežotas piekļuves saņems paziņojumu e-pastu, ja tās neatbilst jūsu uzņēmuma piekļuves prasības. Lai atrisinātu, mēs iesakām vienu vai vairākus no šiem risinājumiem:
  
- Ja tiek uzskatīts, ka ierīce tiks uzņemti, konsultēt lietotāja Web vietas uzņēmuma portāls app iet un pārbaudiet, vai tas parādās uzņēmuma portālā. Ja tā nav, lietotājam vajadzētu uzņemt ierīci.
    
- Debeszils portālā iet uz **Intune \> ierīces atbilstību**. Zem **monitora** noklikšķiniet uz **ierīces atbilstību**. Skatīt ierīces atbilstības ziņojumu, pārliecināties, ka lietotāja ierīces ir atzīmēta kā atbilstošu. 
    
- Debeszils portālā iet uz **Intune \> ierīces atbilstību**. Zem **Pārvaldīt**noklikšķiniet uz **politiku**. Atbilstības politikas sarakstā pārliecinieties, ka profils ir piešķirts jūsu lietotāja ierīces. Ja ir piešķirts neviens profils, tad Intune nevarēs apstiprināt ierīces atbilstības statusu. 
    
- Rediģēt lietotāja nosacījuma piekļuves piešķiršana.
    
1. Debeszils portālā iet uz **Intune \> ierobežotas piekļuves \> politikas**
    
2. Sarakstā atlasiet politiku
    
3. Noklikšķiniet uz **lietotāji un grupas**
    
4. Lai virzītu politiku, ir kāds, pievienot tos sarakstā **iekļaut** . Lai nodrošinātu, ka persona ir izlaists no politikas, pievienot tos sarakstā **neiekļaut** . 
    
Lasīt tālāk: [kā monitors ierobežotas piekļuves iekārtu](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

