---
title: Ierobežotas piekļuves pārraudzība
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702910"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ierobežotas piekļuves Exchange pārraudzība

Lietotāji, kuru mērķis ir ierobežotas piekļuves tiesības, saņem paziņojumu e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām. Lai atrisinātu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:
  
- Ja ierīce ir uzskatāma par piereģistrētu, informējiet lietotāju, ka esat pieteicies uzņēmuma portāla programmā, un pārbaudiet, vai tā ir redzama uzņēmuma portālā. Ja tā nav, lietotājam ir jāreģistrē ierīce.
    
- Azure portālā dodieties uz **Intune \> ierīces atbilstība**. Sadaļā **monitora** noklikšķiniet uz **ierīces atbilstība**. Skatīt ierīces atbilstības atskaiti, lai pārliecinātos, vai lietotāja ierīce ir atzīmēta kā atbilstoša. 
    
- Azure portālā dodieties uz **Intune \> ierīces atbilstība**. Sadaļā **pārvaldība**noklikšķiniet uz **politikas**. Atbilstības politiku sarakstā pārbaudiet, vai profils ir piešķirts jūsu lietotāja ierīcei. Ja nav piešķirts neviens profils, Intune nevarēs apstiprināt ierīces atbilstības statusu. 
    
- Rediģējiet lietotāja nosacījuma piekļuves uzdevumu.
    
1. Azure portālā dodieties uz **Intune \> ierobežotas piekļuves \> politikas**
    
2. Atlasiet politiku no saraksta
    
3. Noklikšķiniet uz **lietotāji un grupas**
    
4. Lai noteiktu konkrētu politiku, pievienojiet to sarakstam **iekļaut** . Lai nodrošinātu to, ka politika nav izlaista, pievienojiet tās sarakstam **neiekļaut** . 
    
Lasiet vēl: [kā pārraudzīt ierobežotas piekļuves ierīces](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

