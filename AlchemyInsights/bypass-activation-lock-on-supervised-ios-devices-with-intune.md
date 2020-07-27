---
title: Apiešanas aktivizēšanas bloķēšana pārraudzītās iOS ierīcēs ar Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424207"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Apiešanas aktivizēšanas bloķēšana pārraudzītās iOS ierīcēs ar Intune

Iespēja apiet aktivizācijas bloķēšanu iOS ierīcēs atvieglo atkopšanos no scenārija, kad lietotājs nodrošina aktivizēšanas bloķēšanu korporatīvā ierīcē un pēc tam atstāj uzņēmumu.

Priekšnosacījumi aktivizācijas bloķēšanas apiešanai ir šādi:

- Ierīce ir "pārraudzība".
- Aktivizēšanas bloķēšana ir veiksmīgi iespējota, izmantojot iOS ierīces ierobežojumu politiku Intune.

Turklāt, apejot aktivizācijas atslēgu, ir jāveic tālāk norādītās darbības.

- Fiziski ir jānoslauka ierīce.
- Kopējiet kodu pirms tīrīšanas izdošanas.

**Piezīme:** Tīrīšanas kods nav reģistrjutīgs, tāpēc "-" rakstzīmes nav vajadzīgas.

Detalizētu informāciju skatiet rakstā [aktivizēšanas bloķēšanas apiešana Uzraudzītās iOS ierīcēs ar Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**BUJ**

J: **es izdevu attālu darbību, lai noņemtu uzņēmuma datus no ierīces, un tagad tas ir iestrēdzis gaidīšanas stāvoklī.**

A: lai attāla darbība būtu sekmīga, mērķtiecīgai ierīcei jābūt tiešsaistē un veselīgai. Tālāk norādītajās situācijās attālā darbība paliek gaidīšanas stāvoklī 30 dienas vai līdz brīdim, kad ierīce atpieņem komandu:

- Nav savienojamības.
- Zaudē pārvaldības statusu ar Intune.

Ja uzskatāt, ka ierīce vairs netiek pārbaudīta, un tā neizņems uzņēmuma datus, atlasiet Dzēst. Dzēšot tiek noņemts ierīces ieraksts, un tas vairs netiek rādīts ierīču Intune sarakstā. Lai ierīce atkal kļūtu aktīva, tās lietotājam ir atkārtoti jāpiesakās ierīcē.

J: **Kāpēc noteiktas attālas darbības nav pieejamas lietošanai?**

A: ne visas platformas atbalsta visas attālās ierīces darbības. Tālāk norādītās attālās darbības ir Platform-specifiskas.

- Apiešanas aktivizēšanas bloķēšana (tikai iOS)
- Jauna startēšana (tikai Windows)
- Pazaudēts režīms (tikai iOS)
- Ierīces atrašana (tikai iOS)
- Restartēt (tikai operētājsistēmā Windows)

Detalizētu informāciju par katru darbību skatiet rakstā [Pieejamās ierīces darbības](https://docs.microsoft.com/intune/device-management#available-device-actions).