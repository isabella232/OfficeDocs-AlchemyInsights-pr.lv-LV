---
title: SharePoint Online terminu krātuvē trūkst terminu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750458"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker šifrēšanas iespējošana ar Intune

Intune Endpoint Protection politiku var izmantot, lai konfigurētu Boitlocker šifrēšanas iestatījumus Windows ierīcēm, kā aprakstīts: Windows 10 (un jaunākas versijas) iestatījumi, lai aizsargātu ierīces, kas izmanto Intune

Ņemiet vērā, ka daudzās jaunākās ierīcēs, kurās darbojas operētājsistēma Windows 10, tiek atbalstīta automātiskā BitLocker šifrēšana, kas tiek palaista, nelietojot MDM politiku. Tas var ietekmēt politikas lietojumu, ja nav konfigurēti noklusējuma iestatījumi. Detalizētāku informāciju skatiet rakstā bieži uzdotie jautājumi.


Bieži uzdotie jautājumi   : kādus Windows izdevumus atbalsta ierīces šifrēšana, izmantojot galapunktu aizsardzības politiku?
 A: Intune Endpoint Protection politikas iestatījumi tiek ieviesti, izmantojot BitLocker CSP.Ne visi izdevumi un būvējumi Windows neatbalsta BitLocker CSP. 
      Šajā laikā Windows izdevumi: Enterprise; Tiek atbalstītas Education, Mobile, Mobile Enterprise un Professional (no būvējuma 1809).




J: ja ierīce jau ir šifrēta ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un Cipher Strength (XTS-AES-128), tiks lietota politika ar dažādiem iestatījumiem, kas automātiski aktivizēs ar jaunajiem iestatījumiem atkārtoti šifrētu disku.

A: Nē. Lai lietotu jaunos Cipher iestatījumus, vispirms diskam ir jābūt atšifrētam.

Piezīme ierīcēm, kas tiek reģistrētas, izmantojot automātisko testēšanu, automātiskā šifrēšana, kas rastos OOBE laikā, netiek aktivizēta, kamēr Intune politika tiek novērtēta, kas ļauj izmantot politikas iestatījumus, kas tiek izmantoti OS noklusējumu vietā




Ja ierīce ir šifrēta atbilstoši Intune politikas lietojumam, tā tiks atšifrēta, kad šī politika tiks noņemta?

: Šifrēšanas saistītās politikas noņemšana neizraisa to disku atšifrēšanu, kas ir konfigurēti.




J: Kāpēc Intune atbilstības politika rāda, ka manai ierīcei nav "BitLocker iespējots", bet tas ir?

A: "BitLocker iespējots" iestatījums Intune atbilstības politikā izmanto Windows ierīces Health atestācijas (DHA) klientu. Šis klients nosaka ierīces stāvokli tikai sāknēšanas laikā. Tāpēc, ja ierīce nav atsāknēta, jo ir pabeigta BitLocker šifrēšana, DHA klienta pakalpojums neziņo par BitLocker aktīvu.