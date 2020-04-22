---
title: Ierobežotas piekļuves pārraudzība
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713725"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ierobežotas pieejamības pārraudzība Exchange

Lietotāji, kuriem ir ierobežotas piekļuves tiesības, saņems e-pasta paziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām. Lai atrisinātu problēmu, iesakām izmantot vienu vai vairākus no šiem risinājumiem:
  
- Ja tiek uzskatīts, ka ierīce ir reģistrēta, ieteikt lietotājam doties uz uzņēmuma portāla lietojumprogrammu un pārliecināties, ka tā parādās uzņēmuma portālā. Ja tā nav, lietotājam vajadzētu uzņemt ierīci.
    
- Azure portālā atveriet ** \> InTune ierīces atbilstību**. Sadaļā **monitors** noklikšķiniet uz **ierīces atbilstība**. Skatiet ierīces atbilstības pārskatu, lai pārbaudītu, vai lietotāja ierīce ir atzīmēta kā atbilstoša. 
    
- Azure portālā atveriet ** \> InTune ierīces atbilstību**. Zem **pārvaldīt**noklikšķiniet uz **politikas**. Atbilstības politiku sarakstā pārbaudiet, vai lietotāja ierīcei ir piešķirts profils. Ja profils nav piešķirts, InTune nevarēs apstiprināt ierīces atbilstības statusu. 
    
- Rediģējiet lietotāja ierobežotas piekļuves piešķiri.
    
1. Azure portālā atveriet **InTune \> ierobežotas piekļuves \> politikas**
    
2. Atlasiet politiku no saraksta
    
3. Noklikšķiniet uz **lietotāji un grupas**
    
4. Lai adresēt noteiktu politiku kādam, pievienojiet tos sarakstam **iekļaut** . Lai nodrošinātu, ka no politikas tiek izlaista kāda persona, pievienojiet tās **izņēmumu** sarakstam. 
    
Lasīt tālāk: [kā pārraudzīt ierobežotas piekļuves ierīces](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

