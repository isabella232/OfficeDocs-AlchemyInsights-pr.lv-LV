---
title: Pazudušu iOS ierīču atrašana ar Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439629"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Pazudušu iOS ierīču atrašana ar Intune

Ja iespējojat pazaudētu režīmu iOS ierīcē, administratoram ir parādīts ziņojums un kontaktpersonas tālruņa numurs bloķēšanas ekrānā.

Pēc tam, kad ir iespējots pazaudēts režīms, administrators var izmantot darbību atrast ierīci, lai noteiktu ierīces fizisko atrašanās vietu.

Opcija atrast ierīces darbību Intune darbojas ar iOS ierīcēm, lai kartē rādītu noteiktas ierīces atrašanās vietu.

Šīs darbības veikšanai nepieciešama iOS ierīces lietošana:

- Pārraudzīts režīms
- Zaudētais režīms

Papildinformāciju skatiet rakstā [pazaudēta režīma iespējošana iOS/iPadOS ierīcēs ar Intune](https://docs.microsoft.com/intune/device-lost-mode) un [atrodiet pazudušas vai nozagtas iOS/IPadOS ierīces ar Intune](https://docs.microsoft.com/intune/device-locate).

**BUJ**

J: es izdevu attālu darbību, lai noņemtu uzņēmuma datus no ierīces, un tagad tas ir iestrēdzis gaidīšanas stāvoklī.

A: lai attāla darbība būtu sekmīga, mērķtiecīgai ierīcei jābūt tiešsaistē un veselīgai. Tālāk norādītajās situācijās attālā darbība paliek gaidīšanas stāvoklī 30 dienas vai līdz brīdim, kad ierīce atpieņem komandu:

- Ja ierīcei nav savienojamības
- Kad ierīce zaudē pārvaldības statusu ar Intune

Ja uzskatāt, ka ierīce vairs netiek pārbaudīta un nevarēs noņemt uzņēmuma datus, atlasiet Dzēst. Dzēšot tiek noņemts ierīces ieraksts, un tas vairs netiek rādīts ierīču Intune sarakstā. Ja ierīce atkal kļūst aktīva, tās lietotājam tas būs atkārtoti jāreģistrē.

J: Kāpēc noteiktas attālas darbības nav pieejamas lietošanai?

A: ne visas platformas atbalsta visas attālās ierīces darbības. Tālāk norādītās attālās darbības ir platformas, tāpēc tās ir pieejamas tikai norādītajām platformām.

- Apiešanas aktivizēšanas bloķēšana (tikai iOS)
- Jauna startēšana (tikai Windows)
- Pazaudēts režīms (tikai iOS)
- Ierīces atrašana (tikai iOS)
- Restartēt (tikai operētājsistēmā Windows)

Detalizētu informāciju par katru darbību skatiet rakstā [Pieejamās ierīces darbības](https://docs.microsoft.com/intune/device-management#available-device-actions).