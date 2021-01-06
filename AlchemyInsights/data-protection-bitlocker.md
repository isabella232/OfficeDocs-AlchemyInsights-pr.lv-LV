---
title: Aspektus-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768824"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker šifrēšanas iespējošana ar Intune

 Intune galapunkta aizsardzības politika var tikt izmantota, lai konfigurētu BitLocker šifrēšanas iestatījumus Windows ierīcēm. Papildinformāciju skatiet rakstā [Windows 10 (un jaunākas versijas) iestatījumi, lai aizsargātu ierīces, kas izmanto Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Ņemiet vērā, ka daudzās jaunākās ierīcēs, kurās darbojas operētājsistēma Windows 10, tiek atbalstīta automātiskā BitLocker šifrēšana, kas tiek palaista, nelietojot MDM politiku. Tas var ietekmēt politikas lietojumu, ja tiek konfigurēti noklusējuma iestatījumi. Papildinformāciju skatiet tālāk norādītajos bieži uzdotajos jautājumos.
 
Informāciju par BitLocker problēmu novēršanu skatiet rakstā [BitLocker politikas problēmu novēršana pakalpojumā Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**BUJ**

J: kādi Windows izdevumi atbalsta ierīces šifrēšanu, izmantojot galapunktu aizsardzības politiku?<br>
A: Intune Endpoint Protection politikas iestatījumi tiek ieviesti, izmantojot [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne visi Windows izdevumi un būvējumi neatbalsta BitLocker CSP. <br><br>

J: kā ierīcēs var iespējot BitLocker, nepieprasot lietotāja mijiedarbību?<br>
A: kamēr ir izpildīti nepieciešamie priekšnosacījumi, ir iespējams iespējot BitLocker "kluso šifrēšanu", izmantojot Intune. Skatiet detalizētu informāciju par ierīces prasībām un piemēra politikas iestatījumiem, lai iespējotu kluso šifrēšanu tālāk esošajā dokumentā [.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

J: ja ierīce jau ir šifrēta ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un Cipher Strength (XTS-AES-128), vai tiek lietota politika ar atšķirīgiem iestatījumiem, kas automātiski aktivizē šī diska atkārtotu šifrēšanu ar jaunajiem iestatījumiem?<br>
A: Nē. Lai lietotu jaunos Cipher iestatījumus, vispirms diskam ir jābūt atšifrētam.<br><br>
**Piezīme:** Ierīcēm, kuras tiek reģistrētas ar Autopilot, automātiskā šifrēšana, kas notiek OOBE laikā, netiek aktivizēta, kamēr Intune politika tiek novērtēta, kas ļauj izmantot politikas iestatījumus OS noklusējumu vietā.
 
J: ja ierīce ir šifrēta atbilstoši Intune politikas lietojumprogrammai, tā tiks atšifrēta, kad šī politika tiks noņemta?<br>
: Ar šifrēšanu saistītas politikas noņemšana neizraisa konfigurēto disku atšifrēšanu.
 
J: Kāpēc Intune atbilstības politika rāda, ka manā ierīcē nav iespējots līdzeklis BitLocker, kaut gan tas ir?<br>
A: "BitLocker iespējotais" iestatījums Intune atbilstības politikā izmanto Windows ierīces darbspējas atestācijas (DHA) klientu. Šis klients nosaka ierīces stāvokli tikai sāknēšanas laikā. Tāpēc, ja ierīce nav atsāknēta, jo BitLocker šifrēšana ir pabeigta, DHA klienta pakalpojums neziņo par BitLocker aktīvu.
 
 