---
title: Tīmekļa programmu veikalā SharePoint trūkst terminu
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106433"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker šifrēšanas iespējošana ar Intune

Intune galapunktu aizsardzības politiku var izmantot, lai konfigurētu Boitlocker šifrēšanas iestatījumus Windows ierīcēs, kā aprakstīts rakstā : Windows10 (un jaunākas versijas) iestatījumi ierīču aizsardzībai, izmantojot Intune

Ņemiet vērā, ka daudzas jaunākas ierīces, kurās darbojas Windows 10 automātisko bitlocker šifrēšanu, kas tiek izraisīta bez MDM politikas lietojumprogrammas. Tas var ietekmēt politikas lietojumprogrammu, ja ir konfigurēti iestatījumi, kas nav noklusējuma iestatījumi. Papildinformāciju skatiet bieži uzdotajos bieži uzdotajos bieži uzdotajos jautājumus.


Bieži uzdotie jautājumi: kuri Windows atbalsta ierīču šifrēšanu, izmantojot galapunktu aizsardzības politiku?
A: Intune galapunktu aizsardzības politikas iestatījumi tiek ieviesti, izmantojot Bitlocker CSP.  Ne visi grupas izdevumi un būvējumu Windows atbalsta Bitlocker CSP. Pašlaik Windows izdevumi: Enterprise; Education, Mobile, Mobile Enterprise un Professional (no 1809. būvējuma) tiek atbalstītas.




J: Ja ierīce jau ir šifrēta ar Bitlocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un šifrēšanas spēkam (XTS-AES-128), politika tiks lietota ar dažādiem iestatījumiem, automātiski aktivizēs diska atkārtotu šifrēšanu ar jaunajiem iestatījumiem?

A: Nē. Lai lietotu jaunos cipher iestatījumus, diskam vispirms jābūt atšifrētam.

Piezīme. Ierīcēs, kas ir reģistrētas, izmantojot autopilot automātisko šifrēšanu, kas tiek veikta OOBE laikā, netiek izraisīta, kamēr netiek novērtēta Intune politika, kas ļauj izmantot politikas iestatījumus OS noklusējuma atrašanās vietā




J Ja ierīce tiks šifrēta Intune politikas programmas rezultātā, tā tiks atšifrēta, kad šī politika tiks noņemta?

A. Ar šifrēšanu saistītas politikas noņemšana NEšifrēt konfigurētos diskus.




J: Kāpēc intune atbilstības politika rāda, ka manā ierīcē nav iespējots Bitlocker, bet tā ir?

A: Iestatījums "Bitlocker iespējots" intune atbilstības politikā izmanto Windows ierīces darbspējas atestācijas (TUN) klientu. Šis klients tikai mēra ierīces stāvokli sāknēšanas laikā. Tāpēc, ja ierīce nav atkārtoti palaista kopš bitlocker šifrēšanas pabeigšanas IEGUVES klienta pakalpojums ne ziņos par bitlocker kā aktīvu.