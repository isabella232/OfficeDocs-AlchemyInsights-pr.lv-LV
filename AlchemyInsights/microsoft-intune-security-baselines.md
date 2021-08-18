---
title: Drošības bāzlīniju Microsoft Intune, lai konfigurētu Windows 10 ierīces
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
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331992"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Drošības bāzlīniju Microsoft Intune, lai konfigurētu Windows 10 ierīces

Intune drošības bāzes datus, kas palīdz aizsargāt lietotājus un ierīces. Drošības bāzes datu bāzes Windows ar iestatījumiem iepriekš konfigurētām grupām, ko izmanto, lai lietotu zināmu iestatījumu grupu un noklusējuma vērtības, ko iesaka attiecīgās drošības grupas. Izveidojot drošības bāzlīniju profilu inTune, jūs izveidojat veidni, kas sastāv no vairākiem ierīču konfigurācijas profiliem.

Izvietojot drošības bāzlīnijus lietotāju grupām vai ierīcēm, iestatījumi tiek lietoti ierīcēm, kuras darbojas Windows 10 versijā. Piemēram, Microsoft mobilo ierīču pārvaldības (MdM) drošības bāzlīnija automātiski iespējo BitLocker noņemamiem diskiem, pieprasa paroli ierīces atbloķēšanai un atspējo pamata autentifikāciju. Ja noklusējuma vērtība jūsu vidē nedarbojas, varat pielāgot bāzes datu bāzes informāciju, lai lietotu iestatījumus.

Drošības bāzes datu bāzes arī palīdz izveidot drošu darbplūsmu programmā Microsoft 365. Drošības bāzlīnija ietver labāko praksi un ieteikumus iestatījumiem, kas ietekmē drošību. Intune partneri ar Windows grupu, kas izveido bāzes datu bāzes datu grupas politikām, tāpēc šie ieteikumi ir balstīti uz nepārtrauktām vadlīnijām un plašas pieredzes.

Ja esat jauns Intune lietotājam un neesat pārliecināts par to, ar ko sākt, drošības bāzes rādītāji palīdz ātri izveidot un izvietot drošu profilu. Ja pašlaik izmantojat grupas politiku, migrēšana uz Intune pārvaldības nolūkiem ir daudz vienkāršāka, izmantojot drošības bāzes datus, jo tie ir iebūvēti intune un ietver modernas pārvaldības iespējas.

Papildinformāciju skatiet rakstā [Drošības Windows un Mobilo](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) ierīču [pārvaldība.](https://docs.microsoft.com/windows/client-management/mdm/)

