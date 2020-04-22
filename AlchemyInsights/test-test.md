---
title: SharePoint Online terminu krātuvē trūkst terminu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766860"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker šifrēšanas ar InTune iespējošana

InTune galapunkta aizsardzības politiku var izmantot, lai konfigurētu Windows ierīču Boitlocker šifrēšanas iestatījumus, kā aprakstīts: Windows10 (un jaunākām versijām) iestatījumus, lai aizsargātu ierīces, izmantojot InTune

Ņemiet vērā, ka daudzas jaunākas ierīces, kurās darbojas operētājsistēma Windows 10, atbalsta automātisku BitLocker šifrēšanu, kas tiek izraisīta, nepiemērojot MDM politiku. Tas var ietekmēt politikas piemērošanu, ja nav noklusējuma iestatījumi ir konfigurēti. Detalizētāku informāciju skatiet sadaļā BUJ.


FAQ  Q: kādi Windows izdevumi atbalsta ierīču šifrēšanu, izmantojot galapunktu aizsardzības politiku?
 A: InTune galapunkta aizsardzības politikas iestatījumi tiek ieviesti, izmantojot BitLocker CSP.Ne visi izdevumi, ne arī veido Windows atbalsta BitLocker CSP. 
      Šajā laikā Windows izdevumi: Enterprise; Education, Mobile, Mobile Enterprise un Professional (no Build 1809 gada) tiek atbalstīti.




Q: ja ierīce jau ir šifrēts ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un šifra stiprums (XTS-AES-128), piemērojot politiku ar atšķirīgiem iestatījumiem, automātiski aktivizēs diska atkārtotu šifrēšanu ar jaunajiem iestatījumiem?

A: Nē. Lai lietotu jaunos šifra iestatījumus, vispirms disks ir atšifrēts.

Piezīme ierīcēm, kas uzņemti ar Autopilot automātiskās šifrēšanas, kas varētu rasties OOBE laikā nav aktivizēta līdz InTune politika tiek novērtēta, kas ļauj politikas iestatījumus izmantot vietā OS noklusējumus




Q Ja ierīce tiek šifrēta, kā rezultātā lietojumprogrammas InTune politika tiks atšifrēti, šī politika tiek noņemta?

A: noņemšana šifrēšanas saistīto politiku nerada atšifrēšana diskus, kas tika konfigurēts.




Q: kāpēc InTune atbilstības politika parāda, ka mana ierīce nav "BitLocker iespējota", bet tas ir?

: "BitLocker iespējots" iestatījums InTune atbilstības politika izmanto Windows Device Health apliecinājums (DHA) klientu. Šis klients tikai mēra ierīces stāvokli sāknēšanas laikā. Tātad, ja ierīce nav rebooted tā kā BitLocker šifrēšana tika pabeigta, DHA klienta pakalpojums neziņos par BitLocker kā aktīvu.