---
title: Drošības Microsoft Intune bāzes datu izmantošana, lai konfigurētu Windows 10 ierīces
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793897"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Drošības Microsoft Intune bāzes datu izmantošana, lai konfigurētu Windows 10 ierīces

Intune drošības bāzes datus, kas palīdz aizsargāt lietotājus un ierīces. Drošības bāzes datu bāzes Windows ar iestatījumiem iepriekš konfigurētām grupām, ko izmanto, lai lietotu zināmu iestatījumu grupu un noklusējuma vērtības, ko iesaka attiecīgās drošības grupas. Izveidojot drošības bāzes datu profilu intune, jūs izveidojat veidni, kas sastāv no vairākiem ierīču konfigurācijas profiliem.

Izvietojot drošības bāzlīnijus lietotāju grupām vai ierīcēm, iestatījumi tiek lietoti ierīcēm, kuras darbojas Windows 10 versijā. Piemēram, Microsoft mobilo ierīču pārvaldības (Mobile Device Management — MDM) drošības bāzlīnija automātiski BitLocker iespējo datu iespējošanu noņemamiem diskiem, pieprasa ierīces atbloķēšanu ar paroli un atspējo pamata autentifikāciju. Ja noklusējuma vērtība jūsu vidē nedarbojas, varat pielāgot bāzes datu bāzes informāciju, lai lietotu iestatījumus.

Drošības bāzes datu bāzes arī palīdz izveidot drošu darbplūsmu programmā Microsoft 365. Drošības bāzlīnija ietver labāko praksi un ieteikumus iestatījumiem, kas ietekmē drošību. InTune partneri ar Windows grupu, kas izveido bāzes datu bāzes kodus grupas politikām, tāpēc šie ieteikumi ir balstīti uz nepārtrauktām vadlīnijām un plašas pieredzes.

Ja esat jauns Intune lietotājam un neesat pārliecināts par to, ar ko sākt, drošības bāzes rādītāji palīdz ātri izveidot un izvietot drošu profilu. Ja pašlaik izmantojat grupas politiku, migrēšana uz Intune pārvaldības nolūkiem ir daudz vienkāršāka, izmantojot drošības bāzes datus, jo tie ir iebūvēti intune un ietver modernas pārvaldības iespējas.

Papildinformāciju skatiet rakstā [Drošības Windows un Mobilo](/windows/security/threat-protection/windows-security-baselines) ierīču [pārvaldība.](/windows/client-management/mdm/)

