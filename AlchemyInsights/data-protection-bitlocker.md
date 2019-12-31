---
title: DataProtection — BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908716"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker šifrēšanas ar InTune iespējošana

 InTune galapunkta aizsardzības politiku var izmantot, lai konfigurētu BitLocker šifrēšanas iestatījumus Windows ierīcēm. Lai iegūtu papildinformāciju, skatiet [Windows 10 (un jaunākām versijām) iestatījumus, lai aizsargātu ierīces, izmantojot InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Ņemiet vērā, ka daudzas jaunākas ierīces, kurās darbojas operētājsistēma Windows 10, atbalsta automātisku BitLocker šifrēšanu, kas tiek izraisīta bez MDM politikas lietojumprogrammas. Tas var ietekmēt politikas piemērošanu, ja nav noklusējuma iestatījumi ir konfigurēti. Detalizētu informāciju skatiet tālāk sadaļā BUJ.
 
Informāciju par BitLocker problēmu novēršanu skatiet [problēmu novēršana saistībā ar BitLocker politikām Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Faq**

 Q: kādi izdevumi Windows atbalsta ierīču šifrēšana, izmantojot galapunktu aizsardzības politiku?<br>
 A: InTune galapunkta aizsardzības politikas iestatījumi tiek ieviesti, izmantojot [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne visi izdevumi vai būvējumi Windows atbalsta BitLocker CSP. <br><br>
      Šajā laikā tiek atbalstīti šādi Windows izdevumi: Enterprise, Education, Mobile, Mobile Enterprise un Professional (būvējums 1809 un jaunākas versijas).
 
Q: ja ierīce jau ir šifrēts ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodi un šifra stiprums (XTS-AES-128), piemērojot politiku ar dažādiem iestatījumiem automātiski izraisīt atkārtotu šifrēšanu disku ar jaunajiem iestatījumiem?<br>
A: Nē. Lai lietotu jaunos šifra iestatījumus, vispirms disks ir atšifrēts.<br><br>
**Piezīme:** Ierīces tiek uzņemti ar Autopilot, automātiskā šifrēšana, kas varētu rasties OOBE laikā nav aktivizēta līdz InTune politika tiek novērtēta, kas ļauj izmantot politikas iestatījumus vietā OS noklusējumus.
 
Q: ja ierīce tiek šifrēta, kā lietojumprogrammas InTune politikas dēļ, tas tiks atšifrēts, tiek noņemta politika?<br>
A: noņemšana šifrēšanas saistīto politiku nerada atšifrēšana diskus, kas tika konfigurēts.
 
Q: kāpēc InTune atbilstības politika parāda, ka mana ierīce nav iespējots BitLocker, pat ja tas ir?<br>
: "BitLocker iespējots" iestatījums InTune atbilstības politika izmanto Windows Device Health apliecinājums (DHA) klientu. Šis klients tikai mēra ierīces stāvokli sāknēšanas laikā. Tāpēc, ja ierīce nav rebooted tā kā BitLocker šifrēšana ir pabeigta, DHA klienta pakalpojums neziņos BitLocker par aktīvu.
 
 