---
title: Microsoft Intune drošības bāzes izmantošana, lai konfigurētu Windows 10 ierīces
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573538"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Microsoft Intune drošības bāzes izmantošana, lai konfigurētu Windows 10 ierīces

Intune drošības bāzlīnijas palīdz aizsargāt lietotājus un ierīces. Drošības bāzlīnijas ir Windows iestatījumi iepriekš konfigurētās grupas, ko izmanto, lai lietotu zināmo iestatījumu grupu un noklusējuma vērtības, ko iesaka atbilstošās drošības komandas. Izveidojot drošības bāzes profilu pakalpojumā Intune, izveidojiet veidni, kas sastāv no vairākiem ierīces konfigurācijas profiliem.

Kad izvietojat drošības bāzes līnijas lietotāju vai ierīču grupām, iestatījumi tiek lietoti ierīcēs, kas darbojas operētājsistēmā Windows 10 vai jaunākā versijā. Piemēram, MDM drošības bāzlīnija automātiski (1) iespējo BitLocker noņemamiem diskiem (2), ir nepieciešama parole ierīces bloķēšanai, un (3) atspējo pamata autentifikāciju. Ja jūsu vidē noklusējuma vērtība nedarbojas, pielāgojiet bāzes līniju, lai lietotu iestatījumus, kas nepieciešami.

Drošības bāzlīnijas palīdz arī izveidot end-to-end Secure Workflow pakalpojumā Microsoft 365. Tālāk ir norādītas dažas priekšrocības:

- Drošības sākumdokumentā ir iekļauta paraugprakse un ieteikumi par iestatījumiem, kas ietekmē drošību. Tā kā Intune partneriem ir Windows drošības grupa, kas izveido bāzes politikas bāzlīnijas, šie ieteikumi pamatojas uz stabilu orientāciju un plašu pieredzi.
- Ja esat iesācējs darbā ar Intune un neesat pārliecināts par to, kur sākt, pēc tam drošības bāzlīnijas palīdzēs ātri izveidot un izvietot drošu profilu.
- Ja pašlaik izmantojat grupas politiku, pēc tam migrēšana uz Intune pārvaldības vajadzībām ir daudz vienkāršāka ar drošības bāzes līnijām, jo tās ir iebūvētas Intune un ietver visprogresīvākās iespējas pārvaldībai.

Papildinformāciju skatiet rakstā [Windows drošības bāzlīnijas](https://go.microsoft.com/fwlink/?linkid=2141503) un [mobilo ierīču pārvaldība](https://go.microsoft.com/fwlink/?linkid=2141701).