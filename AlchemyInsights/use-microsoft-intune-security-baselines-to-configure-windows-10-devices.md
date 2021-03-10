---
title: Microsoft Intune drošības bāzes izmantošana, lai konfigurētu Windows 10 ierīces
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694435"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Microsoft Intune drošības bāzes izmantošana Windows 10 ierīču konfigurēšanai

Intune drošības bāzlīnijas palīdz aizsargāt lietotājus un ierīces. Drošības bāzlīnijas ir Windows iestatījumi iepriekš konfigurētās grupas, ko izmanto, lai lietotu zināmo iestatījumu grupu un noklusējuma vērtības, ko iesaka atbilstošās drošības komandas. Izveidojot drošības bāzes profilu pakalpojumā Intune, izveidojiet veidni, kas sastāv no vairākiem ierīces konfigurācijas profiliem.

Kad izvietojat drošības bāzes līnijas lietotāju vai ierīču grupām, iestatījumi tiek lietoti ierīcēs, kas darbojas operētājsistēmā Windows 10 vai jaunākās versijās. Piemēram, automātiski izmantojot Microsoft mobilo ierīču pārvaldības (MDM) drošības bāzlīniju (1), tiek iespējots BitLocker noņemamajiem diskiem (2) ir nepieciešama parole ierīces atbloķēšanai, un (3) atspējo pamata autentifikācija. Ja jūsu vidē noklusējuma vērtība nedarbojas, varat pielāgot bāzes līniju, lai lietotu iestatījumus, kas nepieciešami.

Drošības bāzlīnijas palīdz arī izveidot end-to-end Secure Workflow pakalpojumā Microsoft 365. Tālāk norādītas šīs funkcionalitātes priekšrocības:
- Drošības sākumdokumentā ir iekļauta paraugprakse un ieteikumi par iestatījumiem, kas ietekmē drošību. Tā kā Intune partneriem ir Windows drošības grupa, kas izveido bāzes politikas bāzlīnijas, šie ieteikumi pamatojas uz stabilu orientāciju un plašu pieredzi.
- Ja esat iesācējs darbā ar Intune un neesat pārliecināts par to, kur sākt, pēc tam drošības bāzlīnijas palīdzēs ātri izveidot un izvietot drošu profilu.
- Ja pašlaik izmantojat grupas politiku, pēc tam migrējot uz Intune pārvaldības vajadzībām, ir daudz vienkāršāks ar drošības bāzes līnijām, jo šīs drošības bāzes ir iebūvētas Intune, kas ietver visprogresīvākās iespējas pārvaldībai.

Papildinformāciju skatiet rakstā [Windows drošības bāzlīnijas](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) un [mobilo ierīču pārvaldība](https://docs.microsoft.com/windows/client-management/mdm/).