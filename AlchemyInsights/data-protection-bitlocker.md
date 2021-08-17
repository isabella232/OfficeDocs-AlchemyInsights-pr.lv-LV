---
title: DataProtection — Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118601"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker šifrēšanas iespējošana ar Intune

Intune galapunktu aizsardzības politiku var izmantot, lai konfigurētu Bitlocker šifrēšanas iestatījumus Windows ierīcēs. Papildinformāciju skatiet rakstā [Windows 10 (un jaunāku versiju) iestatījumu aizsardzība ierīcēs, izmantojot Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Papildus galapunktu aizsardzības politikai ir arī šifrēšanas atskaite, kas nodrošina detalizētāku ierīču šifrēšanas statusa skatu. Šai atskaitei var piekļūt no MEM portāla sadaļā Ierīces, **> Monitors** un pēc tam sadaļā **Konfigurācija** atlasiet [Šifrēšanas atskaite](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Ja bitlocker nav iespējots, kā paredzēts, vai kāds profils, kas tiek izmantots Bitlocker iespējošanai, ir kļūdas stāvoklī, lūdzu, pārskatiet šifrēšanas atskaiti, lai iegūtu labāku izpratni par darbības iemesliem.

Lai uzzinātu, kā interpretēt atskaiti, tostarp par dažādām šifrēšanas statusa vērtībām, skatiet rakstu [Ierīču šifrēšanas pārraudzība, izmantojot Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Ņemiet vērā, ka daudzas jaunākas ierīces, Windows 10 izmanto automātisko Bitlocker šifrēšanu, kas tiek izraisīta bez MDM politikas lietojumprogrammas. Tas var ietekmēt politikas lietojumprogrammu, ja ir konfigurēti iestatījumi, kas nav noklusējuma iestatījumi. Detalizētu informāciju skatiet tālāk bieži uzdoto jautājumu sadaļā.

Informāciju par bitlocker problēmu novēršanu skatiet rakstā [BitLocker politiku problēmu novēršana programmā Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**BUJ**

J: Kuri Windows atbalsta ierīču šifrēšanu, izmantojot galapunktu aizsardzības politiku?<br>
A: Intune galapunktu aizsardzības politikas iestatījumi tiek ieviesti, izmantojot [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Ne visi grupas izdevumi vai būvējumu Windows atbalsta Bitlocker CSP. <br><br>

J: Kā Bitlocker var iespējot ierīcēs, neprasot lietotāja mijiedarbību?<br>
A. Ja vien ir izpildīti nepieciešamie priekšnosacījumi, ir iespējams iespējot Bitlocker kluso šifrēšanu, izmantojot Intune. Skatiet detalizētu informāciju par ierīces prasībām un politikas iestatījumu piemēriem, lai iespējotu kluso šifrēšanu, šajā dokumentā: [Klusa Bitlocker šifrēšanas iespējošana.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

J. Ja ierīce jau ir šifrēta ar Bitlocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un šifrēšanas spēkam (XTS-AES-128), vai politika tiks lietota ar dažādiem iestatījumiem, automātiski aktivizēs diska atkārtotu šifrēšanu ar jaunajiem iestatījumiem?<br>
A: Nē. Lai lietotu jaunos cipher iestatījumus, diskam vispirms jābūt atšifrētam.<br><br>
**Piezīme.** Autopilot reģistrētajās ierīcēs OOBE laikā notiek automātiskā šifrēšana netiek izraisīta, kamēr nav novērtēta Intune politika, kas ļauj izmantot uz politiku balstītus iestatījumus OS noklusējuma vērtību vietā.
 
J: Ja ierīce tiks šifrēta Intune politikas programmas rezultātā, vai tā tiks atšifrēta, kad šī politika tiks noņemta?<br>
A. Ar šifrēšanu saistītas politikas noņemšana NERADA konfigurēto disku atšifrēšanu.
 
J: Kāpēc Intune atbilstības politika rāda, ka manā ierīcē nav iespējots Bitlocker, lai gan tā ir?<br>
A: Iestatījums "Bitlocker iespējots" Intune atbilstības politikā izmanto Windows ierīces darbspējas atestācijas (TUN) klientu. Šis klients tikai mēra ierīces stāvokli sāknēšanas laikā. Tāpēc, ja ierīce nav atkārtoti palaista kopš Bitlocker šifrēšanas pabeigšanas, REBOOT klienta pakalpojums ne ziņos, ka Bitlocker ir aktīvs.
 
 