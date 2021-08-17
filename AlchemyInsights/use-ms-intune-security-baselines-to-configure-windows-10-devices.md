---
title: Drošības Microsoft Intune bāzes datu izmantošana, lai konfigurētu Windows 10 ierīces
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104351"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Drošības Microsoft Intune bāzes datu izmantošana, lai konfigurētu Windows 10 ierīces

Intune drošības bāzes datus, kas palīdz aizsargāt lietotājus un ierīces. Drošības bāzlīnijas Windows ar iestatījumiem iepriekš konfigurētām grupām, ko izmanto, lai lietotu zināmu iestatījumu grupu un noklusējuma vērtības, ko iesaka attiecīgās drošības grupas. Izveidojot drošības bāzes datu profilu intune, jūs izveidojat veidni, kas sastāv no vairākiem ierīču konfigurācijas profiliem.

Izvietojot drošības bāzlīnijus lietotāju grupām vai ierīcēm, iestatījumi tiek lietoti ierīcēm, kuras darbojas Windows 10 versijā. Piemēram, MDM drošības bāzlīnija automātiski (1) iespējo BitLocker noņemamiem diskiem, (2) pieprasa ierīces atbloķēšanu, un (3) atspējo pamata autentifikāciju. Ja noklusējuma vērtība jūsu vidē nedarbojas, pielāgojiet bāzes datu bāzes informāciju, lai lietotu iestatījumus.

Drošības bāzes datu bāzes arī palīdz izveidot drošu darbplūsmu programmā Microsoft 365. Tam ir dažas priekšrocības:

- Drošības bāzlīnija ietver labāko praksi un ieteikumus iestatījumiem, kas ietekmē drošību. Tā kā Intune darbojas Windows drošības grupu, kas izveido bāzes datu grupas politikām, šie ieteikumi ir balstīti uz nepārtrauktām vadlīnijām un plašas lietošanas iespējas.
- Ja esat jauns Intune lietotājam un neesat pārliecināts par to, ar ko sākt, drošības bāzes rādītāji palīdzēs ātri izveidot un izvietot drošu profilu.
- Ja pašlaik izmantojat grupas politiku, migrācija uz Intune pārvaldības nolūkos ir daudz vienkāršāka, izmantojot drošības bāzes datus, jo tie ir iebūvēti Intune un ietver visas iespējas pārvaldībai.

Papildinformāciju skatiet rakstā [Drošības Windows un Mobilo](https://go.microsoft.com/fwlink/?linkid=2141503) ierīču [pārvaldība.](https://go.microsoft.com/fwlink/?linkid=2141701)